# supervisor-healthcheck

A simple health check for [Supervisor](http://supervisord.org/), uses [XML-RPC API](http://supervisord.org/api.html)

## Configuration

- `HOST` - Supervisor host
- `PORT` - Supervisor port

## Endpoints

- `/` - always returns 200 and "ok"
- `/health/check` opens Supervisor RPC and returns result based on running tasks

## Examples

```json
{
  "status": true,
  "supervisor_state": {
    "state_code": 1,
    "state_name": "RUNNING"
  }
}
```

