### How to view the presentation
- The presentation was written in RevealJS, a first time experience for me.
- You can either
  - Download the Presentation folder and open the index.html file
  - or view here: [I use Arch btw](https://htmlpreview.github.io/?https://github.com/Majestic9169/legendary-chainsaw/blob/main/Presentation/index.html)
    - Vertical slides seem to be giving me an issue when using this link, if pressing SPACE doesn't keep you moving forward in the presentation then please download the entire Presentation folder and view the index.html file
    - I also request that view the presentation in full screen, I include a bunch of screenshots of my own desktop that get cropped if you aren't on a fullscreen display (preferably 16:9)
 
### What is in the config files?
Here you will find the configuration files for 
+ fish: my default shell
  - all I did was add neofetch as a default command to run whenever a new shell instance is opened
+ hyprland: my window manager and compositor
  - here you will find all my keyboard shortcuts
  - and my window decorations: copied from hyprdots' Material Sakura theme
+ hyprpaper: the wallpaper manager for hyprland
  - I didn't really do anything to this, but I used another shell script that randomly changes the wallpaper loaded into the config file. This is triggered by SUPER+X.
+ hyprdots
  - this isn't really a config file, it's a collection of scripts for the custom modules used by waybar. As I initially copied my waybar configs from hyprdots I am using his scripts too, however the main scripts that I needed are not present and I will have to eventually write them myself
+ kitty: my terminal emulator
  - I was originally going to go with Konsole as my terminal but most posts that I saw on r/unixporn used kitty instead, so I went with this
  - kitty has fantastically written default documentation, it was very comprehendable
  - for my modifications all I did was change the default colors to the Material Sakura theme colors from hyprdots, and decrease the background opacity. I tried to change the background blur too, but that's controlled by the hyprland config instead
+ neofetch
  - all I did was change the default image used, however even that was quite difficult
  - aparently you can't just directly add the path of the image required, the config file I saw had some weird piped command that originally would randomise the picture. Since I couldn't get it to work by just directly adding the path I had to modify that weird command to use my image.
  - I went through the neofetch documentation but I couldn't understand what went wrong, I will revisit this again.
+ waybar: my status panel
  - waybar was easily the most annoying thing to configure. It was also the first thing I had to configure besides hyprland so I wasn't reading the documentation as much as I should have been.
  - Just getting the clock module took me some 3-4 hours. To be fair to me though, the troubleshooting for the clock module in the documentation was hard to find. And the issue was essentially an Arch issue, just setting the locales like mentioned in the wiki wasn't enough because that never works for some reason, however the clock module doesn't look for the defaut locale. So I had to manually tell it to use the default "C" locale for it to work.
  - I copied my waybar configs from hyprdots and removed almost every unnessecary module. However the only interesting modules didn't end up working because he didn't provide the scripts needed. So eventually I will add a script for those modules.
+ wofi: my application manager
  - rofi is typically the common application manager, however it doesn't have wlroots support, so wofi is used instead.
  - wofi can be customised in some really cool ways but there isn't really any documentation for that, so I didn't do any of that.
  - Instead all I did was change the location to the top-left and make it display icons.
  - Other than that I copied the style.css from auspacious dots to make it look decent. It must be said, wofi and waybar both come with some really bad looking defaults. 

### Some Updates
Since the submission of this repo (2nd April 2024) I have added some more cool stuff to my Arch setup
+ I added a SUPER cool grub theme today, without using grub-customised (because it didn't work, if it did I would have done this before the submission)
+ I changed my Neofetch image to an image of Aqua crying (from Konosuba)
+ I downloaded pywal, changed my waybar config and style.css, and configured it to use the generated theme from pywal on every reload of my wallpaper. I am still playing with this.
+ I downloaded and set up the Graphite GTK theme using lxappearance, infact this is what led me to changing my grub theme as well
+ I installed hyprlock and actually setup a lockscreen, I kept it quite close to the image I showed in the presentation, even downloading a custom font and learning more about fonts via the process.
+ I tried setting up cava, but didn't work :(
+ I got better at using vim and ranger, and setup image previews on ranger on the kitty terminal. Kitty can quite easily display images and gifs, however I needed to download a python-pillow package to get it to work with ranger, which I don't get
                
### Update

I lost all my configs recently, all these dotfiles are now outdated as I have since recreated my setup                    
