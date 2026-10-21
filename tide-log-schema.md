# Tide Log Schema

Data captured by the tide-logger hackathon build.

| field           | type      | notes                                |
| --------------- | --------- | ------------------------------------ |
| station_id      | string    | Coastal station identifier           |
| recorded_at     | ISO-8601  | UTC timestamp of the reading         |
| tide_level_m    | float     | Water level in meters (MLLW datum)   |
| sensor_status   | enum      | ok, drift, or fault                  |

## Example record

```json
{
  "station_id": "buoy-114",
  "recorded_at": "2024-06-01T18:02:00Z",
  "tide_level_m": 1.42,
  "sensor_status": "ok"
}
```
