# VLAN
`sudo himage -e pc4` mi da nome esperimento

`sudo ovs-vsctl set port i0c41.n0.e0 tag=10` setta una particolare interfaccia `e0` con il tag 10 e quindi la vlan 10

`sudo ovs-vsctl show` se non vedi tante righe non funziona 

`sudo ovs-vsctl list-br | while read br; do sudo ovs-vsctl del-br "$br"; done` pulisce tutte le simulazioni e svuta l'output di `sudo ovs-vsctl show`
