# loading-screen
Just a loading screen with logo reacting to music and js particles made by KeepCool

Requirements :

- A PNG LOGO in 1:1 scale
- A Music on discord past 24 hours

How to add it to your server :

Easy Way :
- Download the files
- Rename the folder "loadingscreen"
- Add this line to your server.cfg : "start loadingscreen"

Hard Way (don't add a resource) :
- Download the files
- remove fxmanifest.lua
- create a folder in your core / es_extended for esx users named "load"
- drag the files in the folder
- add this to fxmanifest.lua / _resource.lua :
```lua
files {
	"load/index.html",
	"load/music/load.mp3",
	"load/img/*.jpg",
	"load/img/*.png",
	"load/css/*.css",
	"load/js/*.js"
	}
	
loadscreen "load/index.html"
```

How to change the music :

- Upload the music somewhere and copy the music link (mp3 format)
- Replace the link on js/spykemusic.js:72

How to change the logo :

- Upload the logo somewhere and copy the logo link (png 1:1 scale)
- Replace the link on index.html:31

Enjoy the loading screen :D
