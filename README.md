# How to setup

Install dependencies for zephyr according to the guide: https://docs.zephyrproject.org/latest/develop/getting_started/index.html

Create and dir with this repo inside and create an Python venv on it

```
sudo apt install python3-venv
python3 -m venv .venv
.venv/bin/activate
pip install -r requirements.txt
west init .
west update
west zephyr-export
west packages pip --install
```

## To build and flash
Go to the repository folder and execute:

```
west build -p
west flash
```

To use the serial monitor provided by Espressif:
```
west espressif monitor
```


