# Seismic Encrypted Contract

# Setup Guide
## Install Dependecies
**Install Rust**
```bash
curl https://sh.rustup.rs -sSf | sh
. "$HOME/.cargo/env"
```

**IF you’re on Mac Terminal, Install Jq if you don’t have it installed**
```bash
brew install jq
```

**Install sfoundryup**
```bash
curl -L \
     -H "Accept: application/vnd.github.v3.raw" \
     "https://api.github.com/repos/SeismicSystems/seismic-foundry/contents/sfoundryup/install?ref=seismic" | bash
source ~/.bashrc
```

**Run sfoundryup**
```bash
sfoundryup 
```

**Clone repository**
```bash
git clone --recurse-submodules https://github.com/SeismicSystems/try-devnet.git
cd try-devnet/packages/contract/
```

**Deploy contract**
```bash
bash script/deploy.sh
```

*** A new wallet will be generated for you, copy it and head over to the link below, enter wallet address and claim test token**
- Visit: https://faucet-2.seismicdev.net/


**Install Bun**
```bash
curl -fsSL https://bun.sh/install | bash
```

**Install node dependencies**
```bash
cd try-devnet/packages/cli/
bun install
```

**Send transactions**
```bash
bash script/transact.sh
```