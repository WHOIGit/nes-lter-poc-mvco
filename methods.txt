# About Martha's Vineyard Coastal Observatory

The Martha's Vineyard Coastal Observatory (MVCO) Air-Sea Interaction Tower (ASIT) is located at 41.325 N, 70.567 W. See https://mvco.whoi.edu/about/ for more site information. Samples were collected in the vicinity of the tower.

# Equipment preparation

New 25 mm Whatman Glass Microfiber Filters (GF/F) (Fisher catalog number 09-874-64) were placed in a 25 ml glass beaker covered with double-layered aluminum foil and combusted at 450 degC for at least 4 hours. GF/Fs were never combusted more than once. Brown polycarbonate sample bottles were filled with 10% hydrochloric acid and soaked for at least 4 hours, then triple-rinsed with water purified using a Millipore Milli-Q lab water system (MilliQ), thoroughly dried, and capped. A freshly acid-washed bottle was used for each sample collected. When circumstances allowed prior to sample filtration, filter funnel cups and frits were soaked in 10% hydrochloric acid and soaked for at least 1 hour, then triple-rinsed with Milli-Q water; otherwise the funnels and frits were triple-rinsed with distilled water and dried.

# CTD Rosette Bottle and Bucket Sampling

Samples were collected from the water column at multiple depths using Niskin bottles on a CTD rosette system. Some samples were collected at the surface with a bucket. In the event_number_niskin field of the data table, MVCO event number is combined with a suffix indicating a bucket sample (_00) or Niskin bottle number (e.g. _01). The depth for bucket samples is 0 m; some surface Niskin samples also have depth recorded as 0 m. For each sample, a clean half liter sample bottle was triple rinsed with sample water and filled. Sample bottles were filled from each Niskin, stored in a cooler, and filtered as soon as possible (within 4 hours). Approximately 10% replicate samples were collected over time to check for sampling precision.

# Filtering Protocol

For each sample, a known volume was filtered through a combusted GF/F filter under low vacuum suction (~5 in. Hg). Upon filtering completion, using gloves and dedicated clean forceps, each filter was carefully placed into a clean labeled polystyrene petri dish with particle side facing up and placed in a 60 degC drying oven and left overnight, then stored in a desiccator until further processing.

# Sample Analysis

Wearing gloves on a clean work surface, the samples were folded into a 30 mm ultra clean tin disk (Part no. CE Elantech Inc 25208015) using clean forceps, compressed into a pellet, and stored in a clean polystyrene well plate in a desiccator until analysis.

Samples were submitted to the Woods Hole Oceanographic Institution's Nutrient Analytical Facility (https://web.whoi.edu/nutrient/current-rates/) where they were analyzed using a Flash EA1112 CHN analyzer with the operational detection limit based on the lowest detectable value of the standard processed with each analyzed batch of samples. The CHN analyzer manufacturer states detection limits of 0.01% or 100 ppm for carbon and nitrogen. The instrument measured organic carbon and nitrogen using 4 pairs of thermal conductivity detectors after high temperature combustion and separation through chemical traps. Certified reference material Acetanilide (Certificate#293514) was combusted with every run and an average recovery was provided with the sample results.

One or more blanks were collected from each combusted batch of GF/Fs per analysis batch. Starting in 2012, blanks were taken from the combusted stock beaker of filters, placed in a clean polystyrene labeled petri dish, and placed directly into the dessicator. In 2017, the protocol was updated and some blanks were put on the filter rig to mimic standard filtering protocol before being placed into the clean petri dish, but no liquid was filtered. Blanks were then placed directly into the dessicator. Blanks were pelletized using ultra clean tin disks as for samples.

# Data Calculations and Quality Control

The lab group made calculations to account for volume filtered and corrected for blanks. Blank values were inspected, averaged, and subtracted from initial results. If in the event no blanks were analyzed for a batch of samples, blank values were estimated based on adjacent blank values. Blank-corrected molar values were divided by volume filtered for a final concentration in micromoles per liter. Carbon and nitrogen atomic weights were used to calculate mass in micrograms per liter. The carbon to nitrogen ratio is reported as a molar ratio.

We provide columns in the data table to indicate quality for carbon and nitrogen values: 1 good; 2 questionable/suspect; 3 bad; 6 below detection limit; 9 missing data. Samples with a flag of 3 (bad) are provided with a value of NaN. The carbon to nitrogen ratio is set to NaN when the ratio is unable to be calculated (missing data, nitrogen below detection limit, flagged bad values). Factors considered in quality control were magnitude of sample, the carbon to nitrogen ratio, and any additional notes during sample collection or sample analysis. For suspicious samples, CHN analyzer output of carbon and nitrogen peaks were manually inspected by the analytical lab and some peak integrations were manually adjusted.

# Data Cleaning

All below detection limit values were set to zero and quality flag set to 6.
We rounded POC, PON, and the ratio; added ship name and R/V Tioga event number when applicable; and ensured that rows were arranged in chronological order.

# Data package assembly

Data package assembly with metadata templates was completed in R, with documentation available at https://github.com/WHOIGit/nes-lter-poc-mvco

# References

CE Instruments Flash EA 1112 CHN Analyzer Technical Manual. 1999.

M. Ehrhardt and W. Koeve. 1999. Determination of particulate organic carbon and nitrogen in Methods of Seawater Analysis (3rd edition), edited by K. Grasshoff, K. Kremling, and M. Ehrhardt. pp 437-444. Wiley. https://doi.org/10.1002/9783527613984.ch17

Sharp, J. H. 1974. Improved analysis for particulate organic carbon and nitrogen from seawater. Limnology and Oceanography, 19, 984-989.
 
# Related Packages

Event logs from Northeast U.S. Shelf Long Term Ecological Research (NES-LTER) cruises to the Martha's Vineyard Coastal Observatory (MVCO), are in the following package:

Sosik, H.M., E.T. Crockford, E. Peacock, and J.K. Llopiz. 2025. Event logs from Northeast U.S. Shelf Long Term Ecological Research (NES-LTER) cruises to the Martha's Vineyard Coastal Observatory (MVCO) ongoing since 2017 ver 2. Environmental Data Initiative. https://doi.org/10.6073/pasta/efff67e138fe866c2e763e2ae68e2d34 (Accessed 2025-07-21).

Particulate organic carbon (POC) and nitrogen (PON) from NES-LTER Transect cruises, which cover a larger geographic area of the same region, are in the following package:

Sosik, H.M., E.T. Crockford, and E. Peacock. 2025. Particulate organic carbon (POC) and nitrogen (PON) from Northeast U.S. Shelf Long Term Ecological Research (NES-LTER) Transect cruises, ongoing since 2017 ver 3. Environmental Data Initiative. https://doi.org/10.6073/pasta/79463e428673133dd9f7994e54e7daf6 (Accessed 2025-07-21).




