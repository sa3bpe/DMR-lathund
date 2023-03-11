# Komma igång på DMR - ett exempel

Denna text riktar sig till dig som beslutat dig för att prova DMR och ska ses som en första guidning in i denna spännande värld. Texten är generell och begreppen som förekommer kan skilja sig mot de begrepp som används i de olika radiotillverkarnas språkbruk/definitioner. I detta exempel används repeatern SK3RHU (VHF) som underlag.

Nummer ett är att skaffa sig ett unikt DMR-id för sin signal. I DMR-världen heter du exempelvis inte bara SA3BPE. Servrar och system är inte uppbyggt för att klara bokstäver och siffror utan klarar bara av att hantera siffror. Ditt DMR-id ansöker du om här; [https://www.radioid.net/](https://www.radioid.net/) Notera att det skiljer sig i registreringen om du ska registrera en repeater eller hotspot. Registreringen av hotspots eller repeatrar behandlar vi inte i detta exempel.

Nummer två är att programmera sin nyinköpta DMR-terminal. Enklaste är väl att leta reda på en sk codeplug för din radio. Det finns en hel uppsjö av olika codeplugs på Internet. Vi kommer därför enbart gå igenom och visa hur man ska konfigurera och programmera sin terminal för SK3RHU VHF. Följande ska programmeras in på kanalen;

SK3RHU VHF TS1

* Frekvens – 145,7125 MHz -0,6 MHz skift.
* ColorCode (CC) – 3 (för tredje distriktet)
* Groupcall – 240324
* TimeSlot 1
* Default TG – 2403

Nu har vi specat terminalen att lyssna på en repeater som heter SK3RHU. Men… Förmodligen är det nu ganska tyst i radion?(!) Detta beror på att du nu behöver speca din terminal att släppa igenom trafik som kommer från repeatern på TimeSlot 1. Detta sätter du upp i något som vanligtvis kallas för RX-Group Lists.  Notera här att det är ofta förekommande att du behöver lägga in respektive talgrupp i din terminals kontaktbok för att sedan hämta in dessa till RX-Group List. När vi nu lagt in alla talgrupper i vår kontaktbok så går vi in och lägger in rätt talgrupper som repeatern är uppsatt som default i vår RX-Group List på TimeSlot 1. Exakt vilka talgrupper som ligger som statiska kan du se här; [https://brandmeister.network/?page=repeater\&id=240324](https://brandmeister.network/?page=repeater\&id=240324) Här kan du även se de dynamiska (läs; tidsinställda talgrupper), clusters och last heard på repeatern.

Rätt grund för en korrekt RX-Group List för SK3RHU VHF är följande;

TimeSlot 1:

* TG91
* TG92
* TG927

TimeSlot 2:

* TG240
* TG240240
* TG2400 – TG2407
* TG2410
* TG7
* TG8
* TG9

Värt att notera är att nu behöver du programmera in en ny kanal i din terminal för SK3RHU VHF TimeSlot 2. Den setupen ser ut såhär;

SK3RHU VHF TS2

* Frekvens – 145,7125 MHz -0,6 MHz skift.
* ColorCode (CC) – 3 (för tredje distriktet)
* Groupcall – 240324
* TimeSlot 2
* Default TG – 2403

Detta innebär att varje repeater tar upp två minnesplatser i din terminal pga de två timeslots som finns på frekvensen. Du kan här nu använda dig av samma inställningar i RX-Group List som vi konfigurerade tidigare. I vissa terminaler finns något som kallas Promiscuous Mode, då detekterar radion all trafik oavsett vilken talgrupp som repeatern sänder ut.

Nu! Nu kan du köra ditt första DMR-QSO! Och gör du inget mer än att väljer minnesplatsen för SK3RHU VHF TS2 som kommer du prata över talgruppen 2403 som är lokaltalgrupp för SM3.

Det är mycket viktigt att titta på de respektive repeatrar som finns då det skiljer sig markant över vilka talgrupper som respektive repeater är konfigurerad med som default.

Nu har vi använt oss v en hel del nya termer så vad passar då inte bättre än att söka efter dessa här i lathunden?

Lycka till!
