#
This repository matches Indian pincodes to various other relevant attributes. e.g. censuscodes from census 2011 down t0 village level. Also lat, long data. This is only one component of creating a comprehensive system of crossmatching codes for various geographical and administrative units. A lot of this work is incomplete.

According to the data available at data.gov.in, there are approximately 154,000 available pincodes linked post offices.

This main data - a master file of sorts for pin codes, is in postofficeswithpins.csv

This data is then split into different components as follows : 

This site, from the governments PMJDY project, has geolocations of post offices among other POIs. http://pmjdy.gov.in/g-i-s.aspx
There are approximately 142,000 post offices with pincodes and geocodes given in this data.
Data for post offices from this site, matched to the pincodes from the 'master' file above, are pincodes_lat_lon.txt. This file contains pins vs geocodes data for 135,000 locations.
Data that could not be matched to pincodes as yet, roughly 7k-8k locations are in the 'lat_lng_unjoined' file. (These two files put together comprise all the data from the PMJDY page referred to above)

pincodes_censuscodes.zip: 
The district handbooks released by census provide pincode details for village areas. For each village / location code, they provide the relevant pincode which covers that village. This file collates that data.
Unfortunately, the district handbooks only provide such pincode data for villages, not towns or wards. And even within villages, a number of locations dont have the relevant pincode info (a large part of Madhya Pradesh is blank for instance). Another bunch of villages have pincodes in less than 6 digits. Despite these issues however, there are still 413,000 villages out of a total of 640,000 for whom six digit pincodes are given.
the handbooks are here:
http://www.censusindia.gov.in/2011census/dchb/DCHB.html
(For the sake of completeness, i have not removed entries for those villages for which pincodes are not given)

