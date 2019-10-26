# How to create and edit a bot in Discord
## In this tutorial I'm going to show how to make an own interactive bot that works with some few commands.
<p align="center">
  <img src="https://miro.medium.com/max/1838/1*L613vjPIEp0o2TeZnEbg0w.jpeg" width="50%" height="50%"/></p>

Discord is a Skype/Whats-app social media app like that brings gamers together. They can have an own channel, check which game each friend is playing, call each other and chat with each other. One of the possibilities is to add a bot to the server. This can either be an automated bot, or a bot that plays music for example. The possibilities for a bot is endless in fact, because you can program the bot how you want. All the commands you give to the bot are in JavaScript. So if you're handy with JavaScript, you can program the bot just the way you want them to be a bot!

## Prerequisites:
- Internet ofcourse (doh!)
- Discord app
- Node.js & npm
- Basic knowlegde of executing commands in Terminal


## Step 1: Download the Discord App & create an account
### 1.Download the Discord app
This app is a multi-device app that can be downloaded from https://discordapp.com

### 2. Create an account
The username you create has a unique number to it attached, seen as the picture below.
<p align="left">
<img src="https://cvws.icloud-content.com/B/ATowdPt17A8PUox68fbKkDZC43s2AckEmyfFj94KE8GPqAcLN7bh0tyq/Screenshot+2019-10-16+at+11.51.55.png?o=AlKmUA0qsR3qZfjqA38tA8Wny_g5ujA3CXahzrvc9SGK&v=1&x=3&a=CAogDmDZBrYjh5h-EL5QlplTJyPjABcBWfmfYcV4NqWpT_kSHRCw8qjz3i0Y0Onf894tIgEAUgRC43s2WgTh0tyq&e=1571663901&k=w2BW8rH-hS2Rkq5q82JSSg&fl=&r=a86effdb-6698-4fc5-a421-3d47b7e71e4a-1&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=52&s=XAxbmtGI-ca_-7QuMt-7I8NS7JI&cd=i" width="20%" height="20%"/></p>

## Step 2: Setting Up Your Own Channel
In order for the bot to be created, we have to make our own server.

### 1. Login to discord
When you are logged into Discord you should see something like this:

<p align="center">
<img src="https://cvws.icloud-content.com/B/AfWkk3-OS5MptLh6RbL_tmm0oYySASER5LhKOGM-AEizAAVg9irpALEC/Screenshot+2019-10-16+at+11.55.13.png?o=At1XYnvPd8u7ssjPhF4zRixOy8TOK_CsCrThhmxNn2O5&v=1&x=3&a=CAogJ6Eg9thPWgwd18Ljw7u7fd08px4HLkIlrXgZEeayBNwSHRDb9Y_13i0Y--zG9d4tIgEAUgS0oYySWgTpALEC&e=1571667687&k=rnSuzGQfAdFzCNnFzs6kgA&fl=&r=8c15db3a-397e-41eb-bfef-c945e14580c9-1&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=52&s=Kggs8Rszs3fZ1g3PKN2qZMMvlRQ&cd=i"/></p>

### 2. Create a server
For the server to create, we have to click the '+' in the bottom left corner highlighted in red.

Give your server a name and enter the server region. Optionally you could add an image to your server. Once you completed these steps, you should see the server listing.

<p align="center">
<img src="https://cvws.icloud-content.com/B/AVmH7LZQCSgeucARqroxx6lEXf_zAb2l8NaYSBO5251cvXsgYHPFK2en/Screenshot+2019-10-16+at+12.08.44.png?o=AjnaFnt4z5M03JIB-sOTLAmG9wDlzYavwBul9fG1XfAA&v=1&x=3&a=CAogaKythc2GH7mkex9I7BQHf33pQvlzOYtvt9p0NlffGwASHRCWwP_03i0Ytre29d4tIgEAUgREXf_zWgTFK2en&e=1571667418&k=oPNZNqjU131NzUiffI_DbQ&fl=&r=54612dce-f425-4562-a859-a6cce8124eb0-1&ckc=com.apple.clouddocs&ckz=com.apple.CloudDocs&p=52&s=ldbmeXFC3KYIy0BsSj2PzNwBUzs&cd=i"/></p>

Once you've done creating your own server, discord asks to invite friends to your server. Skip this step and voilá! Your own server has been made.

## Step 3: Install Node.js and Npm
### If you already have node.js and npm, you can proceed to step 4.
### 1. Check for node.js and npm
First we need to make sure that we need to make a local directory. To do this, we have to add some lines in the terminal. To open terminal, press CMD + spacebar and search for terminal. If you done this correct, the terminal should show up as the image above.

<img src="https://lh3.googleusercontent.com/dFrVaG3ZNfBd_TGNx5mcFeE1FdJH-cV9R0NfAC7p_RBaurLWiAJ6ntuCzZ-X3wVztrKLs2rUCs6DOlkwNMjoh3nY1JtzcCNm1ianwkfaDVTayfSjxh6rxREZQjUW3ZtjKkDlKLcGvRemH44HiV9ND376Ebdlv6bQfjQsfItr-gD3m2_C7z_H2_CuRryWejdTYS5k765oizJZ_CS0Ee3340BPTLeiNvRGNI9gQx_HkCrGJaoP9NeL24H7nZZySGvWp7kmzdzJhbNpRXQjk7J2J8vNbmsdUG3VbQm1c_LkJ20przcqurMrIwHuEu3M5yP5WC4CPuO_nGf5d51WZcjpgIo21NtPt3f_6T-2SYsmyRRe0ercQGlDgtwjTU1EFRHb_ewAcSpANnHe7vybH4khf0On4_wbfUNVAO15VIQ-RoqY8dhjAN5zPhGe0RsnuLEq1gHJC_-Tkeczm0GM73OKDOGv2Xcml2kBYZ2X2Owyo8-lO5Cr4OCHCLZgGEGgVoA5MzrrmCw0Guxrzngi46gH2yOEjmqD-5lIqKVj9nAOcfOE1L8gy7OptgQDWM4XODbAwofIDqPKzUNqy216KMjkv_LbvMTDQpXA5q-1cVwGx1SWuj23XPp_ZYmgjPxAcMhQWguGn2PjAuW3zrCnFVjIWLrDvznqg8kJlzwnVdKWmjqL49m2c-TrazXbvBY-i2HXEnPhs2ViLkhzMFd8Do5tRxP_ofxrMct_NSVJYN0zsg6WJ1Q=w1138-h724-no" width="50%" height="50%" /></p>

To check whether you've installed node.js and npm, type the following code:

**For node.js:**

```node -v```

**For npm:**

```npm -v```

If you both have node.js installed and npm, you shoud see the version.

<img src="https://lh3.googleusercontent.com/Wn3cKZ_1cdphxXZSBmL_qlg241uVMTU00StnCON1x2MDNOw15Lh_ufxNCL3yn-eYQH_jRsNLEK8Mh_p9G8qn6AT2OkSzQmlCRBu-li1sknZNqWJTg2vE6Ib1Zqu9YcjTNmVj_qak49uhVA9rGaDbPQ1MRgpNBK0jw0n9claWtaAlq7cM6hYvEiRt2NFMVLfSgmbzNWvY3of8-g4OMPJK4jLpWuhUdztoMmq1xO2rLxNre9HU0Ra443_vilTIF6paOkITGPtChf7klMjA0OX_PFSPKBEGaufqYtbtrQUrl1PYXgLjaI8IlzODbJGd-m28gFfURRtJ48MqqrvKPLg-YzTkj2MUdJw9FEQGWJTks1MyFTt2cxh06hsP9M2wxfi-Q2JbpF6kOjZ6DnsGzDxmOtAoLTXL0EXCZKeIGzyRULrAF6qk1W5_W0G77iRebUAYfJ_BqWo4HYFP0W4QrvOEDP-0jWxvdgWBqkpP-7UqJh6nRCcOQm9XZpUa9lN_BoN9tFh2SGTPiJP8EmEEM-RgO8buirQfKLrARc6anvUsDWXmYjOKq5oijq5mRJuPnSuY-jyQEEHk1Z961a8UB0v2L_XAd5QIqqNbigPRyO2XFMI5mFx-xvTV-RDdHjyMpnz-DmOxHSr6drsRvQGDEabzW2muykmsry3uUywaR2mv76-yFXeegMBlkyRuWZAJAaDlxbkpBAkeyNJlM5vig6CFyKmx-G1AOEIdh78bBji2h_Vt4c0=w1134-h654-no" width="50%" height="50%" /></p>

If not, install both node.js and npm by entering the following code (node.js will be installed along with npm):

**For npm:**

```npm install npm@latest -g```

For a full guide on how to install node.js and npm: https://nodejs.dev/how-to-install-nodejs

## Step 4: Create the Bot
We need to make an application and bot in order for our bot to work. We also need to send it to our discord server in order for it to show.

### 1. Create the application & bot:
First, head to discordapp.com/developers/applications/me. Log in with your account. Click New Application to get started, and give your application a name then click create. On the left tab, select Bot. Create the bot. If the bot is created, you will receive a message in the picture above that the bot has been created.

<img src="https://photos.google.com/share/AF1QipPOiCaoDnBDYWDjH9z2zoO5RBj4Lpy8jpAfTuAQFMt-sBLi_mu0NJ7NLXUgZNgpYQ/photo/AF1QipNfd-cqpvo-DEp9xQp2HbIi_mvPbtKMiABN-fOY?key=VHVOamZGVmFfNEl5Rng3REhJMXFUU2ZEZVZFTEln" width="50%" height="50%" /></p>

### 2. Send the bot to your Discord server.
In the first tab of www.discordapp.com/developers, select OAuth2. Scroll a bit down and select bot from the Scope list.

<img src="https://photos.google.com/share/AF1QipPOiCaoDnBDYWDjH9z2zoO5RBj4Lpy8jpAfTuAQFMt-sBLi_mu0NJ7NLXUgZNgpYQ/photo/AF1QipNNILERhp_4pD3oWb-r7u0aNxjGAsyBcxZuj9SW?key=VHVOamZGVmFfNEl5Rng3REhJMXFUU2ZEZVZFTEln"/></p>

Then, in the list beneath, tick the following boxes:

<img src="https://photos.google.com/share/AF1QipPOiCaoDnBDYWDjH9z2zoO5RBj4Lpy8jpAfTuAQFMt-sBLi_mu0NJ7NLXUgZNgpYQ/photo/AF1QipM9r1Z0Skxxw3SgcQy8fr9oKjCcJ_gGiDS4iZTM?key=VHVOamZGVmFfNEl5Rng3REhJMXFUU2ZEZVZFTEln"/></p>

At last, copy the link between the scope and permissions on the same page and paste in in your webbrowser's address bar.


## Step 5: Create a Local Directory
We need to make a folder on your pc that will store all of your bot's files. Name it something like discordBot or something that can recognized easily.

### 1. Create a folder and three files
We have to create three in that folder.

Execute the following code in the terminal by opening the terminal again using CMD + spacebar and search for 'Terminal':

```mkdir discordBot```

Navigate though the folder by typing in the following code:

```cd discordBot```

Then type the following line:

```npm init -y```

This will create a package.json file inside the project folder.

Let’s start first by installing a well known Javascript library for interacting with Discord API called discord.js. Type in:

```npm install --save discord.js```

Ignore the warnings for now.



### 2. Creating a file for the token
Using any text editor, create a file and name it "auth.json".

Paste the following code:

```
{
“token”: “Your Bot Token”
}
```

Then, replace the "Your Bot Token" with your token. This can be found at: https://discordapp.com/developers/applications/

Login, Click Client Secret and replace the Bot Token.

Save the file and make a new file.

The next file, name this file package.json, paste the following code:

```{

“name”: “discordBot”,

“version”: “1.0.0”,

“description”: “My First Discord Bot”,

“main”: “bot.js”,

“author”: “Your Name”,

“dependencies”: {}

}
```

Replace the author name with the name you want.
Save this file as “package.json” in your Discord bot folder.

At last, the last .json file will be called bot.js and paste the following code:

```
const Discord = require('discord.js');
const client = new Discord.Client();
const auth = require('./auth.json');client.on('ready', () => {
    console.log(`Logged in as ${client.user.tag}!`);
});

client.on('message', msg => {
  if (msg.content === 'ping') {
    msg.reply('pong');
  }
});client.login(auth.token);
```

Save this last text file as “bot.js” in your Discord bot folder. I added a simple command that if you say "ping", the bot will reply with "Pong!"


## Step 6: Last Step & Testing the Bot
### 1. Open terminal
In the Terminal, we need to check if we did everything correctly. Navigate to the folder by typing in the following command:

```cd discordBot```

### 2. Run the bot!
Then at last, run the command as shown below:

```node bot.js```

If you've done everything, it should say: Logged in as discordBot#xxxx!

Et voilà! the bot has been made for your discord server! You can message "Ping" in the channel to get a reply "Pong!"

This is just a basic bot for your discord channel. For more cool ideas check out: https://beebom.com/useful-discord-bots/
