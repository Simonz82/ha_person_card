<h2><span style="text-decoration: underline;"><strong>🧑🏻 Person card for home assistant</strong></span></h2>

CARD con SWIPE laterale e nel mio caso con 3 viste:

<p><img src="example/example1.jpg" alt="" /></p>

<p>Volevo condividere una scheda che ho creato con l'aiuto delle varie community per visualizzare le informazioni di una persona tramite l'utilizzo dell'app HA companion.</p>

<p dir="auto">Istruzioni:</p>

da Hacs, installare:
1. swipe-card
2. stack-in-card
3. mushroom

poi ...
1. nel file sensor.yaml, inserire il contenuto di sensor.yaml, se non si dispone del file:
    - è necessario creare sensor.yaml nella cartella config/
    - aprire il file configuration.yaml e inserire questa riga: sensor: !include sensor.yaml
    - all'interno del codice, dovete andare a sostituire tutti i miei sensori chiamati "simone", con i vostri appena abilitati
2. Installare nel menù impostatione - dispositivi e servizi: l'integrazione prossimità
3. sul vostro smartphone installare l'app Home Assistant companion
4. dall'app andate in impostazioni, app complementare, gestione sensori
5. abilitate tutti i sensori che servono e che trovare nei vari file di configurazioni: sensori di rete,sensori ultimo riavvio, sensori di prossimità, sensori batteria, sensori di archiviazione, sensori di attività, sensori di posizione.
6. in HA create una card manuale e incollate il contenuto del file: person_card.yaml
7. copiate il contenuto del file script.txt e create uno script in home assistant e incollare il testo, rinominate "simone" con il nome del vostro device

<strong>Alla fine ci troveremo ad avere:</strong><br />
<strong>1. Prima schermata (in ordine dall'alto e da sinistra a destra):</strong>
1. Persona con simbolo se è in casa o no, e testo con dichiarata la zona dove si trova (in base alle zone impostate in HA)
2. % batteria con cambio colore in base al livello, presa di corrente per capire se è sottocarica o no, % memoria libera interna dello smartphone, tipo di rete (se è wifi o 5G)
3. a sinistra: ultimo aggionamento effetuato, a destra: la distanza che la persona si trova da casa

<p><img src="example/example1.jpg" alt="" /></p>

<p><img src="example/example5.jpg" alt="" /></p>

<strong>2. Seconda schermata:</strong>
1. router al quale si è connessi
2. se siamo fermi o in movimento, simbolo del telefono rosso, se lo si clicka attiva lo script: find phone, farà suonare il vostro telefono per trovarlo in caso di smarrimaneto.
3. indirizzo in cui ci si trova nel momento dell'ultima rilevazione
4. numero civico in cui ci si trova nel momento dell'ultima rilevazione

<p><img src="example/example2.jpg" alt="" /></p>

<strong>3. Terza schermata:</strong>
1. è solo un titolo: other info:
2. IP esterno della reta (non ip di casa se siamo in wifi)
3. ultimo riavvio dello smartphone

<p><img src="example/example3.jpg" alt="" /></p>

Risultato finale:

<p><img src="example/example4.gif" alt="" /></p>

<p>Enjoy!</p>

----------------------------------------
<p>Would you like to give me a hand?<br />The content of this page is completely free of charge and the purpose is certainly not to make money.<br />If you would like to lend me a hand to help with expenses and lost time, you have the following ways:</p>

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/C0C713VTGJ)

[![PayPal](https://github.com/Simonz82/desktop-tutorial/blob/main/paypal.svg)](https://www.paypal.com/paypalme/simongmail)

Make your Amazon purchases from this link:

[![Amazon](https://github.com/Simonz82/desktop-tutorial/blob/main/Amazon_logo.png)](https://amzn.to/3XWWTgz)

Join our Telegram channel dedicated to Home Assistant news:

[![Home_Assistant_News](https://github.com/Simonz82/desktop-tutorial/blob/main/home_assistant_news.jpg)](https://t.me/Home_Assistant_News)

Join our Telegram channel dedicated to home automation products, there are lots of offers:

[![Offerte Domotica](https://github.com/Simonz82/desktop-tutorial/blob/main/offerte_domotica.jpg)](https://t.me/offerte_domotica_ita)

