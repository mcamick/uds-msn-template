run `docker build -t custom-nginx:latest ../src/hello-world/`

`cd` into UDS directory and `zarf package create --set ENABLE_SSO=true` to create your zarf package.

Then to deploy your package, run `zarf package deploy zarf-package-hello-world-arm64-*.tar.zst`
