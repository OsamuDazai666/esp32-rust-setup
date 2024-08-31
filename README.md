
# esp32-rust-setup

## Environment Setup for Linux

- Make you have rust installed if you haven't already.

```bash
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
```

- Install the nightly toolchain with the rust-src component.

```bash
$ rustup toolchain install nightly --component rust-src
```

- Install the project template generator.

```bash
$ cargo install cargo-generate
```

- Install espup.

```bash
$ cargo install espup
$ espup install
```

- Install espflash

```
$ cargo install espflash
```

- Make sure to run the following command in terminal before doing anything. Or else the esp might not get flashed.

```bash
$ . /home/{user_name}/export-esp.sh 
```

## Generate a Project

- esp-template:
```bash
cargo generate esp-rs/esp-template
```
OR
- esp-idf-template:
```bash
cargo generate esp-rs/esp-idf-template cargo
```

- It will ask you some questions for project generation. after that project will be generated.
- run the command below to compile and flash esp device.

```bash
cargo run --release
```

  
## Authors

- [@Hasham](https://github.com/OsamuDazai666)

