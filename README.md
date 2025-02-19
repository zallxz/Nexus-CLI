# Nexus-CLI
How to run Nexus Node

![image](https://github.com/user-attachments/assets/ca6aff98-5366-4775-8d69-7334fc390765)

| X        | Minimum              |
|------------------|----------------------------|
| **CPU**          | 4 |
| **RAM**          | 9++ GB                     |
| **Storage**      | 50 GB SDD                   |
| **Network**      | 100 Mbps (1 Gbps+ recommended) |
| **Image**      | Ubuntu 22.04 |

# Web / Sing Up : 

-  https://app.nexus.xyz/ - Register on the site with your wallet and email at the top right - it's better to use the same one you used on the old testnet.

## 1. Server Update : 

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. Install Packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen unzip lz4 -y
```

```bash
sudo apt install build-essential pkg-config libssl-dev git-all protobuf-compiler
```


```bash
sudo apt remove -y protobuf-compiler
wget https://github.com/protocolbuffers/protobuf/releases/download/v25.2/protoc-25.2-linux-x86_64.zip
sudo apt install unzip
unzip protoc-25.2-linux-x86_64.zip -d $HOME/.local
export PATH="$HOME/.local/bin:$PATH"
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

```bash
cargo clean
cargo build --release
```
# 3. Nexus CLI : 

```bash
screen -S nexus
```

```bash
curl https://cli.nexus.xyz/ | sh
```

## Link : https://app.nexus.xyz/


<p align="center">
  <img src="https://komarev.com/ghpvc/?username=FurkanL0&style=flat-square&color=red&label=Profile+Views+/+Repo+Views+" alt="Repo / Profile Views" />
</p>
