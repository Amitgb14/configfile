
# configfile

Used to read configuration files in golang.

### Syntax

```go

	content, err := config.Yaml(configFile)
	if err != nil {
		log.Fatalf("Read config: %v", err, content)
	}
```

```yaml
host: localhost
port: 8080
thread: 1
loop: 1
requests:
  - path: /status
    method: GET
    status: 200
```