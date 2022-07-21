# Audacity-Discord-Sync
Discord Bot for syncing Audacity recordings for podcasts through Discord. 


# Description:
This is a personal project that was written for recording a podcast through Discord. We were disappointed that multiple online issues existed due to poor internet connections, which lead us to needing to do local recordings of each persons audio. This essentially is a discord "Clapperboard" for starting the recordings at the same time. 

# Warnings:
Technically there are two security concerns to keep in mind:
1. Firstly Enabling mod-script-pipe in Audacity does have some security concerns due to a remote object running commands through the program. Please see https://manual.audacityteam.org/man/scripting.html
2. Secondly each member of the recording will need to be running the bot. This allows all of them to sync to the same command at the same time. But does expose your Bot Key. This is a very high risk, and as such should not be given to anyone without trust. 
