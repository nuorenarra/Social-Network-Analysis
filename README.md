# Social-Network-Analysis
Methods for deriving life-span-overlap-corrected association indices from spatio-temporal co-occurrence data of wild animals. Suitable also for non-group-living animal species with a non-modula social organisation

c: Aura Raulo and Josh Firth 2021

SUMMARY
Many animal social network analyses are based on group-by-individual data, where social association is inferred from the frequency at which two individuals are observed in the same group/flock weighted by the sum of their observation records. This method has two caveats: a) it does not take in account differences in lifespan overlap between pairs and b) it is less suitable for non-group living semi-social species with less modular and more continuous social structure

Here we described a method for constructing association matrices from individual-wise spatio-temporal occurrence data (such as pit-tag station/logger data), using a life-span-overlap corrected social association index (corrected SRI, based on Firth & Sheldon 2016, Ecol. Letters) and an edge definition with user-definable intimacy threshold based on sliding time window criterion (= how close in time two individuals need to be observed in the same location to be considered "associated").

DATA
this method assumes you are working with occurrence data, perhaps a data frame with time-stamped observations of individual X in location Y as rows. The actual location does not need to be known, just the labels of unique locations/stations/loggers, unless you want to work with social patterns controlled for spatial distance effects later on. The example data here is wood mouse logger detection data from Raulo et al. 2021, ISMEJ.

References:

Firth, J. A., & Sheldon, B. C. (2016). Social carry‐over effects underpin trans‐seasonally linked structure in a wild bird population. Ecology letters, 19(11), 1324-1332.

Raulo, A., Allen, B. E., Troitsky, T., Husby, A., Firth, J. A., Coulson, T., & Knowles, S. C. (2021). Social networks strongly predict the gut microbiota of wild mice. The ISME journal, 1-13.
