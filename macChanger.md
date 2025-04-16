// identifico il nome della rete, di solito: wlp16s0
ifconfig
//metto la rete in down
sudo ifconfig wlp16s0 down
//oppure
sudo ip link set dev wlp16s0 down
// cambio MAC
sudo macchanger -r wlp16s0              --> indirizzo mac completamene randomico
sudo --mac = 00:00... wlp16s0        --> indirizzo mac specifico
//reset mac address (the if must be down)
sudo macchanger -p wlp16s0

// per riattivare l'interfaccia si usa lo stesso comand per disattivarla ma con up
