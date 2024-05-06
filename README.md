# Cyrex Enterprise Go Linter config (golangci-lint)

Usage examples:

```
golangci-lint run -c <(curl https://raw.githubusercontent.com/Cloudoki/rexe-golint-config/main/config.yaml)
```

```
/tmp/.golangci.yml:
	curl https://raw.githubusercontent.com/Cloudoki/rexe-golint-config/main/config.yaml --output /tmp/.golangci.yml

.PHONY: lint
lint: /tmp/.golangci.yml
	golangci-lint run --config=/tmp/.golangci.yml
```
