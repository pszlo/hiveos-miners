# minershive
Custom miners integration to Hive OS

Donate:

BTC: 34BdxtsApDAgUKHUvqxKUoA17VeKYBt2Kw
Etherium: 0x0509Fc09d1a237bffc5382E62d1Aa900bC7D913a
ETC: 0xcd2c58eced4f54dc9450f85d396867d638301a40


# Custom miner integration in Hive OS

You can integrate any miner to Hive. 
For this need to implement several scripts which will be callbacks for Hive scripts. 
Other miners implementations are good points to start your own.

All files should be stored in `/hive/custom/mysuperminer` folder. Don't forget about execute permission for `.sh` files.

`CUSTOM_MINER` - this variable in wallet.conf will hold currently selected miner, like `mysuperminer`. 

##### h-manifest.conf
This is a general config for Hive, not for the miner.
```bash
# The name of the miner like "mysuperminer" 
CUSTOM_NAME=
# Optional version of your custom miner package
CUSTOM_VERSION=
# Full path to miner config file, e.g. /hive/custom/mysuperminer/mysuperminer.json
CUSTOM_CONFIG_FILENAME=
# Full path to log file basename. WITHOUT EXTENSION (don't include .log at the end)
