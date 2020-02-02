Náš kurz začneme stručným shrnutím základních kvantově mechanických
představ. Kde se kvantová mechanika vzala? Jak vůbec někoho napadlo
vymýšlet nové pohybové rovnice mikrosvěta?

Kvantová mechanika se dříve také nazývala mechanikou vlnovou. Oba tyto
názvy reflektují jisté překvapivé rysy této nové mechaniky, které se
zdají být v rozporu s každodenní zkušeností. Přídavné jméno odkazuje na
nespojitost energetických hladin, pojem pak na podvojný charakter
částic, které se za jistých okolností mohou chovat jako vlny. Tyto dva
rysy kvantové mechaniky jsou hluboce provázány.

Částice a vlny
--------------

Pojďme si na začátek zopakovat, jaký je rozdíl mezi částicemi a vlnami.
Oba tyto pojmy odkazují na nějakou formu pohybu. Částice představují
objekty s definovanou hmotností, polohou a hybností. Polohou a hybností
je určen stav částice. Jestliže pro danou částici známe její polohu a
hybnost v určitém čase, pak s pomocí pohybových rovnic (například rovnic
Newtonových) můžeme určit polohu a hybnost částice v libovolném čase
budoucím – budeme tedy znát trajektorii. Uvažujme nejjednodušší případ
v jedné dimenzi. Částice se na počátku, $t_0$, nachází v bodě $x_0$. Pro
částici pohybující se podél osy $x$ v potenciálu V($x$) můžeme zapsat
pohybovou rovnici jako
$$m \frac{\dd ^2 x}{\dd t^2} = -\frac{\dd {V}}{\dd x}  
\label{rov:Castice}$$ přičemž řešením bude poloha částice v čase $t$,
$x(t; x_0,p_0)$.

Newtonova rovnice má povahu základního zákona, ve kterém jsou další
mechanické zákony obsaženy. Takto můžeme například získat zákon
zachování energie. Definujme si funkci $H$, tzv. Hamiltonovu funkci
$$H = \frac{p^2}{2m}+V
\label{rov:hamiltonfce}$$

Tato funkce je funkcí času, neboť částice se pohybuje a mění se tak její
rychlost (a tedy i hybnost a kinetická energie), stejně jako její poloha
(a tedy energie potenciální). Snadno nyní dokážeme, že $H$ se s časem
nemění. Bude nás zajímat výraz $\frac{\dd H}{\dd t}$. S uvážením, že
$$\frac{\dd V}{\dd t} = \frac{\dd V}{\dd x} \frac{\dd x}{\dd t}
\label{rov:Castice2}$$ a
$$\frac{\dd (p^2)}{\dd t}= 2p\frac{\dd p}{\dd t} = 2m^2v\frac{\dd v}{\dd t} = 2m^2\frac{\dd x}{\dd t}\frac{\dd^2x}{\dd t^2}
\label{rov:Castice3}$$ vidíme, že
$$\frac{\dd H}{\dd t} = \frac{\dd x}{\dd t}\left ( m\frac{\dd ^2x}{\dd t^2}+\frac{\dd V}{\dd x}\right)
\label{rov:Castice4}$$ Výraz v závorce je ovšem dle Newtonova zákona
(rovnice ) roven nule a tedy i $\frac{\dd H}{\dd t}$ je rovno nule.
Energie se tudíž v klasické mechanice zachovává. Dlužno podotknout, že
pokud umístíme částici například do časově proměnného pole, Hamiltonova
funkce se bude měnit s časem explicitně a energie se pak již zachovávat
nebude.

Newtonova mechanika popisující částice (případně některá
z ekvivalentních formulací jako jsou formulace Lagrangeova či
Hamiltonova) byla historicky mimořádně úspěšná. Za všechny úspěchy
můžeme jmenovat například správnou předpověď existence planety Neptun.

V klasické fyzice vidíme rozdíl mezi vlnou a částicí v tom, že při
pohybu částic se prostorem přenáší hmota, při vlnění se naproti tomu
prostorem přenáší energie. Vlna není na rozdíl od částic plně
lokalizovatelná. Hlavní rozdíl mezi vlnou a částicí je ale schopnost vln
se skládat, jev, který označujeme jako **interferenci**. Při
interferenci je amplituda složené vlny rovna součtu amplitud
jednotlivých vln. Pokud mají v daném bodě jednotlivé amplitudy stejné
znaménko, pak mluvíme o konstruktivní interferenci. Tam, kde mají
amplitudy jednotlivých vln opačná znaménka, dochází k destruktivní
interferenci. Takový interferenční obrazec je možné pozorovat například
při průchodu světla dvojštěrbinou (viz obrázek \[obr:Interference\]).
Vlny procházející štěrbinami interferují a na stínítku tak vzniká
interferenční obrazec.

\[ht\]

Bude užitečné si na začátek zopakovat některé veličiny, které
charakterizují vlnění (viz obrázek \[obr:Vlna\]). Pohyb vlny (zde
v jedné dimenzi) je určen velikostí nějaké veličiny (například výšky
vodní hladiny či intenzity elektrického pole) měnící se v prostoru a
v čase, označme si tuto veličinu $A(x,t)$.

\[ht\] ![Schematické znázornění
vlny[]{data-label="obr:Vlna"}](vlna-bw.pdf "fig:")

V nejjednodušším případě se bude vlna šířit harmonicky ve směru osy $x$
$$A(x, t) = A_0 \sin\left[2\pi \left ( \frac{x}{\lambda}-\frac{t}{T} \right)\right]
\label{rov:Vlna}$$ kde $\lambda$ je **vlnová délka**, udávající
vzdálenost mezi dvěma nejbližšími maximy vlny pro určitý čas a $T$ je
**perioda**, udávající časový interval mezi dosažením maxima dvou po
sobě jdoucích vln pro určité místo. Reciprokou hodnotu periody $T$
označujeme jako **frekvenci** $\nu = \frac{1}{T}$. Mezi vlnovou délkou a
frekvencí platí vztah $$\lambda = \frac{c}{\nu}
\label{rov:Vlna2}$$ K popisu vlny se také používá veličina **vlnočet**
$\widetilde{\nu}=\nicefrac{\nu}{c}$. Ten nám udává, kolik vlnových délek
se vměstná na 1m. Často se místo vlnové délky a frekvence setkáváme se
zápisem pomocí **vlnového čísla** $k$ a **úhlové frekvence** $\omega$
$$k = \frac{2\pi}{\lambda}
\label{rov:Vlna3}$$ $$\omega = 2\pi\nu
\label{rov:Vlna4}$$ Postupné vlnění ve směru osy $x$ pak můžeme zapsat
pomocí těchto veličin $$A(x,t)=A_0 \sin(kx - \omega t)
\label{rov:Vlna5}$$ Jak jsme již zmínili výše, k základním rysům vlnění
patří jeho skládání. Složme teď dvě vlny o stejné frekvenci, které se
pohybují proti sobě $$A(x,t)=A_0[sin (kx-\omega t)+ \sin (kx+\omega t)]
\label{rov:Vlna6}$$ S takovouto situací se setkáváme třeba při rozvlnění
struny na kytaře. S využitím vzorců pro sinus součtu úhlů
$$\sin(\alpha \pm \beta) = \sin \alpha\cos\beta \pm \cos\alpha\sin\beta
\label{rov:Vlna7}$$ získáme úpravou
$$A(x,t)=2A_0\sin (kx) \cos (\omega t) = A'(x)\cos (\omega t)
\label{rov:Vlna8}$$ Vidíme tak, že v tomto případě bude tvar vlny stále
stejný a celá vlna bude pouze periodicky růst a klesat. Mluvíme
o stojatém vlnění. Uvidíme dále, že tento typ vlnění je pro chemii velmi
důležitý.

Ukazuje se, že každé vlnění je možné popsat **vlnovou rovnicí** (zde
opět pro jednorozměrný problém)
$$\boxed{\frac{\pd ^2A(x,t)}{\pd x^2} = \frac{1}{\nu^2}\frac{\pd^2A(x,t)}{\pd t^2}}
\label{rov:Vlna9}$$ Z matematického hlediska jde o parciální
diferenciální rovnici druhého řádu. Tuto rovnici lze kupříkladu pro
popis pohybu struny na kytaře odvodit z Newtonovy mechaniky, v případě
elektromagnetického záření pak zase z Maxwellových rovnic.

Experimenty, které změnily svět
-------------------------------

Na konci devatenáctého století se fyzika zdála být skoro dobudována.
Objekty světa byly uspokojivě popsány buď Newtonovou mechanikou
(částice) či Maxwellovou elektrodynamikou. Velké soubory částic pak
zpracovávala statistická fyzika a termodynamika. Ve století dvacátém
nicméně došlo k zásadnímu obratu a mnohé jistoty vzaly za své. Níže
zběžně popíšeme některé základní experimenty, které lidstvo přivedly od
světa klasického do světa kvantového. Tyto experimenty z různých pohledů
ukazovaly na dva základní rysy kvantové mechaniky (a) **kvantování
energie**, (b) **vlnově-částicový dualismus**.

### Záření absolutně černého tělesa

Absolutně černým tělesem máme na mysli objekt, který pohltí veškeré
dopadající záření, žádné záření tedy není odraženo. Může být realizováno
třeba dutinou s malým otvorem – světlo mnohokráte narazí na stěny
nádoby, takže pravděpodobnost, že by odražené světlo vylétlo otvorem
zase ven, je mizivá. Černé těleso ale zároveň musí energii vyzařovat,
jinak by se v něm hromadila. Badatele zajímalo, jakým způsobem intenzita
vyzářeného světla závisí na jeho frekvenci. Experimentálně bylo
zjištěno, že hustota záření pro malé frekvence je velmi malá a roste se
zvyšující se frekvencí. V závislosti na teplotě pak dosahuje svého
maxima a posléze zase klesá. Maximum hustoty se navíc posunuje
s teplotou k vyšším frekvencím. Je to v souladu se zkušeností – horká
kamna vyzařují v infračervené oblasti spektra, zatímco rozžhavené železo
již vyzařuje ve viditelné oblasti.

Při teoretickém modelování předpokládáme, že k vyzařování světla
o určité frekvenci dochází při oscilacích elektrického dipólu – podobně,
jako je tomu u antény vysílače. Oscilující dipól vzniká díky pohybu
nabitých částic. Z teorie plyne vztah mezi hustotou záření $\rho(\nu,T)$
a střední energií oscilátoru $\bar{E}_{\mathrm{osc}}$ při dané teplotě
$$\rho(\nu,T)=\frac{8\pi\nu^2}{c^3}\bar{E}_{\mathrm{osc}}
\label{rov:Cerneteleso1}$$ V klasické statistické mechanice ale platí,
že střední energie každého (harmonického) oscilátoru je nezávislá na
frekvenci a rovna $k_{\mathrm{B}}T$. To by ale znamenalo, že vyzářená
energie poroste se čtvercem frekvence! To je sice pravda pro malé
frekvence, ale předpověď naprosto selhává pro frekvence vysoké. Vždyť by
to znamenalo, že rozžhavený kámen by měl být intenzivním zdrojem
rentgenového záření.

Max Planck přišel s myšlenkou, že souladu s experimentem můžeme
dosáhnout za předpokladu, že elektromagnetický oscilátor[^1] nemůže
nabývat libovolných hodnot, nýbrž pouze hodnot $$E=nh\nu
\label{rov:Cerneteleso2}$$ kde $h$ je Planckova konstanta a $n$ je celé
číslo. Záření pak může být předáváno pouze po minimálních balíčcích
$h\nu$, což je nejmenší rozdíl energie mezi dvěma hladinami oscilátoru.
Při konečné teplotě je střední hodnota energie oscilátoru rovna
$$\bar{E}_{\mathrm{osc}}=\frac{h\nu}{\mathrm{e}^{\frac{h\nu}{k_{\mathrm{B}}T}}}-1
\label{rov:Cerneteleso3}$$ a po dosazení do vztahu pak získáme
$$\rho(\nu,T) = \frac{8\pi h\nu^3}{c^3}\frac{1}{\mathrm{e}^{\frac{h\nu}{k_{\mathrm{B}}T}}-1}
\label{rov:Cerneteleso4}$$ Tento vztah báječným způsobem souhlasil
s experimentem, pokud za hodnotu konstanty $h$ dosadíme číslo
$6{,}626\cdot10^{-34}$ J$\cdot$s.

Je třeba ale vidět, že souladu s experimentem bylo dosaženo za použití
v té době dosti bláznivých předpokladů. Předně předpokládáme, že pohyb
částic je omezen jen na určité hodnoty energie, je kvantován. Za druhé,
předpokládáme, že světlo je předáváno do okolí ve formě jakýchsi dále
nedělitelných balíčků energie. Není proto nijak podivné, že Planck celou
věc nebral příliš vážně. Planckovu představu ale tvůrčím způsobem využil
Albert Einstein ve své teorii fotoelektrického jevu, díky které se
právem počítá mezi zakladatele kvantové mechaniky.

### Teorie fotoelektrického jevu

Základní schéma fotoelektrického jevu je zobrazeno na
obrázku \[obr:Fotoefekt\]. V elektrickém obvodu měříme elektrický proud
přenášený elektrony, které jsou uvolňovány z ozařovaných kovových
destiček. Ze závislosti prošlého fotoelektrického proudu na vloženém
napětí můžeme zjistit jak maximální kinetickou energii vyražených
elektronů tak i jejich celkové množství.

\[ht\]

Co bychom předpokládali z hlediska klasické teorie? K vyražení elektronů
by mělo dojít světlem každé vlnové délky, pokud bude mít dostatečnou
intenzitu. Ukázalo se však, že k průchodu fotoelektrického proudu
nedocházelo pro frekvence světla nižší než určitá mezní frekvence
$\nu_0$, charakteristická pro daný kov. Energie vyražených elektronů pak
lineárně rostla s frekvencí. Albert Einstein tyto výsledky interpretoval
velmi odvážně. Konstatoval, že světlo představuje proud částic o energii
$h\nu$ a vyražení elektronu si pak představoval jako srážkový děj mezi
touto světelnou částicí a elektronem. Hypotéza musela působit velmi
podivně, vždyť Newtonův pohled na světlo jako na proud částic byl již
dávno opuštěn a Maxwellova elektrodynamika měla za sebou mnoho úspěchů.
Pro závislost kinetické energie elektronů na frekvenci záření by pak
měla platit rovnice $$E_{kin} = h\nu - \phi
\label{rov:Fotojev1}$$ kde $\phi = h\nu_0$ se nazývá výstupní práce.
Rovnice vyjadřuje zachování energie – energie fotonu se musí rovnat
výstupní práci elektronu a jeho kinetické energii.

Jestliže nafitujeme hodnotu experimentálních dat na rovnici , získáme
hodnotu $h = \SI{6.626e-34}{\J\s}$. Einsteinův balíček energie je
charakterizován úplně stejně jako Planckův balíček energie!

[Fotoelektronová spektroskopie]{} Fotoelektrický jev je principem
techniky nazvané fotoelektronová spektroskopie. Pokud ozařujeme vzorek
zářením o dostatečné energii, dojde k vyražení elektronů, jejichž
rychlost můžeme měřit. S využitím vztahu pak získáme hodnotu výstupní
práce pro daný vzorek. Tato práce představuje vlastně vazebnou energii,
kterou je držen elektron v dané molekule či v materiálu. Z hodnoty
vazebné energie se pak dá například zjistit složení vzorku či chemická
forma, ve které se nachází určitý atom. Fotoelektronová spektroskopie je
hojně používaná zejména v oblasti vědy o površích, neboť detekovány jsou
především elektrony pocházející z povrchových vrstev vzorku. Je ale
možné provádět měření i v plynné fázi.

Interpretaci fotoelektronového spektra si můžeme vyzkoušet například na
spektru neznámého prvku na následujícím obrázku.

![image](pes-Mg.png)

Víme, že ve fotoelektronovém spektru je vynesena hodnota vazebné energie
jednotlivých elektronů. Pro elektrony ve vnitřních slupkách je vazebná
energie nejvyšší, tj. elektrony jsou drženy u jádra nejsilněji, pro
elektrony ve valenční sféře je hodnota ionizační energie naopak
nejnižší. Ve spektru se nacházejí 4 píky, pík s nejvyšší energií (cca
1350 eV) přísluší 1s elektronům, pík s energií cca 105 eV (a stejnou
intenzitou jako pík s nejvyšší energií) přísluší elektronům z orbitalu
2s. Další pík s energií cca 65 eV pak odpovídá ionizaci elektronů
v orbitalu 2p. Intenzita tohoto píku je trojnásobná oproti předešlým,
v p orbitalech je tedy třikrát více elektronů. Poslední pík s energií
cca $7{,}5$ eV, opět se stejnou intenzitou jako první dva píky, odpovídá
ionizaci elektronů z 3s orbitalu. Předpokládaná elektronová konfigurace
je tedy 1s$^2$2s$^2$2p$^6$3s$^2$, což odpovídá elektronové konfiguraci
hořčíku v plynné fázi.

**Zadání:** Pokud budeme ozařovat páry atomu hořčíku ultrafialovým
zdrojem světla He II o energii 52 eV (odpovídá vlnové délce ), jaká bude
kinetická energie vyražených elektronů? Využijte vazebné energie hořčíku
v předchozím boxu. 0.3cm

**Řešení:** Zdroj světla o energii 52 eV má dostatečnou energii pouze
k vyražení elektronu z orbitalu 3s. Kinetickou energii odletujících
elektronů zjistíme využitím vztahu , kde za výstupní práci dosadíme
ionizační energie pro orbital 3s (tedy 7[,]{}5 eV). Kinetická energie
elektronů je 44[,]{}5 eV.

Einstein šel ve svých úvahách ještě dále. Je-li podle něj světlo
částicí, měla by tato částice (později nazvaná foton) mít také nějakou
hybnost. Jelikož se ale pohybuje rychlostí světla, měla by tato hybnost
být dána již relativistickým výrazem
$$p = mv = \frac{m_0 v}{\sqrt{1-\frac{v^2}{c^2}}}
\label{rov:Fotojev2}$$ kde $m_0$ je klidová hmotnost fotonu a $c$ je
rychlost světla ve vakuu. Výraz ve jmenovateli je nulový, takže aby
hybnost byla konečné číslo, musí mít foton nutně nulovou klidovou
hmotnost. Upravme nyní výraz pro relativistickou hybnost
$$p^2c^2 = \frac{m_0^2v^2c^2}{1-\frac{v^2}{c^2}} = \frac{m_0^2 c^4 (\frac{v^2}{c^2}-1)}{1-\frac{v^2}{c^2}} + \frac{m_0^2 c^4}{1-\frac{v^2}{c^2}} = -m_0^2 c^4 + m^2c^4
\label{Fotojev3}$$ Do posledního členu v předchozí rovnici nyní dosadíme
známý vzorec $E=mc^2$, čímž dostaneme $$E^2 = p^2c^2+ m_0^2c^4
\label{Fotojev4}$$ Jelikož ale pro foton platí $m_0$ = 0, tak také
$$E=pc
\label{rov:Fotojev5}$$ S použitím Planckova vztahu
$E = h\nu = \frac{hc}{\lambda}$ dostáváme
$$\boxed{\lambda = \frac{h}{p}}
\label{rov:Fotojev6}$$

[Laserové chlazení atomů]{} Světlo si většinou nespojujeme s chlazením,
spíše máme zkušenost, že nás světlo dokáže zahřát. Světlo je ale
částice. Když se srazí s atomem, předá mu svou hybnost a může jej tím
zpomalit! Pro získání představy si vypočítejme následující úlohu.

**Zadání:** Kolik fotonů o vlnové délce zastaví atom vápníku
$^{40}\mbox{Ca}$ s molární hmotností
$M(\text{Ca}) = \SI{39{,}96}{\g\per\mol}$ vypařovaný z kovového vápníku
v pícce o teplotě $600\,^{\circ}$C?\
**Řešení:** Atomy vápníku v pícce mají kinetickou energii danou vztahem
$$E = \frac{3}{2} k_{\mathrm{B}}T = \SI{1{,}81e-20}{\J}$$ Hybnost je
dána jako $$p = \sqrt{2 m E} = \SI{4,90e-23}{\kg\m\per\s}$$ z čehož
dopočítáme střední kvadratickou rychlost
$$v = \frac{p}{m} = \SI{738}{\m\per\s}$$ Atom vápníku můžeme zářením
ionizovat, vzniklý ion uvěznit v iontové pasti a v ní ho bombardovat
zářením. Fotony světla udané vlnové délky mají hybnost
$$p_{\mbox{foton}}= \frac{h}{\lambda} = \SI{1{,}66692e-27}{\kg\m\per\s}$$
Při pohlcení jednoho fotonu dojde tedy pouze k docela malé změně
rychlosti
$$\Delta v = \frac{p_{\mbox{foton}}}{m} = \SI{2{,}515e-2}{\m\per\s}$$
Počet fotonů $n$ nutných k zastavení atomu vápníku pak zjistíme
z rovnice $v = n \Delta v$. Dosazením dojdeme k hodnotě asi
$n=3 \cdot 10^4$ fotonů, aby se atom vápníku zastavil.

### Spektrum atomu vodíku

V roce 1897 objevil Joseph John Thompson elektron a v roce 1911 pak
Ernest Rutherford objevil atomové jádro. Bylo pak asi přirozené nahlížet
na atom jako na soustavu , kde okolo těžkého, nabitého jádra obíhá lehký
elektron. Takováto představa má ale ve skutečnosti řadu potíží. Předně
není vůbec jasné, proč by takovýto atom měl být stabilní. Nabitá částice
by dle klasické teorie měla velmi rychle ztrácet energii ve formě
záření. Rozžhavené atomy navíc vyzařují světlo jen zcela určitých
vlnových délek, tj. atomy mají čárové emisní spektrum (viz
obrázek \[obr:spectrumH\]), což ale klasická mechanika nedokáže
vysvětlit.

\[ht\]

Spektrum atomu vodíku představuje řada čar, které je možné sdružit do
určitých sérií (Lymanova, Balmerova, Paschenova$\dots$). Experimentálně
se ukázalo, že vlnočet těchto čar závisí na celých číslech $n_1$ a $n_2$
podle vztahu
$$\widetilde{\nu} = \num{10973731} \left( \frac{1}{n_1^2} - \frac{1}{n_2^2}\right ) \si{\per\cm}
\label{rov:Spektrumvodiku1}$$ Niels Bohr dokázal tento vztah v roce 1913
dát do souvislosti s planetárním modelem atomu a jeho model měl v sobě
již některé z rysů kvantové teorie. Předpokládal, že se elektron
pohybuje po kruhové dráze, na které musí být odstředivá síla rotující
částice kompenzována přitažlivou silou elektrostatickou
$$\frac{\me v^2}{r} = \frac{1}{4\pi \varepsilon_0}\frac{Ze^2}{r^2}
\label{rov:Spektrumvodiku2}$$ Nyní ale máme nekonečné množství stavů, po
kterých se částice mohou pohybovat – podle toho, jakou zvolíme rychlost,
musíme zvolit také příslušný poloměr. Bohr ale navíc předpokládal, že
moment hybnosti může nabývat pouze hodnot celistvých násobků konstanty
$\hbar=\nicefrac{h}{2\pi}$ $$\me vr = \hbar n 
\label{rov:Spektrumvodiku3}$$ Proč ho něco takového napadlo? Aby to
vyšlo! Z podmínky vyjádříme rychlost $v$ jako funkci $r$ a dosadíme do
podmínky . Získáme vztah
$$r = \frac{4\pi\varepsilon_0\hbar^2}{Z\me e^2}n^2
\label{rov:Spektrumvodiku4}$$ a pro rychlost
$$v = \frac{Ze^2}{4\pi\varepsilon_0\hbar}\frac{1}{n}
\label{rov:Spektrumvodiku5}$$ Po dosazení do vztahu pro energii
dostaneme
$$\boxed{E = \frac{1}{2}\me v^2 - \frac{Ze^2}{4\pi\varepsilon_0r} = - \frac{Z^2\me e^4}{8 \varepsilon_0^2 h^2}\frac{1}{n^2} = -\frac{13{,}6 Z^2}{n^2}\si{\eV}}
\label{Spektrumvodiku6}$$ Poloměr, rychlost i energie jsou tedy
kvantovány. K přechodu mezi dvěma elektronovými stavy může dojít pouze
tehdy, jestliže rozdíl energií počátečního a konečného stavu je roven
energii fotonu $$E_2-E_1 = h\nu
\label{rov:Spektrumvodiku7}$$ tedy
$$\frac{Z^2\me e^4}{8\varepsilon_0^2h^2}\left( \frac{1}{n_1^2} - \frac{1}{n_2^2} \right ) = h\nu = hc\widetilde{\nu}
\label{rov:Spektrumvodiku8}$$ Pro vlnočet fotonu tak dostaneme
$$\widetilde{\nu} = \frac{Z^2\me e^4}{8\varepsilon_0^2 h^3c}\left( \frac{1}{n_1^2} - \frac{1}{n_2^2} \right ) = \num{10973731} \left( \frac{1}{n_1^2} - \frac{1}{n_2^2} \right ) \mathrm{cm} ^{-1}
\label{rov:Spektrumvodiku9}$$ Což je přesně experimentálně pozorovaný
vztah. Zdá se tedy, že kvantována není pouze energie, ale také moment
hybnosti částice. Kvantování jako by bylo obecným rysem světa molekul.

### Další experimenty

Na kvantování energie poukazovaly také další experimenty, které bylo
v rámci klasické teorie těžké vysvětlit. Kvantování energie hraje roli
například i pro tak jednoduchou veličinu, jako je **tepelná kapacita**.
Podle klasické teorie by tepelná kapacita atomárního krystalu měla
nabývat konstantní hodnotu 3$R$. Experimenty ale ukazovaly něco úplně
jiného – tepelná kapacita se snižující se teplotou klesala a při teplotě
absolutní nuly nabývala nulové hodnoty. Vysvětlení přinesla opět
představa kvantování energie. A opět to byl Albert Einstein, kdo vše
jako první pochopil. Tepelná kapacita představuje schopnost materiálu
pohlcovat energii. Pokud ale energetické hladiny nejsou spojité, tak při
nízké teplotě materiál teplo vůbec není schopen pohlcovat. Tepelná
kapacita se tak snižuje (viz také kapitola \[kap:Einstein\]).

Další z významných experimentů je **FranckůvHertzův pokus**. James
Franck a Gustav Hertz zkoumali průchod elektrického proudu skrze rtuťové
páry. Se vzrůstajícím napětím rostl i procházející proud, ale při
určitém napětí (a tedy při určité kinetické energii elektronů) začal
najednou klesat. Tato energie totiž odpovídá energetickým rozdílům
v atomu rtuti. Jakmile byl dosažen tento rozdíl, elektrony se začaly
srážet s atomy rtutí neelasticky a ztrácely svou energii. Jde tak
o další důkaz kvantování energie.

Dualismus vln a částic
----------------------

Einstein svou analýzou fotoelektrického jevu ukázal, že i objekt tak
nepochybně vlnový, jakým je světlo, se za jistých okolností může chovat
jako částice. Tato skutečnost je vyjádřena v rovnicích a . V roce 1924
přišel Louis de Broglie s myšlenkou, že vztah se dá číst také opačně –
každá hmotná částice s hybností $p=mv$ je charakterizována vlnovou
délkou $\lambda$ dle vztahu $$\boxed{\lambda = \frac{h}{mv}}
\label{rov:Dualismus1}$$ což je **de Broglieův vztah**. Sám de Broglie
asi příliš netušil, o jakou vlnu by mělo jít. Nicméně jeho vztah sehrál
v dalším vývoji kvantové teorie zásadní roli.

De Broglieův vztah umožňuje také interpretovat Bohrovu kvantovou
podmínku . Elektron kolem atomového jádra si pak můžeme představit jako
stojaté vlnění, kdy na obvod kruhu je třeba vměstnat celistvý násobek de
Broglievých vlnových délek $$2\pi r = n \frac{h}{\me v}
\label{Dualismus2}$$ tedy $$\me vr = \frac{h}{2\pi}n = \hbar n
\label{Dualismus3}$$

[Experimentální důkazy interference částic]{} Pokud by částice,
například elektrony, skutečně představovaly vlny, měly by vykazovat
vlastnosti pro vlny typické, tj. zejména interferenci. Pro pozorování
interference je potřeba, aby vzdálenost štěrbin byla srovnatelná
s vlnovou délkou příslušné vlny. Pro světlo to jde zařídit celkem
snadno, stačí udělat mřížku s mikrometrovými rozměry. V případě
vysokoenergetického záření (například Rentgenova záření) nebo částic je
ale třeba použít mřížek podstatně menších. Interferenci Rentgenova
záření můžeme pozorovat například při difrakci (ohybu) světla na
krystalické mřížce, kdy dochází k interferenci vln odražených z různých
rovin krystalů. V závislosti na úhlu pak dochází k zesílení či
k zeslabení intenzity odraženého světla. Ve dvacátých letech **Davisson
s Germerem** provedli experiment s proudem elektronů posílaných na
krystal niklu. Závislost intenzity rozptýlených elektronů na úhlu
vykazovala maxima a minima, podobně jako v případě obrazců získávaných
difrakcí rentgenového záření na krystalech!

Kvantová povaha částic je ale patrná i u daleko těžších objektů než je
elektron. V roce 1930 Stern a Estermann pozorovali difrakci paprsku
helia rozptylovaného na krystalu LiF. V roce 1999 pak byla pozorována
interference asi nejtěžšího objektu, fullerenu C$_ {60}$, se kterým byl
proveden dvouštěrbinový experiment (M. Arndt, O. Nairz, J. Vos-Andreae,
C. Keller, G. van der Zouw, A. Zeilinger, *Nature*, 401, 680 (1999)). Na
naměřeném interferenčním obrazci byla patrna maxima nultého a prvního
řádu. Přibližný nákres interferenčního obrazce je na následujícím
obrázku.

![image](fullerene_diffraction2-bw.png)

Elektronová difrakce je využívána v některých experimentálních
technikách jako je LEED (*Low Electron Energy Diffraction*). Elektrony
jsou zde fokusovány na povrch materiálů a z pozorovaných difrakčních
obrazců se usuzuje na strukturu povrchu. Rozptyl helia patří také
k dodnes využívaným technikám studia povrchů.

Pohybové rovnice kvantově-mechanických částic: Schrödingerova rovnice
---------------------------------------------------------------------

Bohrova teorie dokázala popsat atom vodíku, ale brzy začalo být zřejmé,
že teorie má své limity. Ve dvacátých letech se odehrálo mnoho chytrých
pokusů spojit klasickou mechaniku s experimentálním pozorováním
kvantování energie, ale průlom přišel až s vytvořením zcela nové,
kvantové mechaniky. Ta se na konci dvacátých let objevila ve dvou
formách, Heisenbergově maticové mechanice a Schrödingerově vlnové
mechanice, i když na první pohled nebylo vůbec zřejmé, že tyto dvě
mechaniky mají něco společného. My zde budeme alespoň náznakem sledovat
myšlenkový postup Erwina Schrödingera.

Na začátku je třeba říci, že kvantová mechanika je založena na
postulátech a jako takovou ji nemůžeme odvodit. Můžeme ji pouze
uhodnout. To ale neznamená, že bychom neměli žádné indicie. Schrödinger
mohl postupovat takto. Řekněme, že nás zajímají stacionární stavy
částic, například atomů. Tedy stavy, ve kterých se částice pohybují
periodicky. Nás bude zajímat, s jakou energií se částice mohou
pohybovat. Stacionární stavy budou nejspíše popsány stojatou vlnou
$$\Psi(x,t) = \psi(x)\cos(\omega t)
\label{rov:Pohyboverovnice1}$$ kde $\Psi(x,t)$ představuje vlnovou
funkci, o které budeme mluvit dále. V tuto chvíli nechme otázku, co se
vlastně vlní, otevřenou. Pro všechny vlny platí vlnová rovnice, měla by
proto platit i pro vlnu popisující elektron. Tj.
$$\frac{\pd^2\Psi(x,t)}{\pd x^2} = \frac{1}{v^2}\frac{\pd^2\Psi(x,t)}{\pd t^2}
\label{rov:Pohyboverovnice2}$$ Po dosazení ze vztahu
$$\frac{\dd^2\psi(x)}{\dd x^2} + \frac{\omega^2}{v^2}\psi(x) = 0 
\label{rov:Pohyboverovnice3}$$ Uvažme nyní, že
$$\omega = 2\pi\nu = \frac{2\pi v}{\lambda}
\label{rov:Pohyboverovnice4}$$ a dosaďme za vlnovou délku z de Brogliova
vztahu $\lambda = \frac{h}{p}$ a za $\frac{p^2}{2m}=E-V$. Úpravou
dostáváme
$$\frac{\dd^2\psi(x)}{\dd x^2} + \frac{8\pi^2 m}{h^2}(E - V(x))\psi(x) = 0 
\label{rov:Pohyboverovnice5}$$ nebo též
$$\boxed{-\frac{\hbar^2}{2m}\frac{\dd^2\psi(x)}{\dd x^2} + V(x)\psi(x) = E\psi(x)}
\label{rov:historie:bezcasova_SCHR_1D}$$ Vztah je bezčasová
**Schrödingerova rovnice**. Kompaktně jí můžeme napsat ve tvaru
$$\hat{H}\psi = E\psi
\label{rov:Pohyboverovnice7}$$ kde symbolem $\hat{H}$ rozumíme operátor
(více si o operátorech povíme v příští kapitole)
$$\hat{H} = -\frac{\hbar^2}{2m}\frac{\dd^2}{\dd x^2} + V
\label{rov:Pohyboverovnice8}$$ Jejím řešením jsou možné hodnoty energie
a jím příslušející vlnové funkce. Je to poněkud zvláštní rovnice, neboť
má dvě neznámé veličiny, $E$ a funkci $\psi$. Zdálo by se tedy, že
kupříkladu energii si můžeme zvolit a vlnovou funkci k ní dopočítat.
Energie by tak nebyla kvantována – níže se dozvíme, kde se kvantování
energie bere.

Bornova interpretace vlnové funkce {#kap:Bornova interpretace vlnové funkce}
----------------------------------

Co to vlastně je ona vlnová funkce? Můžeme vyjít z analogie z optiky.
Roli vlnové funkce zde hraje kupříkladu vektor intenzity elektrického
pole. Intenzita světla v určitém bodě je pak dána jako čtverec intenzity
elektrického pole. Vedeni touto analogií, můžeme s Maxem Bornem
interpretovat vlnovou funkci jako amplitudu pravděpodobnosti. Čtverec
vlnové funkce bude mít pak význam hustoty pravděpodobnosti nalezení dané
částice v určitém bodě $$f(x)\dd x = |\Psi (x)|^2\dd x 
\label{rov:Born1}$$

[Co máme na mysli hustotou pravděpodobnosti?]{} Existuje nekonečně mnoho
poloh $x$, kam můžeme částici umístit. Pravděpodobnost nalezení částice
v jedné konkrétní poloze je tudíž nulová. Můžeme se ale ptát, jaká je
pravděpodobnost, že se částice bude nacházet v intervalu $x$, $x$+d$x$.
Tato pravděpodobnost $P(x, x+\dd x)$ bude záviset na velikosti intervalu
d$x$. Pro nekonečně malý interval d$x$ bude opět nekonečně malá.
Vydělením $P(x,x+\dd x)$ intervalem d$x$ získáme konečnou veličinu,
hustotu pravděpodobnosti $f$ $$f(x) = \frac{P(x, x+\dd x)}{\dd x}$$ pro
kterou musí platit normalizační podmínka $$\int f(x) \dd x = 1$$

Z Bornovy interpretace pak plyne normalizační podmínka pro vlnovou
funkci $$\int |\Psi(x)|^2 \dd x = 1
\label{rov:Born2}$$ která říká, že částice musí být někde v prostoru.
Tato podmínka vlastně představuje další rovnici, kterou musíme dodat ke
Schrödingerově rovnici . Na vlnovou funkci pak s ohledem na obě rovnice
klademe několik podmínek

-   Vlnová funkce musí být jednoznačně definovaná (tj. musí to být
    funkce, jedné hodnotě nezávisle proměnné přísluší jedna hodnota
    závisle proměnné, v angličtině bychom řekli, že vlnová funkce musí
    být *single valued*).

-   Vlnová funkce musí být kvadraticky integrovatelná, tj. musí
    platit[^2] $$\int |\Psi|^2 < \infty$$

-   Vlnová funkce musí být spojitá.

-   Vlnová funkce musí mít spojité první derivace.

**Zadání:** Které z funkcí a) - f) mohou být vlnovými funkcemi?

![image](funkce-bw.pdf)

**Řešení:** a) ne, není spojitá b) ne, není funkce c) ano d) funkce nemá
spojitou první derivaci, nicméně funkce může představovat vlnovou funkci
pro singulární potenciál (jako například pro atom vodíku) e) ne, není
kvadraticky integrovatelná f) ano.

Časově závislá Schrödingerova rovnice
-------------------------------------

Výše jsme navodili časově nezávislou Schrödingerovu rovnici, jejímž
řešením získáme možné energie, se kterými se částice může pohybovat.
Časově nezávislá Schrödingerova rovnice se dá odvodit z časově závislé
Schrödingerovy rovnice
$$\boxed{\ii\hbar \frac{\pd\Psi}{\pd t} = \hat{H}\Psi}
\label{rov:Casovachr1}$$ Tato rovnice nám ukazuje vývoj stavu v čase.
Známe-li vlnovou funkci v nějakém čase $t$, integrací Schrödingerovy
rovnice získáme vlnovou funkci v libovolném čase příštím (a minulém).
V chemii tato rovnice hraje roli třeba ve spektroskopii – máme molekulu
v základním stavu a zajímá nás, v jakém stavu se bude molekula nacházet
po vnějšího časově závislého elektromagnetického pole. Z časově závislé
Schrödingerovy rovnice tak odvozujeme například tzv. výběrová pravidla,
která nám říkají, které přechody jsou ve spektroskopii zakázané (tj.
probíhají s velmi malou rychlostí) a které přechody jsou povolené.
V dalším výkladu v rámci tohoto kurzu se ovšem s časově závislou
Schrödingerovou rovnicí nesetkáme.

[Souvislost časově závislé a časově nezávislé Schrödingerovy rovnice ]{}
Časově nezávislou Schrödingerovu rovnici je možné odvodit z časově
závislé Schrödingerovy rovnice, pokud předpokládáme, že hamiltonián
systému nezávisí na čase
$$\hat{H} = -\frac{\hbar^2}{2m}\frac{\pd^2}{\pd x^2} + V(x)
\label{rov:}$$

Za tohoto předpokladu můžeme použít metodu separace proměnných a hledat
řešení Schrödingerovy rovnice ve tvaru součinu
$\Psi (x, t) = \psi(x)\phi(t)$. Schrödingerovu rovnici pak můžeme napsat
ve tvaru
$$\ii \hbar \psi(x) \frac{\pd \phi(t)}{\pd t}=-\frac{\hbar^2 \phi(t)}{2m}\frac{\pd^2\psi(x)}{\pd x^2}+V(x)\psi(x)\phi(t)
\label{rov:Bezcasova1}$$ Pokud vydělíme celou rovnici členem
${\psi(x)\phi(t)}$, získáme rovnici v následujícím tvaru
$$\ii \hbar \frac{1}{\phi(t)} \frac{\pd \phi(t)}{\pd t}=-\frac{\hbar^2}{2m}\frac{1}{\psi(x)}\frac{\pd^2 \psi(x)}{\pd x^2} + V(x)
\label{rov:Bezcasova2}$$ Levá strana rovnice závisí pouze na čase, pravá
strana rovnice pouze na poloze. Aby byla rovnice splněna pro libovolné
hodnoty času a polohy, musí být obě strany rovny konstantě. Tuto
konstantu si označíme písmenem $E$. Snadno se přesvědčíte, že konstanta
by skutečně měla mít rozměr energie. Získáme tak dvě rovnice. Rovnice
vycházející z pravé strany není než časově nezávislou Schrödingerovou
rovnicí
$$E{\psi(x)}= -\frac{\hbar^2}{2m}\frac{\pd^2 \psi(x)}{\pd x^2} + V(x)\psi(x)
\label{rov:Bezcasova3}$$ Rovnici vycházející z levé strany musíme
dořešit $$\ii \hbar \frac{1}{\phi(t)} \frac{\pd \phi(t)}{\pd t}=E
\label{rov:Bezcasova4}$$

což po separaci proměnných a integraci vede k
$$\ii \hbar \ln\phi(t) = Et + C
\label{rov:Bezcasova5}$$ kde $C$ je konstanta. Funkce $\phi(t)$ má pak
tvar
$$\phi(t) = \ee^{C} \ee^{-\ii Et/\hbar}=\ee^{-\ii Et/\hbar} = \ee^{-\ii\omega t}
\label{rov:Bezcasova6}$$

kde za $C$ jsme dosadili nulu z důvodů normalizace vlnové funkce.
Vlnovou funkci systému tedy můžeme zapsat jako
$$\Psi(x,t) =  \psi(x) \ee^{-\ii\omega t}
\label{rov:Bezcasova7}$$ Je patrné, že v tomto případě je řešení časově
závislé rovnice současně i řešením časově nezávislé rovnice. Tvary
vlnových funkcí se totiž liší pouze fázovým faktorem členem
$\ee^{-\ii\omega t} $, který neovlivňuje hustotu pravděpodobnosti
$$\Psi(x,t) \Psi^{*}(x,t) = \psi(x)\ee^{-\ii\omega t}\psi^{*} \ee^{\ii\omega t} = \psi(x)\psi^{*}(x)
\label{rov:Bezcasova8}$$ Využili jsme zde některých vlastností
komplexních funkcí, se kterými se blíže seznámíme v oddíle
\[kap:KomplexniCisla\]. Jelikož hustota pravděpodobnosti se nemění
s časem, mluvíme v tomto případě o stacionárních stavech.

Relace neurčitosti {#kap:relace-neurcitosti}
------------------

Měření veličin v kvantové mechanice má určitá specifika. Existují
skupiny veličin, tzv. komplementární veličiny, které nelze měřit zároveň
s libovolnou přesností. K těm patří například dvojice poloha-hybnost či
$x$-ová a $y$-ová souřadnice momentu hybnosti. Ze Schrödingerovy rovnice
se dá dokázat, že $$\boxed{\Delta x \Delta p \geq \frac{\hbar}{2}}
\label{rov:Neurcitost1}$$ kde $\Delta x$ je neurčitost polohy a
$\Delta p$ je neurčitost hybnosti. Čím přesněji měříme polohu, tím méně
přesnou máme hybnost. Důsledkem je mimo jiné neexistence pojmu
trajektorie částice v kvantové mechanice a nerozlišitelnost identických
částic. Představme si totiž, že ve dvou okamžicích po sobě nalezneme na
stejném místě dvě částice. Pokud ovšem neznáme přesně jejich polohy i
hybnosti, nemůžeme vyloučit možnost, že se mezitím tyto částice
prohodily.

**Zadání:** Elektronový svazek má rychlost
$1000 \pm 0{,}01\,\si{\m\per\s}$. Jak přesně můžeme určit v daném
okamžiku polohu elektronu?

**Řešení:** Neurčitost hybnosti elektronu je dána vztahem
$$\Delta p_x = (0{,}01)(9{,}11 \cdot 10^{-31}) = \SI{9{,}11e-33}{\kg\m\per\s}$$
Neurčitost polohy je potom dána vztahem
$$x\geq\frac{\hbar}{2\cdot 9{,}11\cdot 10^{-33}} = \SI{0{,}0058}{\m} = \SI{0{,}58}{\cm}$$

Relace neurčitosti se dají také z částicové povahy světla. Pokud chceme
měřit přesně polohu částice, můžeme ji pozorovat pomocí světla.
Nepřesnost měření bude dána vlnovou délkou světla $\lambda$, její
snižování tak povede ke zvětšování přesnosti. Interakce světla
s pozorovaným objektem na druhou stranu povede k předání hybnosti
o řádové hodnotě $$\Delta p = \frac{h}{\lambda}
\label{rov:Neurcitost2}$$ Což povede k neurčitosti měření hybnosti.
Zároveň $\Delta x \approx \lambda $. Vynásobením pak získáme vztah
$$\Delta x \Delta p \approx h 
\label{rov:Neurcitost3}$$ který je v souladu s obecnějším vztahem .

Vztah neurčitosti platí také mezi energií a časem
$$\boxed{\Delta t \Delta E \geq \frac{\hbar}{2}}
\label{rov:Neurcitost4}$$ což má podstatné důsledky například ve
spektroskopii. V daném časovém intervalu $\Delta t$ jsme schopni změřit
energii pouze s přesností $\Delta E$. Pokud bychom měřili energii
přesněji, museli bychom zvětšit $\Delta t$, což může být doba
experimentu nebo doba, po kterou daný stav existuje. Pokud nás tedy
zajímají procesy s velmi krátkou dobou života, musíme počítat s velkou
neurčitostí energie.

                                              klas. mech.                                         kvant. mech
  -------------------------- ---------------------------------------------- -------------------------------------------------------
  Stav                                  $\vec{r}(t), \vec{p}(t)$                               $\Psi(\vec{r},t)$
  Pohybové rovnice            $m\frac{\dd ^2 \vec{r}}{\dd t^2} = \nabla V$      $ \ii\hbar\frac{\pd \Psi}{\pd t} = \hat{H}\Psi$
  Časově nezávislé rovnice            $\frac{mv^2}{\vec{r}} = F $                            $\hat{H}\psi = E\psi$
  Relace neurčitosti                               -                         $\Delta x \Delta p \geq \frac{\hbar}{2} \mbox{ atp.}$

  : Srovnání klasické a kvantové mechaniky

**Zadání:** Atom kyslíku, ze kterého je vyražen vnitřní elektron, má
dobu života asi 4 fs. Jakou můžeme očekávat nejmenší šířku spektra
v rentgenových absorpčních spektrech pro tento atom? Výsledek uveďte
v jednotkách eV.

**Řešení:** Neurčitost energie je dána vztahem
$$\Delta E \geq \Delta t  \frac{\hbar}{2} = 4\cdot 10^{-15} \frac{1{,}054\cdot 10^{-34}}{2} = \SI{0{,}0822}{\eV}
\label{rov:Neurcitost5}$$

Šířka spektra bývá ve skutečnosti větší, kupříkladu díky tzv.
dopplerovskému rozšíření spektra. Šířka spektra daná relacemi
neurčitosti ale nemůže být zmenšena kupříkladu vylepšenými
experimentálními technikami.

Kde se dozvíte více? {#kde-se-dozvíte-více .unnumbered}
--------------------

Populární úvod do kvantové mechaniky spolu s diskuzí základních
experimentů je možno nalézt v knize J. Pišút, R. Zajac, *O atomoch a
kvantovaní*, Alfa, Bratislava, 1988. Základní úvod do kvantové mechaniky
lze nalézt kupříkladu v Atkinsově učebnici fyzikální chemie. Pěkně jsou
úvodní kapitoly kvantové mechaniky diskutovány také ve starší knize A.
Beiser, *Úvod do moderní fyziky*, Academia, Praha, 1978. Zájemcům
o hlubší pohled na historii a filozofické otázky spojené s kvantovou
mechanikou lze doporučit knihu M. Jammer, *The Philosophy of Quantum
Mechanics*, John Wiley, New York, 1974. Na populárnější úrovni je
historie kvantové mechaniky dobře shrnuta v knize J. Kvasnica,
*Priekopnici modernej fyziky*, Smena, Bratislava, 1987.

[^1]: Elektromagnetický oscilátor si můžeme představit jako kladný a
    záporný náboj spojený pružinkou.

[^2]: K uvedeným podmínkám by se slušelo přidat různé dodatky. Vlnová
    funkce nemusí například mít spojité první derivace pro nespojitý či
    singulární potenciál, ve fyzice se setkáme i s vlnovými funkcemi,
    které nejsou kvadraticky integrovatelné atd. Zde je pro nás
    důležité, že na vlnovou funkci klademe některá omezení.
