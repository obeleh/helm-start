# Helm start

This repo contains the most simple helm chart possible. It doesn't contain any of the best practices for deploying a production-grade application.

## Requirements

```bash
brew install helm
```

## Usage

Render to stdout:
```bash
help template myapp
```

Render to file:
```bash
helm template myapp --output-dir test_output
```

How you would use it:
```bash
helm install myapp ./myapp
```

More detailed
```bash
helm -n my-namespace install myapp -f my-values.yaml ./myapp
```