# FAQ / Ordlista

Här kommer en liten FAQ /ordlista över begrepp som du kan stöta på.&#x20;

## RX Group List

RX Group List – används som en sorts digital squelch där man lägger in de talgrupper man önskar höra. Är det tyst i din radio bör du först kontrollera hur det ser ut i din RX Group List, är den tom så släpper din terminal inte igenom trafik.

## ARS (Automatic Registration Service)

ARS (Automatic Registration Service) – Motorola terminologi som beskriver en terminals funktion om att skicka positionsdata i nätet. Vi radioamatörer kan nyttja detta för att synas på t ex aprs.fi etc.

## RRS (Radio Registration Service)

RRS (Radio Registration Service) – Hytera-terminologi som beskriver en terminals funktion om att skicka positionsdata i nätet. Vi radioamatörer kan nyttja detta för att synas på t ex aprs.fi etc.

Till skillnad från ARS krävs inte denna tjänst för att möjliggöra platsrapportering på Hyteraradios med integrerad GPS-mottagare.

## Code Plug

Code Plug – på svenska kodplugg. Programmeringsfil för en radio.

## DMR-id

Ditt sjusiffriga DMR-id får du här; [https://www.radioid.net/](https://www.radioid.net/)

Historiskt så delades det ut enligt följande princip; 2400001 där 240 är landskoden för Sverige, den fjärde 0:an för distriktet och de sista tre siffrorna ett löpnummer.

Ovanstående princip har man frångått och delar numera enbart ut ID enligt följande princip; 240 för Sverige och sista fyra siffrorna är ett löpnummer.

## Hangtime

Private Call Hangtime och/eller Group Call Hangtime sätter tidslängden som terminalen ger användaren möjlighet att enbart trycka PTT för att svara ett anrop.

Exempel:

SM3UPI ligger med sin terminal på TG2403 och SA3BPE ropar på TG240 så kan man i programmeringen av SM3UPI´s terminal ange Group Call Hang Time på ex vis 6 sekunder. SM3UPI har då 6 sekunder på sig att trycka in PTT för att besvara SA3BPE´s anrop på TG240 utan att göra någon justering av sin terminal.

Detta förutsätter att funktionen överhuvudtaget finns – det skiljer sig (ofta) mellan de olika fabrikaten. Läs din terminals spec för info om detta.

Vidare så krävs det ju förstås att SM3UPI har programmerat sin terminal med rätta uppgifter om den repeater/hotspot som SM3UPI är QRV på.

Repeater/Hotspot´s inställningar och programmering spelar också in. Funktionen måste här vara aktiverad och rätt programmerad. Leta efter Hangtime-begreppet i ditt program (CPS) för respektive terminal.

## Masterserver

Masterserver – En server som håller reda på hotspots, repeatrar och användare. Denna routar oss rätt enligt det ID (talgrupp, individid eller klusterID) vi sänder ut.

## LoopBan

I varje BrandMeister masterserver körs något som kallas LoopBan för att förhindra loopar i nätet.

Om du sänder 5 gånger med en tid av mindre än 2 sekunder inom en period om 60 sekunder kommer du få ett röstmeddelande som säger ”User Blocked”.

Denna blockering är aktiv i 60 minuter på respektive masterserver som detekterat loopen.

Du kan häva blockeringen genom att temporärt ändra masterserver i din Hotspot eller repeater. Eller helt enkelt vänta de 60 minuter som blockeringen ligger aktiv.

Tänk på att inte aktivera funktioner som har liknande sändningsmönster som generar en blockering. För dig med Hotspot se till att BER är mindre än 1%.

## BER - Bit Error Rate

BER står för Bit Error Rate. Detta värde bör ej vara högre än 1 %. Ju närmare 0 % du kommer ju bättre är det. Speciellt viktigt att trimma in detta värde är om du kör hotspot eller repeater baserad på MMDVM-kort.&#x20;
