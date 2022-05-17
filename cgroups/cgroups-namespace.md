# CGROUPS AND NAMESPACES: LE INTERIORA DELLA BALENA BLU
---
## cosa é un container:
quanti di noi utilizzano un container oggi, quasi tutti direi, ma quanti realmente sanno cosa sia un container... quando diciamo: macchina virtuale leggera o esecuzione containerizzata, sappiamo cosa sta realmente succedendo.
Bene questa presentazione cercherá di rispondere a queste domande.

Prima di tutto dobbiamo dire cosa fa un container.
Un container non é altro che una scatola isolata che esegue un eseguibile in un filesystem proprietario virtuale.
In parole povere significa che l'esecuzione dell'eseguibile avviene in un ambiente isolato dalla macchina che ospita il container.

Peró vediamo di mettere questa cosa a confronto con una macchina virtuale, vediamo la definzione di questa:
Una macchina virtuale é un ambiente virtuale che emula l'hardware della macchina fisica.

La differenza sostanziale tra le due definizioni sta nella parte dell'hardware.
Una macchina virtuale crea una partizione dell'hardware fisico e lo utilizza per l'esecuzioni di un kernel completamente nuovo, invece un container esegue l'eseguibile sull'hardware fisico ma generando una sezione di risorse dedicata.

Le macchine virtuali fanno una cosa chiamata "virtualizzazione dell'hardware" 


