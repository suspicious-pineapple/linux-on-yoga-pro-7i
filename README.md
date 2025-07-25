# linux-on-yoga-pro-7i
My journey towards making linux work on a yoga pro 7i

Issues encountered:
- Trackpad and touch not working on mint
- No audio on Pop!_OS by default
- If audio works, very high pitched and low volume
- No WiFI after waking up from suspend


(Using Fedora KDE)
## Steps done:
### Fix audio being high pitched
this is caused by ALSA only using the tweeters by default.</br>
create file at `/etc/modprobe.d/` called `snd.conf` </br>
with content:
```options snd-sof-intel-hda-generic hda_model=alc287-yoga9-bass-spk-pin```

### Fix WiFi not working after suspense
idk yet


Useful links:
https://wiki.archlinux.org/title/Lenovo_Yoga_7i


