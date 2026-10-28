# Kaffeapp

Kalkulator for pourover: velg hvor mye ferdig kaffe du vil ha, så får du gram kaffe, hvor mye vann du skal helle og en helleplan med tidtaker.

**Bruk den her:** https://pedermyhrer.github.io/kaffeapp/

| Side | Innhold |
|---|---|
| `index.html` | Kalkulatoren med beholdere, styrke, helleplan og tidtaker |
| `fremgangsmate.html` | Slik brygger du pourover steg for steg |
| `style.css` | Felles stil, fonter og farger |

## Bruk

- **Antall:** velg en beholder (Camelbak termos 275 g, kopp 200 g eller dine egne) og hvor mange.
- **Totalt:** skriv inn hvor mye ferdig kaffe du vil ha, for eksempel 500 g.
- **Styrke:** forholdet mellom kaffe og vann du heller, fra 1:14 til 1:19. Standard er 1:17.
- **g eller ml:** 1 ml kaffe veier omtrent 1 g, så tallene er de samme.

Egne beholdere og siste innstillinger lagres lokalt i nettleseren.

Lenker kan forhåndsvelge: `?p=termos&n=2`, `?t=500` og `?r=16`.

## Slik regnes det

Kaffegruten holder igjen omtrent 2 g vann per gram kaffe. For å ende på `ut` gram i koppen med forholdet `1:r`:

```
kaffe = ut / (r - 2)
vann  = kaffe × r
```

Eksempel: 275 g i termosen med 1:17 gir 18,3 g kaffe og 312 g vann.

## Personvern

Ingen informasjonskapsler, ingen sporing og ingen eksterne ressurser. Fontene ligger i repoet, og alt regnes ut i nettleseren. GitHub Pages logger besøkendes IP-adresser av sikkerhetshensyn, se [GitHubs personvernerklæring](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Lisens

Koden er lisensiert under [MIT](LICENSE). Skriftene i `fonts/` (Young Serif, Figtree og JetBrains Mono) er lisensiert under SIL Open Font License 1.1, med lisenstekst i samme mappe.
