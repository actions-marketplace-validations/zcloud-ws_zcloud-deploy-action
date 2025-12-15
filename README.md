# zCloud deploy action

This action deploy content on [zCloud](https://www.zcloud.ws) platform

## Inputs

## `user-token`

**Optional** Token to authenticate the user.

## `env-token`

**Optional** Token to authenticate the app environment.

## `env`

**Required** Environment name to create or update.

## `dir`

**Optional** Directory usage as source code to send to deploy (default value is current dir)

## `image`

**Optional** Image name to deploy.

## `app`

**Optional** Name of the app in which the environment will be created or updated (requires usage together with the --create argument).

## `copy-env-vars-from`

**Optional** Name of the environment from which the env vars will be copied to the new environment (requires usage together with the --create argument).

## `api-cli-uri`

**Optional** Custom API URL for full private region deployments.

## `cli-extra-args`

**Optional** CLI extra arguments.

## Example usage

```yaml
uses: zcloud-ws/zcloud-deploy-action@main
with:
  user-token: USER_TOKEN
  env: ENV_NAME
  dir: app1
  cli-extra-args: "--env-var ENV1=VAL1 --env-var ENV2=VAL2"
```

# zCloud CLI

- [Documentation](https://docs.zcloud.ws/docs/cli/)
- [Docker](https://hub.docker.com/r/zcloudws/zcloud-cli)
