# Audacity-Discord-Sync
Discord Bot for syncing Audacity recordings for podcasts through Discord. 


# Description:
This is a personal project that was written for recording a podcast through Discord. We were disappointed that multiple online issues existed due to poor internet connections, which lead us to needing to do local recordings of each persons audio. This essentially is a discord "Clapperboard" for starting the recordings at the same time. 

You're welcome to use the tool, but it will likely have sporatic updates or changes without warning.

# Warnings:
Technically there are two security concerns to keep in mind:
1. Firstly Enabling mod-script-pipe in Audacity does have some security concerns due to a remote object running commands through the program. Please see https://manual.audacityteam.org/man/scripting.html
2. Secondly each member of the recording will need to be running the bot. This allows all of them to sync to the same command at the same time. But does expose your Bot Key. This is a very high risk, and as such should not be given to anyone without trust. 


# Directions:
1. Install any python packages needed:
Discord.py
Discord.ext 
2. Create a new bot at https://discord.com/developers/applications
3. Generate a bot key, and invite it to your private discord guild
4. Edit the Python script, replacing BOTKEY with the authentication key for your bot, in the text: `client.run('BOTKEY')`
5. Install Audacity, and set mod-script-pipe to Enabled under Edit > Preferences > Modules. Exit and re-open to apply
6. Have each member of the recording run the bot

# Commands:
`$start`: Start the recording

`$end`: End the recording


# Packaging:
I personally generated executables for the members of my recordings, as not all of them were familiar with python, pip, or scripts in general. So I built them an executable using PyInstaller following the Quickstart guide located at: https://pyinstaller.org/en/stable/
