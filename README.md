# Unifi USG3 configuration for xs4all
Deze repo bevat configuratie bestanden om de usg3 te configureren zodat de USG3 ipv4, ipv6 en iptv doorgeeft aan een achterliggende switch of switches. Alle dns request gaan niet naar xs4all maar naar dns.google.

## installatie
```bash
scp config.gateway.json <server>:/<path to controler>/sites/default/config.gateway.json
scp knp.sh <usg>:/config/scripts/post-config.d/kpn.sh
ssh <usg>
chmod +x /config/scripts/post-config.d/kpn.sh
```
Inloggen op de unifi controler en de usg een `force probision` opdracht geven.
