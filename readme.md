- [Requirements](#requirements)
- [Setup](#setup)
  - [OBS](#obs)
  - [Script](#script)
  - [Setup environment](#setup-environment)
- [Run](#run)


# Requirements
OBS-Websocket from - https://github.com/Palakis/obs-websocket

# Setup
## OBS
In OBS, Tools->WebSockets Server Settings
- Enable Websockets Server checked
- Server Port 4444
  - Port can be changed, but make sure to update in settings.py
- Enable Authentication checked
- Password - Set one, put it in settings.py
- Enable System Tray Alerts will produce a windows notification every time a connection is made.

## Script
- Copy settings.py.template to settings.py
- Set each value according to your settings, obs_ip is the address of your streaming system.
- aio_user and aio_key are AdafruitIO username and key, enter those.

## Setup environment
- Install pipenv if not already installed
  - ```python -m pip install --upgrade pipenv pip```
- Install dependencies
  - ```pipenv install```



# Run
```pipenv run python obs.py```
