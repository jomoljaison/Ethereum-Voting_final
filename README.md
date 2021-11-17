

1. Clone this repository

   ```shell
   git clone git@github.com:jomoljaison/Voting_final.git
   cd Voting_final
   ```

1. Run local Ethereum blockchain

   ```shell
   ganache-cli
   ```

   > Note: Do not close `ganache-cli` (the blockchain network needs to be running all the time)

1. Configure metamask on the browser with following details

   New RPC URL: `http://localhost:8545`  
   Chain ID: `1337`

1. Import accounts using private keys from ganache-cli to the metamask extension on the browser
1. Deploy smart contract to the (local) blockchain

   ```shell
   # on the Voting_final directory
   truffle migrate
   ```

   > Note: Use `truffle migrate --reset` for re-deployments

1. Launch the development server (fronted)

   ```shell
   cd client
   npm install
   npm start
   ```

