<h1>Soundness Testnet Full Guide</h1>


----

```console
sudo apt update && sudo apt upgrade -y
```

```console
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

```console
source $HOME/.cargo/env
```

```console
rustc --version
cargo --version
```

```console
echo 'source $HOME/.cargo/env' >> ~/.bashrc
```

```console
source ~/.bashrc
```

```console
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```

```console
source ~/.bashrc
```

```console
soundnessup install
soundnessup update
```

```console
soundness-cli generate-key --name my-key
```

Importing a Key Pair
To import an existing key pair from a mnemonic phrase:

```console
soundness-cli import-key --name my-key
```

Listing Key Pairs
To view all stored key pairs and their associated public keys:

```console
soundness-cli list-keys
```

Exporting Key Mnemonic
To export the mnemonic phrase for a stored key pair:

```console
soundness-cli export-key --name my-key
```
