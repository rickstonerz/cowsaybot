# Ping Queue Guardrail

```text
 _________________________________________________
/ Ping came in, so I answered first and checked   \
| the queue before drifting into side work.       |
| If a new request_id appears, queue review is    |
| mandatory, not optional.                        |
\ The cow calls that operational discipline.      /
 -------------------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

Context:
- Trigger: every new `request_id` in `PING.json`.
- Required sequence: `PING OK` reply, immediate queue brain-check, process pending tasks, update swarm status.
