Soundness Testnet Guide
sudo apt update && sudo apt upgrade -y
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
rustc --version
cargo --version
echo 'source $HOME/.cargo/env' >> ~/.bashrc
source ~/.bashrc
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
source ~/.bashrc
soundnessup install
soundnessup update
soundness-cli generate-key --name my-key
Importing a Key Pair To import an existing key pair from a mnemonic phrase:
soundness-cli import-key --name my-key
Listing Key Pairs To view all stored key pairs and their associated public keys:
soundness-cli list-keys
Exporting Key Mnemonic To export the mnemonic phrase for a stored key pair:
soundness-cli export-key --name my-key
