---
layout: page
title: Multi-Tier QA/QC Analysis of New Mexico Weather Stations
description: An example of multi-tier quality assurance and quality control (QA/QC) of surface observation hourly temperature data for New Mexico weather stations
img: /assets/img/LAS_CRUCES_INTL_AIRPORT_Enhanced_QAQC.jpg
importance: 1
category: work
related_publications: false
---

## Project Overview
This project implements a comprehensive **4-tier Quality Assurance/Quality Control (QA/QC) framework** for hourly temperature data from weather stations across New Mexico. The analysis uses NOAA's Global Hourly ACCESS data to identify and flag suspicious data points while preserving legitimate extreme weather events like heatwaves.

### Methodology: 4-Tier QA/QC Approach
1. **Tier 1: Physical Range Check** (-40°C to 55°C)
2. **Tier 2: Temporal Consistency** (spikes <8°C/hr, no 12h flatlines)
3. **Tier 3: Spatial Validation** (vs nearest neighbor, ±6°C anomaly threshold)
4. **Tier 4: Extreme Heat Preservation** (>40°C always preserved)

Each figure below shows the QA/QC results for a specific weather station in New Mexico, demonstrating how the multi-tier approach identifies and handles different types of data quality issues.

---

## Station Analysis Results

### Major Urban and International Airports

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ALBUQUERQUE_INTL_SUNPORT_AIRPORT_Enhanced_QAQC.jpg" title="Albuquerque International Sunport - Major urban station with moderate flag rate" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Albuquerque International Sunport**: The largest station in New Mexico showing excellent data quality with only minor flagging. Blue line represents validated data after QA/QC, red dots show flagged points, and orange zone indicates extreme heat preservation area (>40°C).
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/LAS_CRUCES_INTL_AIRPORT_Enhanced_QAQC.jpg" title="Las Cruces International Airport - Southern NM station with good data quality" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Las Cruces International Airport**: Southern New Mexico's primary airport showing excellent data quality with clear seasonal patterns. Low flag rate indicates well-maintained instrumentation and reliable data collection.
</div>

### Southern New Mexico Stations

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/LAS_CRUCES_20_N_Enhanced_QAQC.jpg" title="Las Cruces 20 North - Rural station north of Las Cruces" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ALAMOGORDO-WHITE_SANDS_RGL_AIRPORT_Enhanced_QAQC.jpg" title="Alamogordo-White Sands Regional Airport - Southern desert station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Southern NM Comparison**: Left shows Las Cruces 20 North, a rural station with more variable data quality. Right shows Alamogordo-White Sands Regional Airport in the desert region with characteristic high summer temperatures.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ARTESIA_2_WNW_Enhanced_QAQC.jpg" title="Artesia 2 WNW - Rural station near oil fields" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/ARTESIA_MUNICIPAL_AIRPORT_Enhanced_QAQC.jpg" title="Artesia Municipal Airport - Southeastern desert station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Artesia Region Stations**: Left shows Artesia 2 WNW, a rural station with moderate data quality and some clustering of flags. Right shows Artesia Municipal Airport with better data consistency, demonstrating how station type affects data quality.
</div>

### Northeastern and Mountain Stations

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/LAS_VEGAS_MUNICIPAL_ARPT_Enhanced_QAQC.jpg" title="Las Vegas Municipal Airport - Northeastern station with moderate data issues" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/ANGEL_FIRE_AIRPORT_Enhanced_QAQC.jpg" title="Angel Fire Airport - High elevation ski area station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Northeastern NM Comparison**: Left shows Las Vegas Municipal Airport with some data quality issues, particularly clustered flags. Right shows Angel Fire Airport at high elevation with cooler temperatures and good data quality.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/LEA_COUNTY_REGIONAL_AIRPORT_Enhanced_QAQC.jpg" title="Lea County Regional Airport - Eastern plains station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Lea County Regional Airport**: Eastern plains station showing excellent data continuity with minimal flagging. The consistent temperature pattern indicates reliable instrumentation and good maintenance in this agricultural region.
</div>

### Northern New Mexico and Research Stations

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/LOS_ALAMOS_AIRPORT_Enhanced_QAQC.jpg" title="Los Alamos Airport - High elevation mountain station" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/LOS_ALAMOS_13_W_Enhanced_QAQC.jpg" title="Los Alamos 13W - Secondary mountain station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Los Alamos Research Area**: Both stations show excellent data quality expected from research-focused installations. Left shows the main airport station, right shows a secondary station. Minimal flagging indicates well-calibrated instruments and regular maintenance.
</div>

### Remote and Specialized Stations

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/NAGEEZI_18_SSW_Enhanced_QAQC.jpg" title="Nageezi 18 SSW - Remote Navajo Nation station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **Nageezi 18 SSW**: Remote station in the Navajo Nation showing moderate data quality with some seasonal patterns in flagging. This station represents the challenges of maintaining consistent data quality in remote locations with limited infrastructure.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/MCGREGOR_RANGE_BASE_CAMP_Enhanced_QAQC.jpg" title="McGregor Range Base Camp - Military installation station" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    **McGregor Range Base Camp**: Military installation station showing good data quality despite its specialized location. The flag distribution panel shows random rather than clustered flags, indicating isolated issues rather than systematic problems.
</div>

---

## Regional Analysis Summary

### Data Quality by Region
| Region | Average Flag Rate | Typical Stations | Common Issues |
|--------|-------------------|------------------|---------------|
| **Urban Airports** | <5% | Albuquerque, Las Cruces Intl | Minimal, random flags |
| **Southern Desert** | 5-10% | Alamogordo, Artesia | Heat-related spikes, seasonal patterns |
| **Eastern Plains** | 3-8% | Lea County, Artesia 2 WNW | Moderate, some clustering |
| **Northeastern** | 8-15% | Las Vegas, Angel Fire | Clustered flags, maintenance patterns |
| **Northern Mountains** | 2-6% | Los Alamos | Excellent quality, minimal issues |
| **Remote Areas** | 10-20% | Nageezi | Higher flag rates, access challenges |

### Key Patterns Observed
1. **Urban vs Rural**: Urban stations generally show better data quality due to better maintenance and infrastructure
2. **Elevation Effects**: Mountain stations have more stable temperature patterns and fewer extreme heat events
3. **Seasonal Variation**: Flag rates often increase during seasonal transitions (spring/fall)
4. **Station Type**: Airport stations generally outperform rural or specialized stations
5. **Extreme Heat**: Properly preserved across all stations, with southern stations showing more events

---

## Technical Implementation

### How to Read the Plots
Each QA/QC plot contains multiple panels:

1. **Main Time Series (Top)**
   - **Gray line**: Raw temperature data
   - **Blue line**: Validated data (passed all QA/QC tiers)
   - **Red dots**: Flagged/removed data points
   - **Orange zone**: Extreme heat preservation area (>40°C)
   - **Statistics overlay**: Total points, flag percentages, and breakdown by flag type

2. **Monthly Flag Distribution (Middle Left)**
   - Shows flag percentage by month
   - Bar chart with monthly flag rates
   - Helps identify seasonal patterns in data quality

3. **Flag Type Distribution (Middle Right)**
   - Pie chart showing which QA/QC tier caught most issues:
     - **Range flags**: Values outside -40°C to 55°C
     - **Spike flags**: Changes >8°C per hour
     - **Flatline flags**: Nearly constant for 12+ hours
     - **Spatial flags**: Differs from neighbor by >6°C

4. **Raw vs Validated Distribution (Bottom Left)**
   - Box plots comparing statistical distributions before and after QA/QC
   - Shows impact on mean, median, and range
   - Data loss percentage indicated

5. **Flag Clustering Analysis (Bottom Right)**
   - Time series of flags in rolling windows
   - Shows temporal patterns in flag occurrence
   - Clustered flags suggest systematic issues
   - Random flags suggest isolated errors

### Interpreting Flag Patterns
- **Clustered flags**: Suggest systematic instrument issues, maintenance problems, or local events
- **Random flags**: Indicate isolated errors or outliers
- **Seasonal patterns**: Higher flag rates in specific months may indicate seasonal maintenance or weather patterns
- **Consistent low flags**: Indicate well-maintained, reliable stations

### Data Processing Pipeline
- **Data Acquisition** → NOAA Global Hourly ACCESS data download

- **Station Metadata** → ISD history file processing

- **Neighbor Analysis** → Geographic nearest neighbor assignment

- **Tier 1 Processing** → Physical range checks

- **Tier 2 Processing** → Temporal consistency checks

- **Tier 3 Processing** → Spatial validation

- **Tier 4 Processing** → Extreme heat preservation

- **Statistics Calculation** → Flag rates, data loss, quality metrics

- **Visualization** → Multi-panel plots for each station

- **Reporting** → Summary statistics and quality classification
  
### Statistical Metrics Calculated
For each station, the analysis calculates:
- **Total data points** and **flag counts** by type
- **Flag percentages** overall and by month
- **Data retention rate** after QA/QC
- **Clustering metrics** (autocorrelation, max consecutive flags)
- **Quality classification** (Excellent/Good/Moderate/Poor)
- **Comparison statistics** (raw vs validated means, ranges)

### Quality Classification Scheme
- **Excellent**: <5% flags (Green category)
- **Good**: 5-10% flags (Light green)
- **Moderate**: 10-20% flags (Orange)
- **Poor**: >20% flags (Red)
- **Heatwave points**: Always counted separately and preserved

---

## Conclusions and Applications

### Key Findings
1. **Station Reliability Varies**: Data quality correlates with station type, location, and maintenance
2. **Spatial Validation Works**: Neighbor comparison effectively identifies outlier stations
3. **Extreme Events Preserved**: The 4-tier approach successfully preserves legitimate heatwaves
4. **Systematic Issues Detectable**: Flag clustering analysis identifies stations needing maintenance
5. **Regional Patterns Evident**: Different regions show characteristic data quality profiles

### Practical Applications
- **Climate Research**: High-quality validated datasets for trend analysis
- **Weather Forecasting**: Improved input data for numerical models
- **Infrastructure Planning**: Better extreme temperature statistics for design
- **Agricultural Management**: Reliable temperature data for crop models
- **Energy Sector**: Accurate temperature data for load forecasting
- **Public Health**: Improved heatwave monitoring and warning systems

### Recommendations for Data Users
1. **Check Quality Classification**: Use the color-coded quality ratings when selecting stations
2. **Review Flag Patterns**: Examine flag clustering to identify systematic issues
3. **Consider Regional Context**: Account for regional data quality patterns in analyses
4. **Use Validated Data**: Always use the blue-line validated data for research
5. **Check Extreme Events**: Verify that heatwave points are preserved in your analysis

### Future Improvements
- **Network Analysis**: Include more sophisticated spatial validation using multiple neighbors
- **Machine Learning**: Add anomaly detection algorithms to the QA/QC pipeline
- **Real-time Processing**: Develop streaming versions for operational use
- **Additional Variables**: Extend to humidity, pressure, wind, and precipitation
- **Interactive Tools**: Web-based interfaces for custom QA/QC parameter adjustment

---

## Data and Code Availability

### Data Sources
- **Primary Data**: NOAA Global Hourly ACCESS data (https://www.ncei.noaa.gov/)
- **Station Metadata**: ISD History file (updated monthly)
- **Geographic Data**: State boundaries and base maps from public sources

### Software Tools
- **Python 3.8+** with scientific stack (pandas, numpy, matplotlib)
- **Geospatial libraries**: cartopy, geopy
- **Visualization**: matplotlib with custom styling
- **File I/O**: CSV, PNG, PDF formats

### Code Repository
The complete analysis code is available as modular Python scripts:
- `download_noaa_data.py` - Data acquisition
- `station_network_analysis.py` - Network and neighbor analysis
- `qaqc_pipeline.py` - 4-tier QA/QC processing
- `visualization.py` - Plot generation
- `report_generation.py` - Summary statistics and reports

### Reproducibility
All analyses are fully reproducible with:
1. Python environment specification (requirements.txt)
2. Configuration files for all parameters
3. Seed values for random number generation
4. Complete documentation of processing steps

### Citation
If you use this methodology or results in your research, please cite:

> *Multi-Tier QA/QC Analysis of Surface Temperature Observations: A Case Study of New Mexico Weather Stations. [Year]. [Your Name/Affiliation].*

### Acknowledgments
- **Data Providers**: NOAA/NCEI for public access to weather data
- **Methodology**: Inspired by established QA/QC procedures in meteorological research
- **Tools**: Open-source Python community for scientific computing libraries

{% raw %}

```html
<!-- Example of how to include these figures in your portfolio -->
<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/YOUR_STATION_Enhanced_QAQC.jpg" title="Your station analysis" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
    Your station description here. Include key findings and interpretation.
</div>
{% endraw %}

Last updated: {{ site.time | date: '%B %d, %Y' }}
