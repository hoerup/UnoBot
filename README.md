# UnoBot

UnoBot is IRC bot that is written in java. It has a pircbot back end so its easy to change settings. 
The bot connects to an IRC server/channel
and allows members of the channel to play a game of uno. It also has an AI so it can play too.

## Installation

1. open the config.ini file
2. edit the values appropriately
3. run the make script in UnoBot
4. run the UnoBot.jar 

### values in the config file

        Server - if no value given it will default to localhost
        Port - if no value given it will default to 6667
        Channel - the channel the bot connects to #uno
        Nick - if no value given it will default to unoBot
        BotOps - if no value given it will default to null
		         this should be a list seperated by ',' and no spaces.
                 the first user in this list should be the owner.

## Usage

Once the bot has connected you can type any of the following commands.

     !uno ------ Starts an new UNO game.
     !join ----- Joins an existing UNO game.
     !deal ----- Deals out the cards to start an UNO game.
                 but only the person that started the game can deal
     !play ----- Plays a card (!play <color> <face>)
                 to play a RED FIVE !play r 5
     !showcards  Shows you your hand. (!hand)
     !draw ----- Draws a card when you don't have a playable card.
     !pass ----- If you don't have a playable card after you draw
                 then you pass.
     !count ---- Show how many cards each player has.
     !leave ---- If you're a fagot and want to leave the game early.
     !what ----- If you were not paying attention this will tell
                 you the top card and whos turn it is.
     !players -- Displays the player list.
     !score ---- Prints out the score board.
     !ai ------- Turns the bot ai on or off.
     !endgame -- Ends the game, only the person who started the
                 game may end it.
     !tell ----- Tell an offline user a message once they join the channel.
     !messages - List all of the people that have messages.
     !help ----- This stuff.    

     ONLY THE MASTER CAN USE THESE COMMANDS
     !nick ----- Tells the bot to change his nick.
     !joinc ---- Tells the bot to join a channel.
     !part ----- Tells the bot to part from a channel.
     !quit ----- Tells the bot to disconnect from the entire server.