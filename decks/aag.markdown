---
title: BI-AAG
layout: page
---


<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>

# Týden 1


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jak zní definice abecedy?|\textbf{Abeceda} \(značíme $\Sigma$ nebo \textit{T}\) je konečná množina prvků, které nazýváme symboly abecedy.\par\textit{Příklady abeced:} &nbsp;\{0,1\}, \{a,b,c,d,e\}, \{jedna, dva\}||
|Jak zní definice řetězce nad abecedou?|Řetězec \(též říkáme slovo nebo věta\) je konečná posloupnost symbolů abecedy.||
|Co reprezentuje znak&nbsp;$\varepsilon$?|prázdný řetězec, prázdnou posloupnost symbolů||
|Jaké čtyři typy gramatik vymezuje Chomského klasifikace gramatik?|regulární gramatika, bezkontextová gramatika, kontextová gramatika, neomezená gramatika||
|Jak značíme a počítáme délku řetězce?|Délka řetězce $x$ \(značíme $\|x\|$\) je nezáporné celé číslo udávající počet symbolů řetězce. Délka prázdného řetězce je nulová \(tj. $\|\varepsilon \| = 0$\). Řetězec, který sestává právě z $k$ výskytů symbolu $a$, se symbolicky značí $a^k$. Například: $a^3 =aaa, a^0 =\varepsilon$.||
|Jak zní definice formálního jazyka nad abecedou $\Sigma$?|Formální jazyk nad abecedou $\Sigma$&nbsp;\(značíme $L$\) je libovolná podmnožina množiny všech možných řetězců nad danou abecedou -- tj. $L \subseteq \Sigma ^ *$.||
|Jak zní definice operace doplněk jazyka $L$ nad abecedou $\Sigma$?|Jazyk, který vznikne doplňkem jiného jazyka \(značíme $\overline{L}$\), obsahuje řetězce, které obsahuje množina všech řetězců nad abecedou $\Sigma$, ale už ne jazyk $L$. \par \textit{Formálně:}\par $\overline{L} = \{x:x\in \Sigma^* \wedge x \notin L\}$\par \textit{Například:}\par $\Sigma = \{a\}$, $L = \{aa\}$,&nbsp;$\overline{L} = \Sigma^* \setminus L = \{\varepsilon, a, aaa, aaaa, \dots\}$||
|Jak zní definice gramatiky?|Gramatika je uspořádaná čtveřice $G = \(N, \Sigma, P, S\)$, kde&nbsp;\begin{itemize}\item N je konečná množina neterminálních symbolů\item $\Sigma$ \(značíme též $T$\) je konečná množina terminálních symbolů \($\Sigma \cap N = \emptyset$\)\item $P$ je množina \(přepisovacích\) pravidel. Je to konečná podmnožina množiny $\(N \cup \Sigma\)^*\cdot N \cdot \(N \cup \Sigma\)^* \times&nbsp; \(N \cup \Sigma\)^*$. Element \($\alpha$, $\beta$\) z $P$ zapisujeme $\alpha \rightarrow \beta$ a nazývame jej pravidlo.\item $S$ je počáteční \(startovací\) symbol gramatiky\end{itemize}<br><br>||
|Jak zní definice konečného jazyka?|Konečný jazyk obsahuje vždy konečný počet řetězců.<br>||
|Který výpočetní model rozpoznává právě třídu regulárních jazyků?|\(ne\)deterministický konečný automat||
|Který výpočetní model rozpoznává právě třídu kontextových jazyků?|lineárně omezený Turingův stroj||
|Který výpočetní model rozpoznává právě třídu rekurzivně spočetných jazyků?|\(ne\)deterministický Turingův stroj||
|Pro které operace je třída bezkontextových jazyků uzavřená?|Třída bezkontextových jazyků je uzavřena pro operace:\begin{itemize}\item sjednocení\item zřetezení \(součin\)<br>\item iterace<br>\end{itemize}||
|Nechť $w$ je řetězec nad abecedou $\Sigma$. Co znamená $w<span style="font-size: 16.6667px;">^R$?&nbsp;|$w^R$<span style="font-size: 16.6667px;">&nbsp;značí reverzi<b>&nbsp;</b>řetězece<b>&nbsp;</b>$w$.Například:&nbsp;$w = aaba; w^R=<sup>&nbsp;</sup>abaa$||
|Co znamená, když je třída jazyků uzavřená pro nějakou operaci?|Provedeme-li se dvěma jazyky z této třídy danou operaci \(pro níž je jim odpovídající třída jazyků uzavřená\), pak&nbsp;výsledkem bude opět jazyk z této třídy.||
|Co reprezentuje $\Sigma^*$?|množinu všech řetězců nad abecedou $\Sigma$ \(včetně prázdného řetězce\)||
|Co reprezentuje $\Sigma^+$?|množinu všech neprázdných řetězců nad abecedou $\Sigma$||
|Jak definujeme větu generovanou gramatikou $G = \(N, \Sigma, P, S\)$?|<img style="height:128px;width:auto;" src="media/paste-9ef34442c44469d6a51486eee50aed67723de2bb.jpg">||
|Kdy řekneme, že jsou dvě gramatiky ekvivalentní?|Gramatiky $G_1$ a $G_2$ jsou ekvivalentní právě tehdy, když generují stejný jazyk -- tj. $L\(G_1\) = L\(G_2\)$.||
|Jaký tvar musí splňovat pravidla regulární gramatiky?|$A \rightarrow a$ nebo $A \rightarrow&nbsp;aB$, kde $a \in \Sigma$, $A, B \in N$\par~\parJedinou povolenou vyjímkou je pravidlo $S \rightarrow \varepsilon$, které může být použito pouze v případě, že se počáteční symbol $S$ nevyskytuje na pravé straně žádného pravidla.<br>||
|Jaký tvar musí splňovat pravidla bezkontextové gramatiky?|$A \rightarrow \alpha$, kde $\alpha \in \(N \cup \Sigma\)^*$, $A \in N$||
|Jaký tvar musí splňovat pravidla kontextové gramatiky?|$\gamma A \delta \rightarrow \gamma \alpha \delta$, kde $\gamma , \delta \in \(N \cup \Sigma \)^*$, $A \in N$, &nbsp;$\alpha \in \(N \cup \Sigma \)^+$\par~\parJedinou povolenou vyjímkou je pravidlo $S \rightarrow \varepsilon$, které může být použito pouze v případě, že se počáteční symbol $S$ nevyskytuje na pravé straně žádného pravidla.||
|Jaký tvar musí splňovat pravidla neomezené gramatiky?|$\alpha A \beta \rightarrow \gamma$, kde $\alpha , \beta , \gamma \in \(N \cup \Sigma\)^*$, $A \in N$||
|Jaké typy gramatik jsou vždy nezkracující?|regulární a kontextová gramatika||
|Regulární gramatika je vždy zároveň\dots|bezkontextová, kontextová a neomezená||
|Bezkontextová gramatika je vždy zároveň\dots|neomezená||
|Kontextová gramatika je vždy zároveň\dots|neomezená||
|Mějmě gramatiku $G=\(N,\Sigma,P,S\)$. Čemu se rovná $N \cap \Sigma$?|$N \cap \Sigma = \emptyset$||
|Jak zní definice operace součin \(zřetězení\) jazyků?|Jazyk, který vznikne součinem \(zřetězením\) dvou jazyků, obsahuje řetězce, které vznikly zřetězením řetězců z prvního jazyka s řetězci z druhého jazyka.\par\textit{Formálně:}\par $L_1 \cdot L_2 = \{w:w = x \cdot y \wedge x \in L_1 \wedge y \in L_2\}$\par\textit{Například:}\par $L_1 = \{a,b\}$, $L_2 = \{c,d\}$ a $L_1 \cdot L_2 = \{ac,ad,bc,bd\}$<br>||
|Jak zní definice operace iterace jazyka $L$ nad abecedou $\Sigma$?|Jazyk, který vznikne iterací jazyka \(značíme $L^*$\), obsahuje řetězce, které vznikly zřetězením řetězců jazyka se sebou samými.\par\textit{Přesněji:}\par $L^* = \bigcup_{n \geq 0} L^n$, kde $L^n = L \cdot L^{n-1}$ pro $n \in N,L^0 = \{\epsilon\}$\par\textit{Například:}\par $L = \{a\}$ a $L^* = L^0 \cup L^1 \cup L^2 \cup \dots = \{\varepsilon, a, aa, aaa, aaaa, \dots\}$||
|Jak zní definice větné formy v gramatice $G = \(N, \Sigma, P, S\)$|<img style="height:128px;width:auto;" src="media/paste-80ae232278b982361bd27b0acc00972f78ef231d.jpg">||
|Klasifikujte následující jazyk: \\(L = \{ \mathtt{a}^n \mathtt{b}^n : n \in \mathbb{N} \}\\)|<ul><li style="text-align: left;">bezkontextový \(proto tedy i kontextový a rekurzivně spočetný\)</li><li style="text-align: left;">není regulární</li></ul>|Gramatika generují jazyk \\(L\\):<br>\\(G = \(\{S\}, \{\mathtt{a}, \mathtt{b}\}, P, S\)\\), kde \\(P = \{ S \rightarrow \mathtt{ab} \mid \mathtt{a}S\mathtt{b} \}\\)|


# Týden 2


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Klasifikujte následující jazyk: $L=\{one, two, three\}$ nad abecedou $\Sigma=\{o,n,e,t,w,h,r\}$|Jazyk je konečný, tedy regulární \(a tedy zároveň bezkontextový, kontextový a rekurzivně spočetný\).&nbsp;||
|Jak definujeme deterministický konečný automat?|Neformálně:&nbsp;<br>Deterministický konečný automat \(DKA\) je neformálně řečeno takový konečný automat, který má vždy jasně dáno, jak ve výpočtu pokračovat \(nemůže si vybrat z více možností\). \\<br><br>Formálně: \\Deterministický konečný automat je uspořádaná pětice$$M = \(Q,\Sigma,\delta,q_0,F\)$$&nbsp;<br>\begin{itemize}&nbsp;\item $Q$ je konečná neprázdná množina stavů\item $\Sigma$ je konečná vstupní abeceda\item $\delta$ je zobrazení z množiny $Q \times \Sigma$ do množiny stavů $Q$ \(tj. $\delta: \;Q \times \Sigma \rightarrow Q$\)\item $q_0 \in Q$ je počáteční stav&nbsp;\item $F \subseteq Q$ je množina koncových stavů\end{itemize}<br><br><br><br>||
|Jak definujeme úplně určený deterministický konečný automat?|Deterministický konečný automat nazveme úplně určený právě tehdy, když má zobrazení $\delta$ definováno pro všechny dvojice stavů $q \in Q$ a vstupních symbolů $a \in \Sigma$.<br>||
|Jak definujeme nedeterministický konečný automat?|Neformálně:&nbsp;<br>Nedeterministický konečný automat \(NKA\) se vyznačuje tím, že si lze v~nějaké fázi výpočtu vybrat, jak pokračovat. \\<br><br>Formálně: \\Nedeterministický konečný automat je uspořádaná pětice$$M = \(Q,\Sigma,\delta,q_0,F\)$$&nbsp;<br>\begin{itemize}&nbsp;\item $Q$ je konečná neprázdná množina stavů\item $\Sigma$ je konečná vstupní abeceda\item $\delta$ je zobrazení z množiny $Q \times \Sigma$ do množiny všech podmnožin \(potenční množiny\) množiny $Q$ \(tj. $\delta: \;Q \times \Sigma \rightarrow 2^Q$\)\item $q_0 \in Q$ je počáteční stav&nbsp;\item $F \subseteq Q$ je množina koncových stavů\end{itemize}<br><br><br>||
|Je pravda, že pokud je daná bezkontextová gramatika zároveň neomezená, pak je také kontextová?|Není. Bezkontextová gramatika je vždy neomezená, avšak pokud je zároveň zkracující, nejedná se o kontextovou gramatiku, jelikož kontextová gramatika nemůže být zkracující.<br><br>||
|Co znamená, že je gramatika nezkracující?|U nezkracující gramatiky musí všechna pravidla splňovat podmínku, že počet symbolů na levé straně pravidla je menší nebo roven počtu symbolů na pravé straně daného pravidla. Jedinou přípustnou výjimkou je pravidlo $S \rightarrow \varepsilon$, a to jen za předpokladu, že se počáteční neterminál $S$ nevyskytuje na pravé straně žádného pravidla.V nezkracující gramatice tedy žádná jiná $\varepsilon$-pravidla nemohou existovat.<br>||
|Je pravda, že konečný jazyk je vždy regulární?|Ano, toto tvrzení platí. Obrácené tvrzení však pravdivé není&nbsp; \(tj. regulární jazyky obsahují i jazyky nekonečné\).<br><br>||
|Kdy DKA nepřijme&nbsp;řetězec na vstupu?|Neformálně: \\DKA nepřijme&nbsp;řetězec na vstupu, pokud nastane jedna z následujících situací:\begin{enumerate}<br>\item Řetězec je celý přečten, ale automat skončí v nekoncovém stavu.\item Během zpracování řetězce dojde k chybě -- zobrazení $\delta$ není definováno pro dvojici aktuální stav a čtený symbol.\end{enumerate}&nbsp;<br>||
|Kdy DKA přijme&nbsp;řetězec na vstupu?|Neformálně:&nbsp;<br>DKA přijme řetězec na vstupu, pokud jej celý přečte a skončí v~některém z~koncových stavů. \\<br><br>Formálně:<br><img style="height:128px;width:auto;" src="media/paste-a89eca4b837429f4a926891b737ea2935f357df8.jpg"><br>||
|Jak definujeme funkci $\varepsilon$-Closure?|Neformálně: \\$\varepsilon$-Closure je funkce, která na vstupu vyžaduje stav automatu, pro nějž vrací množinu všech stavů, které jsou z~daného stavu dosažitelné bez nutnosti čtení vstupního symbolu. Do této množiny tak patří vždy sám stav, pro který $\varepsilon$-Closure počítáme, a všechny další, které jsou z~tohoto stavu dosažitelné pomocí $\varepsilon$-přechodů \(jednoho i více\).\\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-3dc2b93cd2763a7683b99f8a9a8b05ca402be6de.jpg"><br>||
|Jak z daného konečného automatu odstraníme zbytečné stavy?|Neformálně: \\Vytvoříme si prázdnou množinu, do které budeme postupně přidávat užitečné stavy. Nejprve přidáme všechny koncové stavy, neboť ty jsou z definice vždy užitečné. Dále přidáme všechny stavy, ze~ kterých se lze za pomoci jednoho přechodu dostat do některého z užitečných stavů. Stejně pokračujeme pro všechny takto přidané stavy. Pokud už množinu užitečných stavů nelze rozšířit, algoritmus končí a stavy, které nejsou v~množině užitečných stavů, jsou zbytečné. \\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-860b540c22897e436062bf839bb64aa0e75acc3c.jpg"><br>||
|Jak definujeme derivační strom?|<img style="height:128px;width:auto;" src="media/Screenshot_2018-10-12 bi-aag-01-zakladni_pojmy pdf.png">||
|Jak u konečného automatu definujeme dosažitelný stav?|Neformálně: \\Dosažitelný stav je takový stav, pro který v~automatu existuje posloupnost přechodů vedoucí z~počátečního stavu právě do tohoto stavu. Stav, který není dosažitelný, se nazývá nedosažitelný. Nedosažitelné stavy lze z~automatu odstranit, aniž by se změnil jazyk přijímaný daným automatem. \\<br>Formálně:<br><img style="height:128px;width:auto;" src="media/paste-5023ea68dbee4b2e0a6d77dc00833a8931167b73.jpg"><br><br>||
|Kdy NKA přijme řetězec na vstupu?|Neformálně:&nbsp;<br>NKA přijme řetězec na vstupu, pokud v automatu existuje alespoň jedna posloupnost přechodů, kdy je přečten celý řetězec a výpočet skončí v některém z koncových stavů. \\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-66ed1d74135f097e6cbddd52af58e0b555e02a97.jpg"><br>||
|Kdy NKA nepřijme řetězec na vstupu?|Neformálně:&nbsp;<br>NKA nepřijme řetězec na vstupu, pokud neexistuje posloupnost přechodů vedoucí k přijetí daného řetězce. Neboli všechny možné posloupnosti přechodů pro daný řetězec skončí nepřijetím. Posloupnost přechodů skončí nepřijetím, pokud nastane jedna z následujících situací:&nbsp;\begin{itemize}&nbsp;&nbsp;\item řetězec je celý přečten, ale automat skončí v~nekoncovém stavu,&nbsp;\item během čtení řetězce se dostaneme do situaci, kdy výsledkem zobrazení $\delta$ pro dvojici aktuální stav a čtený symbol&nbsp;je prázdná množina stavů.&nbsp;\end{itemize}<br>||
|Jak daný deterministický konečný automat doplníme na úplně určený?|Neformálně:&nbsp;<br>\begin{enumerate}\item Zavedeme nový ,,nulový'' stav $q_{\varnothing}$.\item Ke stavu $q_{\varnothing}$ přidáme smyčku pro všechny symboly vstupní abecedy.<br>\item Ze všech stavů, které nemají definovaný přechod pro nějaký symbol vstupní abecedy, přidáme přechod na tento symbol do stavu $q_{\varnothing}$.<br>\end{enumerate}<br>Formálně:<br><br><img style="height:128px;width:auto;" src="media/paste-0cfb3773700c5defd15bd2a6d84b35598ddffde3.jpg"><br>||
|Jak u konečného automatu definujeme užitečný stav?|Neformálně: \\Užitečný stav je takový stav, pro který v~automatu existuje posloupnost přechodů vedoucí z~tohoto stavu do některého z~koncových stavů. Stav, který není užitečný, se nazývá zbytečný. Zbytečné stavy lze z~automatu odstranit, aniž by se změnil jazyk přijímaný daným automatem. Jedinou výjimkou je případ, kdy je zbytečný počáteční stav automatu. Tím pádem jsou zbytečné či nedosažitelné i všechny zbylé stavy. V~takovém případě ponecháme v~automatu právě jeden stav \(počáteční a nekoncový\), jenž je z~definice zbytečný. Jazyk přijímaný tímto automatem je prázdný. \\<br>Formálně:<br><img style="height:128px;width:auto;" src="media/paste-f6c8087de76969056a54bf6fa08156abd0cf85a5.jpg"><br>||
|Jak definujeme konfiguraci konečného automatu?|Neformálně:<br>Konfigurace konečného automatu je <i>snaphshot </i>jeho výpočtu. Je to dvojice $\(q,w\)$, kde $q$ je stav, kde se aktuálně automat nachází a $w$ je zbývající \(nepřečtená\) část řetězce na vstupu. \\<br>Formálně:<br>Nechť $M = \(Q, \Sigma, \delta, q_0, F\)$ je konečný automat. Dvojici $\(q,w\) \in Q \times \Sigma^*$ nazveme konfigurací konečného automatu $M$.||
|Jak u konečného automatu definujeme počáteční konfiguraci?|Počáteční konfigurace konečného automatu je dvojice $\(q_0, w\)$, kde $q_0$ je počáteční stav automatu a $w$ je řetězec na vstupu.<br>||
|Jak u konečného automatu definujme koncovou konfiguraci?|Koncová konfigurace konečného automatu je dvojice $\(q, \varepsilon\)$, kde $q$ je některý z koncových stavů automatu a $\varepsilon$ značí, že celý vstupní řetězec byl přečten.||
|Jak z daného konečného automatu odstraníme nedosažitelné stavy?|Neformálně:<br>Vytvoříme si prázdnou množinu, do které budeme postupně přidávat dosažitelné stavy. Nejprve přidáme počáteční stav, který je z definice vždy dosažitelný. Poté přidáme všechny stavy, jež jsou z~tohoto stavu dosažitelné pomocí jednoho přechodu. Stejně pokračujeme pro všechny takto přidané stavy. Pokud už množinu dosažitelných stavů nelze rozšířit, algoritmus končí a stavy, jež nejsou v~množině dosažitelných stavů, jsou nedosažitelné. \\<br><br>Formálně:<img style="height:128px;width:auto;" src="media/paste-4fe3b084ca125914129c69ef77f94da830964144.jpg"><br>||
|Jak definujeme nedeterministický konečný automat s $\varepsilon$-přechody?&nbsp;|<img style="height:128px;width:auto;" src="media/paste-3d5b8fce44937fae0fa80e6fe76902708568b63b.jpg"><br>||
|Jak z automatu odstraníme $\varepsilon$-přechody?|Neformálně:<br>Algoritmicky odstraňujeme $\varepsilon$-přechody ve třech krocích: \begin{enumerate}&nbsp;&nbsp;\item Vypočteme funkci $\varepsilon$-Closure pro všechny stavy.&nbsp;\item Z~automatu odstraníme všechny $\varepsilon$-přechody a pomocí $\varepsilon$-closure upravíme&nbsp;zobrazení $\delta$. Pokud máme například $\varepsilon$-Closure$\(S\) = \{S,A,B\}$, pak všechny přechody, které vedou ze stavů $S,A,B$, povedou také ze stavu $S$.&nbsp;\item Upravíme množinu koncových stavů. Koncové stavy jsou ty, které ve svém $\varepsilon$-Closure mají alespoň jeden z~původních koncových stavů.&nbsp;\end{enumerate}<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-56e4db9584ca98732781feea42f6404b2bef488e.jpg"><br><br><br>||
|Jak definujeme nedeterministický konečný automat s více počátečními stavy?|<img style="height:128px;width:auto;" src="media/paste-a52954cd2882f577d500a6e4d66025c56465e086.jpg">||
|Jak převedeme NKA s více počátečními stavy na NKA s jedním počátečním stavem?|Neformálně:<br>Vytvoříme nový počáteční stav \(u~původních počátečních stavů tento příznak zrušíme\). Z~nového počátečního stavu vedeme $\varepsilon$-přechody do všech původních počátečních stavů. \\<br><br>Formálně:<br><img style="height:128px;width:auto;" src="media/paste-9726bce62733966834b6af9197850c81f0c51b80.jpg"><br>||
|Navrhněte bezkontextovou gramatiku generující prázdný jazyk.|Například $G = \(\{S\},\{\texttt{0,1}\},\{S \rightarrow \texttt{0}S\}, S\)$<br>||


# Týden 3


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jak definujeme homogenní konečný automat?|Neformálně:<br>Homogenní konečný automat je takový konečný automat, kde pro každý stav platí, že všechny příchozí přechody jsou ohodnoceny stejným symbolem. Nemůže se tedy například stát, že se do stavu $A$ dostaneme z~nějakého stavu na symbol $\texttt{b}$ a z~nějakého jiného stavu na symbol $\texttt{c}$.\\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-efcb61cd8b04348b2226a12db218e21aa1fcb78b.jpg"><br>||
|Mějme konečný automat $M = \(Q, \Sigma, \delta, q_0, F\)$. Jak získáme automat $M'$, kde $L\(M'\) = \Sigma^* \setminus L\(M\)$?|Jinými slovy, chceme automat, který bude přijímat doplněk jazyka $L\(M\)$. Postupujeme následovně:<br>\begin{enumerate}\item Automat $M$ převedeme na deterministický a úplně určený.\item Následně u automatu $M$ prohodíme koncové a nekoncové stavy a získáme tak automat $M'$.<br>\end{enumerate}<br>||
|Kdy řekneme, že jsou dva konečné automaty ekvivalentní?|<img style="height:128px;width:auto;" src="media/paste-2c29fa3d8b22670325e3c2f6241eccc7ff1c1d89.jpg">||
|Jak definujeme minimální DKA?|Neformálně:<br>Minimální deterministický konečný automat pro jazyk $L$ je DKA s~nejmenším možným počtem stavů přijímající jazyk $L$. Tento automat nemá nedosažitelné stavy, zbytečné stavy ani ekvivalentní stavy. Jedinou výjimkou je automat přijímající prázdný jazyk. Minimální deterministický automat přijímající prázdný jazyk má pouze jeden stav \(počáteční a nekoncový\), jenž je z definice zbytečný. Minimální deterministický automat lze sestrojit pro každý regulární jazyk, přičemž takový automat je pro každý regulární jazyk unikátní \(až na případné pojmenování stavů\). \\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-13f6860767e3ec138c52b7f03d81d099e0bb0d00.jpg"><br>||
|Mějme regulární jazyk $L$. Kolik různých minimálních DKA pro něj lze sestrojit?|Pouze jeden. Minimální DKA je pro každý regulární jazyk unikátní \(až na případné pojmenování stavů\).<br>||
|Popište algoritmus determinizace, tj. algoritmus převodu NKA na DKA pomocí podmnožinové konstrukce.&nbsp;|Neformálně:<br>Determinizace je metoda sloužící k~převodu nedeterministického automatu na deterministický. NKA se během výpočtu v jedné chvíli může nacházet v libovolné podmnožině svých stavů. Determinizace funguje na principu podmnožinové konstrukce, neboť postupně vytváří všechny možné podmnožiny stavů, ve kterých se daný NKA může během výpočtu nacházet. Tyto podmnožiny následně prohlásíme za stavy ekvivalentního deterministického automatu. V~nejhorším možném případě se může NKA během výpočtu vyskytovat ve všech možných podmnožinách svých $n$ stavů. Příslušný DKA by tak měl $2^n$ stavů. Na svém vstupu předpokládá metoda determinizace nedeterministický automat bez $\varepsilon$-přechodů s~jedním počátečním stavem. \\<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-3c89b90368f3244c02d4890c96f1b9d02265d7f7.jpg"><br>||
|Mějme NKA $M$ s $n$ stavy, který převedeme na ekvivalentní DKA $M'$. Kolik minimálně a kolik maximálně může mít $M'$ stavů?|minimálně 1, maximálně $2^n$ \(všechny možné podmnožiny $n$-prvkové množiny\)||
|Pro které operace jsou regulární jazyky uzavřené? Vysvětlete proč.|Regulární jazyky jsou uzavřené pro operace: sjednocení, průnik, doplněk, rozdíl, zřetězení \(součin\) i iterace. Důvodem je existence algoritmů nad konečnými automaty pro sjednocení, průnik, doplněk, zřetězení a iterace. Rozdíl lze vyřešit za pomoci vztahu: $L_1 \setminus L_2 = L_1 \cap \overline{L_2}$.||
|Mějme konečný automat $M = \(Q, \Sigma, \delta, q_0a, F\)$. Jak získáme automat $M^*$, kde $L\(M^*\) = L\(M\)^*$?|Neformálně:\begin{enumerate}&nbsp;\item Přidáme nový počáteční stav, který bude zároveň koncový. U původního počátečního stavu tento příznak zrušíme.&nbsp;<br> \item Z nového počátečního stavu vedeme $\varepsilon$-přechod do původního počátečního stavu.&nbsp; \item Ze všech koncových stavů \(kromě nově přidaného počátečního stavu\) vedeme $\varepsilon$-přechody do původního počátečního stavu.&nbsp;\end{enumerate}<br>Formálně:<img style="height:128px;width:auto;" src="media/paste-dc0a6081f8075147bd2d0eaf7c68ef1cc38f25f5.jpg"><br>||
|Mějme konečný automat $M_1 = \(Q_1, \Sigma, \delta_1, q_{01}, F_1\)$ a konečný automat $M_2 = \(Q_2, \Sigma, \delta_2, q_{02}, F_2\)$. Jak získáme automat $M$, kde $L\(M\) = L\(M_1\) \cup L\(M_2\)$?|Zkonstruovat automat přijímající sjednocení jazyků můžeme třemi různými způsoby:<br> \begin{itemize}&nbsp;\item $\varepsilon$-přechody \(vstup: dva libovolné KA\)&nbsp;\item automat s~více počátečními stavy \(vstup: dva libovolné KA\)\item paralelní činnost automatů \(vstup: dva úplně určené KA\).&nbsp;\end{itemize}<br>Paralelní činnost:<img style="height:128px;width:auto;" src="media/paste-c1acb40aaf09a6e63785ad880540932eaadc2ee0.jpg"><br><br>Formálněji:<img style="height:128px;width:auto;" src="media/paste-c3acbb809885c44866502d942720c24c48af1011.jpg"><br><br><br>||


# Týden 4


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Kdy nazveme dva regulární výrazy identické?|<img style="height:128px;width:auto;" src="media/paste-93b2af9d0491ab5da4d0a7ec6e911f1a88f06dff.jpg">||
|Kdy nazveme dva regulární výrazy ekvivalentní?|<img style="height:128px;width:auto;" src="media/paste-0f6faabe08b28460f609c93d58bbe165ec01baf6.jpg">||
|Kdy nazveme dva regulární výrazy podobné?|<img style="height:128px;width:auto;" src="media/paste-8472ea3376e6d775af6833c405404df9f520277f.jpg">||
|Vyslovte Kleeneovu větu.|<img style="height:128px;width:auto;" src="media/paste-1729c26b6b225e2327fe90a34cd8822372fd1446.jpg">||
|Jak definujeme regulární výraz?|<img style="height:128px;width:auto;" src="media/paste-cef54d9d7c1e9160fcabda6d9812b3226bb5e69a.jpg">||
|Jak definujeme hodnotu regulárního výrazu?|<img style="height:128px;width:auto;" src="media/paste-42d52aa2811e677f6a4274a0757159f8b51730e0.jpg"><br><br>||
|Popište algoritmus, který pro regulární gramatiku $G$ vytvoří konečný automat $M$ takový, že $L\(G\) = L\(M\)$.|<img style="height:128px;width:auto;" src="media/paste-9c2cafc56f6c780b764f880083386548b1e73ce8.jpg">Formálněji:<img style="height:128px;width:auto;" src="media/paste-368e1666b709159e2eec47715e1513dff4cafb1f.jpg"><br>||
|Jak definujeme derivaci regulárního výrazu?|<br><img style="height:128px;width:auto;" src="media/paste-ed1df5f9e82c587df49efd91802d34faa1a66606.jpg"><br>||
|Popište algoritmus, který pro konečný automat $M$ vytvoří regulární gramatiku $G$ takovou, že $L\(G\) = L\(M\)$.|<img style="height:128px;width:auto;" src="media/paste-982dbf80e6d9aaa6aa4469e5257db43ffef06f8e.jpg"><img style="height:128px;width:auto;" src="media/paste-509c9d096643c42a50ccde6f22ecbc489c4027e5.jpg"><br>Formálněji:<img style="height:128px;width:auto;" src="media/paste-23b64c94e05a024b584bdf0189eeb0cc0141eb65.jpg"><br>||


# Týden 5


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jaké máme metody pro převod regulárního výrazu na konečný automat?|<img style="height:128px;width:auto;" src="media/paste-d25592429bd8317e9ccefc9e83bd5d5f18f1dab8.jpg">||
|Jaké máme metody pro převod konečného automatu na regulární výraz?|<img style="height:128px;width:auto;" src="media/paste-5abf0a93d1491570cf8f3c587c5fa935d6b28972.jpg">||
|Jak definujeme rozšířený konečný automat a kde se využívá?|<img style="height:128px;width:auto;" src="media/paste-4342ffbcd4cb5820cf1c374e30c2e968803ca396.jpg">Využití: převod KA na RV pomocí metody elimací stavů<br>||
|Jaké máme metody pro převod regulární gramatiky na regulární výraz?|<img style="height:128px;width:auto;" src="media/paste-552c0beb9eea0076cce419f787c2df47d2c21d13.jpg">||
|Jak definujeme rozšířenou regulární gramatiku a kde se využívá?|<img style="height:128px;width:auto;" src="media/paste-ab2152357294daa9941d25245692be693253d61d.jpg">Využití: převod RG na RV pomocí metody elimací neterminálních symbolů||
|Jaké máme metody pro převod regulárního výrazu na regulární gramatiku?|<img style="height:128px;width:auto;" src="media/paste-d1f2ae6df396001e2b9fc10be37befad385dd7bc.jpg">||


# Týden 6


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Co říká pumping lemma?|<img style="height:128px;width:auto;" src="media/paste-dd9db038b41cb8aeed8046137c3cadd851f9b0c4.jpg"><br><img style="height:128px;width:auto;" src="media/paste-adf1f9f9910837cbc1fc39f2a8ebc2c1022a5b1d.jpg"><br><br><img style="height:128px;width:auto;" src="media/paste-10dce0766e889e02de21526ad4e40b153a09f5ba.jpg"><br><br>||
|Vyslovte Myhill-Nerodovu větu.|<img style="height:128px;width:auto;" src="media/paste-47eaa4ff0e1dcdc379e2cf3e68961aaec769a7ce.jpg">||
|Jak definujeme pravou kongruenci?|<img style="height:128px;width:auto;" src="media/paste-74884659caee62e441bc2852a94e6b7562e0b40a.jpg"><br>||
|Jak definujeme prefixovou ekvivalenci?|<img style="height:128px;width:auto;" src="media/paste-5c8f509dfcf686defd32790f4e34432908bb2ff4.jpg"><br>||
|Definujte index ekvivalence.|<img style="height:128px;width:auto;" src="media/paste-15f507e09a184c7cda8e7579365ef1baa6ecc611.jpg">||
|Definujte rozklad množiny.|<img style="height:128px;width:auto;" src="media/paste-39827c0cd5dafa439d76c988ef57bb881ceae7f5.jpg">||
|Definujte třídu ekvivalence.|<img style="height:128px;width:auto;" src="media/paste-e0b6da1cf845c85dd6b1c3e024791d25f296d2b2.jpg">||


# Týden 7


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Kdy bezkontextovou gramatiku nazveme nejednoznačnou \(víceznačnou\)?|<img style="height:128px;width:auto;" src="media/paste-8bf02eb6bfaa164df69b59a4ae85be44b2150309.jpg">||
|Definujte nedostupný symbol v bezkontextové gramatice $G = \(N, \Sigma, P, S\)$|<img style="height:128px;width:auto;" src="media/paste-ff823c0f513909757eedb2587c34b6f59d9570f3.jpg">||
|Definujte zbytečný symbol v bezkontextové gramatice $G = \(N, \Sigma, P, S\)$|<img style="height:128px;width:auto;" src="media/paste-4bffc7efd3d89b1b1529ee8fae49b2c6b23830e4.jpg">||
|Kdy bezkontextovou gramatiku nazveme redukovanou?|<img style="height:128px;width:auto;" src="media/paste-5b01f8851d66809d8d13bf380dc467f1840bbc15.jpg">||
|Kdy bezkontextovou gramatiku nazveme bez cyklů?|<img style="height:128px;width:auto;" src="media/paste-9eaa401e48519ddfc4d2f9e50a0f5a33a319939d.jpg">||
|Kdy bezkontextovou gramatiku nazveme bez $\varepsilon$-pravidel?|<img style="height:128px;width:auto;" src="media/paste-4e937b5349033b8e708200ae0976ee0fdc903885.jpg">||
|Definujte vlastní bezkontextovou gramatiku.|<img style="height:128px;width:auto;" src="media/paste-aab71f8231abc354ed0e840e1129e517d004f65d.jpg">||
|Definujte Chomského normální tvar pro bezkontextové gramatiky.|<img style="height:128px;width:auto;" src="media/paste-168f041e5051a75702130fd5c139cdce5ebcda15.jpg">||
|Kdy bezkontextovou gramatiku nazveme rekurzivní?|<img style="height:128px;width:auto;" src="media/paste-9094cf60d5b20484a12bc997bbc6203cfca55083.jpg"><img style="height:128px;width:auto;" src="media/paste-bdd8ded01975278b6500a214d570a6384699a85b.jpg"><br>||


# Týden 8


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jak definujeme zásobníkový automat?|<img style="height:128px;width:auto;" src="media/paste-fd0186b389f9c9ac402d661b898cecc3636904f8.jpg">||
|Jak definujeme konfiguraci zásobníkového automatu?|<img style="height:128px;width:auto;" src="media/paste-b5cc555f8f5d7f28903394520da26588616fb93e.jpg">||
|Jak definujeme jazyk přijímaný zásobníkovým automatem?|<img style="height:128px;width:auto;" src="media/paste-e662ee9726b770b0a59b7a90efc10fbef252cadc.jpg">||
|Jak definujeme levou \(pravou\) derivaci v bezkontextové gramatice $G$?|<img style="height:128px;width:auto;" src="media/paste-50c19c3ddefca876b49063b746d1582fa2651364.jpg">||
|Jak definujeme levý \(pravý\) rozklad větné formy?|<img style="height:128px;width:auto;" src="media/paste-09a84ea98d3cb3fc02460d431387f2c268323eff.jpg">||
|Jaké znáte metody syntaktické analýzy?|<img style="height:128px;width:auto;" src="media/paste-87d896bf69fb9c6281d5a6993abbcd03c2b50438.jpg">||
|Jak pro danou bezkontextovou gramatiku $G = \(N, \Sigma, P, S\)$ vytvořit zásobníkový automat jako model syntaktického analyzátoru metodou shora dolů?|<img style="height:128px;width:auto;" src="media/paste-741d3a0d59d1b59578394f92de3a7d4ab5aa73e3.jpg">||
|Jak pro danou bezkontextovou gramatiku $G = \(N, \Sigma, P, S\)$ vytvořit zásobníkový automat jako model syntaktického analyzátoru metodou zdola nahoru?|<img style="height:128px;width:auto;" src="media/paste-2d7c9d1cd6d776cddc8888e2582d605402299610.jpg">||
|Jak definujeme deterministický zásobníkový automat?|<img style="height:128px;width:auto;" src="media/paste-96c0e0eb5b1f12acd146656d73cfce197f3a8205.jpg">||


# Týden 9


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jak definujeme \(počáteční\) konfiguraci zásobníkového překladového automatu?|<img style="height:128px;width:auto;" src="media/paste-94fc0e66f22ac54f0e98525e01ef773a4e4f1031.jpg">||
|Jak definujeme formální překlad?|<img style="height:128px;width:auto;" src="media/paste-c1b33d2eae218fd9affdf150d7f53aec1b0d15b3.jpg">||
|Co je to homomorfismus?|<img style="height:128px;width:auto;" src="media/paste-3585d7b8265bbf3506619651baa4d131e2083612.jpg">||
|Jak definujeme překladovou gramatiku?|<img style="height:128px;width:auto;" src="media/paste-ad500b1621593ed4ceb91f2e1c4a371af3207906.jpg">||
|Jak definujeme vstupní/výstupní homomorfismus?|<img style="height:128px;width:auto;" src="media/paste-37786ac23949d3e4bc7f912ca9b5c3b629a72440.jpg">||
|Jak definujeme překlad definovaný překladovou gramatikou?|<img style="height:128px;width:auto;" src="media/paste-d2e565300c94e49501c1da2c1ca4f75794414495.jpg">||
|Jak definujeme vstupní/výstupní gramatiku překladové gramatiky?|<img style="height:128px;width:auto;" src="media/paste-7974198150637149770ead305d78d31795bf1c0a.jpg">||
|Jak definujeme charakteristickou gramatiku/jazyk/větu?|<img style="height:128px;width:auto;" src="media/paste-94a98efdb7d99ebfd82014d8bd1170cc91dbf538.jpg">||
|Jak definujeme regulární překladovou gramatiku?|<img style="height:128px;width:auto;" src="media/paste-8d4856e6e1c209e54af063ee62d3fc260686a949.jpg">||
|Jak definujeme překlad definovaný konečným překladovým automatem?|<img style="height:128px;width:auto;" src="media/paste-b166caf874b0ab589ac7f92cbe394450db0065d6.jpg">||
|Kdy konečný překladový automat nazveme deterministickým?|<img style="height:128px;width:auto;" src="media/paste-8501ef67c297b52a650089d48673da5454b4df08.jpg">||
|Jak definujeme konečný překladový automat?|<img style="height:128px;width:auto;" src="media/paste-f4f3ed085c05b40b9c13116c8ace2b6cf95e0695.jpg">||
|Jak definujeme \(počáteční/koncovou\) konfiguraci konečného překladového automatu?|<img style="height:128px;width:auto;" src="media/paste-324b2d4875085a38388d50d1a208da5ffd235fa2.jpg">||
|Jak definujeme Mealyho automat?|<img style="height:128px;width:auto;" src="media/paste-2fb17a7752af805ae80b065d025ca5b819d3a9a9.jpg">||
|Jak definujeme Mooreův automat?|<img style="height:128px;width:auto;" src="media/paste-d2cc8e452cb61cf151f38113f2bdb8f086d67e26.jpg">||
|Jak definujeme zásobníkový překladový automat?|<img style="height:128px;width:auto;" src="media/paste-502f6f22bb080cf82ee8e1deac95b57b1729bd3d.jpg">||
|Jak definujeme překlad definovaný zásobníkovým překladovým automatem?|<img style="height:128px;width:auto;" src="media/paste-b94f1f1b69621eb618a3d0a140f16eee2876a15d.jpg">||
|Kdy zásobníkový překladový automat nazveme deterministickým?|<img style="height:128px;width:auto;" src="media/paste-7db863577ed5b275321e54b3738b5a058d6de82e.jpg">||


# Týden 10


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Na které operace jsou uzavřeny kontextové jazyky?|<img style="height:128px;width:auto;" src="media/paste-f590a003fd15c5c02f6a472429de5e8c3f907d4f.jpg"><br>||
|Na které operace jsou uzavřené rekurzivně spočetné jazyky?|<img style="height:128px;width:auto;" src="media/paste-4839237e75c679431596dcbcfdd220ada1517558.jpg">||
|Jak definujeme deterministický Turingův stroj?|<img style="height:128px;width:auto;" src="media/paste-1c121a8826f21e897a4c94d5d03f094f4aff1b1b.jpg">||
|Jak definujeme konfiguraci Turingova stroje?|<img style="height:128px;width:auto;" src="media/paste-43e174edbd6802025504ba6c3a82cbcb859464a1.jpg">||
|Jak definujeme jazyk přijímaný Turingovým strojem?|<img style="height:128px;width:auto;" src="media/paste-05adec171027aff388e151f6c28343493d032f20.jpg">||
|Jak definujeme nedeterministický Turingův stroj?|<img style="height:128px;width:auto;" src="media/paste-26360df89a5c8ef0999ca9d40901e5552d6a1bd0.jpg">||
|Kdy nazveme Turingův stroj lineárně omezený?|<img style="height:128px;width:auto;" src="media/paste-acae78fde1359e527161fae72e546a453da5256c.jpg"><img style="height:128px;width:auto;" src="media/paste-540827745f6b236e2c5e9373f92b8e7f9871f5cc.jpg"><br>||
|Porovnejte výpočetní sílu deterministického a nedeterministického Turingova stroje.|<img style="height:128px;width:auto;" src="media/paste-03c187ffe0371ca1f3dc75ef82b800b1f88957b6.jpg">Tedy: Nedeterministický a deterministický Turingův stroj jsou výpočetně ekvivalentní. Oba přijímají pravě množinu rekurzivně spočetných jazyků. DTS je speciálním případem NTS a každý NTS lze převést na DTS.<br>||
|Lze každou nezkracující gramatiku převést na kontextovou?|<img style="height:128px;width:auto;" src="media/paste-99a4f99e9e072707416cee4018634345a18d1af6.jpg">Důsledek: Nezkracující gramatiky generují právě kontextové jazyky.||
|Co říká Church-Turingova teze?|<img style="height:128px;width:auto;" src="media/paste-413eab5b16feee8b8c1cd96fdb5973ac5d8b3e0f.jpg">||
|Definujte univerzální Turingův stroj.|<img style="height:128px;width:auto;" src="media/paste-b81021bd8df668d7f367de3bcb99f85441a0343f.jpg"><img style="height:128px;width:auto;" src="media/paste-81acc48f4924a5602f6a8af1a637ef4d59c55bb1.jpg"><br>||
|Jak definujeme třídu rekurzivních jazyků?|<img style="height:128px;width:auto;" src="media/paste-0c8ac3323356168abf8620858de639edd3877b80.jpg"><img style="height:128px;width:auto;" src="media/paste-0c71fd60202c082a0fa913159a6e4ab0c58290bf.jpg"><br><br>||
|Definujte třídy P a NP.|<img style="height:128px;width:auto;" src="media/paste-966b28a9d12a99bb6d1a0a2a44e26465d857c8a6.jpg">||
|Co je to polynomiální redukce?|<img style="height:128px;width:auto;" src="media/paste-8a22c4297468bbc67aedf532d4e29e27d4aecad4.jpg">||
|Jak definujeme NP-těžký problém?|<img style="height:128px;width:auto;" src="media/paste-17bba0eef9423aef488d13d381c786f45841311b.jpg">||
|Jak definujeme NP-úplný problém?|<img style="height:128px;width:auto;" src="media/paste-4d322656594a91058ba0b4519fbd3f7d69431360.jpg">||
|Vysvětlete problém zastavení Turingova stroje. Je tento problém rekurzivní?|<img style="height:128px;width:auto;" src="media/paste-a32eb40ebe094243b173e134954af92ca7785cf3.jpg">||


# Týden 11


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Jaké jsou dva základní přístupy programové realizace konečného automatu?|<img style="height:128px;width:auto;" src="media/paste-c7bd5468eeb2ea1de4184fce04a2122152c1eb56.jpg"><img style="height:128px;width:auto;" src="media/paste-0da4c0f0112c927a7d081f2a595f22e00ad29453.jpg"><br>||


# Týden 12


|Otázka|Odpověd|Poznámky // Zdroje |
|--------|---------|----------|
|Popište jak funguje kompilační překladač.|<img style="height:128px;width:auto;" src="media/paste-2fabaf8955677386d207ae63987a7da717d7eb8b.jpg">||
|Popište jak funguje interpretační překladač.|<img style="height:128px;width:auto;" src="media/paste-b4b863968e3901654914047406ea329f8fec3e2c.jpg">||
|Jaká je úloha lexikálního analyzátoru v překladači?|<img style="height:128px;width:auto;" src="media/paste-47bcc4990e486059fd75c92c3666a467628b9f31.jpg">||
