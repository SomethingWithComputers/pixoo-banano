# Pixoo Banano

A simple proof-of-concept for my [Pixoo 64](https://github.com/SomethingWithComputers/pixoo) library.

It displays relevant information for the amazing [Banano](https://banano.cc/) coin. It'll also show your
current [Folding@Home](https://foldingathome.org/) stats (because you're likely folding for Bananos!)

## Installation

Simply install the required dependencies via PIP. Navigate to the directory where you placed the code. Then execute:

```
pip3 install -r requirements.txt
```

And then create a `.env` file in this same directory (notice the leading '.'). This file is used to configure the
application.

Inside, place:

```
FAH_USER_ID=501878621
PIXOO_IP_ADDRESS=192.168.1.137
TIMEOUT=3600
```

Note that `FAH_USER_ID` should be set to your own user id. If you don't know your user id, you can find it by looking
for your username here: https://stats.foldingathome.org/donor

The number behind your donor name is your user id. If you click your stats, it'll take you your donor page and the user
id will be the number at the end of the url (e.g. https://stats.foldingathome.org/donor/501878621)

The `PIXOO_IP_ADDRESS` should be set to the local IP address of your Divoom Pixoo 64.

The `TIMEOUT` is how many seconds the application will wait before updating the stats. I've given 3600 as an example,
which basically means once per hour.

If you like to fiddle with the code, you could also remove the loop and set
a [cronjob](https://en.wikipedia.org/wiki/Cron) to ease the load on your CPU slightly.

## Getting started

This project is made for python 3.x so to be sure you're running the correct version (Mac for example, comes with Python
2 installed by default) execute the following command from the directory you placed the project:

```
python3 main.py
```

## Support

If you have any questions, contact me!

If you like what I do, feel free to **ban** me, it's much appreciated!
![](ban.png)
ban_116q1cpe3ynr5uaqms53uwh1dj7a7157awqx8ye11h45i9yoknwguymo6xgp