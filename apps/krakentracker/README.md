# Adding your project to KrakenTracker

## The easy way
Submit your listing to this form: [link]

The devs will take your info and manually add the listing for you. As this is a manual process, it may take some time to get to, but is the easiest for you.

## The fast way

### Adding to the list
Fork this repo.

go to `assets/apps/krakentracker` and modify the correct token list json, with the correct chain your project is on, i.e. _bnb or _eth

Add your token's information to the bottom of the "tokens" array.

**contract_address**: the contract addresses are case-sensitive, meaning you need to provide the proper checksum version of your contract address

Example - BabyKrakens SRG20 Token on ETH:

- Checksum: `0xF654d4C3CC334324ad474A0d5d3708dCA4c1CB25`
- Lowercase: `0xf654d4c3cc334324ad474a0d5d3708dca4c1cb25`

_a_ is not equal to _A_, it is import that you use the correct one

### Adding your logo

Coineus Assets is used across multiple applications. Token logos are stored in one location for all those apps to use.

The pattern is https://coineus.app/assets/tokens/{chain}/{contract_address}/logo.png

example: https://coineus.app/assets/tokens/fuse/0x4e69Ae0CD024754655b4eF74F24A8DCB39Ba07e8/logo.png

This allows any application on the internet to get a token's logo using this url template.

Go to assets/tokens/{chain} and create a folder using the checksum version of your contract address.

Add your logo file in that directory.
- It **MUST** be a PNG file
- It **MUST** be named `logo.png` 
  - not logo.PNG 
  - not Logo.png 
  - not logo.png.png
- It **SHOULD** be 192x192 in size. 

Submit a Pull Request for your token to be included. Team will review and with the click of a button on our side, be added to KrakenTracker.