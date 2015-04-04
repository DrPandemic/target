# Target
It is a simple bash script to help create keyboard shortcut. They will help you manage your windows without using your mouse.

# How to use it?
```target program [name]```

The goal of the script, is that you can call it anytime. If the app is not running it will launch it and if it's already running it will focus the window containing the ```name``` in its title. If the ```name``` is not present it will use the ```program``` to try focus the window.


# Examples
```target firefox```

```target google-chrome chrome```

# Dependencies
You need to have ```wmctrl``` installed. Also, you need ```pidof``` which is present on linux. I don't think Mac has it by default, but there is simple alternative like : https://gist.github.com/doitian/827854. 
Important : I didn't try to run my script with this alternate ```pidof```.
