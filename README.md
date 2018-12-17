# NDO Masternode Setup Guide

# Linux Installation Portion
1. Install an Ubuntu 16.04 LTS Server
2. Copy and paste the following line in your VPS:
```git clone https://github.com/project-nodeo/ndo-mn.git && cd ndo-mn && bash ndo-mn.sh```
3. Please follow all prompts closely and enter ```y``` if this is your first time installing NDO
4. You will be provided with your IP address and private key at the end of the installation process

# Wallet Portion and Funds
1. Go to your debug console in the Nodeo wallet by going to Tools -> Debug Console
2. Generate a new address with ```getaccountaddress mn1```
3. Send exactly #### NDO to this newly generated address
4. After the transaction has confirmed, find your tx output and ID from the Debug Console with ```masternode outputs```
5. Use your IP address given with your private key, tx ID and tx output number for the masternode config
6. Go to Tools -> Open Masternode Configuration File
7. Enter the information in the following format on a single line
```mn1 127.0.0.1:41960 93HaYBVUCYjEMeeH1Y4sBGLALQZE1Yc1K64xiqgX37tGBDQL8Xg 2bcd3c84c84f87eaa86e4e56834c92927a07f9e18718810b92e0d0324456a67c 0
```
8. Save this file and restart your wallet

# Starting Masternode
1. Wait for your transaction to have 16 confirmations prior to starting the masternode remotely
2. Go to the Masternodes page in your wallet
3. Right click your masternode and click Start alias
4. Congratulations!
