fetch list from [https://anti-ad.net](https://anti-ad.net) every day. for routeros.

save list to memory.

```shell
/ip/dns/set cache-size=20480
/ip/dns/adlist/add url=https://raw.githubusercontent.com/ffff-official/ros-adlist/main/ros-adlist.txt ssl-verify=no
```

save list to file.

```shell
/ip/dns/set cache-size=20480
/tool/fetch url=https://raw.githubusercontent.com/ffff-official/ros-adlist/main/ros-adlist.txt
/ip/dns/adlist/add file=ros-adlist.txt
```

[http://ffff.im/posts/20240604-ros-adlist/](http://ffff.im/posts/20240604-ros-adlist/)
