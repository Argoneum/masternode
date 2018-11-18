### **[Back to guide main site](readme.md)**

## Collateral
To run a masternode, you need to send 10000 AGM coins to a new generated wallet.

1. To generate a new wallet address, open your wallet and goto **File** -> **Receiving addresses...**

    <img src="https://node-support.network/coins/argoneum/04_collateral/1.png">
    
    a new window will open, click on button **New**
    
    <img src="https://node-support.network/coins/argoneum/04_collateral/2.png">

    enter a label for your new wallet (I use mn0X for my masternode wallets) and click on button **OK**

    <img src="https://node-support.network/coins/argoneum/04_collateral/3.png">

    now you see your new generated wallet address in **Receiving addresses** overview

    <img src="https://node-support.network/coins/argoneum/04_collateral/4.png">
    
    copy the wallet address to go forward to next step

2. Send 10000 AGM coins to new wallet address

    Open tab **Send**, enter your new created wallet address in field **Pay To:**, the amount of 10000 AGM coins in field **Amount** and    hit the button **Send**
    
    <img src="https://node-support.network/coins/argoneum/04_collateral/5.png">
    
    a new window opens to enter your wallet password
    
    <img src="https://node-support.network/coins/argoneum/04_collateral/6.png">
    
    after entering your wallet password you will be asked if you confirm to send your coins
    
    <img src="https://node-support.network/coins/argoneum/04_collateral/7.png">
    
    after you confirmend you can you your transaction in your main wallet window.
    
    <img src="https://node-support.network/coins/argoneum/04_collateral/8.png?">
    
    Now you need to wait for 15 confirmations to get your collateral tx & collateral txid.\
    **After 15 confirmations**, open debug console (goto **Tools** -> **Debug console**) and enter
    
    `masternode outputs`
    
    you will see your collateral tx/txid output, like:
    
    `"2efe1f70c61f9e44c0d12e763e461afd6b0cec2f234745b04a82e53d0eef3788": "1"`
    
    which is needed for masternode.conf (will be needed later for wallet configuration)\
    Copy this collateral tx/txid to a text file

### **[Continue to 5. VPS & Masternode setup](mn_guide_create_vps.md)**
