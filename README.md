# Telegram Voice-Chat Bot [ Pytgcalls ]

Telegram Voice-Chat Bot To Play Music With Pytgcalls From Various Sources In Your Group.

<img src="https://hamker.me/wl9twld.png" width="600" height="400">


# Support

1. All linux based os.


## Requirements

- Telegram API_ID and API_HASH
- Python 3.7 or higher 
- Userbot Needs To Be Admin In The Chat
- Install **ffmpeg**

## Run


```sh
$ git clone https://github.com/thehamkercat/Telegram_VC_Bot
$ cd Telegram_VC_Bot
$ sudo apt-get install ffmpeg
$ pip3 install -U pip
$ pip3 install -U -r requirements.txt
$ cp sample_config.py config.py
```
Edit **config.py** with your own values.

```sh
$ python3 main.py
```

## Heroku

#### Generate String session [IMPORTANT]

Download this file [generate_string_session.py](https://raw.githubusercontent.com/thehamkercat/Telegram_VC_Bot/master/generate_string_session.py)


```sh
$ pip3 install pyrogram TgCrypto
$ python3 generate_string_session.py
```
Fork this repository and change name of `sample_config.py` to `config.py`
Then you will need get a session string, copy it, then press heroku deploy button.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/notpeople249/Telegram_VC_Bot/tree/master)


Send [commands](https://github.com/thehamkercat/Telegram_VC_Bot/blob/master/README.md#commands) to bot to 
play music.


## Docker

```sh
$ git clone https://github.com/thehamkercat/Telegram_VC_Bot && cd Telegram_VC_Bot
$ cp sample.env .env
```
Edit **.env** with your own values.

```sh
$ sudo docker build . -t tgvc-bot
$ sudo docker run tgvc-bot
```
To stop use `CTRL+C`


## Commands
Command | Description
:--- | :---
/help | Show Help Message.
/skip | Skip Any Playing Music.
/play [SONG_NAME] | To Play A Song Using YouTube.<br>Service used can be changed in config (`DEFAULT_SERVICE`).
/play youtube/saavn/deezer [SONG_NAME] | To Play A Song Using Specific Service.
/telegram | Play A Song Directly From Telegram File.
/queue | Check Queue Status.
/joinvc | Join Voice Chat.
/leavevc | Leave Voice Chat.
/listvc | List Active Voice Chats.
/volume [1-200] | Adjust Volume.
/pause | Pause Music.
/resume | Resume Music.
/theme [Theme Name] | Change 'Currently Playing' Theme.
/update | Update & Restart.

## Note

1. If you want any help you can ask [here](https://t.me/tgvcsupport)

## Credits

1. @MarshalX [For TgCalls]
2. Everyone who contributed to the project.
