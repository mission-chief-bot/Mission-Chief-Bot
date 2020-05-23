# Free Mission Chief Bot ![MissionChiefBot](https://img.shields.io/github/v/release/jackbayliss/Mission-Chief-Bot.svg) [![Discord](https://img.shields.io/discord/703655404885901393.svg?label=Join%20Our%20Discord&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2)](https://discord.gg/Kp8PtPK)

![Mission Chief Bot Example](https://i.imgur.com/dZR3nhm.gif)
A bot written to automate the general despatching jobs of the bot, simply follow the guide and let it run. No fee to pay, no license required. 

This was made to combat the issue of the [older bot](https://github.com/codesidian/Python-MissionChiefBot) being slow, and also difficult for users to install. Everything is there ready for the user at one click of a button.
Find the scan report of the exe [here](https://www.virustotal.com/gui/file-analysis/ODM5NDNhYjMzNjgwNjI0MDQ2ZDcwNTE4ODZkOTIzNjM6MTU4Nzc3NzYwMQ==/detection) incase you're worried it's a virus. 

## Features
- Send only a batch of missions at a time - set `missions_per_run ` to the amount required in your `config.ini`.
- Super fast, the bot is built with speed in mind! With the ability to despatch around 131 missions in around **6 minutes**.
- Multiple domains supported, .co.uk, .com, .it.
- Multiple accounts at one time, just create another bot in another folder and off you go.


## How to use
1. Ensure you have Python>=3.8.2 installed STRICTLY, it will not work with another version.
2. Download the code [here](https://github.com/jackbayliss/Mission-Chief-Bot/archive/Linux-&-Mac-OS.zip), then extract the files to a folder of your choice (Just keep the files together) - or use apt-get install git, and clone the repo.
3. CD into the file directory and do:
``` python3.8 -m pip install -r requirements.txt ``` this will install the requirements for you.
4. Once done open the `config.ini` inside the config folder and replace corresponding `username` and `password` with your account information, and `server` with the country  your account is registered on such as `uk`. All working countries will be in the `server.ini`
5. Do ``` python3.8 MissionChiefBot.py ```
6. Enjoy

`missions_per_run` is the amount of missions it will do per batch, so if it finds 100 missions and you've set it to 50 it will *ONLY* do 50. Set `show_own `to true if you want to ignore alliance missions, else set it to false.

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
