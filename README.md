# Mod19Chall
This is a project in which I create an app through which you can make an ether transaction to someone [streamlit](https://github.com/streamlit/streamlit) application. This works in connection with the application [Ganache](https://trufflesuite.com/ganache/) which allows you to fire up a personal Ether blockchain. You must install and setup a block chain on Ganache for this app to work.

## Technologies
The following packages were used:
pandas
hashlib
datetime
typing
bip44
mnemonic
dotenv
web3==5.17
os
requests
streamlit

## Installation
Various packages must be installed to run this code. I recommend using `pip install --package name--` to install

For example, to install streamlit, in your terminal run:

`pip install streamlit` and follow any direction prompts.
`pip install web3==5.17`
`pip install mnemonic`
`pip install eth-tester==0.5.0b3`
`pip install bip44`


## Usage

### Code
Code is found in [fintech_finder.py](https://github.com/wcolwellcol/Mod19Chall/blob/main/fintech_finder.py) which imports various functions from [crypto_wallet.py](https://github.com/wcolwellcol/Mod19Chall/blob/main/crypto_wallet.py). Note, the embedded streamlit commands (denoted by `st.[something]`) which enables deployment. To use the app, you will have to create your own `.env` file and set a MNEMONIC variable equal to the mnemonic listed on the top left of your Ganache app blockchain.

### Run the App
With your terminal, navigate to the folder that holds the pychain.py app. Run the script in the terminal with the command `streamlit run fintech_finder.py`

A page should automatically open in your web browser where the app is deployed.

To use the app, select the person you want to pay from the drop down in the sidebar. Then input the amount of hours of work you are paying the person for. A wage should be calculated automatically in Ether. To send a transaction, simply click the Send Transaction button

You can verify that the transaction went through in ganache. I have included evidence of a transaction of 1.9 Ether sent to Jo in my [Evidence](https://github.com/wcolwellcol/Mod19Chall/tree/main/Evidence) folder. There are various screenshots that illustrate that my app worked.
