# Interactive Token Tracker for Summer Swaps 2

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
