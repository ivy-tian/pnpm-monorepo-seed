# Monorepo

## Quick Start

Preinstall

```bash
$ npm i -g pnpm
$ pnpm -v # should >= 6.20.0
# Install Rust and Cargo
$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Install dependencies, it will take a whild pla waite

```bash
$ pnpm install
```
### React App

```bash
# Start React App
$ pnpm --filter "react-app" start
```

![](https://user-images.githubusercontent.com/13595509/146680807-a15b411e-075a-438e-b020-f3d88240c55d.png)

### Vite App

```bash
$ pnpm start --filter "vite-app"
```

![](https://user-images.githubusercontent.com/13595509/146680790-c5b506ae-5006-42a2-b9df-c379499dab3b.png)


#### Node.js App

```bash
$ pnpm --filter "node-app" start
```

![](https://user-images.githubusercontent.com/13595509/146680754-8b6798f4-fa4f-43ff-929e-911e1343ef88.png)

#### Dumi App

```bash
# using `...` will run `start` script of dumi-app and all of its dependencies:
$ pnpm --filter "dumi-app..." --parallel start
```

![](https://user-images.githubusercontent.com/13595509/170510753-df4a6016-46b2-4252-9722-b765261c1a19.gif)

## Packages Development

### packages/shared

```bash
$ pnpm --filter "@infras/shared" dev
```

### packages/ui

```bash
$ pnpm --filter "@infras/ui" dev
```

### packages/native

```bash
$ pnpm --filter "@infras/native" build
```
