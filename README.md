### TV-Headend channel for Plex Media Server

_What can this channel do for you?_

This channel streams content from a [TV-Headend](https://github.com/moxz/tvheadend.bundle) service right
to any of your plex devices. If the TV-Headend system cannot transcode the stream, which is needed by browsers,
iOS and Android devices, the plex service will do it instead. Please keep in mind that this transcoding process need a
bigger CPU.

### Donation

Since I'm developing in my free time I'd like to ask you to support my work.
You can do it by contributing 5 EUR via paypal. This will give me motivation
to keep on coding and fixing bugs.

Thanks in advance

[https://www.paypal.com/cgi-bin/webscr?no_note=0&lc=US&business=realriot%40realriot.de&item_name=GitHub+-+tvheadend-ng.bundle&cmd=_donations&currency_code=USD '''DONATE NOW VIA PAYPAL''']

### Latest notes

* Plex is able to transcode the incoming live stream. Telling TV-Headend to transcode can result in double transcoding
    and an overloaded cpu. Please use the passthrough by default.
* This plex channel for TV-Headend needs the TV-Headend API in version 15. An error message will occur if it's the wrong
    version.
* Additionally this channel supports streaming profiles provided by TV-Headend.
* To see channel logos you have to configure your TV-Headend system to deliver them. A nice manual can be found
   [here](https://tvheadend.org/boards/5/topics/13408?r=13674#message-13674)

### Developing

Make sure you have pip and virtualenv

```sh
sudo easy_install pip
sudo pip install virtualenv
```

Setup a virtualenv to work in

```sh
virtualenv env
```

Whenever you come back to develop just reactive your virtualenv

```sh
source env/bin/activate
```
