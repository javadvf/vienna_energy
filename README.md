# vienna_energy
National 15-minute panel combining Austrian electricity demand, imbalance prices, generation mix, and weather (2019–2024)

This repository contains a national 15-minute resolution dataset for Austria, merging:
- APG imbalance settlement prices (€/MWh)
- E-Control system load and generation mix
- Meteostat weather data (temperature, wind, radiation)
- Cross-border exchange flows

The dataset supports the study:
> Farahani, Javad Vasheghani (2025). *Real-Time Demand Elasticity During Negative Imbalance Price Events.*

### Columns
| column | description | unit |
|--------|--------------|------|
| ts | Timestamp (Europe/Vienna, 15-min) | ISO8601 |
| demand_mw | System load | MW |
| price_eur_mwh | Imbalance settlement price | €/MWh |
| temp_c | Air temperature | °C |
| wind_ms | Wind speed | m/s |
| solar_wm2 | Global horizontal irradiance | W/m² |
| hydro_share | Hydropower share | % |
| import_mw | Net import (positive = import) | MW |
| ... | (extend if more columns exist) | ... |
