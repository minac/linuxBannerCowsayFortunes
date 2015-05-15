Simple script for a few of my favourite "cows" saying fortune cookies for Ubuntu login banners.

# Install

To ensure you have the update message of the day script and git:

```sudo apt-get install update-motd git```

The packages you need to make the magic happen:

```sudo apt-get install fortune cowsay```

Get this code on your server:

```git clone https://github.com/minac/linuxBannerCowsayFortunes.git```

Copy the script into place:

```sudo cp linuxBannerCowsayFortunes/33-cowfortunes /etc/update-motd.d/```

Make it executable:

```sudochmod +x /etc/update-motd.d/33-cowfortunes```

Flush the current motd:

```sudo rm /var/run/motd.dynamic```

Logout and in 2 times to force the refresh. And voila!

<pre>
 _________________________________________
/ You will be reincarnated as a toad; and \
\ you will be much happier.               /
 -----------------------------------------
       \ (__)
         (oo)
   /------\/
  / |    ||
 *  /\---/\
    ~~   ~~
</pre>
