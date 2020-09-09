## Create Your First Substrate Chain

Installation: (Linux, iOS, Windows (Windows Subsystem for Linux))

```curl https://getsubstrate.io -sSf | bash -s -- --fast```

```cargo --version```<br>
cargo 1.46.0 (149022b1d 2020-07-17)

```node --version```<br>
v11.10.1

```yarn --version```<br>
1.22.5

## Compiling Substrate:

#### 1. Clone the Node Template (version v2.0.0-rc6).

``` git clone -b v2.0.0-rc6 --depth 1 https://github.com/substrate-developer-hub/substrate-node-template```

#### 2. Initialize your WebAssembly build environment

```source ~/.cargo/env```
```rustup update nightly```
```rustup update stable```
```rustup target add wasm32-unknown-unknown --toolchain nightly```

#### 3. Compile the Node Template
```cd substrate-node-template/```
```cargo build --release```

Process may take approx 30 mins.

## Front-End Development:

#### 1. Clone the code from github
```git clone -b v2.0.0-rc6 --depth 1 https://github.com/substrate-developer-hub/substrate-front-end-template```

#### 2. Install the dependencies
```cd substrate-front-end-template && yarn install```

## Starting Your Node:
#### 1. Run a temporary node in development mode
```./target/release/node-template --dev --tmp```

#### 2. Run Front-end
```yarn start```

#### 3. Interact
Once the Front-End Template is running and loaded in your browser at ```http://localhost:8000/```, take a moment to explore its components.

#### 4. Transfer
Transfer tokens from one account to another, minimum ```1000000000000```
