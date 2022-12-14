ARG PIHOLE_VERSION
FROM pihole/pihole:${PIHOLE_VERSION:-latest}
RUN apt update && apt full-upgrade && apt install -y unbound

COPY lighttpd-external.conf /etc/lighttpd/external.conf 
COPY unbound-pihole.conf /etc/unbound/unbound.conf.d/pi-hole.conf
COPY 99-edns.conf /etc/dnsmasq.d/99-edns.conf
COPY 04-pihole-static-dhcp.conf /etc/dnsmasq.d/04-pihole-static-dhcp.conf
COPY 40-no-dhcp-interface.conf /etc/dnsmasq.d/40-no-dhcp-interface.conf
COPY 50-dhcp-extra.conf /etc/dnsmasq.d/50-dhcp-extra.conf
RUN mkdir -p /etc/services.d/unbound
COPY unbound-run /etc/services.d/unbound/run

ENTRYPOINT ./s6-init