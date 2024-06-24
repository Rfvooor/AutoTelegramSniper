# AutoTelegramSniper
This is a (solana) telegram alerts sniper, allowing you to never miss a callout again!
Running 24/7 on your own server, keeping keys and your telegram msgs in your control. 
Currently only allows for sniping solana telegram alerts from raydium, but much is planned.

Features Roadmap:
  -  Pump(.)fun sniping
  -  Auto transfering post snipe
  -  Filtering alerts
  -  Take profit strategies
  -  Channel win rates
  -  Additional DEXs
  -  Additional chains
  -  Dynamic snipe amounts based on "risk"

There are no recurring/volume based fees, just a 1 time non-refundable activation fee starting at .75 SOL. 
This will be increasing by .25 with each update, however if you bought earlier you won't need to pay any additional fees.

Eventually once all updates are done, price will be frozen and the plan is to release an NFT pass that will be mintable at final price which all current users will recieve for free. 

# Setup 
Setup is a super simple process, taking at most 15-20 mins depending on technical ability. 
For any questions:
TG: https://t.me/+GwZPCWSKElxjNjY5 or DM me @rfvooor 
Twitter: https://x.com/rfvoooor

## Obtain bot equipment (5 mins)
Get a VM (virtual machine) from a provider such as AWS, Google, Heroku, Digital Ocean.
Many of these platforms provide free sign-up credits and so there shouldn't be costs related to this for a while.
(Would recommend digital ocean, very easy option and this guide wil focus on DO)
- Once signed into DO, you should see a button in the top that says "Create" and a dropdown menu should appear
- Click droplets
![Screenshot 2024-06-24 153405](https://github.com/Rfvooor/AutoTelegramSniper/assets/173009279/01c9df7b-93c5-4c01-a42b-aa8438f6ce37)
- Choose any location, Ubuntu with version 24.04 and the cheapest option under Basic should be good enough.
- Choose Password Auth if unfamiliar with SSH keys
- Click create
  
## Obtain the bot (1 min)
Once you have a VM, you're going to want to install Docker. 
There's many ways to do this but you can use the following command: ```sudo snap install docker```
Once docker is installed, you're going to want to download the bot from docker: ```sudo docker pull rfvoooor/telesolsniper:1```
Once downloaded you can run the bot: ```sudo docker run -t  telesolsniper```
    
## Setup the bot (10 mins)
If it is your first time running the bot you will be presented with a telegram login input. 
This information (along with your private keys!) are only stored on *your* VM and not accessible by anyone other than you or those you grant access to the VM. 
Once signed in, you will be prompted to validate you have an API key. This is done via a telegram bot (https://t.me/tas_apikey_bot). 
To activate the bot, DM the bot "/buykey" and it will guide you through the steps.

## Profit (???)
Once setup you will be presented with a menu allowing you to 
1. Add usernames or channels to snipe from
2. View/Change settings such as snipe amount, slippage etc
3. View your current private key
4. Turn the sniper on/off
5. Exit

And thats it! Once you are ready to start sniping send WSOL to the public key as seen in the settings and some SOL for fees.

## Feedback
I am very open to know what should be improved or what features you'd like to see.
Please put these here: https://github.com/Rfvooor/AutoTelegramSniper/issues
Or, if you aren't a github user, DM me on any of my socials and I'll add it!
