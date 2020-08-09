# iMessageAutoSend for MacOS :D
A simple applescript to send your buddies messages every x minutes from an array of messages :D


Hey guys! 

# save the file in /Application/send_message.applescript

then type in terminal
```
env EDITOR=nano crontab -e
```

then an editor will open up:

```
*/1 * * * *  osascript /Applications/send_message.applescript
```

this will send the message every minute ;) see [cronjobs](https://www.thegeekstuff.com/2009/06/15-practical-crontab-examples/) for other time intervals 


Currently trying to connect it to a chatbot API and let the API chat for me :D

## View and stop running cronjobs

```
crontab -l

crontab -r
```


## you need to save your imessage contact as a buddy on the mac first! then replace it eg 
```
	set theBuddy to buddy "johndoe"

```
