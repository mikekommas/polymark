# Polymarket_AI_M3_Trading_Bot 🚀

The **Polymarket AI M3 (Multi-Model Meta)** bot is a specialized high-speed execution suite designed to replicate the trades of top-tier professional traders in real-time. By monitoring specific "Smart Money" wallet addresses on the blockchain, the bot executes identical positions for your account within milliseconds of the target.

## 📈 How It Works

  *  **Target Mirroring:** You provide a specific wallet address to follow. The bot polls the Polymarket Data API specifically for that user's activity.

   * **In-Memory Tracking:** The bot maintains a local session state to ensure it only copies a specific transaction once, preventing duplicate orders.

   * **Direct CLOB Integration:** Trades are executed directly through the Polymarket Central Limit Order Book (CLOB) for the lowest possible latency.

   * **Automatic Auth Handshake:** The system performs a secure L2 API handshake upon startup to ensure your session is authenticated and ready for high-frequency execution.

## 🛠 Prerequisites (Step 1)

Before running the bot, you must have **Node.js** installed on your computer.

1. **Download:** Go to [nodejs.org](https://nodejs.org/) and click the **"LTS"** version button.
2. **Install:** Run the installer and click "Next" on all prompts.
3. **Verify:** Open your terminal/command prompt and type `node -v`. If it shows a version number, you are ready.

---

## 📥 Installation (Step 2)

### Option A: Git Clone (For Developers)

```bash
git clone https://github.com/YourUsername/Polymarket_AI_M3_Trading_Bot.git
cd Polymarket_AI_M3_Trading_Bot

```

### Option B: Download ZIP (For Non-Developers)

1. Click the green **"<> Code"** button at the top of this GitHub page.
2. Select **"Download ZIP"**.
3. Extract the ZIP file to your **Desktop**.

---

## 🚀 Setting Up the Bot (Step 3)

### 1. Open the Terminal

* **Windows:** Press the `Win` key, type **"cmd"**, and press Enter.
* **Mac:** Press `Cmd + Space`, type **"Terminal"**, and press Enter.

### 2. Enter the Folder

Type `cd` followed by a space, then **drag and drop** the bot folder from your desktop into the terminal window. It should look like this:

```bash
cd C:\Users\YourName\Desktop\Polymarket_AI_M3_Bot

```

Press **Enter**.

### 3. Install Requirements

Copy and paste this command into the terminal and press Enter:

```bash
npm install

```

### 4. Configure Your Key

Rename the file .env.example to .env. Open it with Notepad or any text editor and paste your Private Key in PRIVATE_KEY. 
Also, input the address you will be copy trading in COPY_ADDRESS.

---

## 🔑 How to Get Your Private Key

To trade programmatically, the bot requires your **L1 Private Key**.

### If you use Email / Google (Magic Link):

1. Go to the official reveal page: [https://reveal.magic.link/polymarket](https://reveal.magic.link/polymarket)
2. Log in with your Polymarket email.
3. Click **"Reveal Private Key"** and copy the string starting with `0x`.

### If you use MetaMask:

1. Open MetaMask and select your Polymarket account.
2. Click **Account Details** > **Export Private Key**.
3. Enter your password and copy the key.

---

## ⚡ Starting the Bot (Step 4)

Once your `.env` file is saved with your key, run:

```bash
node src/index.js

```

The bot will now begin scanning the CLOB for profitable opportunities.

---
