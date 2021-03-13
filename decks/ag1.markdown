---
title: BI-AG1
layout: page
---


<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Týden 1


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jak definujeme <b>neorientovaný</b> graf?|<img src="media/paste-2e5785259616cc806a93ffa327562b3ce388a486.jpg"><br>Všimněte si, že \\(V\\) je <b>neprázdná</b> množina. Tedy nebudeme uvažovat prázdné grafy.|<img src="media/paste-de66c93276d32e3f07ab3068f49dce92c18a7ab0.png">|
|[latex]Jak definujeme hranu pro neorientovaný graf?[/latex]|<img src="media/paste-0fdb3385115a1949a3d2c515c9cb3f7203b22eff.jpg"><img src="media/paste-0797643c921491588aba5791b0a7679003d0ff58.jpg"><br>||
|Jak definujeme <b>úplný neorientovaný graf</b> \\(K_n\\)?|<img src="media/paste-338540274a518578e0880a20d6fecf0f4246fd7f.png"><br>|<img src="media/paste-9e6daa36014c394ae2146c001e8e3c284b53d978.png">|
|[latex]Jak definujeme úplný bipartitní neorientovaný graf $K_{n_1,n_2}$?[/latex]|<img src="media/paste-28da7fb935679ecbfee2de33c0c9ba0c0d9cff4a.jpg">||
|[latex]Jak definujeme úplný neorientovaný k-partitní graf?[/latex]|<img src="media/paste-f918d65c51d24c8c01babeef33a0e186c8328420.jpg">||
|[latex]Jak definujeme neorientovaný graf cesta $P_m$?[/latex]|<img src="media/paste-437a91909b672184e529d439e292a5188f2b8440.jpg"><br>||
|[latex]Jak zní definice izomorfismu dvou neorientovaných grafů $G$ a $H$?[/latex]|<img src="media/paste-c01566203c736dde8e7df1994e9d40b45072d214.jpg"><br><img src="media/paste-b3d04dbc22ec6a8ccb36a82236abd9c8d08036a0.jpg"><br>||
|[latex]Jak zní definice automorfismu pro neorientovaný graf?[/latex]|[latex]Neformálně řečeno je automorfismus permutace vrcholů, neměnící zakreslení grafu. Automorfismy ukazují symetrie grafu. Množství automorfismů tedy ukazuje na míru pravidelnosti grafu.[/latex]<br><img src="media/paste-6d5cb4ced969cbe52f361e88e8956688dba0365f.jpg"><br><br>||
|[latex]Kolik neorientovaných grafů existuje na n-prvkové množině vrcholů?[/latex]|<img src="media/paste-c10324d9b0f6648e77fe32221f61bf6328b70521.jpg">||
|[latex]Jak definujeme regulární neorientovaný graf?[/latex]|[latex]Graf je regulární, pokud je r-regulární pro nějaké $r$. Graf je r-regulární, pokud stupeň každého jeho vrcholu je $r$.[/latex]&nbsp;<br>||
|[latex]Jak definujeme izolovaný vrchol v neorientovaném grafu?[/latex]|[latex]Izolovaný vrchol je takový vrchol grafu, který má stupeň 0 \(tedy nemá žádné sousedy\).[/latex]||
|[latex]Jak definujeme matici sousednosti a k čemu slouží?[/latex]|[latex]Slouží k reprezentaci grafů v paměti počítače. \\Následující definice se týká reprezentace neorientovaného grafu:<br>[/latex]&nbsp;<br><img src="media/paste-09b9e44e26f97c600faa82c69d26aa77f70425c1.jpg">[latex]U orientovaného grafu matice zpravidla symetrická není. Buňka $a_{i,j}$ obsahuje hodnotu $1$, pokud $\(v_i,v_j\) \in E$.[/latex]<br>||
|[latex]Jak definujeme kliku v neorientovaném grafu?[/latex]|<img src="media/paste-57ed654d0b1869b0c6431dbf184098e1d654d485.jpg">||
|[latex]Jak definujeme nezávislou množinu neorientovaného grafu?[/latex]|<img src="media/paste-26ee8de9e67c742a64bcf3e8509c727c98398925.jpg">||
|[latex]Jak definujeme uzavřené okolí vrcholu $v$ neorientovaného grafu $G$?[/latex]|[latex]Neformálně: Uzavřené okolí vrcholu $v$ je jeho otevřené okolí plus on sám. Formálně: $N<sub>_G</sub>[v] = N<sub>_G</sub>\(v\) \cup \{v\}$.[/latex]||
|[latex]Jak definujeme \(otevřené\) okolí vrcholu v neorientovaném grafu G?[/latex]|[latex]\(Otevřené\) okolí vrcholu $v$ grafu $G$ \(značíme $N_G\(v\)$\) je množina všech sousedů vrcholu $v$ v grafu $G$.[/latex]||
|[latex]Jaký je vztah mezi stupněm vrcholu a \(otevřeným\) okolím vrcholu v neorientovaném grafu?[/latex]|[latex]$deg<sub>_G</sub>\(v\) = \|N<sub>_G</sub>\(v\)\|$[/latex]||
|[latex]Existuje neorientovaný graf, který má 7 vrcholů a je zároveň 3-regulární?[/latex]|[latex]Takový graf neexistuje. Z věty o principu sudosti plyne důsledek, že v&nbsp;každém grafu je počet vrcholů lichého stupně sudý<b>. </b>V zadaném grafu je však lichý počet vrcholů lichého stupně.<br>[/latex]<br>||
|[latex]Jak lze reprezentovat grafy v paměti počítače?[/latex]|[latex]Například pomocí matice sousednosti nebo seznamu sousedů \(či seznamu následníku v případě orientovaných grafů\).[/latex]||
|[latex]Jak definujeme neorientovaný&nbsp;graf kružnice $C_n$?[/latex]|<img src="media/paste-fd850f3fd7743d61e134ef85f981b5fe091eb1b6.jpg">||
|[latex]Jak definujeme neorientovaný&nbsp;graf hvězda $S_n$?[/latex]|<img src="media/paste-19c3db1d01a0d88f9fe937843aabb9556d86b5e0.jpg">||
|[latex]Jak definujeme a značíme doplňek neorientovaného grafu $G$?[/latex]|<img src="media/paste-87cd4a06035f6ae4a565ebee004050aede0151f6.jpg">||
|[latex]Jak definujeme podgraf neorientovaného grafu?[/latex]|<img src="media/paste-87fde7fff9f014ede40bd7f4cb966d3e12e702e1.jpg">||
|[latex]Jak definujeme indukovaný podgraf neorientovaného grafu $G$?[/latex]|<img src="media/paste-70477dc36b116a5ca3351d833b89e141dda3e943.jpg"><br>||
|[latex]Mějme vrchol $v$ neorientovaného grafu $G$. Jak označíme jeho stupeň a co tento údaj reprezentuje<i>?</i>[/latex]<br>|[latex]Stupeň vrcholu $v$ grafu $G$ označíme $deg_G\(v\)$. Toto číslo reprezentuje počet hran grafu $G$ obsahujících vrchol $v$.[/latex]||
|[latex]Jak zní věta o principu sudosti?[/latex]|<img src="media/paste-167dace1417f0d00db880f5b2b13d87c3ce535a1.jpg">||
|[latex]Jaký je maximální stupeň vrcholu v neorientovaném grafu o $n$ vrcholech?[/latex]|[latex]$n-1$[/latex]||
|[latex]Kolik maximálně hran může mít neorientovaný graf na $n$ vrcholech?[/latex]|[latex]Takový graf se nazývá úplný a má $\binom{n}{2} = \frac{n\(n-1\)}{2}$ hran.[/latex]<br>||
|[latex]Jmenujte alespoň 4 nutné podmínky izomorfismu dvou neorientovaných grafů $G, H$.[/latex]|[latex]\begin{enumerate}\item $\|V\(G\)\| = \|V\(H\)\|$\item $\|E\(G\)\| = \|E\(H\)\|$\item Jsou-li $u, v$ sousední vrcholy, pak i $f\(u\)$, $f\(v\)$ jsou sousední vrcholy\item $G$ a $H$ mají stejné soubory stupňů \(soubor stupňů grafu je posloupnost čísel, kterou získáme, když seřadíme stupně všech vrcholů v grafu od největšího k nejmenšímu\)\item pro každý vrchol $v$ z $V\(G\)$ platí, že jeho stupeň je roven stupni vrcholu $f\(v\)$\item pokud mezi vrcholy $v_1, v_2, \dots, v_k$ v grafu $G$ existovala kružnice, pak bude existovat i mezi vrcholy $f\(v_1\), f\(v_2\), \dots, f\(v_k\)$&nbsp;\end{enumerate}[/latex]<br>||


# Týden 2


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Jak definujeme $u$-$v$-cestu v neorientovaném grafu?[/latex]|[latex]$u$-$v$-cesta v grafu $G$ je cesta \(podgraf grafu $G$ izomorfní s nějakou cestou $P$\) vedoucí z vrcholu $u$ do vrcholu $v$. Připouštíme $u = v$.[/latex]||
|[latex]Jak zní definice souvislého neorientovaného grafu?[/latex]|[latex]Neorientovaný graf $G$ je souvislý, jestliže v něm pro každé jeho dva vrcholy $u, v$ existuje $u$-$v$-cesta. Jinak je $G$ nesouvislý. Alternativně: Graf $G$ je souvislý, obsahuje-li právě jednu souvislou komponentu.[/latex]<img src="media/paste-32499aaed3e6cec1aaf5b1cbcb94c63aaa89b8f8.jpg"><br>||
|[latex]Kdy nazveme neorientovaný graf lesem?[/latex]|<img src="media/paste-362a8df40f84c26707794e760065c8dd46da2b4c.jpg"><img src="media/paste-92c712f83099dab6db9b6ab45350d324d5418d9e.jpg"><br>||
|[latex]Jak definujeme orientovaný graf?[/latex]|<img src="media/paste-c7bff37ea884023a6e812ec76383239780e8584b.jpg">||
|[latex]Jak značíme a definujeme vstupní stupeň vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-7246fc8fab8bb80056bf9396cf116e256520401f.jpg">||
|[latex]Jak definujeme vstupní okolí vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-244447061e99dc2b8bb73df907014c6499ef31ca.jpg">||
|[latex]Jak definujeme list v neorientovaném grafu?[/latex]|<img src="media/paste-a32103e3c9b61b52165dfd554e1a05f9c8341568.jpg">||
|[latex]Jak definujeme symetrizaci orientovaného grafu?[/latex]|<img src="media/paste-f116b7d0935277282d441b54c5be70956130f50f.jpg"><br><br>||
|[latex]Kdy nazveme neorientovaný graf stromem?[/latex]|<img src="media/paste-03db5546da9b3b755f862ad39b245c9aabda8cb0.jpg"><img src="media/paste-d92e783c01ce344c84b71b9a8585c75251fa63cf.jpg"><br>||
|[latex]Vyslovte větu o existenci listů.[/latex]|<img src="media/paste-c60fff4972e2ea59963e7920cbbf403459e26a7c.jpg">||
|[latex]Vyslovte větu o odebírání a přidávání listů.[/latex]|<img src="media/paste-aef504d991d1a25a21c91f1e63f18ac5b61abea8.jpg">||
|[latex]Nechť neorientovaný graf $G = \(V,E\)$ je strom. Vyslovte 3 další tvrzení ekvivalentní s tím, že $G$ je strom.[/latex]|<img src="media/paste-76e0581a4ba2fb655c129e343bf3282b1e15e245.jpg">||
|[latex]Popište algoritmus DFS.[/latex]|<img src="media/paste-ce60b33df2a33e111df6dad400c18490789a5e76.jpg"><br><img src="media/paste-76f35664e453db09e6a2b3b0d5517218ead54426.jpg"><br><br><img src="media/paste-2e97ef4d4201486fe13c090d59924876a7770c7e.jpg"><br><img src="media/paste-36b8e181fd22a9b2339d695dac75695e3d2c551e.jpg"><br>||
|[latex]Jak definujeme cestu v neorientovaném grafu?[/latex]|[latex]Cesta v neorientovaném grafu $G$ je podgraf grafu $G$ izomorfní s nějakou cestou $P_m$, kde $m \geq 0$. Délka cesty je rovna počtu hran. Přípouštíme cestu nulové délky.[/latex]||
|[latex]Jak definujeme graf orientovaná cesta $P_m$?[/latex]|<img src="media/paste-c8cb3d4802a3c29e8a23d419844b9a3a0866e23c.jpg"><img src="media/paste-e5952f2622142b02b69b12e437dcd406a60d5288.jpg"><br><br>||
|[latex]Jak definujeme graf orientovaná kružnice \(orientovaný cyklus\) $C_n$?[/latex]|<img src="media/paste-74c0242bad1e36ac9be18866f96821a16e4e3776.jpg"><img src="media/paste-a1aacfded256b033087a35d00fa166503e314dd0.jpg"><br><br>||
|[latex]Jak definujeme stok v orientovaném grafu?[/latex]|[latex]Stok je takový vrchol orientovaného grafu, ze kterého nevede žádná hrana \(jeho výstupní stupeň je 0\).[/latex]||
|[latex]Jak definujeme slabě souvislý orientovaný graf?[/latex]|<img src="media/paste-a8ff4d32b70bd1e55e385f97ac8528601c204e91.jpg">||
|[latex]Jak definujeme silně souvislý orientovaný graf?[/latex]|<img src="media/paste-ee3290836b78084c121592a72edf49633cb346b0.jpg">||
|[latex]Jak definujeme zdroj v orientovaném grafu?[/latex]|[latex]Zdroj je takový vrchol orientovaného grafu, do kterého nevede žádná hrana \(jeho vstupní stupeň je 0\).[/latex]||
|[latex]Jak bychom pomocí algoritmu DFS mohli ověřit, zdali je zadaný orientovaný graf silně souvislý?[/latex]<br>|[latex]DFS budeme postupně pouštět ze všech vrcholů. Z každého vrcholu musí být všechny ostatní dosažitelné, tedy po průchodu DFS budou všechny vrcholy CLOSED. Před dalším spuštěním DFS \(z dalšího vrcholu\) opět nastavíme všechny uzly zpět na FRESH.[/latex]||
|[latex]Jak v orientovaném grafu $G=\(V,E\)$ definujeme orientovanou hranu?[/latex]|<img src="media/paste-08f6ca648195cb3f8de1eff8233ea3b079ee97a5.jpg">||
|[latex]Jak značíme a definujeme výstupní stupeň vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-a8df71b3764f2a506782c14bb0746ad0d99be330.jpg">||
|[latex]Jak značíme a definujeme stupeň vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-4495f518ea7c452979d3202f2f9fcc6bef2e6d9f.jpg">||
|[latex]Jak definujeme výstupní okolí vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-8115168cc6fd56113614ab8ed244d5ef3398c6f6.jpg">||
|[latex]Jak definujeme okolí vrcholu v orientovaném grafu?[/latex]|<img src="media/paste-9141b54c51be823d352edc8a62d790998ded7a37.jpg">&nbsp;<br>||
|[latex]Jak definujeme izolovaný vrchol v orientovaném grafu?[/latex]|[latex]Izolovaný vrchol v orientovaném grafu je takový, který má stupeň 0 \(tedy jeho vstupní i výstupní stupeň jsou 0\) -- do vrcholu ani z vrcholu nevedou žádné hrany.[/latex]||
|[latex]Jak definujeme souvislou komponentu neorientovaného grafu $G$?[/latex]|[latex]Souvislá komponenta grafu $G$ je souvislý indukovaný podgraf $H$ takový, že neexistuje žádný souvislý podgraf $F$ \($F \neq H$\) v grafu $G$ takový, že $H \subseteq F$. Souvislá komponenta je tedy v inkluzi maximální souvislý podgraf grafu $G$.[/latex]<img src="media/paste-5c94ad86bf82e45d9037d57b891eab27c3d91641.jpg"><br>||


# Týden 3


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Jak zní věta o existenci zdroje a stoku?[/latex]|<img src="media/paste-250896335d89318d451fdfca126180f3420f19b1.jpg">||
|[latex]Jak definujeme kostru neorientovaného grafu?[/latex]|<img src="media/paste-f7b5e0a2beb8c6549104734a9b6e3ca164531c50.jpg">||
|[latex]Jak definujeme vzdálenost dvou vrcholů v grafu?[/latex]|<img src="media/paste-4d5f462ca0a1e6c7b764f0e05d28fc9f31ec4ada.jpg">||
|[latex]Jak definujeme acyklický orientovaný graf?[/latex]|<img src="media/paste-6bd3c14ca2397c6fd10d92ee1c53b6778199db62.jpg">||
|[latex]Jak definujeme topologické uspořádání orientovaného acyklického grafu?[/latex]|<img src="media/paste-0f8cbcc5820c98e398e74241313501eaa1e5d851.jpg"><br><br>||
|[latex]Jakou časovou složitost má algoritmus BFS při reprezentaci grafu seznamem sousedů?[/latex]|    [latex]$O\(\|V\| + \|E\|\)$[/latex]   ||
|[latex]Popište algoritmus BFS.[/latex]|[latex]BFS = breadth-first search \(prohledávání do šířky\), používá se pro nalezení nejkratších cest v grafu[/latex]<img src="media/paste-7ebe2c331f2af14bf9675a34b5f68a08d9c5739e.jpg"><img src="media/paste-96602259bcb02d6fa40e5b3b093046b27b0f0f07.jpg"><br><img src="media/paste-1028e56a7f97e2100cc48519ba2809dafc2fc805.jpg"><br><br>||
|[latex]Popište algoritmus TopSort.[/latex]|[latex]TopSort \(topological sort\) = topologické uspořádání \(TU\). Vstupem je orientovaný&nbsp;graf $G$. Výstupem je nějaké topologické uspořádání vstupního grafu, pokud byl acyklický \(detekce cykličnosti v opačném případě\). TopSort má pro orientovaný graf $G = \(V, E\)$ reprezentovaný pomocí seznamu následníků časovou i paměťovou složitost $O\(\|V \| + \|E\|\)$.<br>[/latex]<br><img src="media/paste-9e2832fc2d26a12c2a4f32e78150e81eb5c4070b.jpg"><br><img src="media/paste-a4b997c608dc5632fd4f6a59bf673ab8f9f77536.jpg"><br><br>||


# Týden 4


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Jak definujeme pojmy otec, syn, předek a potomek u zakořeněného stromu?[/latex]|<img src="media/paste-e214c392f174e27fc8179c1a54cf6852b01503c5.jpg">||
|[latex]Jak v zakořeněném stromu definujeme hloubku vrcholu?[/latex]|<img src="media/paste-1c7e3be4edb68dc71d71f9bc7e9a040e0d558b68.jpg">||
|[latex]Jak definujeme binární minimovou haldu?[/latex]|<img src="media/paste-4ef36fd7daf90876d913823b85183cb63c334b38.jpg">||
|[latex]Kolik má binární halda s $n$ prvky listů a vnitřních vrcholů?[/latex]|<img src="media/paste-afa1952174e985be0c6f2940f65c2d43d4294e4f.jpg">||
|[latex]Popište operaci \texttt{HeapInsert}\($H,k$\), která vloží nový klíč $k$ do binární minimové haldy $H$. Jakou má tato operace časovou složitost?&nbsp;[/latex]|<img src="media/paste-8dae24eb453dd7f3951c6d8a35b63558c1163d56.jpg"><img src="media/paste-ab1f31ac9f95f097a50cbab6cd586b5ee714b413.jpg"><br>||
|    [latex]Jak definujeme zakořeněný strom?[/latex]   |    <img src="media/paste-ed4829af94ecee63d15f3c5d5ce7fcc852d3e103.jpg"><br>   ||
|[latex]Jak v zakořeněném stromu definujeme hladinu?[/latex]|    <img src="media/paste-c3864da4464a2a0d04fc977249761f81e9f2c54d.jpg"><br>   ||
|    [latex]Jak definujeme binární strom?[/latex]   |          <img src="media/paste-690fa66fc7fd9e8806384edad9591747787f094a.jpg"><br>         ||
|[latex]Popište algoritmus \texttt{BubbleSort}.[/latex]|<img src="media/paste-70e5c203333f3efbc7c33485a68ae55758d36a52.jpg"><img src="media/paste-199e214efbcb69292c761ce193be89b0e0cf5e3a.jpg"><img src="media/paste-136154631e89e1e453e3be3ac4392f23f6d3ecec.jpg"><br><br>||
|[latex]Popište algoritmus \texttt{SelectSort}.[/latex]|<img src="media/paste-256edbd213796d4f9f6b9b6a2acf3106d8a8a847.jpg"><br><img src="media/paste-31581c9f255f0da22298130a5c1564773eb5e158.jpg"><img src="media/paste-482f8ddde0acba812e73e9f5556e21debd10eb6f.jpg"><br><br>||
|[latex]Popište algoritmus \texttt{InsertSort}.[/latex]|<img src="media/paste-b3008ad821091fc66e68c269e36d926761dbade7.jpg"><img src="media/paste-4ebe4bf8e9f64abbc94207c644b4b5ba64d9838e.jpg"><br><img src="media/paste-754984713ebe08f0337f4d8f75bed1945a8242ce.jpg"><br>||
|[latex]Kolik hladin má binární halda s $n$ prvky?[/latex]|<img src="media/paste-9ac9f1b14efdce4b46b0b31fd5546c366e671e24.jpg">||
|[latex]Popište operaci \texttt{HeapFindMin}\($H$\), která vrátí minimum ze všech prvků v binární minimové haldě $H$. Jakou má tato operace&nbsp;časovou složitost?&nbsp;[/latex]|<img src="media/paste-515fe9bc56d3653ed7901efe1b6d4d83b4612638.jpg">||
|[latex]Popište operaci \texttt{HeapExtractMin}\($H$\), která odstraní \(a vrátí\) minimum ze všech prvků z binární minimové haldy $H$. Jakou má tato operace časovou složitost?&nbsp;[/latex]|<img src="media/paste-2f97fe5a821a675513675bc7e5be213eb21889e8.jpg"><img src="media/paste-cee095b08d79fa4f52fb365522738c9ad2b4ce1c.jpg"><br>||
|[latex]Popište, jak lze binární minimovou haldu reprezentovat v poli.[/latex]|<img src="media/paste-56b6e7d6c63a9ccbf7617e3737d3db683eb65d3b.jpg">||
|[latex]Popište, jak lze z $n$ prvků zkonstruovat binární minimovou haldu v čase $\mathcal{O}\(n\)$.[/latex]|<img src="media/paste-f6088006e5c85505d5c313bb4e223361686a3e4e.jpg"><img src="media/paste-d1b03aef7ad6d62f6fef325596217bf44f9d8ccb.jpg"><br>||
|[latex]Popište algoritmus \texttt{HeapSort}.[/latex]|<img src="media/paste-c9d580d122e0f60100cdd13d87f2fcc71377e4f8.jpg">||


# Týden 5


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Jak definujeme amortizovanou časovou složitost?[/latex]|<img src="media/paste-6d06a833a67e61bfed9d588396d24af610e58fe4.jpg">||
|[latex]Jak definujeme binomiální strom řádku $k$?[/latex]|<img src="media/paste-dd80fc284d73da8c80e0c042cffa495be2864b66.jpg"><br><img src="media/paste-075274b469de337db094569c5586a2d5513862c9.jpg"><br>||
|[latex]Jaký je počet hladin binomiálního stromu $B_k$?[/latex]|[latex]$k+1$[/latex]||
|[latex]Jakou hloubku má binomiální strom s $n$ vrcholy?[/latex]|[latex]$\log n$[/latex]||
|[latex]Jak definujeme binomiální haldu?[/latex]|<img src="media/paste-c256c308d2e2b7b2d734a247fa0f6737182967c9.jpg">||
|[latex]Z kolika binomiálních stromů se skládá $n$-prvková binomiální halda?[/latex]|<img src="media/paste-27c485b49959cf0c51841b91e601bda9781ef224.jpg">||
|[latex]Jaký stupeň má kořen binomiálního stromu $B_k$?[/latex]|[latex]$k$[/latex]||
|[latex]Kolik vrcholů má binomiální strom $B_k$?[/latex]|[latex]$2^k$[/latex]||
|[latex]Kolik synů má kořen binomiálního stromu s $n$ vrcholy?[/latex]|[latex]$\log n$[/latex]||
|[latex]Kolik vrcholů má binomiální strom $B_k$ v hloubce $i \in \{0, \dots, k\}$?[/latex]|[latex]$\binom{k}{i}$[/latex]||
|[latex]Popište operaci \texttt{BHFindMin}\($H$\), která vrátí minimum ze všech prvků v binomiální \(minimové\) haldě $H$. Jakou má tato operace&nbsp;časovou složitost?&nbsp;[/latex]|<img src="media/paste-f026fd5541c2ef52065c58f8c38b24a85c83486f.jpg">||
|[latex]Popište operaci \texttt{BHMergeTree}, která slije dohromady dva binomiální stromy stejného řádu $B_i$ a vytvoří strom $B_{i+1}$. Jakou má tato operace časovou složitost? [/latex]|<img src="media/paste-ccde4539cd61df7a21d85ec28c9d8f5e005baf64.jpg"><img src="media/paste-0b0dd1f28585160365c3158e3807a979a0e4b23c.jpg"><br><img src="media/paste-d2b64824293098b09e631d6546ce38224c62e11f.jpg"><br>||
|[latex]Popište operaci \texttt{BHInsert}\($H,k$\), která vloží nový klíč $k$ do binomiální \(minimové\) haldy $H$. Jakou má tato operace časovou složitost?&nbsp;[/latex]|<img src="media/paste-0cdbe9f4d7ddb051583a5c275fbbc8f801687b77.jpg"><img src="media/paste-f451b5b8dd1bb9a44d6fb508165269dfc7540fce.jpg"><br>||
|[latex]Popište operaci \texttt{BHExtractMin}\($H$\), která odstraní \(a vrátí\) minimum ze všech prvků z binomiální \(minimové\) haldy $H$. Jakou má tato operace časovou složitost?&nbsp;[/latex]|<img src="media/paste-434aff2c8a7aff29f5802b16d318a014c4aa0e63.jpg"><img src="media/paste-9ec5d2bcb8ba8ee1548c6054bfb22e38586df708.jpg"><br>||


# Týden 6


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Kdy binární vyhledávací strom nazveme dokonale vyváženým?[/latex]|<img src="media/paste-e144c83135177f48b37fb52d87aa2e7a04b9e2f1.jpg">||
|[latex]Jaká je hloubka AVL stromu na $n$ vrcholech?[/latex]|<img src="media/paste-c5ca6851eb3fb14c7db69ba00388f1678fdd21c3.jpg">||
|[latex]Popište operaci \texttt{BVSDelete}$\(v,x\)$, která z $T\(v\)$ odstraní vrchol s klíčem $x$, pokud v něm existuje.[/latex]|<img src="media/paste-461a78067a3caa7d0992df36334fe5e1c8795a7a.jpg"><img src="media/paste-a6d40fc65c143e8df08aa87f2f3d00bb4c693316.jpg"><br><img src="media/paste-46c219d63fa4446d71f364c8af0b3fc721abc59c.jpg"><br><img src="media/paste-1010523f103ec45c9dfb1fabfced70a1e00301fb.jpg"><br>||
|[latex]Popište operaci \texttt{BVSMin}$\(v\)$, která vrátí minimální klíč v $T\(v\)$.[/latex]|<img src="media/paste-942c416d215aac1c7738ab76058a03d67087a25a.jpg">||
|[latex]Kdy binární vyhledávácí strom nazveme AVL stromem?[/latex]|<img src="media/paste-a624c9b5330da9c9f2a0fa5c11ed20ef42d8c4cd.jpg">||
|[latex]Popište operaci \texttt{BVSInsert}$\(v,x\)$, která&nbsp;do $T\(v\)$ vloží nový vrchol s klíčem $x$, pokud v něm ještě neexistuje.[/latex]|<img src="media/paste-755ef1bcc938097d72e1493405e3f6f86d21a18c.jpg">||
|[latex]Popište operaci \texttt{BVSPred}$\(v,w\)$, která vrátí předchůdce vrcholu $w$ v $T\(v\)$.[/latex]|<img src="media/paste-6661ad7248d233ff0336b73125929ba59171b5f8.jpg">||
|[latex]Jak definujeme binární vyhledávací strom?[/latex]|<img src="media/paste-c045c410413925563172f9ad4bed7c590abb21da.jpg">||
|[latex]Jak se kontroluje a případně opravuje hloubková nevyváženost u AVL stromu?[/latex]|<img src="media/paste-906324ec721c2fa8cf8417c3eff836a2a2384e83.jpg">||
|[latex]Jaká je časová složitost operací \texttt{AVLInsert} a \texttt{AVLDelete}?[/latex]|<img src="media/paste-4b645ea7eff1841b29e4e476c0f9b5d8eff79447.jpg">||


# Týden 7


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Jak definujeme jev a jak počítáme jeho pravděpodobnost?[/latex]|<img src="media/paste-c04c74ab7ad161c39569be5fd5fd23829f115c20.jpg">||
|[latex]Kdy dva jevy nazveme nezávislé?[/latex]|<img src="media/paste-66c97aa2ae4bec34f27c9f351c444432f6962854.jpg">||
|[latex]Jak definujeme opačný jev k jevu $A$ a jaká je jeho pravděpodobnost vzhledem k pravděpodobnosti jevu $A$?[/latex]|<img src="media/paste-6e975ede308b226a0a9db66983c8b9dfed1d7e78.jpg"><img src="media/paste-101429088be512eb087f539e6d0cfecc733ceb19.jpg"><br>||
|[latex]Vyslovte větu o linearitě střední hodnoty.[/latex]|<img src="media/paste-bb6aa215c62ebcd87bb63a16be5d1841e90ac9df.jpg">||
|[latex]Jak definujeme střední hodnotu náhodného veličiny?[/latex]|<img src="media/paste-8d1d3e7ea2622d75657682d18fb391479883100d.jpg">||
|[latex]Jak definujeme diskrétní pravděpodobnostní prostor?[/latex]|<img src="media/paste-87ac27453e2d0295df9dc2f90e22fd94bc3a82d8.jpg">||
|[latex]Jak fungují hešovací tabulky?[/latex]|<img src="media/paste-6c5385556f6223faec609db0fd447925f3087e98.jpg">||
|[latex]Jak definujeme diskrétní náhodnou veličinu?[/latex]|<img src="media/paste-b572f4414df39225c792de3e633c4d8d3324771c.jpg"><img src="media/paste-60f5c94e4d9a504d269f051b132744fde5a8a438.jpg"><br>||
|[latex]Definujte datovou strukturu slovník.[/latex]|<img src="media/paste-c29f048b29c5f1a1c25fb5d3e3316bdfcba5e8be.jpg"><img src="media/paste-bf1b5b85a073922f60b985b3b9f43184dcaf1c06.jpg"><br><img src="media/paste-523fa859a890857bf820bcbf7f730b2b8c975c84.jpg"><br>||
|[latex]Vyslovte větu o opakování pokusu.[/latex]|<img src="media/paste-cd4cdc48ea4ecfb29656e8d6dc64024a8e5bfaa2.jpg">||
|[latex]Jaké existují metody řešení kolízí?[/latex]|<img src="media/paste-38458a440d998a6bd77844ecd315d40461d245ef.jpg">||


# Týden 8


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Co je to rekurzivní algoritmus a metoda Rozděluj a Panuj?[/latex]|<img src="media/paste-da3356ae314ed2ecbfac9848996af732702b8fa6.jpg">||
|[latex]Jak funguje algoritmus QuickSelect a jaká je jeho časová složitost?[/latex]|<img src="media/paste-f37a1f01cfebb048684b0cc649f4bbdf748c5720.jpg"><img src="media/paste-96e50009d9f7f151841f388bea5d64e7f8a38db7.jpg"><br><img src="media/paste-645ecf919ace254b581112e49b0a974b01c7aa66.jpg"><br><img src="media/paste-fd4cd337e98fb8683caea446bbb69edd83155e72.jpg"><br><br>||
|[latex]Jaké máme základní typy rekurze?[/latex]|<img src="media/paste-3025615e4c2cf4a7f958d3a6977641238a9f795e.jpg"><br>||
|[latex]Co je to koncová rekurze?[/latex]|<img src="media/paste-304b8d6d37290ef6dcbda0c006a58d2ec6376b6b.jpg">||
|[latex]Co je to lineární rekurze?[/latex]|<img src="media/paste-6b0ee8326b90712dd50382e55ca1a6ed3e8ebbcf.jpg">||
|[latex]Co je to stromová/kaskádní rekurze?[/latex]|<img src="media/paste-b40d0521a0661ebe6c05835368322a0149a70236.jpg">||
|[latex]Co je to skoromedián a jak ho ve vstupní posloupnosti čísel najít?[/latex]|<img src="media/paste-de408142de8c649c0ac803d7b159181d338c466c.jpg"><br><img src="media/paste-1205513327b82b184f37d3783f2c775580a31051.jpg">||
|[latex]Jak funguje algoritmus MergeSort a jaká je jeho časová složitost?[/latex]|<img src="media/paste-bdc1ac7f51e813c4da56cdca0f3bc0a1f90bc84e.jpg"><br><img src="media/paste-1359366af0ad045d7ed61b3ca9f8012560cd9c18.jpg"><br><img src="media/paste-b407d62639b8708fa5eea53e3ade8128b15745e0.jpg"><br><img src="media/paste-5bf57c6c4df7f9018c6931a8464264432a30ef67.jpg"><br>||
|[latex]Jak funguje Karacubův algoritmus a jaká je jeho časová složitost?[/latex]|<br><img src="media/paste-d9f34fd4b69c79b86448dcd71fd15d05e2b22c44.jpg"><br><img src="media/paste-47191297c83c1a9f7480fc74e160af4344c90e5f.jpg"><br><img src="media/paste-b4d1a08c14340d3f1fcecb59aced72672522b122.jpg"><br>||


# Týden 9


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Definujte problém vyhledávání v porovnávacím modelu a formulujte větu o dolní složitosti tohoto problému.[/latex]|<img src="media/paste-190aef51c0ce6fed9baea711403ea551b3ca8ff9.jpg"><br><img src="media/paste-4e66cbb8d3678d99643eea9fc5d6b7617f59cbc0.jpg"><br>||
|[latex]Popište algoritmus \texttt{QuickSort}.[/latex]|<img src="media/paste-1e357d62f20c7e743d5b77e43933f9738b4db451.jpg"><img src="media/paste-3b146b11e8c2bc3536296d891c228aa9bc704261.jpg"><br>||
|[latex]Vyslovte větu o složitosti řazení.[/latex]|<img src="media/paste-3128e59f7962d7a0793b693ed4582c927bb29ad3.jpg">||
|[latex]Popište algoritmus \texttt{CountingSort}.[/latex]|<img src="media/paste-83f354da3f23a6e511afcfd7c7d11ac64a694486.jpg"><br><img src="media/paste-50d89e586ff753bd50b9479adcde7cdf2d2af2ee.jpg"><br>||
|[latex]Popište algoritmus \texttt{LexCountingSort}.[/latex]|<img src="media/paste-168218f604ab8d197df661ff93040400b01b9608.jpg"><br><img src="media/paste-93caf24eea7e21cc33ee2043dc3c60025f3f302d.jpg"><br><img src="media/paste-c3b940f3f47f0a6305cff79da542ccf2d46be921.jpg"><br><br>||


# Týden 10


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Definujte Levenshteinovu vzdálenost \(problém editační vzdálenosti řetězců\).[/latex]|<img src="media/paste-e6c3575963de71d3e7b709d0af280f3d6e548f8b.jpg">||
|[latex]Popište princip dynamického programování.[/latex]|<img src="media/paste-a8bcc54a765d7675b1220b57d60e0c41053c181a.jpg">||
|[latex]Co je to memoizace?[/latex]|[latex]Začneme s rekurzivním algoritmem, který má exponenciální složitost. Odhalíme opakované výpočty stejných podproblémů. Vytvoříme si tabulku, do které budeme zapisovat výsledky již vyřešených podproblémů -- tedy každou spočítanou hodnotu pro dané vstupy si uložíme pro pozdější použití. Jelikož se v&nbsp;průběhu rekurzivního výpočtu často řeší stejné zadání na několika různých místech, můžeme si ušetřit \(až nečekaně!\) výrazné množství času.[/latex]||
|[latex]Popište problém nejdelší rostoucí podposloupnosti \(NRP\).[/latex]&nbsp;|<img src="media/paste-486949250a3c4e42caa6d0c889e09b5416e9d10c.jpg">||


# Týden 11


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Popište problém minimální kostry grafu.[/latex]|<img src="media/paste-22fb1e2add87c057cabfd9b6a97e596ea5182d61.jpg"><img src="media/paste-aa4e083e8f78a00da4bae5c9c4e58587e972edf2.jpg"><br>||
|[latex]Popište Jarníkův algoritmus a jeho složitost.[/latex]&nbsp;|<img src="media/paste-d9494f2c4218a8e7122662f2c15274f8fe924587.jpg"><img src="media/paste-adaedb63de5070db958ef8e00800bf77ab22ba84.jpg"><br><img src="media/paste-9b6e99a51bc3d357a454143be4b8d2aba01dad90.jpg"><br>||
|[latex]Popište Kruskalův algoritmus a jeho složitost.[/latex]|<img src="media/paste-4f59fbee07d801a27ead1cdc9972568cc8a5cb0b.jpg"><img src="media/paste-d9471d4b974ec44f3dfc323ae2fa4dea3c16d1c2.jpg"><br><img src="media/paste-dd8b660ece1796610e074cb1af8dd6237446e947.jpg"><br><img src="media/paste-5967e343e0cdab3594aceff42569410a83ca6862.jpg"><br>||
|[latex]Definujte strukturu Union-Find.[/latex]|<img src="media/paste-d2a14ee4f0403dbedf2057b25fab6aabc4644117.jpg">||
|[latex]Definujte elementární řez grafu.[/latex]|<img src="media/paste-c96537b9ee1e01d22e7a05d4012f4fff06472001.jpg">||
|[latex]Popište implementaci struktury Union-Find pomocí pole a pomocí keříků.[/latex]|<img src="media/paste-b56b7720f6efeebd429d689b656c524328461940.jpg"><img src="media/paste-992082d1a67d935eb97bcd643a042c8d36e33bc9.jpg"><br><img src="media/paste-0e8418049ad8bd7d5ccb53080056d5de850bce35.jpg"><br><img src="media/paste-1277f7d2a2e05a1a16c4b000f7e2ba3f5aa734b0.jpg"><br><img src="media/paste-c190b9d68df1311a863d24da8bb7d40b1f5feba9.jpg"><br><img src="media/paste-890831f7e170312c044e88572b47f189c3f1d565.jpg"><br><img src="media/paste-2e7a44e44b3e85c793613ccc0b920e70461f9117.jpg"><br><img src="media/paste-1b13a2eb84442e1f35f600942c2482efaed43ec0.jpg"><br>||


# Týden 12


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|[latex]Definujte sled v orientovaném ohodnoceném grafu a jeho délku.[/latex]|<img src="media/paste-4a3bf4ddc8f124e3f475116a672cf055b3a52f52.jpg">||
|[latex]Definujte vzdálenost dvou vrcholů v ohodnoceném orientovaném grafu.[/latex]|<img src="media/paste-0a0a71c80601890298df2b44ff64052e86f5ee84.jpg">||
|[latex]Popište Dijkstrův algoritmus a jeho složitost.[/latex]|<img src="media/paste-4338b1888bfc9d39f28bbe3a041a7624a741bc45.jpg"><img src="media/paste-9a50bcfc8954ddcf72385c1600fc4fd5727572a1.jpg"><img src="media/paste-1368426215cd72deac44d54963e285da00f62b4f.jpg"><img src="media/paste-c38b89c55e43cf8bbdbe61ea27a2299d72cf341f.jpg"><br><br>||
|[latex]Popište algoritmus Relaxace.[/latex]|<img src="media/paste-482c05d86168b79e6d8f06d08222013d94194db8.jpg"><br><img src="media/paste-a0571ac232260a9f95e3cb7943196a8f228c58f0.jpg"><br>||
|[latex]Vyslovte lemma o zjednodušování sledů. Jaké má toto lemma důsledky?[/latex]|<img src="media/paste-2573dc08ee50a3fd821e853e7a1114b553625cb6.jpg"><img src="media/paste-64fcce16322a0f31fc76b1efac05590993d172bb.jpg"><br><img src="media/paste-8c0b7b45b622f7f33ebad20a021d30012e8be4c3.jpg"><br><img src="media/paste-f56a1ec85b174aa28c7ed927e8508a3f0ebf220d.jpg"><br>||
|[latex]Popište Bellman-Fordův algoritmus a jeho složitost.[/latex]|<img src="media/paste-598cb67a25dbe97782ba92ed26df65bdae422a69.jpg"><br><img src="media/paste-5ae2a69a2064010b3e65d52889ea6c7d365acab2.jpg"><br><img src="media/paste-91a54c3a0d603cace499313efb3ae089b635b005.jpg"><br>||
|[latex]Definujte ohodnocený orientovaný graf.[/latex]|<img src="media/paste-872e50fbdf14aed854edcd489881962de7447b39.jpg">||
