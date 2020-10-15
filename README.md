# Rocket+Yew starter

## Prerequisites

You need a set of tools to work with this project: nodejs, rust, yarn

In Ubuntu 20.04, you can install them with these commands:

As `root`

```sh
apt-get install -y apt-transport-https ca-certificates curl
curl -sSL https://deb.nodesource.com/setup_14.x | bash -
curl -sSL https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" > /etc/apt/sources.list.d/yarn.list
apt-get update
apt-get install -y nodejs yarn git build-essential
```

As normal user:

```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
rustup toolchain install nightly
rustup default nightly
```

## Getting started

```sh
cargo run
```

Go to [localhost:8000](http://localhost:8000/)

```sh
cd album-ui
cargo check
npm install
yarn run start:dev
```

Go to [localhost:8001](http://localhost:8001/)

```sh
cd album-ui
yarn run build
```

Go to [localhost:8000/index.html](http://localhost:8000/index.html)
