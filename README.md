# Lathund för DMR

![](.gitbook/assets/0)

![](.gitbook/assets/1)

![](.gitbook/assets/2)

**DMR – Digital Mobile Radio i Sverige**

**Lathund**

**En samproduktion mellan SSA & SWEDMR**

### TS – TimeSlot (tidslucka) <a href="#_toc68630449" id="_toc68630449"></a>

Tidsluckor är det som gör DMR-standarden unik. Din sändning är uppdelad i 30 mS digitala paket/luckor och sändaren slås snabbt på och av i denna frekvens. Genom att göra detta kan två signaler dela samma kanal samtidigt. En på Time Slot 1 och en på Time Slot 2.![](.gitbook/assets/4)

_Bildkälla:_ [_https://hvdnnotebook.blogspot.com/2018/06/a-tale-of-two-time-slots.html_](https://hvdnnotebook.blogspot.com/2018/06/a-tale-of-two-time-slots.html)

### TS1 (Time Slot 1) <a href="#_toc68630450" id="_toc68630450"></a>

TG91 ”Världen” länkad till alla repeatrar i hela världen

TG92 ”EU” länkad till alla repeatrar i EU

TG927 ”Norden” länkad till alla repeatrar i Norden (Island ej online ännu)

TG238 ”Danmark” (UA Timeout 15 min)

TG244 ”Finland” (UA Timeout 15 min)

TG242 ”Norway” (UA Timeout 15 min)

Alla andra Nationella / Regionala / Övriga talgrupper är också UA (User Activated) med en timeout på 15 minuter TS2 (Time Slot 2)

### TS2 (Time Slot 2) <a href="#_toc68630451" id="_toc68630451"></a>

TG240 – Svensk nationell talgrupp. Bör användas som talgrupp för anrop och sedan QSY till ledig talgrupp. Utländska samtal till Sverige förekommer och dessa bör besvaras, men håll dessa samtal korta.

TG7 – Cluster – Se respektive repeaterkonfiguration

TG8 – Cluster – Se respektive repeaterkonfiguration

TG9 ”Lokal” går bara ut över lokal repeater (UA Timeout 15 min)

TG2400 ”Regional SM0” länkad till alla repeatrar i SM0 (UA Timeout 15 min i övriga områden)

TG2401 ”Regional SM1” länkad till alla repeatrar i SM1 (UA Timeout 15 min i övriga områden)

TG2402 ”Regional SM2” länkad till alla repeatrar i SM2 (UA Timeout 15 min i övriga områden)

TG2403 ”Regional SM3” länkad till alla repeatrar i SM3 (UA Timeout 15 min i övriga områden)

TG2404 ”Regional SM4” länkad till alla repeatrar i SM4 (UA Timeout 15 min i övriga områden)

TG2405 ”Regional SM5” länkad till alla repeatrar i SM5 (UA Timeout 15 min i övriga områden)

TG2406 ”Regional SM6” länkad till alla repeatrar i SM6 (UA Timeout 15 min i övriga områden)

TG2407 ”Regional SM7” länkad till alla repeatrar i SM7 (UA Timeout 15 min i övriga områden)

TG2410 ”SSA Bulletin” länkad till DCS/XLX010D på D-Star (UA Timeout 15 min)

TG2411 ”Nationell” Taktisk QSO grupp till alla repeatrar i SM (UA Timeout 15 min)

TG2412 ”Nationell” Taktisk QSO grupp (UA Timeout 15 min)

TG2415 ”Nationell Taktisk QSO grupp länkad DCS010V” (UA Timeout 15 min)

TG2416 ”Swedenlink” länkad till Fusion m.m (UA Timeout 15 min

TG240216 ”Swedenhubb” (UA Timeout 15 min)

TG24080 ”SM XIL” (UA Timeout 15 min)

TG24098 ”Robust Packet” (UA Timeout 15 min)

TG24099 ”Normiraringen (UA Timeout 15 min)

TG9990 ”Papegoja” för audiotester (Obs privatecall)

TG240850 ”Tekniksnack” (UA Timeout 15 min)

240999 ARS-ID (För GPS, SMS etc.)

TG240240 ”Brygga till DCS010B/XLX010B” (D-Star)

(TG´s i denna färg är lämpliga talgrupper att QSY till från t ex TG240).

**Alla repeatrar behöver nödvändigtvis inte tillhandahålla allt ovan det är en fråga för respektive repeateroperatör hur de valt att göra… Detta är dock en systematisk rekommendation från sys.admin.**

UA (User Activated) fungerar genom att användare öppnar talgruppen vid första PTT-tryck. Timeout är 15 min efter senaste trafik.

För senaste uppdateringar om talgrupper i det svenska DMR-nätet, se: [www.swedmr.se](http://www.swedmr.se/) Här finns den kompletta listan.

De kanske viktigaste talgrupperna till en början är TG9 för att prata lokalt över en repeater eller DMO. TG240 är samlingstalgruppen för Sverige. TG240X, t.ex. TG2403 är TG för SM3-area.

TG4000 kopplar ner dynamiska talgrupper från respektive hotspot eller repeater du använder vid det givna tillfället. Notera att du ska sända med id 4000 som group call.

### Group Call & Private Call <a href="#_toc68630452" id="_toc68630452"></a>

Group Call är ett anrop från din terminal till en talgrupp.

Private Call är ett anrop mot enskild individ och dess terminal med respektive DMR-id.

### Kodplugg <a href="#_toc68630453" id="_toc68630453"></a>

Den fil som du gör iordning för din terminal kallas kodplugg. Innehåller den programmering som du vill använda terminalen till. T.ex. talgrupper, ditt ID, repeatrar och kontakter. Det rekommenderas varmt att du själv sätter ihop din kodplugg då du får en djupare förståelse om hur DMR fungerar.

### Color Code <a href="#_toc68630454" id="_toc68630454"></a>

För att hålla ett enkelt system kring Color Code, dvs en form av digital PL-ton/CTCSS, bör man följa följande principer (den högra siffran är för framtida bruk):

SM0 - 0 alt 8

SM1 - 1 alt 9

SM2 - 2 alt 10

SM3 - 3 alt 11

SM4 - 4 alt 12

SM5 - 5 alt 13

SM6 - 6 alt 14

SM7 - 7 alt 15

Observera att detta gäller såväl DMO ((Direct Mode Operation) direktförbindelse utan repeater eller hotspot), som TMO ((Trunked Mode Operation) Repeatrar & Hotspots).

### Frekvenser <a href="#_toc68630455" id="_toc68630455"></a>

DMO – enligt gällande bandplan för respektive band.

TMO – enligt gällande bandplan för respektive band, rådgör även/gärna med distriktets repeaterkoordinator om lämplig repeaterfrekvens.

![](.gitbook/assets/5)

_Bildkälla:_ [_https://www.teltronic.es/en/what-is-dmo/_](https://www.teltronic.es/en/what-is-dmo/)

### Trafikexempel <a href="#_toc68630456" id="_toc68630456"></a>

Jag vill ropa på min kompis SA3BPE? Då kan man med fördel göra ett individanrop med private call mot id 2403003 som SA3BPE har.

Jag vill ropa CQ och köra DX? Då gör du lämpligast det på **TG91**, här är det trafik dygnet runt. Se listan om talgrupper.

Jag vill samla min klubb till en informationssändning? Lämpligaste talgruppen för detta är respektive repeaters ID som TG, använd group call.

Jag vill leta efter en kompis i Tyskland? Då söker du upp din kompis DMR-id på [https://ham-digital.org/dmr-userreg.php](https://ham-digital.org/dmr-userreg.php) och ropar sedan med private call.

### Bryggor mellan olika moder – exempel <a href="#_toc68630457" id="_toc68630457"></a>

Här följer ett exempel på en brygga av det lite mer avancerade slaget.

**SK3GA-L – TG7 / TG24033**

SK3GA är QRV med en brygga mellan Echolink och DMR. Denna brygga heter SK3GA-L med nod-id 721188. Bryggan körs på BrandMeister masterserver 2401. På klientsidan körs en AMBEserver på en Raspberry Pi4. Själva AMBE-transcoderingen sker i en AMBE3000 USB-sticka tillsammans med AMBE-servern. AMBE-servern är dessutom ansluten till AMPRnet med fast IP.

Vill du komma åt bryggan från DMR kör du via TG7 över SK3RHU UHF &/eller VHF. Vill du köra över bryggan från annan BrandMeisteransluten repeater eller hotspot kör du med TG24033. För både TG7 och TG24033 gäller group call.

TG7/TG24033 heter på BrandMeister SK3RHU Cluster.

Om man inte har ett DMR/CCS7-id då man sänder från Echolink så kommer den utgående signalen på DMR vara SK3GA.

Som om ovan inte vore nog så är SK3RHU Cluster bryggat till DCS010F på D-Star.

### Att hitta en repeater i närheten <a href="#_toc68630458" id="_toc68630458"></a>

Det finns flera sätt att hitta uppgifter om din lokala repeater. Det kanske enklaste sättet är att leta i databasen [https://www.ssa.se/vushf/repeatrar-fyrar/](https://www.ssa.se/vushf/repeatrar-fyrar/) Detta förutsätter naturligtvis att repeaterägare har registrerat sin repeater i denna databas.

Här följer ett exempel på hur man får fram SK3RHU VHF DMR. Jag har klickat in på länken ovan och zoomat in på Hudiksvall och valt SK3RHU VHF DMR.

![](.gitbook/assets/6)

Om du nu klickar på det jag markerat med gult, ”Brandmeister Network” så kommer du till en sida som ser ut enligt nedan. Här hittar information om vilka TG’s som repeatern är kopplad mot under ”Slot details”.

![](.gitbook/assets/7)

Om vi fortsätter vår djupdykning i detaljerna för fältet ”Slot details” så ser man under timeslot 1 och 2 att det ligger lite olika talgrupper aktiva.

![](.gitbook/assets/8)

TG med hänglås är en statisk talgrupp på repeatern.

TG med blixtsymbol är en dynamisk talgrupp som är User Activated.

TG med klocksymbol är en tidsatt statisk talgrupp.

TG med nio ”pluppar” (7 ->> 24033) är en klustertalgrupp.

### Smarta tjänster - SMS <a href="#_toc68630459" id="_toc68630459"></a>

Här kommer ett litet smart tips om SMS-funktioner i det svenska DMR-nätet (BrandMeister).\
BrandMeister-nätverket har vissa funktioner för att begära information via SMS. För att få åtkomst till dessa funktioner ska specifika nyckelord skickas till **DMR ID 262993** (private call). Då svarar systemet via SMS på dessa förfrågningar. Nedan hittar du en översikt över kommandon med en enkel förklaring. Kommandona är inte skiftlägeskänsliga. Detta är en tysk tjänst och mer info kan hittas här; [http://wiki.bm262.de/doku.php?id=servicenummer](http://wiki.bm262.de/doku.php?id=servicenummer)

| **Kommando**    | **Förklaring**                                                            |
| --------------- | ------------------------------------------------------------------------- |
| help            | Visar en översikt av funktioner                                           |
| echo            | Ett svar fås per omgående om du konfigurerat SMS rätt i din terminal      |
| wx              | Väder på repeatersiten                                                    |
| wx help         | Översikt av tillgängliga kommandon                                        |
| wx Hudiksvall   | Väder i angiven stad ’Hudiksvall’                                         |
| wx zip Town     | Väder i angivet postnummer och stad                                       |
| wx zip, cc      | Väder i angivet postnummer och land                                       |
| wx Town, cc     | Väder i angiven stad och land                                             |
| wx zip Town, cc | Väder i angivet postnummer, stad och land                                 |
| wx gps          | Väder för din senaste sända GPS-position                                  |
| metar xxxx      | METAR flyplatskod ICAO ’xxxx’ (ex: Arlanda = ESSA)                        |
| gps help        | Översikt över alla GPS-kommando som är tillgängliga                       |
| gps             | Visar aktuell GPS-position i förhållande till den repeater du sänder över |
| gps set         | Sparar aktuell GPS-position som din hemposition                           |
| gps home        | Visar avstånd och riktning till din angivna hemposition                   |
| gps callsign    | Visar avstånd och riktning till angivet callsign                          |

### Om dokumentet <a href="#_toc68630460" id="_toc68630460"></a>

Detta dokument är en samproduktion mellan SSA – Föreningen Sveriges Sändareamatörer Digitalsektionen och intressegruppen SWEDMR för att göra det enklare att komma igång med DMR i Sverige.

Lathunden är publicerad under Creative Commons licens CC BY-NC 2.5 SE – se [https://creativecommons.org/licenses/by-nc/2.5/se/](https://creativecommons.org/licenses/by-nc/2.5/se/)

2022-08-01 Hudiksvall

SA3BPE - Henrik

Korrektur och faktagranskning utfördes fram till 2022-07-21 av SM0TSC Johan. Vila i frid Johan! <3

![](.gitbook/assets/9)
