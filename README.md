![alt text](https://iili.io/2ulgAo7.png)

## Description

This project is the first Object-Oriented Programming project of the 42 course, made in C++ (Version 98).

The Goal is to create an [IRC](https://fr.wikipedia.org/wiki/Internet_Relay_Chat) (Internet Relay Chat) server by following the [IRC official norm/protocol](https://modern.ircdocs.horse/).

The server must be able to handle multiple client connexions at once, without blocking any operation. Technically, the server can work with any IRC Client, but we choose to adapt our code for [Hexchat](https://hexchat.github.io/).

Unfortunately, sharing the exercices subjects is forbidden by the school, but you may still be able to find these on the internet :)

## How it works

- git clone https://github.com/timonicolaux/42_IRC.git
- make
- run program with three parameters : PORT, password, database of the project (like this -> ./ircserv 8080 password quizdatabase.txt)

Once the server is running, launch a connexion with Hexchat by completing the right parameters : the port you choose for your server, the IP address of your server, the password.

Also complete nickname, realname, username, unselect "Use SSL for all the servers on this network" + "Use global user information", select "Accept invalid SSL certificates".

That's it, you can now click on connect and you are logged in to the server !

## Intructions for testing program

Here are the available commands :

- /JOIN #[room of you choice] : joins by default a new room, or an existing room (if mode +i is set in the room, you have to be invited first)
- /PRIVMSG username message : sends a private message to the user (if he exists)
- /INVITE username (in an existing room) : invites a user to the room
- /KICK tnicolau (in an existing room) : kick an user from the room (command available for operators only)
- /MODE (in an existing room): displays the availables modes
  - /MODE +i/-i : sets/unsets room on invite only mode
  - /MODE +t/-t : sets/unsets the possibility to modify topic of the room for everyone/operators only
  - /MODE +k/-k password : adds/deletes password for the room (only for operators)
  - /MODE +o/-o username : sets/unsets operator mode for the user targeted (only for operators)
  - /MODE +l limit OR /MODE -l : sets/unsets limit of users for the room (only for operators, minimum 1 and maximum 2000)
 
## Bonus

- /QUIZ number : launches a new Quiz game with the number of questions (min 1, max 10)

You will be able to talk in PRIVMSG to Bot JulienLepers and send your answers to the questions !

Have fun :sunglasses:

![alt text](https://i.makeagif.com/media/9-06-2015/kNlPyX.gif)
