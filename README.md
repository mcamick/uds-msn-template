run `docker build -t custom-nginx:latest ../src/hello-world/`

`cd` into UDS directory and `zarf package create` to create your zarf package.

Then to deploy your package, run `zarf package deploy zarf-package-hello-world-arm64-1.0.0.tar.zst --set DOMAIN=uds.dev --set ENABLE_SSO=true --confirm`
