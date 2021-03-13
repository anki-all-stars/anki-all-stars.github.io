---
title: BI-PSI
layout: page
---


<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Týden 1


|Otázka|Odpověd|Poznámky|
|--------|---------|----------|
|Druhy přepojování sítě|Okruhy - sestavená trasavs<br>Pakety - balíček odesílaných dat||
|Druhy architektury komunikace|- Peer to peer- Client-server||
|Taxanomie sítí dle rozhlehlosti|Personal Area Network - PAN ~~ 1mLocal Area Network - LAN ~~ 100mMetropolitan Area Network - MAN ~~ 10 kmWide Area Network - WAN ~~ 1000km||
|Definuj topologii|Způsob uspořádání propojení mezi stanicemi v síti, nejvhodnější topologie souvisí s kontkrétním použitím||
|Jak vypadá topologie "Ring"?|<img src="media/paste-ab065705de9b427fa7ffd567cfc378c411452f55.jpg">||
|Jak vypadá topologie "Mesh"?|<img src="media/paste-006047b03830c375dd9ed177432c2a50997bb056.jpg">||
|Jak vypadá topologie "Star"?|<img src="media/paste-3bc38dd94610bd03ff683efa0249378b99517b03.jpg">||
|Jak vypadá topologie "Fully Connected"?|<img src="media/paste-303606008db6ffd914db43f45a3f8dcab4823cc0.jpg">||
|Jak vypadá topologie "Line"?|<img src="media/paste-8dc5a83f81a6d6b05a3b564ab36a708ec5946a37.jpg">||
|Jak vypadá topologie "Tree"?|<img src="media/paste-0d68118a5afe0d641c402ae47519bc238c39da9f.jpg">||
|Jak vypadá topologie "Bus"?|<img src="media/paste-8e5de0895f29ad8ac0c5814e92518b182f73f803.jpg">||
|Jaké jsou druhy linek v počítačových sítích?|<img src="media/Isa4AaJm7cZ78h6AnVnaQhIyMxM9Q-BlJlKZ2EGaPdo.original.fullsize.png">||
|Definuj unicast komunikaci|Komunikace mezi dvěma účastníky v síti, identifikovány adresami|musí nutně být cíl zvolen? \( Např DHCP \)|
|Definuj broadcast komunikaci|Komunikace vyslána za účelem přijetí každým účastníkem v sítí||
|Definuj multicast komunikaci|Komunikace, kde pakety jsou adresovány více než jednomu zařízení||
|Definuj anycast komunikaci|Komunikace komunikace zařízení s více možnými destinacemi||
|Vyjmenuj OSI vrstvy|AplikačníPrezentačníRelačníTransportníSíťováSpojováFyzická||
|Kolik bitů má IPv4|32 bitů, 4 byty||
|Definuj síťovou masku|Síťová maska je bitová maska o stejné velikosti jako IP adresa, která vyjadřuje jakou část IP adresy mají všichni členové dané sítě společnou||
|Definuj prefixovou notaci IPv4|X.X.X.X/Y se nazývá prefixová notace IP adresy, právě když X.X.X.X je IP adresa a Y je přesně počet jedniček zleva v bitové masce.&nbsp;<br><img src="media/paste-35957bff68def88904b6547606cfa6ad5234eb83.jpg"><br>||
|Definuj adresu sítě|Adresa sítě je označení všech IP adres, které patří do daného rozsahu. Lze ji vypočítat pomocí ANDu masky a libovolné adresy v síti.<br>Zároveň je to také nejnižší adresa v rozsahu.||
|Definuj broadcast IPv4 adresu v daném rozsahu|Broadcase je nejvyšší adresa v daném rozsahu||
|Jakou adresu typicky má brána v daném rozsahu?|Brána má typicky \( nikoli povinně \) druhou nejvyšší či nejnižší adresy v daném rozsahu||
|Jakým způsobem vypočítáme počet možných stanic v závislosti na délce prefixu L masky?|Nechť&nbsp;\\(K = 32 - L\\)<br>Pro nalezení minimálního&nbsp;\\(N\\), musí platit, že&nbsp;\\( K &lt;= 2^N \\)<br>Počet využitelných stanic v síti je&nbsp;\\(2^N - 3\\) \(odebrána broadcast, adresa sítě, brána\)||
|<img src="media/V-e2fU7xG9iAtF2LxMNbO-a5qSKwBI9CAyuJ8QoNXUo.original.fullsize.png"><br><img src="media/paste-b0ba116779dfdd10209665ad2ecb283941efadb5.jpg"><br>|<img src="media/paste-1c2a2382abb80b550cb828ce3673014b714a2edc.jpg">||
|<img src="media/fTU21cMQivKSNvJJs01JilcAIyjOapAgIpvruYLjcKU.original.fullsize.png"><img src="media/paste-92a20839b5147fbcedb1f57ce48759642580ef2a.jpg"><br>|<img src="media/FJtaP0ndp9yyd0M9QzgP1mhQHl58p3BdrgSw2CE1D6Q.original.fullsize.png">||


# Týden 2


|Otázka|Odpověd|Poznámky|
|--------|---------|----------|
|Jaký je účel linkové vrstvy?|Přenášení dat v rámci LAN či MAN sítě.||
|Jakou základní přenášecí jednotku má linková vrstva?|Rámec||
|Jaké části má rámec?|<img src="media/paste-7efd881ceaec8f86ee01a1e17a807dc0c669aa81.jpg">||
|Co určuje maximální velikost rámce?|MTU - Maximum Transfer Unit - závislé na typu a chybovosti použitého média||
|Co zajišťuje MAC podvrstva? \(3\)|Přístup k médiuSdílení média pomocí multiplexu, popř. přístupových metodFiltrování MAC adres||
|Je MAC podvrstva závislá na použitém médiu?|Ano||
|Co zajištujě LLC podvrstva?|Řízení toku, kontrolu chybRozdělení toku z vyšších vrstev do rámců \( framing \)&nbsp;=&gt; Musí určovat velikost rámce, konec rámce||
|Je LLC vrstva závislá na použitém médiu?|Ne||
|Co je to multiplex?|Technika umožňující současné použití stejného přenosového média více účastníky||
|Co je kolizní doména?|Je množina stanic, které sdílí společné médium. Současné vysílání 2 anebo více stanic vede ke kolizi.||
|Jakým způsobem dělí přístup k médiu časový multiplex? \( TDMA \)|Podle časových intervalů, v jednom konkrétním časovém okamžiku, má přístup k médiu pouze jeden účastník.<img src="media/paste-7199091a72e7c6b8d0d80b402ab89381619428ef.jpg"><br>||
|Jakým způsobem dělí médium frekvenční multiplex? \( FDMA \)|Pomocí frekvenčních pásem - každý účasník používá jiné frekvenční pásmo - díky tomu se neovlivňují<img src="media/paste-d0f6a7c7fa45d11a85035038ecba6a4a9110d1c5.jpg"><br>||
|Kódový multiplex? \( CDMA \)|Médium využívaí v konkrétním časovém okamžiku více účastníků, ale každý účastník zpracovává pouze to, čemu rozumí, co je v jeho kódu.<img src="media/paste-c3a67bdba297b6ce24b02b6609c56443be7616ae.jpg"><br>||
|Prostorový multiplex? \( SDMA \)|Médum současně využívá několik různých účastníků díky tomu, že konrkétní vysílání prochází různými vzájemně se nepřekrývajícími směry.<img src="media/paste-3401187d23fa8434d15fa4f2c54e4e1d9fbcbd4e.jpg"><br>||
|Co je to broadcast doména?|Je množina všech stanic, kterým je doručen rámec s všesmerovou adresou. Jednotlivé broadcastové domény od sebe oddělují až zařízení pracující na síťové \(3.\) vrstvě OSY modelu \( směrovače \)&nbsp;||
|Nakresli princip metody CSMA/CD|<img src="media/paste-e78382aa413815091404ec7b66f1837fb5482eb5.jpg">||
|Nakresli princip metody CSMA/CA|<img src="media/paste-95e8626bce775ae849a78e25ca60baff713da4bb.jpg">||
|Co je kolizní okénko?|KO je doba od začátku vysílání, behem kterého se rozšíří signál po médiu. V tomto čase mohou začít vysílat i další stanice, než k nim dorazí informace, že vysílá někdo jiný.||
|Popiš potvrzovací schéma: Jednotlivé potvrzování|<img src="media/paste-b030b871066d1a13ffaba5e2f80886fe5e1f1785.jpg">||
|Popiš potvrzovací schéma: Kontinuální potvrzování se selektivním opakováním|<img src="media/paste-f7b4a35b494e3c4630e334e8f08f1a92f455c470.jpg">||
|Popiš potvrzovací schéma: Kontinuální potvrzování s návratem|<img src="media/paste-f4b0d5c794ea38011221da6ae6c363344ccc3a45.jpg">||
|Popiš potvrzovací schéma: Klouzavé okénko|<img src="media/paste-4144de99a27b67cbcede20ef2db62a235a5bdc85.jpg">||
|Co slouží pro detecki chyb v rámci linkové vrstvy?|Hammingovy kódy||
|Co je to přepínač?|Zařízení, jehož funkcí je přepínání rámců.<br>Přepínání rámců znamená přijetí tohoto rámce, zpracování a odeslání rámce směrem k příjemci pomocí přepínací tabulky||
|Jaké jsou režimy práce přepínačů?|Store-And-Forward - přepínač přijme celý rámec před odeslánímCut-Trough - přepínač přijme hlavičku, zkontroluje a odesílá zbytek okamžitě||
|Jaký je rozdíl mezi mostem a přepínačem?|Most je jednodušší zařízení, nemá žádný buffer, může být i softwarovýPřepínač je složitější, má hodně portů, má HW podporu pro přepínání||
|Popiš obecný formát rámce ethernetu|<img src="media/paste-096d697a06ef722129d5ae6bc9d38398ea89b52f.jpg">||
|Z čeho se skládá MAC adresa v ethernetu?|<img src="media/paste-47dfa29ffb15d165065d49a734ed823e18f0a5b7.jpg">||
|Jaká je všesměrová \( broadcast \) MAC?|FFFF FFFF||
|Kdy je potřeba autonegociace?|Při poškozém vodiči, nebo u zařízení které nemají stejnou verzi protokolu, novější se přizpůsobí starším||
|Co je autonegociace?|Metoda, kterou si vysílač a příjmač dohodnou parametry přenosu||
|Obsahuje ethernet zaručení spolehlivého doručení dat?|Ne||
|Co je ethernetový příkaz PAUSE?|Pokud přepínač nestíhá, může vyslat příkaz PAUSE aby jeho sousedé zpomalili||
|Jaký je rozdíl mezi přímým \( patch cord \) a skříženým \( crossover \) kabelem?|Crossover kabel není symetrický - příjem jedné strany je opačnou stranu vysíláním a naopak||


# Týden 3


|Otázka|Odpověd|Poznámky|
|--------|---------|----------|
|Co znamená VLAN a k čemu je určená?|<img src="media/paste-dddb7e1e27ee2378ce93cb58c65ee3ec74038ee8.jpg">||
|Jaké jsou výhody VLAN?|<img src="media/paste-f1297e0830916e17eca105a7904697537aad6bfc.jpg">||
|Co je TRUNK port?|<img src="media/paste-0c69a201c8971478a987256bb20247dbe82fa1c2.jpg">||
|Podle čeho se dělí VLAN v režimu dělení dle portů?|<img src="media/paste-54f45de00a09370b770dee6ef4b1ed1215fbd070.jpg">||
|Podle čeho se dělí VLAN v režimu dělení dle adres?|<img src="media/paste-1bdbac87e51f45bfb9a63d695eb5cca70ed91a61.jpg">||
|Podle čeho se dělí VLAN v režimu dělení dle protokolu?|<img src="media/paste-2af44769df7a48fe2c26a99a6eaef59a710734af.jpg">||
|Podle čeho se dělí VLAN v režimu dělení dle značky?|<img src="media/paste-4a2cd3d3d4d00da2000707836959db56006296f3.jpg">||
|Jak vypadá VLAN otagovaný ethernet rámec?|<img src="media/paste-f724e4d07b04bfd3d022095c538b8b42c973f4db.jpg">||
|Jaké je účel síťové vrstvy?|<img src="media/paste-66764930a6e937128d2ee23425da579febad80da.jpg">||
|Co znamená IP? Jak je dlouhá? K čemu slouží?|<img src="media/paste-12364e148326c17f21846dd2b6f19bc8257c31aa.jpg">||
|Jaký je rozdíl mezi CIDR a třídami IP adresace?|<img src="media/paste-c9e0e7d17a07873bf3818da476bb9b8261b9da04.jpg">||
|Jaké jsou unicastové třídy IP adresace a jaké mají masky?|<img src="media/paste-40ee8ef22766f4dc69c8d4ccca2976d94661db7f.jpg">||
|Definuj IP packet|<img src="media/paste-75c80480afa67167a0a8efb643d7aac19affb89d.jpg">||
|Popiš princip IP směrování|<img src="media/paste-e0eac5b4837e553bc9096c57b3241c3d07bfd785.jpg">|FIX THIS|
|Kdy se IP packety fragmentují?|Pokud je velikost IP paketu větší, než maximální velikost datové části rámce.&nbsp;||
|Kdy se fragmentovaný IP datagram skládá?|Až na cílové stanici||
|Je možné zabránit fragmentaci IP paketů?|<img src="media/paste-728b4b99c27f0ed16d295e119b8c18b9a8a8271b.jpg">||
|Co je NAT?|<img src="media/paste-c85621c40054edbc7ebbf6561fa3c217c819b9b3.jpg">|FIX THIS|
|K čemu slouží protokol ICMP?|<img src="media/paste-27b3bd189c77a15ec8f3a9faae15b32cc0118b92.jpg">||
|Jaké utility používají protokol ICMP?|<img src="media/paste-1affacb7c8a5f9792288f6e1644ef90f9f53b396.jpg">||
|K čemu slouží protokol ARP?|<img src="media/paste-db32b2905bba7157ee9146c14b6e23eb47f27bf4.jpg">||
|Jak probíhá ARP spoofing?|<img src="media/paste-fe1317e3962f0e1723256002ed88a3c3789cb080.jpg">||


# Týden 4


|Otázka|Odpověd|Poznámky|
|--------|---------|----------|
|Popiš datagram IPv6|<img src="media/paste-473cec913d01ed0b1a5e6a8371f213fe976f4281.jpg">||
|Co je zřetězování hlaviček v IPv6?|V IPv6 každá hlavička reprezentuje samotný blok dat a pro jejich spojování se používá hlavička "next header". Výhodou j přenášení pouze užitečných informací||
|Definuj příjemce IPv6 unicast adresu|Určené jednoznačnému příjemci||
|Definuj příjemce IPv6 multicastu|určeny pro určitou skupinu příjemců||
|Definuj příjemce IPv6 anycast|doručí se pouze jedinému členu určité skupiny \(alespoň někomu\)||
|Má IPv6 multicast adresy?|Ano||
|Má IPv6 broadcast adresy?|Ne||
|Jak vypadá IPv6 kompatibilní režim s IPv4 adresou A.B.C.D?|::ffff:A:B:C:DAle A, B, C, D musí být zapsané hexadecimálně||
|Jaká je loopback adresa v IPv6?|::1/128||
|Jak odvodit IPv6 adresu z MAC adresy?|Horních 64 bitů je adresa sítě.Spodních 64 bitů je adresa zaříení, odvozena pomocí:<img src="media/paste-5ec06355dd1a97f233797b7143edae7fd1bd38b9.jpg">||
|Jaké jsou lokální IPv6 adresy?|<img src="media/paste-49b8cd20f229124cb613764fa59f1bbe60864808.jpg">||
|Jak vytvořit IPv6 multicast adresu?|<img src="media/paste-bc512d146d36a790c83212abcc6502cd113ed3b9.jpg">||
|K čemu se využívá AnyCast \( v IPv6 \) ?|Např. DNS||
|Jaké funkce má ICMP IPv6?|Testování chybových stavů, dosažitelnost, výměna provozních zařízení, <b>objevování sousedů</b>||
|Co je objevování sousedů v IPv6?|Náhrada protokolu ARPPodporuje:Hledání směrovačů, přesměrování, zjišťování linkových adres, DHCP, ...||
|Jak probíhá výzva směrovači v IPv6? Co se stane potom?|Klient, který se chce připojit do sítě pošle výzvu směrovačiSměrovač odpoví prostřednictvím ohlášení směrovače<br><img src="media/paste-a5cd7697f2113a43946402d043edee0322b703e6.jpg"><br>||
|Jak probíhá zjištění linkové adresy u IPv6?|Pomocí výzvy sousedovi.&nbsp;Používá prefix ff02::1:f00:/1004<br>1. Konstrukce adresy2. Speciální ICMP zpráva -&gt; výzva sousedovi3. Jinde proběhne přijmutí a následné ohlášení souseda4. Přijetí linkové adresy souseda a uložení do cache||
|Jaké jsou stavy adres v tabulce sousedů IPv6?|<img src="media/paste-8823bca60b54e007b54464f49911847694ecfb51.jpg">||
|Co zařizuje IPv6 inverzní objevování sousedů?|Jedná se o inverzní mechanismus objevování sousedů<br>Tj. linková adresa nějakého zařízení je známá a potřebujme znát odpovídající IPv6||
|Co jsou implicitní směrovače u IPv6?|IPv6 uzly jsou většinou schopny směrovat samy, ale u naprosto neznámé adresy musí mít nějaké východisko - implicitní směrovač<br><img src="media/paste-919510c1b9542f8429e4ca1a864adc852252633b.jpg"><br>||
|Popiš proces směrování u IPv6|<img src="media/paste-018086df6d06a6c249e91e1ebf4fe5c082867dfa.jpg">|TODO improve this image|
|Co přiděluje DHCPv6 server?|Pouze adresu||
|Jak probíhá DHCPv6 komunikace?|<img src="media/paste-a60bd487862a6f1dbe025b99c2156288b1234918.jpg">||
