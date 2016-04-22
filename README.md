# Target
It is a simple bash script to help create keyboard shortcut. They will help you manage your windows without using your mouse.

# How to use it?
```target [-p program] [-n name] [-t title] [-a all] [-x WM_CLASS_name]```

The goal of the script, is that you can call it anytime. If the app is not running it will launch it and if it's already running it will focus the window.

The `program` is the command used to launch the application.

The `name` is the name of the program that is running. The script is using this flag to find out if the application is already running on the system.

The `title` is used to target the window. You should put a string always contained by the application window title.

The `WM_CLASS_name` can be used like `title` but this will use the `WM_CLASS` to target the window.

The `all` will replace the other flags if they are not set except `-x`. If `-x`
is used, `title` won't be automatically set.


# Examples
```target -a firefox```

```target -p google-chrome -a chrome```

# Dependencies
You need to have ```wmctrl``` installed. Also, you need ```pidof``` which is present on linux. I don't think Mac has it by default, but there is simple alternative like : https://gist.github.com/doitian/827854.
Important : I didn't try to run my script with this alternate ```pidof```.
