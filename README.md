config.env
- `BOT_TOKEN`: The Telegram Bot Token that you got from [@BotFather](https://t.me/BotFather). `Str`
- `TELEGRAM_API`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Int`
- `TELEGRAM_HASH`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Str`
- `FSUB_ID`: The Force Subscribe Channel, users will not be able to use your bot without joining the Channel. (Enter the Channel/Group ID starting with -100). `Int`
- `DUMP_CHAT_ID`: The Dump Channel, all leeched videos will be Forwared Here. (Enter the Channel/Group ID starting with -100). `Int`

## 😵‍💫 Feature : 

- Public usage & Pvt usage 
- Save all videos into Database Channel 
- Broadcast 
- Total user count
- Admin can download 500MB+
- Force sub | Channel & Group 
- Token verification Feature 
- check token timeout 
- 🆕 check STATUS how many users are verified via token ( current status )
- 🆕 Working on Groups & in PM

## Command:
```
/start - alive or not !
/check - token timeout (user)
/broadcast - media/txt support (a)
/Stats - verified user status (a)
---
## Deploy on VPS
---
## Prerequisites

### 1. Installing requirements

- Clone this repo:

```
git clone / && cd terabox
```

- For Debian based distros

```
sudo apt install python3 python3-pip
```

Install Docker by following the [Official docker docs](https://docs.docker.com/engine/install/#server).
Or you can use the convenience script: `curl -fsSL https://get.docker.com |  bash`


- For Arch and it's derivatives:

```
sudo pacman -S docker python
```

------

### 2. Build And Run the Docker Image

Make sure you still mount the app folder and installed the docker from official documentation.

- There are two methods to build and run the docker:
  1. Using official docker commands.
  2. Using docker-compose.

------

#### Build And Run The Docker Image Using Official Docker Commands

- Start Docker daemon (SKIP if already running, mostly you don't need to do this):

```
sudo dockerd
```

- Build Docker image:

```
sudo docker build . -t phdlust
```

- Run the image:

```
sudo docker run -p 80:80 -p 8080:8080 phdlust
```

- To stop the running image:

```
sudo docker ps
```

```
sudo docker stop id
```

----

#### Build And Run The Docker Image Using docker-compose

**NOTE**: If you want to use ports other than 80 and 8080 change it in [docker-compose.yml](docker-compose.yml).

- Install docker compose

```
sudo apt install docker-compose
```

- Build and run Docker image:

```
sudo docker-compose up --build
```

- To stop the running image:

```
sudo docker-compose stop
```

- To run the image:

```
sudo docker-compose start
```

- To get latest log from already running image (after mounting the folder):

```
sudo docker-compose up
```

--

Cmd to start the Bot: bash start.sh