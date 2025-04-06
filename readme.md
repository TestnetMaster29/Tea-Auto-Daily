Sure! Here's the English translation of your `README.md` for **Skydash.NET - Auto Transfer Token on TEA Sepolia**:

---

# 🚀 Skydash.NET - Auto Transfer Token on TEA Sepolia  
![GitHub repo size](https://img.shields.io/github/repo-size/adryan089/aet-auto?style=flat-square)  
![GitHub stars](https://img.shields.io/github/stars/adryan089/aet-auto?style=flat-square)  
![GitHub forks](https://img.shields.io/github/forks/adryan089/aet-auto?style=flat-square)  
![GitHub license](https://img.shields.io/github/license/adryan089/aet-auto?style=flat-square)  

> **By using this script, you understand and accept any risks that may occur.**  
> **Thanks to clwkevin! for the wallet database** 💙  

---

## ✨ Main Features  
✅ Auto Transfer Custom Tokens  
✅ Auto Transfer TEA Native Token  
✅ Max transaction limit of 98–150 times per day  
✅ Automatic pause & restart at 00:00 UTC / 07:00 WIB  
✅ Random delay between transactions for safety & anti-bot detection  
✅ Destination address is automatically fetched from external sources  
✅ Randomized amount of tokens per transaction  
✅ Supports multiple wallets and multiple contract addresses  
✅ Telegram Bot notifications (optional)

---

## 📌 Requirements  
Before running the script, make sure you have:  
- **Node.js** v18+ ✅  
- **NPM** ✅  
- **Wallet funded with Faucet TEA** ✅  
- **Wallet with deployed token** ✅

---

## 🔧 Installation Guide  
1️⃣ **Clone the repository**  
```bash
git clone https://github.com/TestnetMaster29/Tea-Auto-Daily.git
cd Tea-Auto-Daily
```

2️⃣ **Install dependencies**
```bash
npm install
```

3️⃣ **Configure Wallet**
```bash
cp wallets.json.examples wallets.json
```
Then edit the `wallets.json` file and fill in your wallet and token data:

**Example for a single wallet:**
```json
[
  {
    "PRIVATE_KEY": "your_private_key",
    "TOKEN_ADDRESS": "your_token_contract_address"
  }
]
```

**Example for multiple wallets:**
```json
[
  {
    "PRIVATE_KEY": "private_key_1",
    "TOKEN_ADDRESS": "token_contract_address_1"
  },
  {
    "PRIVATE_KEY": "private_key_2",
    "TOKEN_ADDRESS": "token_contract_address_2"
  }
  // and so on...
]
```

4️⃣ **Configure Telegram Bot (Optional)**

To get automatic notifications via Telegram:

- Create a new bot using [@BotFather](https://t.me/BotFather) and copy its token.
- Get the `chat_id` of the user or group, using a bot like [@userinfobot](https://t.me/userinfobot).
- Create a new file named `.env` and fill it with:
```bash
BOT_TOKEN=your_bot_token
CHAT_ID=your_chat_id
```
- Save this file in the root project folder.

If the `.env` file is not found, the script will still run but without notifications.

---

## 🚀 Run the Script

```bash
node main.js
```

---

## 📜 License

This project is licensed under the MIT License.

```
MIT License

Copyright (c) 2025 Skydash.NET

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

Let me know if you'd like help making this into a proper `README.md` file or turning it into a GitHub landing page!