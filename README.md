My Traffic Control
==================

A really simple experiment to handle traffic on my slow home network to avoid issues when playing real-time Internet games.

I wanted to be able to easily throttle devices that would swallow up my Internet bandwidth, resulting in high lag in games. I wanted it to be easy as finding the IP of the culprit and running `mtc {ip-address}` to temporarily throttle the bandwidth, and then running `mtc clear` to stop the throttling once I'd finished my game to give the bandwidth back.

To be used on OpenWRT. A short demonstration is available [on asciinema](https://asciinema.org/a/46044).

Dependencies
------------

- tc
- ipset
- kmod-sched (for HTB qdisc)
- iptables-mod-conntrack-extra (for connmarking)
- dig (for host lookup functionality)
- [mth](https://github.com/nuviktor/mth) (for automatic addition)
