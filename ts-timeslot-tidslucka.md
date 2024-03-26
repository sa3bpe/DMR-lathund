# TS – TimeSlot (tidslucka)

Tidsluckor är det som gör DMR-standarden unik. Din sändning är uppdelad i 30 mS digitala paket/luckor och sändaren slås snabbt på och av i denna frekvens. Genom att göra detta kan två signaler dela samma kanal samtidigt. En på Time Slot 1 och en på Time Slot 2.![](.gitbook/assets/4)

_Bildkälla:_ [_https://hvdnnotebook.blogspot.com/2018/06/a-tale-of-two-time-slots.html_](https://hvdnnotebook.blogspot.com/2018/06/a-tale-of-two-time-slots.html)

TDMA (Time Division Multiple Access) är en annan benämning på denna funktion i DMR-standarden Tier-2 som nämns i bilden ovan. 

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
