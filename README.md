# Interactive Token Tracker for Summer Swaps 2
![image](https://user-images.githubusercontent.com/12885929/184119859-4a1adb45-98a2-44f1-ad52-edb949d0a720.png)


## General Use
If you've never used the tracker before, I suggest navigating to your club on the webapp, and selecting "SUMMER SWAP TOKENS 2" as the Rarity. This will show you all the players you have already collected and will allow you to claim them on the tracker. 

Expiring Tokens will display a warning exclamation mark if there is less than 24 hours left. This is based on your system time. It SHOULD correctly handle Timezones, but please make sure that the time displayed actually matches the daily reset time where you live. Obviously if your system has a different timezone than the one you are actually in, this will display incorrect information. If your timezone is correct, please create an [Issue](https://github.com/freakpants/tokens/issues/new)

## Copy Player Name
Hovering the Player name will display a clipboard icon as the cursor. Pressing down while this cursor is active will not claim the token, but will copy the Full Name or the "Known As" (e.g. Pele) Name to your clipboard, so you can search the corresponding player in the webapp, if you just need to check whether you do or do not have a specific player.

## Unclaiming Tokens
In case you claimed a token in the Tracker by mistake, you have to hit the unclaim button. This activates unclaim mode (indicated by the button being red). Every claimed token you click while in this mode, will be unclaimed. Clicking the unclaim button will cancel unclaim mode. I solved it this way, because I wanted to make sure you don't accidentally undo progress.

## Multiple Accounts
Handling multiple accounts is possible. There is a default profile. Adding a question mark and any text will create a different profile:
https://freakpants.github.io/tokens/?roadtoglory  
**NOTE:** This does not mean you can access that profile from anywhere else, or that other people can access that profile. The data is still only saved on your machine.

## Attribution
This tracker is inspired by the idea and layout of the trackers that [https://twitter.com/Criminal__x](https://twitter.com/Criminal__x) is updating every day on Twitter.
Images are loaded from the CDN of [WeFUT.com](http://WeFUT.com) and I'm also using player data from them.

There is no license attached, and you are free to use and modify the code however you wish. I would however prefer it if you raised an issue/create a pull request for new features.

## Database
The code to generate the json file with the tokens in it, is not maintained in this repo. That's not because I'm hiding it, but because it's part of a repo that uses the entire database of players, and other functionality that is outside the scope of the tracker. The database is based on player data from WeFUT.com.
Basically, I added a few extra fields to the database that assign a player as a token: 
![image](https://user-images.githubusercontent.com/12885929/184117414-1581c155-dbfb-4b5c-b7e6-87bac08e4e10.png)
Whenever a new token is released, I just update those corresponding fields in my local database and export the whole set of tokens as the [json file](https://github.com/freakpants/tokens/blob/main/players.json) that the tracker uses. The JSON file is basically the pure html of each card, with some modifications in structure for interacting with the cards.

# Other Swaps
This tracker is written in a way, that will make it easy to reuse for future swaps. That is assuming no massive changes to the way Ultimate Team works.



