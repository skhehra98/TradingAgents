# trader-scanner

`scan.py` is vendored unchanged from
[Jakeschincariol/day-trader-skill](https://github.com/Jakeschincariol/day-trader-skill)
(`trader-scanner/scan.py` at 3d0f4ef, MIT license, see `LICENSE`). Standard library only.

`.github/workflows/daily-scan.yml` runs `scan.py universe` then `scan.py daily`
every weekday before the open and saves `trader/watchlist.json` as a run
artifact; the hits are also in the run's summary. Run it by hand from the
Actions tab ("Daily scan" > Run workflow).

A scan is a list of charts that match a rule, not a list of stocks to buy.
