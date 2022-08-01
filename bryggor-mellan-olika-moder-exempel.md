# Bryggor mellan olika moder – exempel

Här följer ett exempel på en brygga av det lite mer avancerade slaget.

**SK3GA-L – TG7 / TG24033**

SK3GA är QRV med en brygga mellan Echolink och DMR. Denna brygga heter SK3GA-L med nod-id 721188. Bryggan körs på BrandMeister masterserver 2401. På klientsidan körs en AMBEserver på en Raspberry Pi4. Själva AMBE-transcoderingen sker i en AMBE3000 USB-sticka tillsammans med AMBE-servern. AMBE-servern är dessutom ansluten till AMPRnet med fast IP.

Vill du komma åt bryggan från DMR kör du via TG7 över SK3RHU UHF &/eller VHF. Vill du köra över bryggan från annan BrandMeisteransluten repeater eller hotspot kör du med TG24033. För både TG7 och TG24033 gäller group call.

TG7/TG24033 heter på BrandMeister SK3RHU Cluster.

Om man inte har ett DMR/CCS7-id då man sänder från Echolink så kommer den utgående signalen på DMR vara SK3GA.

Som om ovan inte vore nog så är SK3RHU Cluster bryggat till DCS010F på D-Star.
