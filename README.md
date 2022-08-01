# Lathund för DMR

![](.gitbook/assets/0)

![](.gitbook/assets/1)

![](.gitbook/assets/2)

**DMR – Digital Mobile Radio i Sverige**

**Lathund**

**En samproduktion mellan SSA & SWEDMR**

### &#x20;<a href="#_toc68630455" id="_toc68630455"></a>

### &#x20;<a href="#_toc68630456" id="_toc68630456"></a>

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
