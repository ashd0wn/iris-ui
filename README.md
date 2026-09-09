# iris-ui

Web interface for the [Iris](https://github.com/ashd0wn/iris) project.
Fork of [datarhei/restreamer-ui](https://github.com/datarhei/restreamer-ui).

## Role in the Iris stack

This repo contains the React frontend only.
It is compiled and embedded into iris-core via go:embed at deploy time.

Do not use standalone -- use the deploy script from iris.

## Build

npm install --legacy-peer-deps
PUBLIC_URL=/ npm run build
# -> build/ ready to be copied into iris-core/app/ui/

## Changes from upstream

- Iris branding (logo, colors, text)
- homepage: / in package.json (no /ui/ prefix)
- No Docker configuration

