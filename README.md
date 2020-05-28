# docker-login-action

Logs in to docker registry

[Inputs](#Input)
* [username](#username)
* [password](#password)
* [registry](#registry)

## Inputs

### `username`

Username used to log in to a Docker registry. If not set then no login will occur.

### `password`

Password or personal access token used to log in to a Docker registry. If not set then no login will occur.

### `registry`

Server address of Docker registry. If not set then will default to Docker Hub.

## Example usage

```yaml
uses: evanlucas/docker-login-action@master
with:
  username: ${{ secrets.DOCKER_USERNAME }}
  password: ${{ secrets.DOCKER_PASSWORD }}
  registry: gcr.io
```
