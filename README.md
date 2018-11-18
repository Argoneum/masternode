# IMPORTANT:
> This script and repository are forked from Argo. The guide can be used as a reference, but script must be revised. It does not suport most features of the new one (visible install, daemon log rotation, sentinel, the final screen, multiplatform support). Please use the officially supported automated masternode install script from release notes: https://github.com/Argoneum/argoneum/releases

------------


# Masternode guide and script files related to Argoneum masternode

Welcome to our Argoneum masternode repository. Here you find guides like how to update your running masternode, how to setup a new masternode and some hints how to fix issues, which we heard about from our community.

## Installing Argoneum masternode:

To install a new Argoneum masternode (including updates and sentinel), just download our script and execute it and follow steps showed in script.

**Important:** Run this script as **_root_**, if you plan to run this script as non-root user, it may fails!\
**Our script is tested on Ubuntu 16.04, 17.10, 18.04 and 18.10**

`sudo bash -c "$(curl -fsSL https://raw.githubusercontent.com/Argoneum/argoneum/master/contrib/masternodes/argoneum_masternode_install.sh)"`

## Issue with Wallet status **_WATCHDOG_EXPIRED_**

If you continue to occurs WATCHDOG_EXPIRED error, check the following:  
`argoneum-cli mnsync status | grep IsSynced`
  
    "IsSynced": true,
  
`argoneum-cli masternode status | grep status`
  
    "status": "Masternode successfully started"
  
`cd ~/argoneum-sentinel/` \
`./venv/bin/py.test ./test`
  
    ===== 23 passed in 0.25 seconds =====
  
`./venv/bin/python bin/sentinel.py`
  
    There should be NO ERROR.
  
  
If there are **no errors**, please wait about 20 minutes.  
After 20 minutes, "WATCHDOG_EXPIRED" will change to "ENABLED". 
