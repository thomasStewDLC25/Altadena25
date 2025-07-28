# Altadena25

# Altadena Fire NBR Animation using Google Earth Engine

This repository includes a Google Earth Engine (GEE) script that computes pre- and post-fire Normalized Burn Ratio (NBR) values over Altadena, CA using Landsat 8 and 9 imagery. The script creates a smooth animation showing NBR changes across 30 blended frames.

The video export is stored in your Google Drive under the `GEE_Exports` folder.

## Requirements
- A Google Earth Engine account
- Export permissions to Google Drive

## Code Summary
- Uses Landsat 9 (pre-fire) and Landsat 8 (post-fire)
- Filters for minimal cloud coverage
- Calculates NBR for each image
- Blends between pre- and post-fire NBR for animation
- Exports as MP4 to Google Drive

## Visualization
The output is an NBR transition animation showing vegetation burn severity over time.

## License
MIT
