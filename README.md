# Cheat-pizzuno
Just copy paste the script in tamper monkey and go to play on https://pizz.uno/

**Note:** If the bot cannot connect anymore it can come from the socket.io version. See `@require` line to try to fix it yourself.

**Note:** Only working for 2 player at the same time I think.

![alt text](https://github.com/oom-/cheat-pizzuno/blob/main/screenshoot.jpg?raw=true)

# Explanation
During the game the websocket is receving events, as the `updateState` event is containing all informations on the actual game. I just connected a second websocket in the room, parsed the payload and edit the DOM to replace the `card card back` by the cards of the opposite player.

![alt text](https://github.com/oom-/cheat-pizzuno/blob/main/why.jpg?raw=true)
