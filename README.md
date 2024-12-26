# Bitcoin Mining
## Setup
Connect and log into the docker Ubuntu 24.10 Linux container with the user created in [Docker Setup](https://github.com/lley154/docker-setup).

In the terminal window, run the follwing commands
```
$ sudo apt update
$ sudo apt install git
$ sudo apt install build-essential
$ sudo apt install automake autoconf libtool
$ sudo apt install libssl-dev
$ sudo apt install libcurl4-openssl-dev
$ git clone https://github.com/lley154/cpuminer-multi
$ cd cpuminer-multi/
$ ./build.sh 
$ ./cpuminer --help
```
## Running the Miner
Use the mining pool worker user & pass provided in class.
```
$ ./cpuminer -a blake2b -o stratum+tcp://btc.f2pool.com:1314 -u user -p pass --debug --protocol-dump
```

