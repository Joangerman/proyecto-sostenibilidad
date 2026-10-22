# PROYECTO SOSTENIBILIDAD:

# Gestió intel·ligent de l'aigua a la UAB

Enfocament: Campus UAB

Tema: Crear un sistema intel·ligent per reduir el consum d'aigua al campus, mitjançant sensors que detectin el consum i les possibles fuites, juntament amb un dashboard que permeti visualitzar les dades i detectar consums anòmals.

1. Context i problema:
El campus de la UAB funciona com una petita ciutat: edificis de docència i recerca, laboratoris, residències, serveis de restauració, instal·lacions esportives i grans zones verdes amb reg. Això genera un consum d'aigua elevat i molt divers. Avui, la gestió es basa sobretot en lectures globals de comptadors i en revisions puntuals, de manera que una fuita o un ús excessiu pot passar setmanes sense detectar-se i només es nota quan arriba la factura. En un context de sequera recurrent a Catalunya, cada metre cúbic perdut té un cost econòmic i ambiental que es podria evitar.

2. Objectiu:
L'objectiu general és reduir el consum d'aigua del campus. Per aconseguir-ho, el projecte es proposa:
- Detectar fuites i usos anòmals gairebé en temps real.
- Saber quins edificis i zones consumeixen més i en quins moments.
- Donar als gestors informació clara i visual per decidir on actuar primer.

3. Descripció del sistema:
El sistema tindria quatre components que treballen en cadena:
- Sensors: comptadors i sensors de cabal instal·lats en punts estratègics, com l'entrada general, els edificis principals, la xarxa de reg i les zones d'alt consum (laboratoris, cafeteries, residències).
- Transmissió: les dades s'enviarien automàticament per una xarxa de baix consum, per exemple LoRaWAN, a una plataforma central.
- Emmagatzematge: la plataforma guardaria les mesures com a sèries temporals, ordenades per edifici, zona i hora.
- Detecció d'anomalies: unes regles senzilles revisarien les dades de manera contínua. Per exemple, un consum constant durant la nit en un edifici buit indicaria una possible fuita, i un pic fora de l'horari habitual o una desviació respecte al comportament normal de la zona generaria una alerta. Més endavant es podrien afegir models estadístics o d'aprenentatge automàtic per afinar la detecció.

4. El dashboard:
El dashboard seria la cara visible del sistema i la manera que tindrien els gestors de treballar amb les dades. Tindria un disseny semblant al que hem construït amb dades obertes, amb aquests elements:
- Mapa del campus amb els edificis acolorits segons el seu consum, per veure d'un cop d'ull on es concentra.
- Indicadors clau: consum total, litres per persona o per m², variació respecte a la setmana anterior i nombre d'alertes actives.
- Gràfics d'evolució diària i horària, i comparació entre edificis.
- Panell d'alertes amb la ubicació, l'hora i la magnitud del consum anòmal.
- Filtres per edifici, zona i període, que actualitzen tota la vista.

5. Beneficis esperats
- Ambientals: menys aigua perduda i un ús més responsable dels recursos.
- Econòmics: estalvi en la factura i reparacions més ràpides, que eviten danys més grans.
- De gestió: dades objectives per planificar inversions, com canviar la grifería o ajustar el reg segons el consum real.
- Educatius i socials: una eina de sensibilització per a la comunitat universitària i un laboratori viu de ciutat intel·ligent i sostenible, replicable en altres entorns urbans.

6. Fases del projecte
1. Diagnòstic: recopilar factures i dades existents, i cartografiar la xarxa d'aigua del campus per saber des d'on partim.
2. Disseny: triar els punts de mesura, els sensors i la xarxa de transmissió.
3. Pilot: instal·lar sensors en 2 o 3 edificis i en una zona de reg, per provar el sistema a petita escala.
4. Dashboard i alertes: desenvolupar la visualització i les regles de detecció, i calibrar els llindars.
5. Avaluació: mesurar l'estalvi aconseguit i ajustar el sistema.
6. Ampliació: estendre'l progressivament a la resta del campus.

7. Riscos i límits
- Cost: la instal·lació i el manteniment dels sensors poden ser elevats.
- Dades: si els sensors fallen o mesuren malament, les alertes perden fiabilitat.
- Coordinació: cal treballar amb el servei de manteniment del campus perquè les alertes es converteixin en actuacions.
- Falses alertes: és normal que n'hi hagi al principi, mentre es calibren els llindars.

8. Indicadors d'èxit
- Percentatge de reducció del consum d'aigua respecte a l'any anterior.
- Temps mitjà entre l'aparició d'una fuita i la seva detecció.
- Nombre de fuites localitzades i reparades.
- Litres estalviats.
- Proporció d'alertes que acaben sent reals.
