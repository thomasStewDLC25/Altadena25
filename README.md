**January 2025 Los Angeles Area Wildfires**

**Vegetation Burn Impact Analysis in Altadena, CA Using Landsat-derived NBR Animation****

**Objective**
The primary objective of this analysis is to visualize the impact of a wildfire event in Altadena, California by
generating a smooth transition animation between pre-fire and post-fire conditions using Landsat surface
reflectance data. The animation is driven by the Normalized Burn Ratio (NBR), a vegetation index sensitive to
fire-related changes.

**Study Area**
The Area of Interest (AOI) is a small polygon covering a portion of Altadena, CA:
- Latitude: ~34.1835 to 34.1995
- Longitude: ~-118.1045 to -118.1325

**Data Sources**
Pre-fire imagery:
- Sensor: Landsat 9 (Collection 2, Tier 1, Level 2 SR)
- Date range: January 14-15, 2025
- Cloud cover: Less than 35%
Post-fire imagery:
- Sensor: Landsat 8 (Collection 2, Tier 1, Level 2 SR)
- Date range: January 22-28, 2025
- Cloud cover: Less than 35%

**Methodology**
1. Data Preprocessing:
Each Landsat image is filtered by AOI, target date, and cloud cover. Surface reflectance values from bands 5
(NIR) and 7 (SWIR2) are scaled using:
Reflectance = DN × 0.0000275 - 0.2
2. NBR Calculation:
Vegetation Burn Impact Analysis in Altadena, CA Using Landsat-derived NBR Animation
NBR = (NIR - SWIR2) / (NIR + SWIR2)
3. Temporal Aggregation:
Median NBR is calculated for pre- and post-fire periods.
4. Animation Creation:
Linear blending across 30 frames simulates vegetation transition. Each frame is generated using:
Blended = PreFire × (1 - ?) + PostFire × ?
Where ? ranges from 0 to 1.
5. Export:
A 30-frame video is exported as .mp4 (10 fps, 720p) using Export.video.toDrive.

**Results**
- Pre-Fire NBR: Healthy vegetation in blue/white tones.
- Post-Fire NBR: Burned areas shift toward red.
- Animation Output: Smooth transition shows impact progression.

**Conclusion**
This animation provides a visual tool for assessing wildfire impacts. The use of multi-temporal Landsat NBR
enables monitoring of vegetation changes. The method can be applied to other fire-affected areas with minor
adjustments.
