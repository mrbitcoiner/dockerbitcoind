# Dockerized Bitcoind
## Run your bitcoin node from source on multiple architectures with a few commands

* Tested on aarch64 and x86_64
* Keeping only the last 10GB of timechain in the default mainnet config. You can override this changing the main (or regtest) configuration files.
* For fast sync, proxying bitcoin connections through tor is disabled by default. Check the main configuration file to change this behavior.

### Check (or change) the configurations
```
vi containers/bitcoind/volume/config/main
```

### Start:
```
./control.sh up
```

### Stop:
```
./control.sh down
```

### Clean data:
```
./control.sh clean
```
