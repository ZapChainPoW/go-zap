# ⚡ ZapChain

Miner-focused decentralized layer 1 blockchain: no premine, no dev fees, no instamine. Built to be the open data & logic layer for forums, blogs, and mini-sites.

🌐 Website: [https://zapchain.io/](zapchain.io)

---

## ✨ Features

- ⛏️ **Proof-of-Work** — Ethash consensus, battle-tested and secure.
- 💠 **EVM Compatible** — Fully supports Ethereum tooling, dApps, and smart contracts.
- 📦 **Fixed Supply** — Transparent and predictable emission.
- 🚫 **No Premine** — The team holds no coins at genesis.
- 🚫 **No Instamine** — 1T genesis difficulty to avoid early exploitation.
- 🚫 **No Dev Fees** — 100% of block rewards go to miners.
- 🚫 **No Uncle Rewards** — Simplified and fair issuance.
- ♾️ **Infinite Supply** — keeps PoW incentives alive indefinitely.

---

## 📊 Configuration

- 🏷️ **Chain ID** — 757
- ⛏️ **Block Reward** — 0.10 ZAP
- ⏱️ **Block Time** — ~12.5 seconds

---

## 🚀 Getting Started

### 🔧 Build from source

(To build from source requires Golang **1.20.x** or **1.21.x**)
```bash
git clone https://github.com/ZapChainPoW/go-zap
cd go-zap
go build -o build/bin/geth ./cmd/geth
````

### ⛏️ Run a node

```bash
./build/bin/geth --networkid 757 --datadir ./data --http --http.api "eth,net,web3,miner"
```

### ⛏️ Start mining

```bash
./build/bin/geth --mine --miner.threads=4 --miner.etherbase=0xYourAddressHere
```

