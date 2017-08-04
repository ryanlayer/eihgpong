# EIHG Pong Ladder Bracket CLI

### Installation
Open up a Terminal or Command Prompt window, and either
```
git clone https://github.com/ryanlayer/eihgpong.git
```
or
```
wget http:/tiny.cc/eihgpong
```

### Usage
To access the ladder bracket CLI, simply run the `eihgpong` bash script with 

```
bash eihgpong
```

Alternatively, make `eihgpong` executable and run it.

All options are viewable by running:
```
eihgpong -h
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
