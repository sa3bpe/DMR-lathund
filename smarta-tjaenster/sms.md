# SMS

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

För att aktivera "TextCapture" (så att dina SMS når dig fast din terminal är avslagen), se; [https://news.brandmeister.network/new-textcapture-feature-the-sms-store-and-forward-service-you-can-now-enable-in-your-self-care/](https://news.brandmeister.network/new-textcapture-feature-the-sms-store-and-forward-service-you-can-now-enable-in-your-self-care/)
