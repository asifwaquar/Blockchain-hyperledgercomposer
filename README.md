# Blockchain-Hyperledger Composer
We are going to setup Hyper-ledger Composer Playground with some examples.

### Hyperledger Composer Installation

 cd $HOME
 curl -O -k https://hyperledger.github.io/composer/latest/prereqs-ubuntu.sh
 chmod u+x prereqs-ubuntu.sh
 
 ### run the command to install the:
 
  sudo apt-get install -y software-properties-common
 
 [![image]](https://miro.medium.com/max/553/1*EJT5Y64NLeXFA8Zu16vd6g.png)
 
 ### Install Required Components
 
   npm install -g composer-cli@0.20
   npm install -g composer-rest-server@0.20
   npm install -g generator-hyperledger-composer@0.20
   npm install -g yo

### Install Playground

 npm install -g composer-playground@0.20
 
### Install Hyperledger Fabric

Create a directory fabric-dev-servers at your home directory.

 mkdir ~/fabric-dev-servers && cd ~/fabric-dev-servers
 
And run curl command to download the tool and unzip it.

  curl -O https://raw.githubusercontent.com/hyperledger/composer-tools/master/packages/fabric-dev-servers/fabric-dev-servers.tar.gz
  tar -xvf fabric-dev-servers.tar.gz
  
 ### Download the runtime:
 
  export FABRIC_VERSION=hlfv12
 ./downloadFabric.sh

### Running on the First Time

    cd ~/fabric-dev-servers
    export FABRIC_VERSION=hlfv12
   ./startFabric.sh
   ./createPeerAdminCard.sh
   
    [![image]](https://miro.medium.com/max/700/1*c30OC-_LfLff1ueYjm-5-Q.png)

### To stop, run this command:
  ~/fabric-dev-servers/stopFabric.sh
  
 ### Start the Playground
 
   composer-playground
   
   [![image]](https://miro.medium.com/max/700/1*X9Is0z2ogFkDGJu1cRrB7A.png)
   
   
