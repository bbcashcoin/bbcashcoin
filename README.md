BBCashCoin (BBX)
===========


The BBCASHCOIN Source Code for Daemon 

COMPILE INSTRUCTION:
-----------------------

Ubuntu 14.04 LTS

sudo apt-get install build-essential
sudo apt-get install libssl-dev

Boost 4.8
----------
wget 'http://download.oracle.com/berkeley-db/db-4.8.30.NC.tar.gz'
tar -xzvf db-4.8.30.NC.tar.gz
cd db-4.8.30.NC/build_unix/
../dist/configure --enable-cxx --disable-shared --with-pic --prefix=/home/your_username/your_path/
make install
----------

libdb4.8
----------
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev
---------

sudo apt-get install libboost-all-dev (1.5.x)
sudo apt-get install libqrencode-dev

optional miniupnpc
--------------------
http://miniupnp.tuxfamily.org/files/
tar -xzvf miniupnpc-1.6.tar.gz
cd miniupnpc-1.6
make
sudo su
make install

Compile & run
----------------
make -f makefile.unix USE_UPNP=- USE_IPV6=1 BDB_INCLUDE_PATH='/usr/include/db4.8'
strip bbcashcoind
./bbcashcoind (src ordner)

Configuration
-------------
Add rpcuser, rpcpassword & nodes @ conf 
/home/your_username/.bbcashcoin/bbcashcoin.conf

Nodeserver:
23.95.214.101
23.95.11.84

