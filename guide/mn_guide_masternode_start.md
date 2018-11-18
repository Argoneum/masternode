### **[Back to guide main site](readme.md)**

## Masternode start

To start your masternode, open your wallet and goto **Tools -> Open Masternode Configuration File**

<img src="https://node-support.network/coins/argoneum/07_masternode_start/1.png">

Notepad opens the masternode.conf file and you see an example how to add a complete entry for masternode:

<img src="https://node-support.network/coins/argoneum/07_masternode_start/2.png">

now we need to add some informations in this file:
1. Masternode alias\
    You can choose a masternode alias name yourself (e.g. mn01)
    
2. IP-Address:port\
    IP-Address of your VPS and Argoneum predefined port 9898

3. masternode genkey\
    Masternode genkey which was generated via setup script, or via local desktop wallet

4. Collateral tx / txid\
    Collateral tx / txid which you get via wallet debug console

All informations should be added **in one line** to masternode.conf as you can see my example:

`mn01 95.179.156.105:9898 92bMhjrGjiwDb42M75bGzLcCLdDZ9sSLi63TR29E7BTVDX43y3d 2efe1f70c61f9e44c0d12e763e461afd6b0cec2f234745b04a82e53d0eef3788 1`

<img src="https://node-support.network/coins/argoneum/07_masternode_start/3.png">

**Save the masternode.conf file**, close and start your wallet again. Goto **Settings -> Options -> Wallet and enable Show Masternodes Tab** and hit **OK** button

<img src="https://node-support.network/coins/argoneum/07_masternode_start/4.png">

Now goto **Masternodes** tab and you should see one entry\
**Note: I use here a different Port, beacause I'm on our testnet. You need to use Port 9898 !**

<img src="https://node-support.network/coins/argoneum/07_masternode_start/5.png">

to start the masternode select the entry and hit **Start Alias** button

<img src="https://node-support.network/coins/argoneum/07_masternode_start/6.png">

you will be asked if you want to start masternode, just hit **Yes** button

<img src="https://node-support.network/coins/argoneum/07_masternode_start/7.png">

you get a confirmation that masternode is successfully started

<img src="https://node-support.network/coins/argoneum/07_masternode_start/8.png">

status of masternode in **Masternodes** tab will change to **WATCHDOG_EXPIRED**

<img src="https://node-support.network/coins/argoneum/07_masternode_start/9.png">

after ~ 30 mins masternode status should change to **ENABLED**

<img src="https://node-support.network/coins/argoneum/07_masternode_start/10.png">

Finally your masternode is started and activated. If you have any issues, feel free to contact us.
