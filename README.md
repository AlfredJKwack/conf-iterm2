# conf-iterm2
 Hold iTerm2 configuration files

# Installation

Using the iterm profiles from this repository can be done in one of 3 ways

You can [download the json file](https://raw.githubusercontent.com/AlfredJKwack/conf-iterm2/main/iTerm2-Profile.json) and import it as a new profile in iTerm via `iTerm2 > Preferences > Profiles > Other actions > import JSON profile ...`

Alternatively you can put the profile in as a Dynamic Profile. The upside is Dynamic profiles have a higher priority than plists but are non destructive.

        cd ~/Library/Application\ Support/iTerm2/DynamicProfiles/ && { curl -O https://raw.githubusercontent.com/AlfredJKwack/conf-iterm2/main/iTerm2-Profile.json ; cd -; }


Move the plist in this repo to its normal place in your OS, essentially **wiping your own setup**.

        cd ~/Library/Preferences && { curl -O https://raw.githubusercontent.com/AlfredJKwack/conf-iterm2/main/com.googlecode.iterm2.plist ; cd -; }

# Rolling your own

1. Fork this library and clone it locally
2. copy `~/Library/Preferences/com.googlecode.iterm2.plist` into the respository
3. Save your profile(s) (iTerm2 > Preferences > Profiles > Other actions) in the repository
4. Push the repo and it's available wherever you need it.

# Reference formation
The iTerm2 app sypports [Dynamic Profiles](https://iterm2.com/documentation-dynamic-profiles.html) and [this StackOverflow question](https://stackoverflow.com/questions/35211565/how-do-i-import-an-iterm2-profile) got me the rest of the way.
