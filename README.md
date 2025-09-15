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

### 🔧 Official Peer List
```
enode://940fa2f88bd7d9fba64b0763216370adae3a1d5c960865f91e7803f30746871617682d13d1088716789036ac5da064c1c222f4763b847e2bdc15d67aeea7dde3@209.74.80.15:30757

enode://948b52cd2b8123909dcc127785cc6b2e7a45ad577a9ca6cca6e236cb9290818cd8ff7d5e9c4c7cc32791fd8d94a0afcbf53172bcecbbd9c8a3b599b4b0edef1a@167.179.96.193:30757

enode://cb067e7a5499234ae03c7d752b618ec4ec6c1fc0a77ed6a68b552bd590d8641d2a8e894253ebef714118bf8815b401fe25120ca0b560dd9a29fb7248e12f952f@64.176.72.221:30757

enode://7b392e35d6c20276500deefdbb388913920aa599f97297b24a06125fad3589c351cef4e51a2c5fd3c3e733104d53071ac7c25f1734682aaa1af95ac22f78b373@45.77.231.99:30757
```

### ⛏️ Start mining

```bash
./build/bin/geth --mine --miner.threads=4 --miner.etherbase=0xYourAddressHere
```

