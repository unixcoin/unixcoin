
About Unixcoin
===========================
Unixcoin is a cryptocurrency,It’s owned and operated by PayCash Europe S.A, LUXEMBOURG. PayCash Europe S.A authorized by Financial Conduct Authority (FCA) under the Electronic Money Regulations 2011 for the issuing of Electronic Money & Provide Payment Services, Reg No-900554. As a fully licensed service, all transaction are protected under industry standards.

Development process
===========================
New Pool: http://node.unixcoin.com
Block Explorer: http://block.unixcoin.com:2750/chain/Unixcoin

Official Details
===========================
Official Website:
http://www.unixcoin.com
Official Facebook Page: https://www.facebook.com/unixcoin
Official Twitter Page: https://twitter.com/unix_coin
Official Google+ Page: https://twitter.com/unix_coin

UNIXCOIN STEP BY STEP COMPILING GUIDE
Below ARe full details of compiling unixcoind:
Step-1:
#sudo apt-get update
#sudo apt-get upgrade

Step-2
#sudo apt-get install build-essential libssl-dev libdb-dev libdb++-dev libboost-all-dev git libssl1.0.0-dbg
#sudo apt-get install libdb-dev libdb++-dev libboost-all-dev libminiupnpc-dev libminiupnpc-dev libevent-dev libcrypto++-dev libgmp3-dev

Step-3
#git clone https://github.com/unixcoin/unixcoin.git
#cd unixcoin/src
#make –f makefile.unix USE_UPNP=-
#strip unixcoind
#sudo cp unixcoind /usr/bin

Final Step-4
#cd /usr/bin
#./unixcoind


If error shows on compiling unixcoind:
"src/leveldb/libleveldb.a: No such file or directory
/src/leveldb/libmemenv.a: No such file or directory"

Solution:
#cd leveldb
#chmod 755 *
#cd

and compile again
#cd unixcoin/src
#make –f makefile.unix USE_UPNP=-
