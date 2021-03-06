docker-shadowsocks
==================

Easy
====

    $ docker run -d \
                 --name shadowsocks \
                 -p 3108:3108 \
                 hbrls/shadowsocks
    # the default password is "youshallnotpass"

Expert
======

    $ docker run -d \
                 --name shadowsocks \
                 -p your_port:your_port \
                 -v /path/to/your/log:/var/log/supervisor \
                 -e SS_PORT=your_port \
                 -e SS_PASSWORD=your_password \
                 -e SS_TIMEOUT=your_timeout \
                 -e SS_METHOD=your_method \
                 hbrls/shadowsocks

1. [Ri Xu Online: ShadowSocks Setup Guide](https://xuri.me/2014/08/14/shadowsocks-setup-guide.html)

2. [Using Shadowsocks with Command Line Tools](https://github.com/shadowsocks/shadowsocks/wiki/Using-Shadowsocks-with-Command-Line-Tools)

MIT License
===========

*I saw a lot of people use 1984 as the default port. To be more optimistic, I use [3108](http://page.renren.com/600803046/note/755367068?op=pre&curTime=1314684352000).*

