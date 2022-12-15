# Pi-Hole + Unbound - 2 Containers

## Description

This Docker deployment runs both Pi-Hole and Unbound in separate containers on a Synology DS918+

Done:
Enabled MACVLAN BRIDGING:
    https://www.wundertech.net/how-to-setup-pi-hole-on-a-synology-nas-two-methods/
    https://blog.thelazyfox.xyz/adguard-home-a-world-without-ads-and-trackers/
    https://blog.thelazyfox.xyz/give-access-to-host-from-docker-containers-macvlan/
    https://discourse.pi-hole.net/t/alternative-synology-installation-method/5454?u=diginc
    http://tonylawrence.com/posts/unix/synology/free-your-synology-ports
    https://tonylawrence.com/
    https://tonylawrence.com/posts/unix/synology/running-pihole-inside-docker/
    https://gitlab.com/tonyklawrence/files.tonylawrence.com/-/tree/master

Pull Unbound and Copy in personalised .conf file
    https://github.com/chriscrowe/docker-pihole-unbound
    https://github.com/MatthewVance/unbound-docker
Pull PiHole and Copy in personalised .conf files
    https://github.com/pi-hole/docker-pi-hole

To Do:
Enable Unbound DNS Resolver Loggin:
    https://forums.freebsd.org/threads/unbound-logfile-how-does-it-work.48136/
    https://snippets.khromov.se/enable-logging-of-dns-queries-in-unbound-dns-resolver/
Convert to Environment variable and .env file
    https://github.com/pi-hole/docker-pi-hole/#environment-variables
Enable DHCP from PiHole
    https://docs.pi-hole.net/docker/DHCP/
Enable update of Docker Tag Programmatically
    https://github.com/pi-hole/docker-pi-hole/releases

Additional Reading:
    https://sandro-keil.de/blog/docker-compose-with-named-volumes-and-multiple-networks/
    https://sreeninet.wordpress.com/2016/05/29/docker-macvlan-and-ipvlan-network-plugins/
    https://docs.docker.com/network/network-tutorial-macvlan/
    https://hicu.be/category/networking
    https://github.com/AdguardTeam/AdguardHome#comparison-pi-hole
    https://blog.thelazyfox.xyz/adguard-home-a-world-without-ads-and-trackers/
    https://blog.thelazyfox.xyz/give-access-to-host-from-docker-containers-macvlan/
    https://www.networkshinobi.com/docker-host-cant-access-containers-running-on-macvlan/
    https://docs.docker.com/compose/compose-file/build/
    https://hub.docker.com/r/pihole/pihole
    https://nlnetlabs.nl/projects/unbound/about/
    https://docs.docker.com/engine/reference/commandline/build/
    https://docs.docker.com/compose/compose-file/compose-file-v3/#ipam
    