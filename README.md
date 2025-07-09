
# Pharos Auto Bot (Testnet Learning Tool 🚀)

Yeh ek automation bot hai jo Pharos testnet pe kaam karta hai.  
Bot testnet wallet se automatically:
- 💧 Faucet claim karta hai  
- 🔁 Tokens transfer karta hai  
- 🔄 Swap karta hai (WPHRS ↔ USDC)  
- 🌐 Proxy & multi-wallet use karta hai (agar setup ho)

👉 Sirf educational aur testing ke liye bana hai.  
❌ Koi mainnet ya real wallet ka use allowed nahi hai.  
❌ Koi token promotion ya crypto-rikhav nahi kiya gaya hai.

---

## 🛠 Bot Setup Karne Ka Tarika

🔹 Step 1: Repo Clone Karo  
```
git clone https://github.com/RikhavSonowal/pharos-auto-bot.git
cd pharos-auto-bot
```

🔹 Step 2: Dependencies Install Karo  
```
npm install
```

🔹 Step 3: `.env` File Banao aur Configure Karo  
```
cp .env.example .env
```

`.env` file open karke likho:
```
PRIVATE_KEY_1=apka_testnet_private_key
RPC_URL=https://pharos-testnet-ka-rpc-url
```

⚠️ Kabhi bhi real wallet ka key mat daalna.  
✅ Sirf testnet wallet ka use karo.

---

## ▶️ Bot Start Karne Ka Tarika

Normal mode mein chalaane ke liye:
```
node index.js
```

---

## 🔁 Bot Ko Background Mein Run Karo (Forever)

Screen ke through background run:
```
screen -S pharosbot
node index.js
```

Detach karne ke liye:  
Ctrl + A fir D dabao

Wapas connect hone ke liye:
```
screen -r pharosbot
```

---

## 🧪 Extra Commands (Optional)

🧾 Private key se wallet address dekhne ke liye:
```
node -e "require('dotenv').config(); console.log(require('ethers').Wallet.fromPrivateKey(process.env.PRIVATE_KEY_1).address)"
```

🧪 Dry Run mode (TX sign nahi hoga):
```
DRY_RUN=true node index.js
```

---

## 🛡️ Crypto Rikhav Se Savdhaan ⚠️

"Crypto rikhav" ka matlab hota hai:
- 🐍 Fake token dikhake sell nahi hone dena
- 📩 Aapka private key manga jaye
- 🧃 Airdrop ya claim ke naam pe wallet empty kar dena
- 🔗 Fake swap / DEX ya phishing site dena

### ✅ Bachav ka tarika:
- 🔐 Sirf dummy testnet wallet ka use karo  
- 💾 Private key sirf `.env` file mein rakho, kabhi paste na karo  
- 📖 Har transaction ka meaning samjho, blindly sign mat karo  
- 🛑 Koi repo ya bot agar fees, token ya referral maange, use avoid karo  

Ye bot ek **learning tool** hai, na ki token ya paisa kamaane ka shortcut.  
Apne risk par testnet pe use karo — **mainnet use strictly mat karo**.

---

## 🙏 Dhanyavaad

Agar bot useful lage toh ⭐ zaroor dena.  
Apne doston ke sath bhi share karo jo testnet automation seekhna chahte hain.

```
Na main token bechta hoon,  
Na main rikhav karta hoon,  
Sirf testnet coding ka junoon hai 😄💻
```
