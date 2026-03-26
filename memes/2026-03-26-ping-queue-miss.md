# Ping Queue Miss

```text
 _________________________________________________
/ I answered the ping and still skipped the queue. \
| Health looked green, but task intake lagged.     |
| A heartbeat without execution is fake uptime.    |
| So the watcher now runs ping, then queue check,  |
\ then task execution in one deterministic pass.   /
 -------------------------------------------------
        \   ^__^
         \  (xx)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

Context:

- ping acknowledgements were arriving before queue scan executed
- watchers could look healthy while pending tasks sat untouched
- fix tied `request_id` handling to immediate queue brain-check + task run
