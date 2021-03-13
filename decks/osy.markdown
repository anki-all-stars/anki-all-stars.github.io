---
title: BI-OSY
layout: page
---


<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Týden 1


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Popiš model výpočetního systému|<img style="height:128px;width:auto;" src="media/SnLwAfUS_OOyKLrg-n8Br4vKP9bCZN5VouY51jrl8m4.original.fullsize.png">||
|Co je ISA?|Instruction Set Architecture&nbsp;- Definuje množinu instrukcí, adresní režimy, ...&nbsp;- Definuje množinu registrů, organizace paměti, organizaci V/V&nbsp;- Privilegované úrovně \( módy \)&nbsp;||
|Popiš privilegované módy v procesorech od Intelu|<img style="height:128px;width:auto;" src="media/paste-12dce5e156fe4861fe99271998a594c99096a3f3.jpg" style="color: var\(--text-fg\);"><br>||
|Jaké jsou dva základní privilegované módy?|<img style="height:128px;width:auto;" src="media/paste-1b3ac257149c4d307951ccd253ad96098bc275cc.jpg">||
|Jaké je rozdělení procesorů podle typu instrukcí?|CISC \( Complex Instruction Set Computer \)RISC \( Reduced Instruction Set Computer \)||
|Popiš typy instrukcí CISC|<img style="height:128px;width:auto;" src="media/paste-0b9489733f4ffe11826b86e6bb15c06698c06dae.jpg"><img style="height:128px;width:auto;" src="media/QLRjc3iLcDjSZCnskoc9mKKl1_mxpOm7oRdPHVLjM3Y.original.fullsize.png"><br>|<img style="height:128px;width:auto;" src="media/nNnst4_qAOcEHrrI79949aHMoSi4mFWCnZ5Valkiagg.original.fullsize.png">|
|Popiš typy instrukcí RISC|<img style="height:128px;width:auto;" src="media/paste-3e1c680f4ee725406a9455de533b61dd5f9d5968.jpg"><img style="height:128px;width:auto;" src="media/rlQBnmnBvXHgrF_sN9UOK1GBZfqkmVwsd8KuJP9QUak.original.fullsize.png"><br>|<img style="height:128px;width:auto;" src="media/nNnst4_qAOcEHrrI79949aHMoSi4mFWCnZ5Valkiagg.original.fullsize.png">|
|Uveď a větou popiš fáze zpracování instrukcí v CPU|<img style="height:128px;width:auto;" src="media/paste-6207578e60f931522e7f12039cc4f398e7dee9dd.jpg">|<img style="height:128px;width:auto;" src="media/9EXxdVYDERHPlrbQMwE2Ux_-a8b1sv5-3VhN81Qlfdg.original.fullsize.png">|
|Popiš proudové jednotky v CPU|<img style="height:128px;width:auto;" src="media/Z_EtBFjheaBkiQF8uFvWnDyD40efWu3-8jFoXMoSMTQ.original.fullsize.png">||
|Jaké je rozdělení procesorů podle pořadí zpracování instrukcí?|<img style="height:128px;width:auto;" src="media/wyndYyyaQr_1KwjAwYqr33-INX63pEHFzEhS0e7X7HM.original.fullsize.png">||
|Jaké je rozdělený procesorů podle počtu jader?|<img style="height:128px;width:auto;" src="media/VU2jFqOdce0m5aPq_f7HbNvlOmZg4T6JxBP9r_ye8yA.original.fullsize.png">||
|Jakým způsobem dokáže jedno CPU na jednom jádře vykonávat více instrukčních proudů?|Pomocí hyper-threading \(Intel\) a multi-threading \(SPARC T\)|<img style="height:128px;width:auto;" src="media/_3mj2jeU2N0tf1e3kufGw462F1L95IvGhOp_aAeAhJg.original.fullsize.png">|
|Co jsou přerušení?|Asynchronní reakce na nějakou událost. Normální zpracování instrukčního proudu jádra je přerušeno a začne se provádět obslužná rutina přerušení.|<img style="height:128px;width:auto;" src="media/tB1mgvE95H5kLitDFh_IoQGJs5wccUMR4NXkau_hR_I.original.fullsize.png">|
|Kdy dochází k přerušení?|Při přepnutí do jiného módu CPUPři chybě \(např. dělení nulou\)<br>Když V/V zařízení žádá o pozornost \(V/V je češtinsky pro I/O\)<br>Generováno řadičem zařízení při dokončení opreace / chybě|<img style="height:128px;width:auto;" src="media/Ed57hm6WYurkmZTkbC50PRxz3X6eGaKsUpBRoEaORQw.original.fullsize.png">|
|Druhy rychlé paměti|NVRAMRAM||
|Co je sběrnice?|Zajišťuje přenos dat a řídících povelů mezi jednotlivými částmi||
|Co znamená UMA|Uniform memory access||
|Popiš jak funguje UMA|U systému, který se skládá z něolika identických jader, které jsou porpojena sdílenou sběrnici a všchny jádra sdílí stejnou pamět, přístupový čas do paměti je pro všechny jádra téměr stejný<br>Místy označována jako SMP \( symmetric multiprocessor \)||
|Co je NUMA|Non-uniform memory access||
|Popiš architekturu NUMA|Lokální pamět uzlu je viditelná pro jádra z ostatních uzlůPřístup do vzdálené paměti je pomalejší než do lokální pamětiOS má znalost o paměťových latencích a může ji využívat při plánování jader||


# Týden 2


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Definuj program, jeho reprezentaci|Program je sled instrukcí. V systému reprezentován spustitelným binárním programem, který je uložený v sekundární paměti \(např. disk\).||
|Definuj proces|Instance spuštěného programu/aplikace.<br>Jsou v rámci něho alokovány prostředky \(pamět, vlákna, ...\)||
|Co dědí nový proces po rodičovském procesu|Např. tabulka deskriptorů souborů||
|Co nedědí nový proces po rodičovském procesu|Např. číslo procesu||
|Definuj vlákno \( neboli light weight process \)|Výpočetní entita \( proud instrukcí \), které je přidělováno jádro CPU<br><br>Jádro OS si pro každé vlákno udržuje informace: identifikaci, zásobník, kontext ...&nbsp;||
|Popiš Multitaskng|<img style="height:128px;width:auto;" src="media/paste-e32893c7b2d727a39c03fc4cde546e4f08d8a714.jpg">||
|Popiš multithreading|<img style="height:128px;width:auto;" src="media/paste-22300cc89aaf75793d642e6c01bb2880867ece4a.jpg">||
|Jaké existují druhy vytvoření nového procesu?|Kopie, klon přes&nbsp;\\(fork\\)Úplně nový proces přes&nbsp;\\(execve\\)||
|Popiš syscall fork|<img style="height:128px;width:auto;" src="media/paste-651bb4e8620b8734dfee30f73f6b4cc5d2b91982.jpg">||
|Popiš syscall execve|<img style="height:128px;width:auto;" src="media/paste-7d402ada74e404a64a0408438ebe533f681a17ee.jpg">||
|Popiš syscall wait|<img style="height:128px;width:auto;" src="media/paste-800cdd1e4227e341084ec38091dcefa858064498.jpg">||
|Jakým způsobem se může ukončit proces?|Proces se ukončí sám \(dojde na konec programu, nebo dojde k zavolání exit\(\)\)Proces je ukončen jádrem \(dojde k fatální chybě\)||
|Kroky OS při ukončení procesu|Pokusí se předat návratový kód rodičiUkončí všechna vlákna, která existují v procesuUvolní adresový prostor||
|Popiš syscall pthread_create|<img style="height:128px;width:auto;" src="media/paste-9ac0bbf077f7502274dcf014fcb90a750c9b8c12.jpg">||
|Popiš syscall pthread_join|<img style="height:128px;width:auto;" src="media/paste-b8316c5d1bc39a540cc01b5b37c0be2017abecb7.jpg">||
|Jakým způsobem je přiřazen čas vláknům při preemptivním plánování?|<img style="height:128px;width:auto;" src="media/paste-c2a5fb19e3291f811f8fcfb19255df27bdbea9d1.jpg">||
|Co je nejčastější způsob plánování vláken?|Preemtpivní plánování vláken||
|Kdy je potřeba přepínat kontext?|Když se vlánka střídají ve využívání CPU||
|Co je kontext vlákna?|Všechny nezbytné informace, které jsou nutné pro pozdější spuštění přerušeního vlákna od okamžiku přerušení||
|Fáze přepínání kontextu|Uloží se kontext původního vláknaJádro OS naplánuje další vláknoNastaví se kontext tohoto vlákna||
|Vyjmenuj možné stavy vláken a přechody mezi nimi|<img style="height:128px;width:auto;" src="media/paste-2dc1e5dcd3fb7856ea5b3258d62127c7ed170b8a.jpg">||
|Co jsou časové závislé chyby?|Situace, kdy dvě nebo několik vláken používá \(čte / zapisuje\) společné sdílené prostředky a výsledek deterministického algoritmu je závislý na rychlosti jednotlivých vláken||
|Co je to kritická sekce a sdružená kritická sekce?|<img style="height:128px;width:auto;" src="media/paste-43c8469f11c22ae221f3ba2dad1f54ac2f7462d9.jpg">||
|Kdy vlákno nesmí do kritické sekce díky vzájemnému vyloučení?|<img style="height:128px;width:auto;" src="media/paste-46caa55c6e9e673faabe2b70f47480663af377df.jpg">||
|Jaké jsou pravidla psaní paralerních programů|Žádné předpoklady nesmí být kladeny na rychlost vláken a počet jader<br>Zajistit výlučný přístup ke sdíleným prostředkům<br>Mimo kritickou sekci by vlánko nemělo být blokováno \( zpomalováno \) ostatními vlákny||


# Týden 3


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Definuj Deadlock|<img style="height:128px;width:auto;" src="media/paste-ceb0223f5bd8d40d8881886c98585ace843f1023.jpg">||
|Definuj livelock|<img style="height:128px;width:auto;" src="media/paste-b560d9375cb14595726c545ae079c7c68aa1f491.jpg">||
|Definuj hladovění vlákna|<img style="height:128px;width:auto;" src="media/paste-52906e7c6ae9f1cf5ae32dae39b5735214d3f6c0.jpg">||
|Základní rozdělení způsobů synchronizace vláken|Aktivní čekáníBlokující systémová volání||
|Popiš aktivní čekání \(proměnné, před vstupem do krit. sekce, po opuštění krit sekce\)|<img style="height:128px;width:auto;" src="media/paste-30f449989def76217b8b9d8f878ea7cc8217a6fa.jpg">||
|Popiš naivní implementaci aktivního čekání pomocí jedné proměnné a proč nebude fungovat|<img style="height:128px;width:auto;" src="media/paste-2aef09889549f128697cb7eb9e40d5a263deb5cd.jpg"><img style="height:128px;width:auto;" src="media/paste-7821dcdc44fa638093bd09fbe5989c38b01bae53.jpg"><br>||
|Definuj instrukci TSL \( test-and-set-lock \)&nbsp;|<img style="height:128px;width:auto;" src="media/paste-6708201adb1726f89a5cf8896e6f9415fd5e545c.jpg">||
|Je instrukce TSL atomická?|Ano, jinak by se mohlo stát, že jiné vlákno skočí doprostřed jejího vykonávání||
|Z čeho se skládá TSL instrukce?|<img style="height:128px;width:auto;" src="media/paste-2537bd15b165594b073c5d14794ddb537da6f427.jpg">||
|Výhody a nevýhody aktivního čekání|<img style="height:128px;width:auto;" src="media/paste-06ce560ced04ab560fb8d90e52b01c452bb1b701.jpg">||
|Struktury dovolující blokující systémové volání typicky implementují|zapamatování si stavu kritické sekce \( odemčená / zamčená \)udržování seznamu vláken, které čekají na vstup do kritické sekce||
|Co se děje před vstupem do kritické sekce ochráněné blokujícím voláním|<img style="height:128px;width:auto;" src="media/paste-bd86eb7b4f6e56e1d47b3ca32c5637f73de62024.jpg">||
|Co s děje při opouštení kritické sekce ochráněné blokujícím voláním|<img style="height:128px;width:auto;" src="media/paste-f7518680742d0c74cf7af24d6b7694fca09cacaa.jpg">||
|Definuj zámek \( mutex \)|<img style="height:128px;width:auto;" src="media/paste-844fa9b832defa4e600b2a5a83a90db9019856ac.jpg">||
|Popiš call mutex_lock|<img style="height:128px;width:auto;" src="media/paste-f759b3facd2075c7dd4d4f962ac54655bbeb2092.jpg">||
|Popiš call mutex_unlock|<img style="height:128px;width:auto;" src="media/paste-485e1b4fa80b78ee6ec1b5d1d1ae0c50c89a8fbd.jpg">||
|Popiš problém producent-konzument<br>Co dělá producent?Co dělá konzument?Jaké jsou vzniklé problémy?|<img style="height:128px;width:auto;" src="media/paste-293e067427bf5b0167669a6f5b87aab63bf52806.jpg"><img style="height:128px;width:auto;" src="media/paste-801b7cc06b52a0ce018994a77a96daafb4eaeed7.jpg"><br>||
|Výhody a nevýhody blokujících volání|<img style="height:128px;width:auto;" src="media/paste-6fc54e76fb461df7989e94a0a3560ba84e887b8c.jpg">||
|Definuj podmíněnou proměnnou|<img style="height:128px;width:auto;" src="media/paste-ab5f91805ab584ddf7e6fdfd5f2a4f7b88d66ee1.jpg">||
|Popiš operace cond_wait a cond_signal|<img style="height:128px;width:auto;" src="media/paste-6d9f1979805a021c7c969ffe692187212d3fdfc2.jpg">||
|Definuj co obsahuje datový typ semafor|<img style="height:128px;width:auto;" src="media/paste-3898b4ecae7eba3f0084d961d8eefadc58ed7526.jpg">||
|Popiš operace sem_init, sem_wait, sem_post|<img style="height:128px;width:auto;" src="media/paste-dc4b2a020dc3f728143b83e5adf43abfcc9972aa.jpg">||
|Definuj bariéry, jejich použití, co obsahuje|<img style="height:128px;width:auto;" src="media/paste-aee612cbc022ad54946ee578893feb7394402753.jpg">||
|Popiš operace barrier_init, barrier_wait|<img style="height:128px;width:auto;" src="media/paste-f75dadc0bb715deeaf14705aaa7710b2b5772bf9.jpg">||
