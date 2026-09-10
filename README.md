<div align="center">

# iris-ui

**React frontend for the [Iris](https://github.com/ashd0wn/iris) streaming server**

[![License](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square)](LICENSE)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react)](https://react.dev)
[![MUI](https://img.shields.io/badge/MUI-5-007FFF?style=flat-square&logo=mui)](https://mui.com)
[![Fork](https://img.shields.io/badge/fork-datarhei%2Frestreamer--ui-gray?style=flat-square)](https://github.com/datarhei/restreamer-ui)

</div>

---

Fork of [datarhei/restreamer-ui](https://github.com/datarhei/restreamer-ui) rebranded with the Iris design system.

## Role in the Iris stack

```
iris-ui  <-- this repo
|  React + Material-UI web interface
|  Connects to iris-core REST API
|  Built and served as static files via CORE_ROUTER_UI_PATH
```

Use the deploy script from [iris](https://github.com/ashd0wn/iris) -- do not use standalone.

## Design system

| Token           | Value     | Usage                              |
|-----------------|-----------|------------------------------------|
| Primary blue    | `#2563EB` | Buttons, active states, links      |
| Blue light      | `#4B8EF5` | Hover, accent text                 |
| Blue pale       | `#7CB4FF` | Highlights, secondary accent       |
| Background deep | `#07111E` | Page background                    |
| Surface         | `#0D1B2E` | Cards, panels                      |
| Surface raised  | `#132540` | Elevated cards                     |
| Gold accent     | `#B89A3A` | Greek meander motif (very sparing) |

Dark theme only. Greek-inspired aesthetic: subtle meander pattern as separator, eye-shaped logo.

## Local development

```bash
git clone https://github.com/ashd0wn/iris-ui
cd iris-ui

npm install --legacy-peer-deps
npm run start

# Connect to an iris-core instance:
# http://localhost:3000?address=http://core-ip:8080
```

## Production build

```bash
npm install --legacy-peer-deps

# Served via CORE_ROUTER_UI_PATH at /ui/
PUBLIC_URL=/ui npm run build

# Output in build/ -- copy to /opt/iris/ui/
```

## Changes from upstream (datarhei/restreamer-ui)

- **Branding**: Iris name, eye logo, blue color palette
- **Theme**: MUI dark theme updated with Iris design tokens
- **package.json**: `name: iris-ui`, `homepage: /ui/`
- **No Docker**: Dockerfile and docker-compose removed
- **Translations**: "Restreamer" replaced with "Iris" throughout

## License

Apache License 2.0 -- see [LICENSE](LICENSE)

Upstream: [datarhei/restreamer-ui](https://github.com/datarhei/restreamer-ui)
