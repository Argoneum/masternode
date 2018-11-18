### **[Back to guide main site](readme.md)**

## Masternode Setup

Easiest way is to use our Argoneum masternode setup script, copy and paste this command and hit enter:
    
    sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/Argoneum/argoneum/master/contrib/masternodes/argoneum_masternode_install.sh)"
       
Script begins it's work and asks you if you want to **Install masternode and build environment**:

<img src="https://node-support.network/coins/argoneum/06_masternode_setup/1.png">

Bext question you will be asked is to enter a **masternode genkey**. You have 2 options to generate a masternode key:
    
1. Via Argoneum masternode setup script

    Hit enter and script creates a masternode genkey for you which you have to use for your local wallet masternode.conf (we'll get to that in next guide page)

2. Via your local deskop wallet

    To generate a masternode genkey, open **Debug console** in your wallet
    
    <img src="https://node-support.network/coins/argoneum/06_masternode_setup/2.png">
    
    enter **masternode genkey** in the command line
    
    <img src="https://node-support.network/coins/argoneum/06_masternode_setup/3.png">
    
    and the masternode genkey is generated
    
    <img src="https://node-support.network/coins/argoneum/06_masternode_setup/4.png">
    
Now copy your genkey and paste it to PuTTY SSH session and hit enter

<img src="https://node-support.network/coins/argoneum/06_masternode_setup/5.png">

script continues with work and after everything is done, you get all needed informations at the end

<img src="https://node-support.network/coins/argoneum/06_masternode_setup/6.png">

Keep this window open, or copy **VPS_IP:PORT** and **MASTERNODE PRIVATEKEY** to a text file.

### **[Continue to 7. Masternode start](mn_guide_masternode_start.md)**
