# THEWALLETBOT manual      
Cryptocurrency wallet based on instant communicators.      
## Notes:      
* Set up your nickname at Telegram. You will be able to receive payments by giving your @nickname  to your counterparty.      
* This is just test software. Alpha, beta or however you want to call it. As a tester you will get some TESTNET BITCOINS each few hours. Remember - they are worth ZERO.      
## Commands for everybody, for non-users as well:      
### <strong>help [command]</strong>      
Displays more detailed help about chosen command.      
      
### <strong>rates [coin]</strong>      
Displays the current rates for all cryptocurrencies supported by <a href="http://thewalletbot.com/">TheWalletBot</a> or just the rates for a chosen coin.      
examples: _rates | rates LTC | rates BTC_      
      
### <strong>coins</strong>      
Displays coins currently supported by <a href="http://thewalletbot.com/">TheWalletBot</a>.      
      
### <strong>start [coin]</strong>      
Creates a new wallet for the chosen coin. BTC is the default. You must have a BTC wallet as your first one. Only with the BTC wallet activated, can more coins be added. When your wallet is created, you will be assigned a new address. The QR code and blockchain link will be displayed alongside. This is a one-off operation. To change your address, you should use the <strong>new address [coin]</strong> command.      
examples: _start | start LTC | start BTC_      
      
## Commands for users only:      
### <strong>show [coin]</strong>      
Displays your address for the chosen coin with the QR code and blockchain link. You can use the QR code to receive payments, i.e. from a phone. BTC is the default.      
examples: _show | show LTC | show BTC_      
### <strong>balance [coin]</strong>      
Displays the balance for the chosen coin. If a coin name is omitted, balances for all addresses of your coins will be shown.      
examples: _balance | balance LTC | balance BTC_      
### <strong>send address amount coin</strong>      
Sends the specified amount of coins to the recipient. BTC is the default. The amount must be less than your balance. The recipient can be stated as a:      
- valid address for the chosen coin (i.e. 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB),      
- Telegram nickname (i.e. @NickNameOfFriend), or      
- full phone number as on Signal (+446011234567).      
For any existing recipient that is on a specific instant messenger, even if they are not a TheWalletBot client, a new wallet and address of the chosen coin will be created. So, the funds sent will be delivered, and the recipient will be informed. If the transaction is successful, you will get a link to the transaction at blockchain.      
Donâ€™t forget the transaction fee. You have to pay it to the network. The sufficient balance is needed in your account to pay this. If you want to send the whole balance, enter the <strong>send address all coin</strong> command. The relevant fee will be deducted from your balance.      
Examples of standard send commands:      
<strong>send 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB 1.2 BTC      
send @NickNameOfFriend 32 LTC      
send +446011234567 all ETH</strong>      
      
### <strong>new address [coin]</strong>      
Creates a new address for the chosen coin. BTC is the default. The whole balance (less only the transaction fee) of your old address is sent to the new one. For the transaction to be successful, you must have sufficient balance to pay the transaction fee. If your balance is zero, a new address will be created for you, and no send transaction will be effected, so there will be no fee for this.      
examples: _new address BTC | new address LTC_      
      
### <strong>forward [coin {address | cancel}]</strong>      
Displays, sets or cancels forwarding of all coins. The coin name is required. No default value. Only a valid coin address can be used here. Examples of standard use of this command:      
<strong>forward</strong> - displays all your existing forwards.      
<strong>forward BTC 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB</strong> - sets a new forward for the chosen coin (BTC). From that moment all funds incoming to your address for this coin will be sent (every 10 minutes) to the specified address.      
<strong>forward BTC cancel</strong> - cancels any previously set forward.      
      
### <strong>mix [coin]</strong>      
Mixes your coins. No default value. Not all cryptocurrencies can be mixed. Mixing is a process of coin anonymization. You will receive different coins at the new address to replace your existing coins. This will prevent anyone from knowing where you got your coins from and what you do with them. It costs some % + transaction fee. For now, it is possible to mix testnet bitcoin (BTC) [fee: 1% + transaction fees]\nlitecoin (LTC) [fee: 3% + transaction fees]      
Remember, your mixed coins will come to your new address.      
examples: _mix LTC | mix BTC_      
      
### <strong>history [coin] [number]</strong>      
Displays your transaction history. The default number is 10. If no coin name is entered, transactions for all your coins will be listed. If any additional information (sender, recipient, transaction type - forwarding or mixing) is available, it will be listed too.      
examples: _history | history LTC | history BTC 5_      
      
## Commands to configure your account:      
      
### <strong>email [email_address]</strong>      
Displays, sets or updates your email address for notifications and account recovery. If you lose access to your phone or instant messenger, this will be the only way to contact us, confirm your identity and recover your account. Just send us an email from the registered email address and we will contact you for further verification. The command with no email entered displays the valid email. To change your email, just set a new one.      
examples: _email | email your_nick@your_domain.com_      
      
### <strong>fee [low | normal | high]</strong>      
Displays, sets or updates the transaction fee. The more you pay â€“ the faster your transaction is confirmed. <strong>normal</strong> is the default.      
examples: _fee | fee low_      
      
### <strong>lang [pl | en]</strong>      
Displays, sets or updates your preferred language. All commands - are always in English. Descriptions and help files are multilingual so you can choose. The command itself, with no language parameter entered, displays the valid language.      
examples: _lang | lang en_       
      
