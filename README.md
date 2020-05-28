# Free Mission Chief Bot ![MissionChiefBot](https://img.shields.io/github/v/release/jackbayliss/Mission-Chief-Bot.svg) [![Discord](https://img.shields.io/discord/703655404885901393.svg?label=Join%20Our%20Discord&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Kp8PtPK)
![Mission Chief Bot](https://camo.githubusercontent.com/7ebf2f540206248fc4ee737e4d6989d7c4f9920e/68747470733a2f2f692e696d6775722e636f6d2f645a52336e686d2e676966)


A Mission Chief bot written to automate the general despatching jobs of the bot, simply follow the guide and let it run. No fee to pay, no license required.

## Supported Servers
![au](https://img.shields.io/badge/-AU-green)
![de](https://img.shields.io/badge/-DE-green)
![fr](https://img.shields.io/badge/-FR-green)
![it](https://img.shields.io/badge/-IT-green)
![nl](https://img.shields.io/badge/-NL-green)
![pl](https://img.shields.io/badge/-PL-green)
![pt](https://img.shields.io/badge/-PT-green)
![ro](https://img.shields.io/badge/-RO-green)
![ru](https://img.shields.io/badge/-RU-green)
![tu](https://img.shields.io/badge/-TU-green)
![uk](https://img.shields.io/badge/-UK-green)
![us](https://img.shields.io/badge/-US-green)

Your region missing? Ask in Discord or create an issue.



This was made to combat the issue of the [older bot](https://github.com/codesidian/Python-MissionChiefBot) being slow, and also difficult for users to install. Everything is there ready for the user at one click of a button.
Find the scan report of the exe [here](https://www.virustotal.com/gui/file-analysis/ODM5NDNhYjMzNjgwNjI0MDQ2ZDcwNTE4ODZkOTIzNjM6MTU4Nzc3NzYwMQ==/detection) incase you're worried it's a virus. 

## Features
- Send only a batch of missions at a time - set `missions_per_run ` to the amount required in your `config.ini`.
- Super fast, the bot is built with speed in mind! With the ability to despatch around 131 missions in around **6 minutes**.
- Multiple domains supported, .co.uk, .com, .it.
- Multiple accounts at one time, just create another bot in another folder and off you go.


## How to use
If you'd prefer to see a video tutorial you can watch it [here](https://www.youtube.com/watch?v=9adxIIqONTw) or follow the below:

1. Download the code [here](https://github.com/jackbayliss/Mission-Chief-Bot/archive/master.zip), then extract the files to a folder of your choice (Just keep the files together)

2. Once done open the `config.ini` inside the config folder and replace corresponding `username` and `password` with your account information, and `server` with the country  your account is registered on such as `uk`. All working countries will be in the `server.ini`

`missions_per_run` is the amount of missions it will do per batch, so if it finds 100 missions and you've set it to 50 it will *ONLY* do 50. Set `show_own `to true if you want to ignore alliance missions, else set it to false.


### Windows
Just double click the .exe and you're up and running!

### Linux
Please see the mac/linux branch [here](https://github.com/jackbayliss/Mission-Chief-Bot/tree/mac)
 
 ### Mac
Please see the mac/linux branch [here](https://github.com/jackbayliss/Mission-Chief-Bot/tree/mac)


## How to use 24/7 via server

1. First of all I'd recommened setting up a Digital Ocean account, or any other cloud provider that you can use Docker with. You can set an account for Digital Ocean [here](https://m.do.co/c/741cf5923606) (It's a referral link)

(Make sure you install docker if you're going outside of DO)

2. Once you've signed up to Digital Ocean simply create a droplet. You can install docker straight to it via the marketplace so i'd suggest doing that. (You can use any droplet, this will work on the smallest $5 A month one)

3. Connect into the droplet, you can do this via going to the Access Console or alternatively SSH into the droplet.

4. Once you're in type in `docker pull jjbayliss/mission-chief-v2`, let it run it'll set up the image for the bot. 
 
5. Once the image is done simply run `docker run -it -d jjbayliss/mission-chief-v2`. This will create a container for you.

6. Run `docker ps -a` and copy the name of your container there should only be one, then run `docker exec -it [container name] bash` this will take you into the container in a bash.

7. You should be brought straight into a container, all you'll need to do is `cd Mission-Chief-Bot` and then do `vim config.ini` 
You'll want to press the `I` key to edit the document, and add your username, password and region etc. Once done press `ESC` and type `:wq` this will save the document.

8. Run `python3 MissionChiefBot.py` to run the base bot, and you're done!

9. To exit the docker container press `CTRL + D`, and if you need to enter the bot again just follow from step 6.

## Issues / Bugs / Errors

If you have any issues and would like to let us know directly, please join our discord.
<p align="center">
  <a href="https://discord.gg/Kp8PtPK">
    <img src="https://discordapp.com/api/guilds/703655404885901393/widget.png?style=banner2" />
  </a>
</p>

If you have any issues please create an issue [here](https://github.com/codesidian/Python-MissionChiefBot/issues)

## Why is the source code hidden?
This is to mainly prevent the developers of the website seeing exactly how the bot is able to do it so quickly, this is more of a prolonging the life of the bot exercise. 

## Contributing

If you'd like to contribute please feel free to contact me via PM or email. If you check out I'd be more than happy to share the source code, in which you can contribute.

## Donations
Although this bot is completely free and there's no cost, if you'd like to support the Bot you can [buy me a beer](https://www.paypal.me/jackbaylissdev) :beer:

## License

This work is licensed under the Creative CommonsAttribution-NonCommercial-NoDerivs 4.0 Unported see license : http://creativecommons.org/licenses/by-nc-nd/4.0/



## Disclaimer
Section 7.2 of the MissionChief official rules state:
`Use of tools, scripts, bots or other computer programs:Users are not allowed to use tools, scripts, bots or other computer programs which are suitable for the automatic execution of actions in a game.`

No developers of this bot hold any responsibility for your use of it. We make no warranties about the effectiveness, or performance of this bot. If you're banned, that's on you. 

**USE AT YOUR OWN RISK**
