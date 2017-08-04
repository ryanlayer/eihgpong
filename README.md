# EIHG Pong Ladder Bracket CLI
```
  ______ _____ _    _  _____   _____   ____  _   _  _____
 |  ____|_   _| |  | |/ ____| |  __ \ / __ \| \ | |/ ____|
 | |__    | | | |__| | |  __  | |__) | |  | |  \| | |  __
 |  __|   | | |  __  | | |_ | |  ___/| |  | | . ` | | |_ |
 | |____ _| |_| |  | | |__| | | |    | |__| | |\  | |__| |
 |______|_____|_|  |_|\_____| |_|     \____/|_| \_|\_____|

                             O .
                           _/|\_-O
                          ___|_______
                        /     |     \
                       /      |      \
                      #################
                     /   _ ( )|        \
                    /   ( ) | |         \
                   /  \  |_/  |          \
                  /____\/|____|___________\
                     |   |             |
                     |  / \            |
                     | /   \           |
                     _/    /_
```

### Installation and player registration
Open up a Terminal or Command Prompt window, and either
```
wget http:/tiny.cc/eihgpong
chmod +x eihgpong
mkdir -p $HOME/bin
mv eihgpon $HOME/bin
PATH=$PATH:$HOME/bin
eihgpong -p ShortName:your.email@your.domain
```

You can also checkout the repo
```
git clone https://github.com/ryanlayer/eihgpong.git
```

### Usage
To access the ladder bracket CLI, simply run the `eihgpong`

```
eihgpong
```

```
All options are viewable by running:
```
eihgpong -h
```

#### View leader and challenge board
```
eihgpong
```

#### Sign-up
```
eihgpong -p <name>:<email>
```
You should receive a confirmation email upon successful registration.

#### Challenge a player
```
eihgpong -c -a <player1name> -b <player2name>
```

Challenged player will receive a email with the name of their challenger, and challenge will be added to the "Challenge Board." Any player who is currently on the challenge board will be unable to initiate another challenge until the current one has been resolved.

#### Report the results of a challenge match
```
eihgpong -m -a <player1name> -A <player1wins> -b <player2name> -B <player2wins>
```
Currently, individual game scores are not reported. Rather, report the total number of games won by each player during the challenge match. 
