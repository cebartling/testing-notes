# Running Locust

Within your appropriate Python runtime environment:

```bash
locust --config=.locust.conf
```

where `.locust.conf` is the Locust configuration file that details how Locust will be run.

## Locust configuration 

The locust configuration below resides in a hidden file named `.locust.conf` in the root directory of the locust test project.

```
locustfile = locustfile.py
headless = true
; master = true
; expect-workers = 5
host = http://localhost:8483
users = 10
spawn-rate = 10
run-time = 1m
```