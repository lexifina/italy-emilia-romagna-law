<!-- lawwatch: written from data/checks by the check trail; edit the records, not this page -->

# Monitoring: what is read and what came of it

[Italiano](README.md)

How global-law monitors every country: [global-law monitoring/](https://github.com/lexifina/global-law/tree/main/monitoring). This page is the same for Emilia-Romagna only: every time an official source is read, when, and what came of it (acts added, changed and removed). The machine-readable form is [data/checks/](../data/checks/) (JSON Lines, schema `lexifina-check/1`), in `git log` as `Kind: check` commits, and month by month in [checks/](checks/).

**Last check:** 2026-11-24 00:34 UTC, Demetra (Assemblea legislativa della Regione Emilia-Romagna): 19 addresses read; 0 added, 0 changed, 0 removed; no change; 1 not published, 0 of them with no reason.

## Sources

| Source | Folders | How often | Last successful check | Last result | State |
| --- | --- | --- | --- | --- | --- |
| [Demetra (Assemblea legislativa della Regione Emilia-Romagna)](https://demetra.regione.emilia-romagna.it/al/) | `lr/`, `statuto/` | daily | 2026-11-24 00:34 UTC | no change | watched: Demetra sends no Last-Modified: each zip is read again when its length changes and at least every 11 days |

## The last 30 days

| Started (UTC) | Source | Read | Added | Changed | Removed | Not published (no reason) | Result | Commits |
| --- | --- | ---: | ---: | ---: | ---: | ---: | --- | ---: |
| [2026-11-24 00:33](checks/2026-11.md#it-demetra-20261124t003330z) | demetra | 19 | 0 | 0 | 0 | 1 (0) | no change | — |
| [2026-11-24 00:28](checks/2026-11.md#it-demetra-20261124t002845z) | demetra | 30 | 0 | 0 | 0 | 1 (0) | changes found | [7](https://github.com/lexifina/italy-emilia-romagna-law/compare/32a1b2ceb54d...f830d8faf955) |

## Check it yourself

```
python tools/checktrail.py                      # the latest check of every source
python tools/checktrail.py --day 2026-11-23     # every check of a day
python tools/checktrail.py --act <id>           # when an act was seen and published
git log --grep='^Kind: check' --format='%ci %s'  # the checks in the history
```

Only the official publication has legal force; the texts here are copies for reading and searching.
