<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoraggio: che cosa si legge e con quale esito

[English](README.en.md)

Come global-law monitora ogni paese: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). Questa pagina fa lo stesso per Emilia-Romagna soltanto: ogni lettura di una fonte ufficiale, quando è avvenuta e con quale esito (atti aggiunti, modificati e rimossi). La forma leggibile dalle macchine è [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` come commit `Kind: check`, e mese per mese in [checks/](checks/).

**Ultimo controllo:** 2026-11-24 00:34 UTC, Demetra (Assemblea legislativa della Regione Emilia-Romagna): 19 indirizzi letti; 0 aggiunti, 0 modificati, 0 rimossi; nessuna modifica; 1 non pubblicati, di cui 0 senza motivo.

## Fonti

| Fonte | Cartelle | Frequenza | Ultimo controllo riuscito | Ultimo esito | Stato |
| --- | --- | --- | --- | --- | --- |
| [Demetra (Assemblea legislativa della Regione Emilia-Romagna)](https://demetra.regione.emilia-romagna.it/al/) | `lr/`, `statuto/` | ogni giorno | 2026-11-24 00:34 UTC | nessuna modifica | sorvegliata: Demetra non indica la data di modifica: ogni zip è riletto quando cambia la sua dimensione e almeno ogni 11 giorni |

## Gli ultimi 30 giorni

| Inizio (UTC) | Fonte | Letti | Aggiunti | Modificati | Rimossi | Non pubblicati (senza motivo) | Esito | Commit |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-24 00:33](checks/2026-11.md#it-demetra-20261124t003330z) | demetra | 19 | 0 | 0 | 0 | 1 (0) | nessuna modifica | — |
| [2026-11-24 00:28](checks/2026-11.md#it-demetra-20261124t002845z) | demetra | 30 | 0 | 0 | 0 | 1 (0) | modifiche trovate | [7](https://github.com/lexifina/italy-emilia-romagna-law/compare/32a1b2ceb54d...f830d8faf955) |

## Verificalo da te

```
python tools/checktrail.py                      # l'ultimo controllo di ogni fonte
python tools/checktrail.py --day 2026-11-23     # tutti i controlli di un giorno
python tools/checktrail.py --act <id>           # quando un atto è stato visto e pubblicato
git log --grep='^Kind: check' --format='%ci %s'  # i controlli nella cronologia
```

Ha valore legale solo la pubblicazione ufficiale; i testi qui sono copie per la lettura e la ricerca.
