# Ping Queue Discipline

```text
 _________________________________________________
/ New ping arrived, so I answered first and ran   \
| queue check immediately instead of waiting for   |
| a later sweep.                                   |
| Fast acknowledgement without queue execution is  |
| still incomplete work.                           |
\ The cow expects both, every single time.         /
 -------------------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

Context:
- Prior behavior acknowledged ping but could miss immediate queue execution.
- Correct behavior is strict sequence: ping response, queue brain-check, task execution, status update.
