# Håndbold

Håndboldspil til browser og mobil i top-down-stil, i samme familie som Sensible fodbold og Ishockey.

- Spil online: https://seranodk.github.io/handbold/
- Kode: https://github.com/seranodk/handbold
- Spil lokalt: åbn `index.html`. Hver version gemmes også som `haandbold-vX.Y.Z.html`
- Releaselog: se `CHANGELOG.md`
- Sværhedsgrad: Let, Normal eller Svær (Indstillinger)
- Kamptid: 2 × 3 min (standard), 2 × 5 min eller 2 × 10 min (Indstillinger). Uret viser rigtig håndboldtid (0-60 min)
- Hovedmenu: Hurtigkamp, Venskabskamp, Turneringer, Sæson og Indstillinger
- Turneringer: EM 2026 eller Champions League 2026/27 med gruppe, mellemrunde, semifinale og finale (gemmes i browseren)
- Sæson: Herreligaen 2026/27 (26 runder + slutspil) eller Bundesliga 2026/27 (34 runder) (gemmes i browseren)
- Idéer til kommende versioner: `ROADMAP.md`

## Styring
- Mobil: venstre tommel styrer, Skud og Aflever til højre (i forsvar: Skud = takl eller blok-hop, Aflever = skift spiller)
- Mobil: Aflever under Skud og Finte til venstre for Aflever (sidestep når du styrer til siden, ellers skudfinte)
- Tastatur: piletaster/WASD, Mellemrum = skud/blok, X eller J = aflever/skift, F = finte, P = pause
- Bagspillere: kort tryk på Skud = stående skud eller underhåndsskud, hold knappen = skudtype efter situationen
- Sigte: hold retning mens du skyder. Venstre/højre = hjørne, frem = højt, tilbage = lavt
- Når din målmand har bolden: Skud = langt udkast til en fløj (styr til siden for at vælge), Aflever = kort udkast

## Hold og spillere
Landsholdene fra EM 2026 ligger i `EM_TEAMS`, klubberne fra EHF Champions League 2026/27 i `CL_TEAMS` og ligaholdene fra Herreligaen og Bundesliga i `LG_TEAMS` (holdlisterne i `LEAGUES`) i scriptet i `index.html`. Hvert hold har landekode, navn, styrke (`tier`, 1-10), hjemme- og udetrøje (`[trøje, kant, shorts, nummer]`) og en trup i formatet `POS NR Navn*`, fx `RB 19 Gidsel*`. Positioner: `G`, `LW`, `LB`, `CB`, `RB`, `RW`, `P`. Stjerne markerer en nøglespiller, `^` en fast starter, `~` en fast straffekaster, `!` vender kastehånden, og `@196` angiver højden i cm (højre back og højre fløj er ellers venstrehåndede, resten højrehåndede).

Spillernes værdier beregnes ud fra position, holdets styrke og stjerne og har værdier fra 1 til 10:

| Værdi | Betydning |
|---|---|
| fart | løbehastighed |
| skud | skudkraft og evne til at score langt fra (9-11 m) |
| praecision | hvor præcist skuddet rammer |
| vinkel | fløjskud og skud fra spidse vinkler |
| aflevering | hurtighed og præcision i afleveringer |
| forsvar | blokering, takling, holde fast, opsnappe |
| styrke | svær at holde fast i og tackle |
| reaktion, placering | kun målmænd: reaktionstid og rækkevidde |

5 svarer til en gennemsnitlig spiller.

Holdstil sættes i `STYLE` (kontra, tempo, taktisk, fysisk). Hver spiller får et signaturskud ud fra position og navn.

## Demoer
Mappen `demo/` indeholder testvideoer og demosider af idéer, før de blev indført (redninger, grafik, angrebsspil).

## Udvikling
Alt ligger i én fil uden build-trin. Ved ny version: opdater `VERSION` og `<title>` i `index.html`, gem en kopi som `haandbold-vX.Y.Z.html` og tilføj en sektion i `CHANGELOG.md`.
Tilføj `#auto` til adressen for at se computer mod computer.
