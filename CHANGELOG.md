# Releaselog – Håndbold

Releaseloggen findes kun her. Ved ny version: opdater `VERSION` i `index.html`, versionen i `<title>` og filnavnet (`haandbold-vX.Y.Z.html`).

## v0.28.3 – 2026-11-07 – Kastehånd: landshold og Champions League gennemgået
- Gennemgang af EM- og CL-trupperne: højre back og højre fløj er venstrehåndede, alle andre højrehåndede, med kendte undtagelser
- Rettet til venstrehåndede: Nedim Remili (Veszprém, playmaker), Kent Robin Tønnesen (GOG, venstre back), Magnus Abelvik Rød (Szeged)
- Bekræftet: Gidsel, Hoxer, Kirkeløkke, Alex Dujshebaev, Richardson, Janc, Šoštarić m.fl. er venstrehåndede; Lasse Andersson er højrehåndet

## v0.28.2 – 2026-11-07 – Frikast ved 9-meter-linjen, fløjen bliver i kæden
- Frikast tæt på mål (inden for ca. 12 m) tages nu ved den stiplede 9-meter-linje: skytten går derud, angriberne går uden for 9 m, og forsvarerne går 3 m væk. Rettet en fejl fra v0.28.1, hvor skytten blev stående, hvor frikastet blev dømt
- Fløjen i forsvaret træder ikke længere ud mod en bagspiller med bolden (så han løb frem uden grund) – kun mod en angriber ude i hjørnet. Ellers er det halvspilleren, der træder ud

## v0.28.1 – 2026-11-07 – Ingen spillere skubbet meters væk i tacklinger
- Årsag 1: ved frikast inden for 9 m blev angriberen flyttet direkte ud til 9-meter-stregen (2-3 m) i samme øjeblik. Nu går han selv hen til stedet, og frikastet venter, til han er der
- Årsag 2: under dødbold blev kropskontakten ved med at virke – forsvareren, der lige havde tacklet, gik ind i angriberen og skubbede ham 2-3 m hen ad gulvet. Under dødbold er der nu ingen skubben
- Forsvarerne går 3 m væk fra frikastskytten, som reglerne siger

## v0.28.0 – 2026-11-06 – Smarte skud og fløjene bliver i forsvarskæden
- Smarte skud (kan slås fra under Indstillinger → Smarte skud): du vælger stadig skudtype med tryk og placering med joysticket, men skuddet får den teknik, situationen kræver
  - Lavt med en forsvarer foran: hofteskud forbi blokken (sjældnere blokeret)
  - Lavt tæt på mål: gulvskud, der rammer gulvet foran målmanden og springer op (svært at redde)
  - Højt med en forsvarer foran: skud over blokken med armen helt strakt (sjældnere blokeret)
  - Kontra alene, målmanden er løbet ud, og du sigter højt: hurtig lobning over ham
- Rettet: fløjene stormede frem fra forsvarskæden ved hvert skud og blev ved, selv om skuddet blev blokeret, eller angriberne fik returbolden. Nu starter de kun kontraløbet, mens skuddet er i luften, når målmanden har bolden, ved målkast, eller når en returbold er på vej til eget hold – ellers bliver de i kæden
- Tilbagerulning: v0.27.0 (commit 6af0e82) er sidste version før smarte skud

## v0.27.0 – 2026-11-06 – Balance, afleveringer, vægt i løbet og målmandens placering
- Balance afgør præcisionen: skud i fart mod mål og på toppen af hoppet er mere præcise, skud i et sving, væk fra mål eller med en forsvarer hængende på spreder mere (gælder både dig og computeren)
- Afleveringer: lukket bane giver en høj aflevering hen over forsvarerens arme; under pres kan afleveringen blive upræcis og lande bag modtageren eller ved fødderne; modtageren vender sig mod bolden og griber med armene frem
- Vægt i løbet: spillerne tager et par skridt om at komme op i fart og bremse, en vending i fuld fart koster mere, og forsvarerne flytter sig med tydelige sideskridt
- Målmanden placerer sig bedre: træder frem mod langskud for at mindske vinklen, står tættere på stregen ved skud tæt på, og på kontra 1 mod 1 går han ud tidligt og trækker sig tilbage, når skytten kommer tæt på

## v0.26.6 – 2026-11-06 – Pause ved halvleg og slut, opstilling til 2. halvleg
- Ved halvleg og når kampen er slut, stopper spillet: spillerne går i stå, der skydes og afleveres ikke, og resultatet vises
- 2. halvleg starter med det angribende hold stillet op ved midterlinjen og forsvaret ved 9 m, ligesom ved en rigtig kampstart

## v0.26.5 – 2026-11-06 – Computeren går mod mål i kontra, Normal er standard
- Har computerens boldholder fri eller rimelig fri bane (ingen forsvarer foran, eller én langt væk), løber han direkte mod mål og afslutter i stedet for at spille bolden tilbage. Han spiller kun frem til en medspiller, der er længere fremme og fri
- Normal er nu standard-sværhedsgrad. Har du selv valgt en sværhedsgrad, huskes den stadig

## v0.26.4 – 2026-11-06 – Mere retfærdige straffekast
- Straffekast dømmes kun, når angriberen er på vej igennem mod mål (i fart mod mål, i skudhop eller i skud) og har en fri chance
- Retningen betyder noget: en forseelse bagfra giver næsten altid straffekast, fra siden ca. hver anden gang og forfra kun sjældent (ellers frikast)
- Forseelser på fri chance uden straffekast fløjtes ikke længere som frikast, så spillet flyder
- Animationen: forsvareren og angriberen er i kontakt hele vejen – han hænger på, river ned, sparker benene væk eller skubber i luften, og forfra går han ind i ham, så han falder bagover
- Lidt færre frikast fra tætte dueller (ca. 7 pr. kamp)

## v0.26.3 – 2026-11-06 – Målmændene redder lidt færre
- Målmændenes ekstra redninger fra v0.26.0 er halveret: de redder stadig lidt flere langskud og fløjskud end før v0.26.0, men det er ikke længere så let for dem. Kontra er stadig næsten sikre mål

## v0.26.2 – 2026-11-06 – Faldskud ca. 10 %
- Faldskud udgør nu ca. 10 % af skuddene (før ca. 5 %): stregspilleren, fløjene, gennembrud og spillere med plads foran sig tæt på 6 m falder oftere ind over stregen

## v0.26.1 – 2026-11-05 – Underhåndsskud, faldskud og målmandsredninger
- Underhåndsskud er lette at se: skytten går dybt i knæ med et bredt udfald, lægger sig ind over og trækker armen lavt bagud, før den piskes frem i hoftehøjde. Bolden slippes lavere og flyver lavt mod mål. Bagspillerne bruger det nu også selv af og til, når en forsvarer står foran
- Færre faldskud (ca. 5 % af skuddene mod før ca. 15 %): kun stregspilleren, fløjene og gennembrud tæt på 6 m falder. Bagspillere tæt på stregen hopper i stedet. Faldskuddet ender på maven med armene strakt frem, og spilleren glider lidt hen ad gulvet
- Målmanden dykker oftere og længere ud efter skud i hjørnerne, griber bolden ind til brystet, når han holder den, og står med hænderne i siden efter et mål

## v0.26.0 – 2026-11-05 – Mere rigtig håndbold: målmænd, frikast, fejl, kontra og streg
- Målmændene redder flere skud, mest dér hvor de også gør det i virkeligheden: flere redninger på langskud (ca. 44 % mod før 39 %) og lidt flere på fløjskud. Skud fra 6 m og stregspilleren er uændrede
- Målmanden holder oftere bolden efter en redning (ca. halvdelen mod før hver femte), især på skud i kroppen og højt. Lave skud i siden giver stadig returbolde
- Kontra er næsten sikre mål (ca. 80 %), så det betaler sig at løbe hjem
- Lidt flere frikast: når en forsvarer står tæt på boldholderen, bliver angrebet oftere stoppet. Ca. 6 pr. kamp mod før 5
- Tekniske fejl: i tætte dueller kan bolden blive slået eller glide ud af hånden. I alt ca. 4-5 tekniske fejl pr. kamp
- Stregspilleren trækker oftere frikast og straffekast, når han bliver holdt, og står for ca. hvert femte mål

## v0.25.4 – 2026-11-05 – Ingen utilsigtet zoom på mobil
- Dobbelttryk og knib med to fingre zoomer ikke længere ind på siden, heller ikke i Safari på iPhone, som ignorerer den almindelige zoomlås. Hurtige tryk på knapperne virker stadig

## v0.25.3 – 2026-11-05 – Rigtig størrelse på mobil
- GitHub-udgaven manglede viewport-indstillingen, så mobilen viste spillet som en lille desktopside med bittesmå spillere og tekst. Nu fylder banen, spillerne og menuerne skærmen

## v0.25.2 – 2026-11-03 – Klogere modstander på Normal og Svær
- Modstanderen rammer bedre: skyder sikrere ind i hjørnet væk fra målmanden, spreder mindre og slår oftere målmanden. Hans egen målmand læser dine skud bedre
- Bedre skudvalg: tager de åbne chancer og venter med de dårlige, og spiller oftere bolden til den mest frie medspiller
- Tættere forsvar: forskyder mere mod bolden, naboen hjælper mere, stregspilleren dækkes på målsiden, fløjene dækkes tæt, forsvareren træder længere ud, blokerer oftere og løber hurtigere hjem
- Testet med computer mod computer: Let ca. lige, Normal ca. 3 mål bedre og Svær ca. 7 mål bedre pr. kamp (før ca. 2 og 4)

## v0.25.1 – 2026-11-02 – Sværhedsgrader
- Ny indstilling: Sværhedsgrad med Let (som hidtil), Normal og Svær. Den valgte sværhedsgrad vises på forsiden
- På Normal og Svær bliver modstanderen bedre (højere værdier i skud, præcision, forsvar, fart og målmandens reaktion), tænker hurtigere med bolden, tackler oftere og opsnapper flere afleveringer
- Tempoet er det samme. Simulerede kampe i turneringer og sæsoner påvirkes ikke

## v0.25.0 – 2026-11-02 – Løbeanimation, bolden i luften, boldfysik og kropskontakt
- Løbeanimation: armene svinger modsat benene med bøjede albuer, spillerne læner sig frem og hopper let i skridtet
- Forsvarsstilling: tæt på eget mål står forsvarerne bredt og bøjet i knæene med armene oppe og bevæger sig sidelæns
- Bolden i luften: bolden bliver lidt større, jo højere den er, og skyggen bliver mindre og svagere, så høje afleveringer og hopskud er lettere at aflæse
- Boldfysik: en håndbold hopper lavt og dødt, så løse bolde og returbolde bliver liggende tættere på. Stødafleveringen til stregspilleren hopper nu i gulvet og op til ham
- Kropskontakt: forsvarerne spærrer fysisk vejen for boldholderen, som glider langs dem i stedet for at løbe igennem. Styrke og forsvar afgør, hvem der giver sig. Kommer angriberen forbi forsvareren efter kontakt (gennembrud), får han et kort øjeblik med ekstra fart

## v0.24.1 – 2026-11-02 – Komplette ligatrupper og trøjefarver
- Alle 32 ligahold har nu hele den aktuelle trup (14-26 spillere), ikke kun et udvalg:
  - Herreligaen fra tophaandbold.dk med positioner og højder, også for Aalborg, GOG og SAH (fx Lindskog, Sagosen, Norlyk hos Aalborg og Pellas, Boysen, Tonnesen hos GOG)
  - Bundesliga fra sportschau.de (kampkader 2026/27), også for Füchse Berlin, Magdeburg og Melsungen
- Trøjefarver fundet for klubberne, hvor de før var gættet: Skjern grøn, Bjerringbro-Silkeborg sort, KIF Kolding hvid (blå udebanetrøje), HC Erlangen mørkeblå/rød, TVB Stuttgart hvid/himmelblå, Balingen rød/blå og Bergischer HC blå/rød (før forkert grøn)
- GOG i Champions League: nr. 79 er Emil Tonnesen (venstre back), Hjalte Lykke spiller højre back og Óli Mittún playmaker

## v0.24.0 – 2026-11-02 – Ny hovedmenu, hurtigkamp og sæson
- Ny hovedmenu: Hurtigkamp, Venskabskamp, Turneringer, Sæson og Indstillinger (og Fuld skærm) nederst
  - Hurtigkamp: to tilfældige hold, enten landshold mod landshold eller klub mod klub, og kampen starter med det samme
  - Venskabskamp: vælg landshold, Champions League, Herreligaen eller Bundesliga og begge hold
  - Turneringer: EM 2026 eller Champions League 2026/27 som før
  - Sæson: spil en hel sæson i Herreligaen eller Bundesligaen
- Holdvalg i gitter: landshold med flag, navn og en lille hjemmebanetrøje. Klubhold med klubmærke (et skjold i klubbens farver med forkortelsen, ikke klubbens rigtige logo), navn og hjemmebanetrøje
- Herreligaen 2026/27: alle 14 hold med den aktuelle trup fra tophaandbold.dk, med positioner og højder. Aalborg, GOG og SAH bruger Champions League-trupperne
- Bundesliga 2026/27: alle 18 hold med den aktuelle trup fra sportschau.de. Füchse Berlin, Magdeburg og Melsungen bruger Champions League-trupperne. Venstre/højre for bagspillere og fløje er sat ud fra kendte spillere
- Hvert ligahold har styrke, nøglespillere, holdstil og hjemme- og udetrøje
- Sæsontilstand:
  - Herreligaen: 26 runder (alle mod alle, hjemme og ude) og slutspil for de 4 bedste med semifinaler og finale
  - Bundesliga: 34 runder, flest point bliver mester
  - Du spiller dit holds kampe, resten simuleres ud fra holdenes styrke (med lille hjemmebanefordel). Stilling, seneste runde og topscorerliste vises, og sæsonen gemmes i browseren

## v0.23.5 – 2026-11-02 – Mål tilbage på skærmen
- MÅL! med målscorerens navn vises igen (også STOLPE IND! og OVERLIGGER IND!)
- Frikast vises kun som "Frikast" uden forklaring
- Scoretavlen markerer diskret, at der er scoret: det scorende holds tal lyser kort op i gult og vokser en anelse

## v0.23.4 – 2026-11-02 – Færre tekster på skærmen
- Alle statusbeskeder på banen er fjernet undtagen frikast, straffekast og halvleg med stillingen
- Når kampen er slut, står SLUT og resultatet på banen i ca. 2,5 sekunder, før menuen kommer frem

## v0.23.3 – 2026-11-02 – Kamera og straffekast-besked
- Kameraet kan gå ca. 12 % længere op, så scoretavlen ikke længere dækker det øverste mål og målmanden
- Ved straffekast står der nu kun STRAFFEKAST (ikke længere hvem der blev fældet, eller hvem der skal skyde)

## v0.23.2 – 2026-11-02 – Hurtigere boldhentning og automatisk hjemløb
- Målmanden henter bolden hurtigere ved målkast: han løber hurtigere, griber bolden på længere afstand og får en ny bold fra siden, hvis den er trillet langt væk. Tid fra bolden går ud, til målkastet tages: ca. 0,9 sek. mod ca. 2,8 før
- Din spiller løber nu også selv tilbage i forsvar, når modstanderen får målkast, eller når modstanderens målmand griber bolden (ligesom efter et mål). Han stopper, når han er hjemme, eller når dit hold får bolden

## v0.23.1 – 2026-11-02 – Hurtigere målkast
- Målmanden sætter bolden hurtigere i gang ved målkast: pausen før spillet går i gang er kortere (0,25 sek. mod 0,9), og målmanden venter kortere på et fløjløb. Fra målkastet gives, til målmanden kaster ud: ca. 0,5 sek. mod ca. 1,2 før
- Din målmand: du kan kaste ud med Skud (langt) eller Aflever (kort) med det samme ved målkast

## v0.23.0 – 2026-11-02 – Alle CL-hold, højde og målmandens navn
- Champions League: også de sidste 12 hold (Porto, Partizan, Nantes, Vardar, Zagreb, Celje, Szeged, Kristianstad, Montpellier, SAH, Kriens-Luzern, Kolstad) har startere ud fra de seneste kampe og EHF's spillerprofiler
  - Rettede positioner: Lumbroso (playmaker), Bialiauski (playmaker), Llamazares og Jerome Müller (højre back)
  - Tilføjet: Vasco Costa (Porto, venstre back), Fadhuile (Vardar, venstre fløj) og Biel Nielsen (Kristianstad, højre back)
  - Spillere uden for kamptruppen er ikke længere startere eller nøglespillere (fx Odriozola, Pešić, Bánhidi, Johannessen, Milosavljević, Gunnarsson)
- Niklas Landin starter i målet for Aalborg
- Højde: spillere kan have en højde i truppen (`@196`). Høje forsvarere blokerer flere skud, høje skytter slipper bolden højere og kommer lettere over muren, og figuren er en anelse større eller mindre. Højden fra EHF's spillerprofiler er lagt ind for de spillere, hvor den kunne hentes (fx Jeppsson 205, Kulesh 206, Lærke 203, Lumbroso 172). Andre får en standardhøjde efter position
- Målmandens navn og nummer står nu over ham ligesom over den spiller, du styrer

## v0.22.0 – 2026-11-01 – CL-hovedrunden, spillernes egne skud og holdstil
- De 12 hold i Champions League-hovedrunden har fået startopstillinger ud fra de seneste gruppekampe og målstatistik fra EHF (history.eurohandball.com): Veszprém, PSG, Melsungen, Płock, Aalborg, Füchse Berlin, Barça, Sporting, Magdeburg, Kielce, GOG og Dinamo
  - Spillere, der ikke har været i kamptruppen i de seneste kampe (fx Lichtlein, Kastening, Moryto, Sićko, Saugstrup, L. Jørgensen), er ikke længere startere eller nøglespillere
  - Rettelser: Yahia Omar spiller højre back for PSG, "Baszek" hos Płock hedder Daszek, og Kent Robin Tønnesen er med hos GOG
- Spillernes egne skud: hver spiller har et foretrukket skud efter position (langt hjørne, mellem benene, oppe i hjørnet, ved hoften eller kanonskud). Nøglespillerne bruger det oftere og lidt mere præcist, og det vises af og til, fx "Gidsel: kanonskud"
- Holdstil: hvert hold har en stil, som vises i menuen
  - Kontra (fx Danmark, Sverige, Aalborg, GOG, Füchse): fløjene løber altid, anden bølge varer længere, og målmanden kaster oftere langt
  - Højt tempo (fx Norge, Island, Magdeburg, Sporting): bolden spilles hurtigere videre
  - Taktisk (fx Frankrig, Spanien, Barça, PSG, Veszprém): flere afleveringer før skud, forsvaret træder længere ud
  - Fysisk (fx Tyskland, Ungarn, Kielce, Płock): mere stregspil, forsvaret træder længere ud og laver flere forseelser

## v0.21.0 – 2026-11-01 – Mere realistisk grafik
- Dommere på banen: én dommer løber bag angrebet i siden, den anden står på mållinjen. De bytter roller, når spillet skifter retning. De løfter armen ved 7-meter og passivt spil og peger mod midten efter mål. Dommerdragten får en farve, der skiller sig ud fra begge hold
- Dybde: spillerne er en anelse større tæt på kameraet og mindre længere væk (højst ±4 %), og trøje og shorts har en lys og en skyggefuld side
- Bolden roterer i flugten og ved dribling, og hårde skud og afleveringer får et let fartslør
- Nettet bølger ud ved mål
- Omkring banen: udskifterne rejser sig og jubler ved mål, der står et dommerbord med to officials ved midterlinjen, og banderne har fiktive sponsorer

## v0.20.2 – 2026-11-01 – Naturligt opgiverkast
- Efter et mål tager målmanden bolden i målet og kaster den hurtigt op til stregspilleren, som griber den i løbet og løber det sidste stykke ind på midten og kaster op. Før dukkede stregspilleren op på midten med bolden. Det tager ca. 1,3 sekunder fra målmanden har bolden, til der kastes op

## v0.20.1 – 2026-11-01 – Landsholdenes startere og fløjene i kontra
- Startopstillinger gennemgået for EM-holdene: faste startere (`^`) på Spanien, Portugal, Frankrig, Sverige, Kroatien, Slovenien, Ungarn, Island og Norge, og nøglespillere som startere på Østrig (Frimmel på venstre fløj), Schweiz (Manuel Zehnder på venstre back), Holland, Serbien, Færøerne og Polen
- Fri fløj i kontra løber helt ind til ca. 6 m, før han hopper og skyder

## v0.20.0 – 2026-11-01 – 7-meter-situationer, kastehånd og landshold
- 7-meter vises nu med det, der førte til straffekastet. En kort slowmotion efter situationen:
  - Hevet ned bagfra: forsvareren tager om angriberen, som falder bagover
  - Fældet: forsvareren glider ind med benet, og angriberen falder forover
  - Slag på armen: angriberen bliver ramt på kastearmen i skuddet og går i knæ
  - Skubbet i luften: angriberen bliver skubbet i hopskuddet og lander på siden
  - Derefter tones skærmen kort ned (ca. 0,5 sek.) og op igen ved 7-meter-opstillingen
- Computerens forsvarere laver af og til forseelser på en fri chance, så der kommer 1-3 straffekast i en kamp
- Straffekasteren er holdets bedste skytte på banen (en fast straffekaster kan markeres med `~` i truppen). Han venter lidt, laver af og til en skudfinte, og ca. 3 ud af 4 går ind
- Fejlrettelse, kastehånd: Hold A ses bagfra og Hold B forfra, men kastearmen blev tegnet, som om spillerne blev set fra siden, så højrehåndede så venstrehåndede ud. Nu går armen op på den rigtige side, og bolden bæres i kastehånden. Kun højre back og højre fløj er venstrehåndede
- Hele spillet kører 7 % langsommere. En halvleg varer stadig det valgte antal minutter
- Landshold:
  - Danmark og Tyskland har fået truppen fra EM-finalen 2026 og rigtige startere (Danmark: E. Nielsen, Jakobsen, Pytlick, Lauge, Gidsel, J. Hansen, Saugstrup. Tyskland: Wolff, Mertens, Köster, Knorr, Uscins, Zerbe, Golla)
  - Island starter med Viktor Gísli Hallgrímsson i mål, Frankrig med Dika Mem på højre back og Sverige med Eric Johansson på venstre back

## v0.19.3 – 2026-11-01 – Tyvstart og fløjene over midten
- Fløjene tyvstarter: når modstanderen afslutter, sætter forsvarets fløje i ca. 60 % af tilfældene i løb op langs sidelinjen, så de er klar til kontra eller hurtigt oppe efter et mål
- Ved opgiverkast må fløjene stå et par meter inde på modstanderens banehalvdel
- Ingen står helt stille ved opgiverkast: spillerne tripper på pladsen, mens de venter
- Tid fra opgiverkast til begge fløje står i hjørnet: ca. 2,3 sekunder (2,6 i v0.19.2, 4,8 i v0.19.1)

## v0.19.2 – 2026-11-01 – Fløjene hurtigt op efter opgiverkast
- Fejlrettelse: angriberne joggede i hele angrebet, også på vej op ad banen efter opgiverkast, så fløjene kom sidst. De jogger nu først, når de er oppe ved ca. 13 m
- Fløjene løber 10 % hurtigere op ad banen og er blandt de første oppe sammen med stregspilleren. Tid fra opgiverkast til begge fløje står i hjørnet: ca. 2,6 sekunder mod ca. 4,8 før

## v0.19.1 – 2026-11-01 – Fløjløb og målmandens udkast
- Hængning er slået fra igen. Det var den, der gav de pludselig langsomme skud
- Fløjene løber kontra igen: de sprinter ud langs sidelinjen et godt stykke foran bolden (langt op, når målmanden har den) i ca. 95 % af kontraerne. Før joggede de kun et par meter foran sig selv. Går kontraen i stå, stiller de sig i hjørnet
- Målmandens udkast: ca. 80 % korte til en nærliggende medspiller og ca. 20 % lange, hårde udkast til en fri fløj. Det gælder begge hold
- Når din målmand har bolden: Skud = langt, hårdt udkast til en fløj (styr til siden for at vælge fløj, ellers den mest frie), Aflever = kort udkast

## v0.19.0 – 2026-11-01 – Anden bølge og fløjskud
- Anden bølge: er der ingen fri fløj i kontra, og er forsvaret ikke på plads, sprinter bagspillerne op i deres baner. Boldholderen går mod 9 m og afslutter, eller spiller den frie bagspiller i fart, før forsvaret står
- Målmandens placering:
  - Ved fløjskud dækker målmanden den nærmeste stolpe
  - I fri kontra går målmanden ud mod skytten for at lukke vinklen
- Fløjens skudvalg (computeren): oftest det lange hjørne, af og til nærmeste hjørne højt eller mellem benene på målmanden. Mellem benene er sværere for målmanden at læse
- Hængning: er målmanden gået ud, kan bolden løftes over ham. Computeren gør det selv, og du gør det ved at sigte højt (frem på joysticket) i skuddet
- Spillet ligger nu på GitHub: https://github.com/seranodk/handbold

## v0.18.1 – 2026-11-01 – Fløjene i hjørnet under opspil
- Under opspillet driver bagspillerne bolden op ad banen, og fløjene løber ned og stiller sig i hjørnet. Fløjene får kun bolden langt fra mål, når de står fri i kontra (afleveringer til fløjen i opspillet: fra ca. 27 til ca. 2-3 pr. kamp)
- I kontra, hvor fløjen ikke er fri, løber han ned i hjørnet i stedet for at blive stående foran bolden
- Din egen spiller er 10 % kvikkere til at accelerere og skifte retning

## v0.18.0 – 2026-11-01 – Rytme, skudvalg og fart
- Afleveringer i rytme: korte afleveringer i positionsspil er ca. 15 % hurtigere, bolden spilles hurtigere videre efter stødet, lange tværafleveringer er sjældnere, og stregspilleren får en lav stødaflevering
- Skudvalg: computerens bagspillere skyder efter et stød fremad og ikke stående uden pres. Står forsvareren tæt, går skuddet over blokken, ellers lavt forbi ham ved hoften
- Fart og inerti: angribere uden bold jogger i positionsspillet og sprinter kun, når de skal langt eller modtage bolden (gælder ikke din egen spiller). Et retningsskift i høj fart tager et kort øjeblik, også for din spiller, så finter og stød betyder mere

## v0.17.1 – 2026-11-01 – Sikre opgiverkast
- Afleveringen ved opgiverkast er nu ca. 95 % sikker: den kan næsten ikke opsnappes. Bolden mistes efter opgiverkast i ca. 1 % af tilfældene mod ca. 10 % før

## v0.17.0 – 2026-11-01 – Stød, opbakning og forsvar der træder ud
- Positionsangreb (når forsvaret er på plads) spilles mere stationært og i bølger:
  - Bagspilleren, der får bolden, støder frem mod hullet mellem de to forsvarere foran ham (ca. 8 m) og spiller derefter bolden videre eller skyder
  - Modtageren tager fart frem mod bolden, og den, der lige har afleveret, trækker sig tilbage til ca. 10 m
  - Bolden kører videre i samme retning til næste mand. Lange tværafleveringer over flere spillere er sjældnere
  - Fløjen får kun bolden, når han står fri, og en dækket fløj spiller tilbage i stedet for at skyde
- Forsvaret træder ud og tilbage:
  - Én forsvarer møder boldholderen, men træder højst ud til ca. 9 m og falder tilbage, når bolden er spillet videre
  - Naboen på indersiden hjælper ind mod boldholderen. Binder stødet to forsvarere, bliver der plads længere ude, så bolden kan gå videre til den frie mand og til sidst fløjen
- Hopskud er lidt mere præcise, så antallet af mål er det samme som før (ca. 20-25 i en kamp på 2 x 3 min)

## v0.16.2 – 2026-11-01 – Intet utilsigtet skud efter takling
- Vinder dit hold bolden på egen banehalvdel (takling, opsnapning eller løs bold), bliver et tryk på Skud de første 0,6 sekunder ignoreret, så et dobbelttryk fra taklingen ikke bliver til et skud fra egen halvdel
- På modstanderens halvdel kan du stadig skyde med det samme

## v0.16.1 – 2026-11-01 – Kort tryk og underhåndsskud
- Bagspillere (venstre back, playmaker og højre back): et kort tryk på Skud giver et stående skud (ca. 80 %) eller et underhåndsskud (ca. 20 %)
- Holder du Skud nede lidt længere, vælges skudtypen efter situationen som før (hopskud, faldskud osv.)
- Nyt skud: underhåndsskud. Armen svinger lavt bagud og frem, og bolden slippes i hoftehøjde og går oftest nede i målet

## v0.16.0 – 2026-11-01 – Kastehånd og Aalborgs startopstilling
- Spillerne kaster med deres rigtige hånd. Højre back og højre fløj er venstrehåndede, de andre højrehåndede. Venstrehåndede kaster med venstre arm, også når de vender den anden vej
- Skyder en spiller næsten lige mod mål, vender han kroppen, så kastearmen ses
- Nyt i truppformatet: `^` markerer en fast starter, og `!` vender kastehånden i forhold til positionen
- Aalborg Håndbold starter som i de seneste kampe mod Skive og PSG: Norsten i mål, M. Landin og T. Nielsen på fløjene, Arnoldsen, Knorr og Hoxer i bagkæden og Hald på stregen
- Aalborg: P. Larsen hedder nu Wiesmach (Patrick Wiesmach Larsen), og Munk er gjort til nøglespiller

## v0.15.4 – 2026-11-01 – Sidenet, skudhøjde og CL-gulv
- Fejlrettelse: skud mod det nederste mål blev tegnet bag nettet, selvom bolden var foran mållinjen, så det så ud, som om fløjskud gik ind gennem sidenettet. Bolden tegnes nu oven på nettet, indtil den er inde i målet
- Skud går oftest enten nede eller oppe i målet, lidt tilfældigt (du styrer stadig selv højden med joysticket, hvis du vil)
- Målmandens rækkevidde afhænger ikke længere af skuddets højde, så redningsprocenten er den samme
- Nyt hallgulv: Champions League (blå bane, røde målfelter). Det vælges automatisk, når du vælger klubhold

## v0.15.3 – 2026-11-01 – Champions League i det rigtige format
- Champions League-turneringen følger nu det rigtige 2026/27-format:
  - Gruppespil i de rigtige seks grupper, hjemme og ude (6 kampe)
  - Hovedrunde i to grupper af 6 mod de 4 hold, man ikke mødte i gruppen, hjemme og ude (8 kampe). Point tages ikke med fra gruppespillet
  - Nr. 1-4 i hver hovedrundegruppe går i kvartfinale over to kampe (samlet resultat, uafgjort afgøres på straffekast)
  - Final4 i Köln med semifinale, bronzekamp og finale. I alt 18 kampe for et hold, der når finalen
- EM-turneringen beholder EM-formatet (grupper med 3 kampe, mellemrunde med point med fra gruppen, semifinale og finale)
- I turneringstilstand vises kun dit eget holds opstilling i menuen

## v0.15.2 – 2026-11-01 – Ny knapplacering
- Aflever sidder nu lige under Skud, og Finte sidder til venstre for Aflever

## v0.15.1 – 2026-11-01 – Færre udskiftninger
- Højst 10 udskiftninger pr. hold i en kamp (både ved bænken og i pausen)
- Spillerne bliver halvt så hurtigt trætte

## v0.15.0 – 2026-11-01 – Turnering, udskiftninger og stolpefysik
- Turneringstilstand for både EM 2026 og Champions League 2026/27: vælg Turnering i hovedmenuen og dit hold
  - Gruppespil med de rigtige grupper (3 kampe), mellemrunde/hovedrunde i to grupper af 6 (4 kampe, point mod holdet fra egen gruppe tages med), semifinale, bronzekamp og finale (Final4 i Köln for Champions League)
  - Du spiller dit holds kampe, og de andre kampe spilles i baggrunden ud fra holdenes styrke
  - Turneringsskærm med næste kamp, stillinger, seneste resultater og topscorerliste
  - Uafgjort i slutspillet afgøres på straffekast
  - Turneringen gemmes, så du kan fortsætte senere
- Træthed: spillere bliver trætte af at sprinte, løber langsommere og skyder lidt mindre præcist. En bjælke under din spiller viser, hvor frisk han er
- Udskiftninger uden pauser: en træt spiller skiftes kun, når han løber forbi sin bænk på vej tilbage i forsvar (og bolden er langt fra eget mål), og i halvlegspausen. En bjælke under scoreboardet viser, hvem der kom ind og ud
- Bænkene står ved midterlinjen på hvert holds banehalvdel med en udskiftningszone, og byttes ved halvleg
- Stolpe og overligger med rigtig fysik: bolden preller af efter vinklen, den rammer med, og om den går ind eller ud afgøres af den nye bane
- Skrueskud: fløjspillere med god vinkelværdi kan af og til skrue bolden, så den starter udad og drejer ind mod målet. Målmanden læser den oftere forkert, og bolden får et lille spor efter sig

## v0.14.0 – 2026-11-01 – Champions League 2026/27
- Nyt valg i hovedmenuen: Landshold (EM 2026) eller Klubhold (EHF Champions League 2026/27)
- Alle 24 klubber fra Champions League 2026/27 med spillere fra gruppespillets trupper, 14-17 spillere pr. hold, og trøjer i klubbernes farver
- Kilderne skelner kun mellem bagspiller, fløj og streg, så venstre/højre position er sat ud fra kendte spillere. Værdierne er skøn ud fra holdets styrke og nøglespillere
- Valgt hold huskes for både landshold og klubhold

## v0.13.2 – 2026-11-01 – Bedre flow
- Hurtigere opgiverkast efter mål for begge hold, især computeren: stregspilleren står klar efter ca. 0,7 sekund og kaster op med det samme
- Spillere, der løber tilbage i forsvar (og alle spillere efter et mål), løber ca. 15 % hurtigere

## v0.13.1 – 2026-11-01 – 3 minutters halvlege
- En halvleg varer nu 3 minutter som standard. 5 og 10 minutter kan vælges under Indstillinger
- Uret viser stadig rigtig håndboldtid (0-60 min)

## v0.13.0 – 2026-11-01 – Finteknap og kampur
- Ny knap: Finte (tastatur: F). Finten vælges efter situationen:
  - Sidestep, når du styrer til siden: kroppen og skulderen viser den ene vej, så kommer et eksplosivt skridt den anden vej. Lykkes det, går forsvareren den forkerte vej og kan hverken takle eller holde fast et øjeblik. Holder du selv fast i forsvar, kan du miste grebet
  - Skudfinte, når du ikke styrer til siden: armen går op som til et skud, men bolden holdes tilbage. Målmanden kan bide på og flytte sig, og forsvarere kan hoppe op for at blokere. Skyder du lige efter, reagerer målmanden langsommere
- Om finten virker afhænger af spillernes værdier (fart mod forsvar, præcision mod målmandens reaktion), og samme finte mange gange i træk virker dårligere
- Computeren bruger også finter, når en forsvarer står tæt foran
- Kampuret viser nu rigtig håndboldtid: 0:00 til 30:00 i 1. halvleg og 30:00 til 60:00 i 2. halvleg, selvom en halvleg kun varer 5 eller 10 minutter

## v0.12.0 – 2026-11-01 – EM 2026, stregspil, 7-meter og passivt spil
- Alle 24 hold fra herrernes EM 2026 med rigtige spillere fra EHF's officielle trupliste, 15-17 spillere pr. hold
- Spillerne spiller på deres rigtige positioner, og startopstillingen vælges ud fra positionen og spillerens værdier
- Hjemme- og udetrøjer i holdenes farver. Udeholdet skifter automatisk til udetrøjen, hvis farverne ligner hinanden, og målmændene får en farve, der skiller sig ud
- Vælg dit hold og modstanderen i menuen, hvor startopstillingerne vises
- Spillerværdierne er skøn ud fra position, holdets styrke og kendte nøglespillere
- Mere stregspil: stregspilleren finder hullet mellem to forsvarere, og bagspillerne spiller ham oftere fri, når han står frit
- 7-meter: holder forsvaret fast i en spiller med en fri chance inden for 9 m, bliver det 7-meter
- Passivt spil: varer et angreb for længe, vises PASSIV ved uret med de afleveringer, der er tilbage. Efter 4 afleveringer uden afslutning går bolden til modstanderen

## v0.11.0 – 2026-11-01 – Spillerprofiler
- Alle spillere har nu individuelle værdier fra 1 til 10: fart, skud, præcision, vinkel (fløjskud), aflevering, forsvar og styrke. Målmænd har også reaktion og placering
- Værdierne påvirker spillet:
  - Fart: løbehastighed (fløjene er stadig hurtigst)
  - Skud: skudkraft og hvor godt spilleren scorer langt fra
  - Præcision: hvor præcist skuddet rammer
  - Vinkel: fløjskud og spidse vinkler. Andre end fløjene kan stadig tage fløjskud, men rammer dårligere
  - Aflevering: hurtigere og mere præcise afleveringer, der er sværere at opsnappe
  - Forsvar: blokering, takling, at holde fast og opsnappe afleveringer
  - Styrke: sværere at holde fast i og at tackle
  - Målmand: reaktionstid og rækkevidde
- Computeren skyder kun langt fra med spillere, der har høj skudværdi
- Spillerne har navne. Din spiller vises med nummer og navn, og målscoreren nævnes ved mål
- Holddata ligger samlet i ét format (navn, farver, trup med position, nummer og værdier), klar til landshold

## v0.10.4 – 2026-11-01 – Kortere afvisninger og målkast
- Redninger, der styres ud til siden, går langsommere og kortere ud, så bolden ikke ryger langt væk
- Bolden bremses hurtigt uden for banen og stopper kort bag baglinjen, så målmanden ikke skal løbe langt efter den
- Målkast: center og bagspillere venter på deres egen banehalvdel og tilbyder sig til målmanden i stedet for at løbe op ad banen. Fløjene kan stadig sætte i løb for at muliggøre en kontra

## v0.10.3 – 2026-11-01 – Opgiverkast til de nærmeste
- Ved opgiverkast spiller stregspilleren altid til en af de tre nærmeste medspillere (center eller bagspillerne) i stedet for næsten altid til fløjene
- Det gælder også, når du selv kaster op: du kan pege mod én af de tre nærmeste

## v0.10.2 – 2026-11-01 – Hurtigere hentning og sænkede arme
- Målmanden løber hurtigere ud og henter bolden ved målkast
- Målmanden sænker armene, når hans eget hold har bolden, og løfter dem igen, når modstanderen får den

## v0.10.1 – 2026-11-01 – Målmanden henter bolden
- Når bolden ryger ud over baglinjen (efter en redning, et skud forbi eller i sidenettet), triller den videre uden for banen, og målmanden løber hurtigt ud og henter den
- Han løber uden om målet, samler bolden op og løber tilbage i feltet, før målkastet tages. Bolden dukker ikke længere pludselig op i hans hænder
- Kameraet følger med ud bag baglinjen, mens han henter bolden

## v0.10.0 – 2026-11-01 – Nye redningsanimationer
- Målmanden redder nu primært med reflekser (ca. 85-90 % af redningerne): stor grundstilling med armene oppe, spagat med benet ved lave skud, armen ud i siden ved mellemhøje, hop med armen op ved høje og stjernen ved hopskud tæt på
- Af og til dykker han, især når han står i den ene side, og bolden kommer i den anden. Dykket er kort og kontrolleret og går ikke så langt ud til siden
- Den arm og det ben, der er på boldens side, bruges til redningen, så armene ikke længere krydser kroppen
- Lille stød i kroppen og en hvid ring, hvor bolden rammer målmanden, og et kort hop tilbage i grundstilling

## v0.9.1 – 2026-11-01 – Målmanden samler returen op
- Målmanden kan samle returen op i sit eget målfelt
- Nogle redninger dæmper bolden, så den falder næsten død ned foran målmanden, og han samler den op
- Kun når bolden styres ud til siden af målet, kan målmanden ikke nå den selv, så den ryger ud til målkast

## v0.9.0 – 2026-11-01 – Redninger, stolpe og sidenet
- Redninger giver ikke længere lange returbolde op ad banen. Bolden styres enten ud til siden af målet (målkast) eller giver en kort retur foran målet, som medspiller eller modspiller kan samle op
- Udfaldet afhænger af skuddets vinkel og redningen: skrå skud og strakte redninger ryger oftest ud til siden, centrale redninger giver oftere retur
- Målmanden kan ikke samle sin egen retur op med det samme
- Ca. 10 % flere skud rammer stolpen
- Stolpe ind eller stolpe ud afhænger af, hvor bolden rammer stolpen, og hvilken vej den bevæger sig
- Fejlrettelse: skud fra en meget spids vinkel kunne snige sig forbi stolpen og se ud, som om de gik gennem sidenettet. Nu rammer de stolpen, eller ender i sidenettet og giver målkast

## v0.8.3 – 2026-11-01 – Spillerne bliver på deres side
- Fejlrettelse: forsvarspladserne var spejlvendt, så alle spillere krydsede banen ved hvert skifte mellem angreb og forsvar (fx løb venstre fløj fra venstre side i angreb over til højre side i forsvar). Det var en væsentlig årsag til, at spillerne klumpede sammen
- Nu forsvarer hver spiller på samme side af banen, som han angriber på. Venstre fløj står ude til venstre i både angreb og forsvar og dækker modstanderens højre fløj

## v0.8.2 – 2026-11-01 – Hurtigt opgiverkast
- Ingen kunstig pause efter mål: stregspilleren står klar på midten efter ca. 1 sekund, og du kan kaste op med det samme (hurtigt opgiverkast)
- Stregspilleren står fast på midten, indtil han har kastet op, og holdkammeraterne bliver på egen banehalvdel indtil da
- Center og bagspillere stiller op helt tæt på stregspilleren ved opgiverkast
- Når du har scoret, løber din spiller helt hjem til sin forsvarsplads, før du får styringen igen. Du får den tidligere, hvis I vinder bolden, eller hvis modstanderen kommer tæt på jeres mål med bolden

## v0.8.1 – 2026-11-01 – Opgiverkast og målfeltet
- Opgiverkast: holdet, der skal kaste op, stiller op spredt på egen banehalvdel i stedet for at klumpe ved midterlinjen
- Stregspilleren tager opgiverkastet fra midten
- Når du har scoret, løber din spiller selv hjem. Du får styringen igen, når han er nede i jeres egen tredjedel af banen (eller hvis en modstander med bolden kommer tæt på)
- Markspillere kan ikke samle bolden op eller gribe en aflevering inde i målfeltet. De venter ved 6 meter, og målmanden tager bolden

## v0.8.0 – 2026-11-01 – Hold fast i forsvar
- Skud i forsvar tæt på boldholderen tager nu fat i ham i stedet for at takle
- Et kort tryk giver et let greb. Holder du knappen inde, holder du fastere, og boldholderen bremses mere
- En måler over din spiller viser, hvor fast du holder (gul, orange, rød)
- Holder du knappen inde hele vejen (ca. 0,8 sek.), bliver det frikast hver gang. Mens du holder fast, kan modstanderen ikke spille bolden af
- Slipper du halvvejs, kan det blive frikast. Bolden kan kun sjældent snuppes
- Takling erobrer nu kun bolden i 20 % af de tilfælde, hvor det skete før. Det gælder også computerens forsvarere

## v0.7.1 – 2026-11-01 – Alle løber hjem efter mål
- Efter mål (og ved halvleg) tager spillet over, og din spiller løber selv hjem på sin plads, ligesom resten af holdet
- Du får styringen tilbage, når spillet går i gang igen

## v0.7.0 – 2026-11-01 – Formation, præcise afleveringer og indkast
- Holdene holder formationen: spillerne holder afstand til hinanden og klumper ikke sammen efter redninger og boldtab
- En løs bold (fx retur fra målmanden) skifter ikke hold, før nogen har samlet den op, så forsvarerne bliver tilbage og samler op
- Kun fløjene sætter i løb ved kontra, og det sker i ca. 88 % af tilfældene. Resten jogger op i formation som anden bølge
- Fløjspillere er altid ca. 15 % hurtigere end de andre spillere
- Fløjhop: der skydes ikke længere automatisk. Gør du ingenting i luften, tabes bolden i feltet, og det bliver målkast
- Målmanden træder ud i siden og tager langskud (også de langsomme) i stedet for at stå stille
- Afleveringer er ca. 15 % hårdere og følger modtagerens løb, så de rammer præcist (ca. 85 % lander direkte hos modtageren)
- Lange afleveringer over banen går af og til højt over forsvaret, oftest fra målmanden
- Ingen spillere kan løbe uden for banen
- Indkast: spilleren er låst på sidelinjen, indtil han har afleveret, og 2-3 medspillere tilbyder sig

## v0.6.0 – 2026-11-01 – Kontraangreb og fløjhop
- Efter mål holder kun målscoreren hænderne over hovedet, og begge hold løber straks hjem som før
- Kontraangreb: fløjene er nu markant hurtigere end resten og sprinter ude langs sidelinjen foran bolden
- Er der fri bane, skærer fløjen ind mod midten. Får han ikke bolden, trækker han ud på sin fløjplads i hjørnet
- Kontra starter også efter målkast, og boldholderen spiller hurtigere op til den løbende fløj
- Fløjspillere: løber man fra hjørnet ind mod feltet med bolden, hopper fløjen automatisk ind over feltet og åbner skudvinklen
- I luften kan du selv vælge at skyde (Skud) eller aflevere (Aflever). Gør du ingenting, skyder han lige før landing
- Gælder kun fløjspillerne

## v0.5.1 – 2026-11-01 – Realistisk scoringschance
- Skud bliver mere upræcise og lidt langsommere, jo længere væk fra mål de tages
- Målmanden redder langt flere langskud og griber oftest skud fra over 12 meter
- Computeren skyder aldrig fra mere end 11 meter, og stregspilleren skyder kun tæt på 6 meter (før kunne han skyde fra egen banehalvdel i kontra)
- Kun skud kan gå i mål: afleveringer og løse bolde, der triller mod målet, samles op af målmanden
- Målmanden redder lidt færre af de korte skud, så scoringsprocenten ligger tættere på rigtig håndbold (ca. halvdelen af skuddene går ind)

## v0.5.0 – 2026-11-01 – Sideskift, nye animationer og ny menu
- Holdene skifter side ved halvleg, og kameraet vender, så du stadig angriber opad
- Målmandens stjerne: ved hopskud, fløjskud og faldskud tæt på springer målmanden op med arme og ben spredt
- Forsvarere griber om boldholderen, når de kommer helt tæt på
- Stregspilleren og hans forsvarer kæmper om pladsen ved 6 meter
- Jubel efter mål: målscoreren løber ud mod tilskuerne, og holdkammeraterne hopper med armene i vejret
- Releaseloggen er fjernet fra spillet og findes kun i CHANGELOG.md
- Start kamp ligger nu nederst i menuen, og på mobil sidder menuen i bunden af skærmen, så knappen er nem at ramme
- Blokering mod kroppen uden hop er sænket til ca. 6 %

## v0.4.1 – 2026-10-31 – Færre blokeringer
- Blokeringer sker langt sjældnere: ca. 20 % når skuddet går gennem armene på en hoppende forsvarer, og ca. 10 % mod kroppen uden hop
- Gælder både dig og computerens forsvarere

## v0.4.0 – 2026-10-31 – Takling på Skud-knappen
- Knapperne skifter ikke navn længere: de hedder altid Skud og Aflever
- I forsvar takler **Skud** boldholderen, når du er tæt på ham (det mest almindelige)
- Er du længere væk, eller er modstanderen allerede i gang med at skyde, hopper **Skud** op med armene og blokerer
- **Aflever** skifter altid til spilleren tættest på bolden i forsvar
- Blokeringer rammer oftere: større rækkevidde og højere arme ved blok-hop

## v0.3.0 – 2026-10-31 – Hurtigere afleveringer og takling
- Afleveringer er hurtigere og fladere og beregnes, så de rammer modtageren i løbet i stedet for at falde bag ham
- Modtageren løber videre mod mødepunktet i stedet for at vende om mod bolden
- Ny takling: i forsvar bliver Aflever-knappen til **Takl** (orange), når du er tæt på boldholderen, og ellers **Skift**
- Takling forfra kan erobre bolden eller give frikast, takling bagfra giver frikast, og en forbier sender forsvareren i gulvet
- Frikast tages ved 9 meter-linjen
- Computer-forsvarere takler også, i stedet for at stjæle bolden ved berøring

## v0.2.0 – 2026-10-31 – Halvlege, formationer og kontra
- Kampen spilles i 2 halvlege: 2 × 5 min (standard) eller 2 × 10 min, med halvlegspause og nyt midterkast
- Forklaringen til spillet er flyttet ind under Indstillinger (sammen med hallgulv og kamptid)
- Strammere angrebsformation: angrebet forskydes samlet mod boldsiden, bagspillerne holder dybde og afstand, stregspilleren følger bolden langs 6 meter
- Spillerne har forskellig fart efter rolle, og fløjene er hurtigst
- Kontraangreb: fløjene sætter i løb langs sidelinjen med det samme efter redning eller erobring, og resten følger i anden bølge
- Målmanden kaster langt til en fri fløj
- Kontraangreb afsluttes med hopskud i fart
- Forsvaret spurter hjem og stiller op i 6-0, før det begynder at glide med bolden

## v0.1.0 – 2026-10-31 – Første spilbare prototype
- Stil 2B: stående figurer med løbe-animationer, skygger og trøjenumre
- 5 hallgulve: Landskamp, Trægulv, Grøn hal, Klubhal, Pokalfinale (valget huskes)
- Hold A (spiller) mod Hold B (computer) med 6 markspillere + målmand
- Afleveringer med føring, opsnappede bolde og løse bolde
- Skudtyper efter situation:
  - Fløjskud: fløjspilleren hopper ind over målfeltet før skuddet
  - Hopskud: når forsvaret står tæt foran, eller i fuld fart
  - Stående skud: når der er plads
  - Faldskud: tæt på 6-meter-linjen
- Sigte med retning under skuddet (hjørne, højt/lavt)
- Stolpe- og overliggerskud med retur eller ind, ryst i målrammen og net der buler
- 6-0 forsvar der glider med bolden, træder ud mod boldholderen og blokerer med armene oppe
- Målmand med reaktionstid, placering på vinklen, dyk og redning med greb eller retur
- Indkast, målkast, midterkast efter mål og kampur (3/5/10 min)
- Mobil (joystick + knapper) og tastatur, fuld skærm og pause
