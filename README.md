# tfl-status

A 10-minute mirror of the TfL line-status feed
(`/Line/Mode/tube,overground,dlr,elizabeth-line/Status`), kept in `status.json`
by the GitHub Action in `.github/workflows/refresh.yml`. Exists because some
sandboxes that need the data can reach raw.githubusercontent.com but not
api.tfl.gov.uk. The Action amends a single rolling commit, so history stays
flat; `updated` inside `status.json` is the fetch time (UTC). All data is
public TfL open data.
