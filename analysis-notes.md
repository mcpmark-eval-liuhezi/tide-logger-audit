# Analysis Notes

Working notes from the tide-logger hackathon.

- The nightly low/high tide extraction still uses a fixed 24h window; a rolling
  window per station would be more robust across time zones.
- Sensor drift is visible on station `buoy-114` after ~10 days of continuous
  deployment; recalibration cadence should be documented before handover.
- Data quality checks should be rerun on the archived logs before any release.

## Open questions for the handover

1. Which station inventory does the lab maintain going forward?
2. Do they need the raw CSV dumps or only the cleaned JSON?
