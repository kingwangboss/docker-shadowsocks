docker-shadowsocks
==================

I think docker is better than a one-click-install-script.

Easy
====

    $ sudo docker run -d \
                      --name shadowsocks \
                      -p 3108:3108 \
                      hbrls/docker-shadowsocks
    # the default password is "youshallnotpass"

Expert
======

    $ sudo docker run -d \
                      --name shadowsocks \
                      -p your_port:your_port \
                      -e SS_PORT=your_port \
                      -e SS_PASSWORD=your_password \
                      -e SS_TIMEOUT=your_timeout \
                      -e SS_METHOD=your_method \
                      hbrls/docker-shadowsocks

Todo
====

1. `supervisord` it so that it will not down.


MIT License
===========

*I saw a lot of people use 1984 as the default port. To be more optimistic, I use [3108](http://page.renren.com/600803046/note/755367068?op=pre&curTime=1314684352000).*
