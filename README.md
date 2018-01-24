BBCashCoin (BBX)
===========


The BBCASHCOIN Source Code for Daemon 

COMPILE INSTRUCTION:
-----------------------

Ubuntu 14.04 LTS

sudo apt-get install build-essential<br>
sudo apt-get install libssl-dev

Boost 4.8
----------
wget 'http://download.oracle.com/berkeley-db/db-4.8.30.NC.tar.gz'<br>
tar -xzvf db-4.8.30.NC.tar.gz<br>
cd db-4.8.30.NC/build_unix/<br>
../dist/configure --enable-cxx --disable-shared --with-pic --prefix=/home/your_username/your_path/<br>
make install

libdb4.8
----------
sudo add-apt-repository ppa:bitcoin/bitcoin<br>
sudo apt-get update<br>
sudo apt-get install -y libdb4.8-dev libdb4.8++-dev<br>


sudo apt-get install libboost-all-dev (1.5.x)<br>
sudo apt-get install libqrencode-dev

optional miniupnpc
--------------------
http://miniupnp.tuxfamily.org/files/<br>
tar -xzvf miniupnpc-1.6.tar.gz<br>
cd miniupnpc-1.6<br>
make<br>
sudo su<br>
make install

Compile & run
----------------
make -f makefile.unix USE_UPNP=- USE_IPV6=1 BDB_INCLUDE_PATH='/usr/include/db4.8'<br>
strip bbcashcoind<br>
./bbcashcoind (src ordner)

Configuration
-------------
Add rpcuser, rpcpassword & nodes @ conf 
/home/your_username/.bbcashcoin/bbcashcoin.conf

Nodeserver:<br>
23.95.214.101 <br>
23.95.11.84

 
 
