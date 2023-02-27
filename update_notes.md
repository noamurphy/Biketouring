## Update notes

Commit 3: city_bikes.ipynb
- Added time.sleep(1) under each API call to avoid data loss while response is being gathered
- Integrated getNetworks_df() into getNetwork_id to reduce redundancy
- Standardized delay after calls into new constant CALL_DELAY

Commit 5: yelp_foursquare_EDA.ipynb
- changes to reduce calls made to foursquare API:
    - getPOIDetails_FSQR() function has been assimilated into getPOIs_FSQR()
    - adjusted call to provide 'rating' and 'stats'
- Added manual insertion of params into url
- Added call delay
- Changed API_KEY to FOURSQUARE_API_KEY for clarity
- Removed popularity and total_stats from Foursquare results

Commit 6: yelp_foursquare_EDA.ipynb
- Completed framework for interfacing with Yelp API
- Added API columns to tag the originating API

Commit 7: city_bikes.ipynb, yelp_foursquare_EDA.ipynb
- Ingested name and unique id for each bike station into to the pipeline at the city_bikes notebook
- adjusted yelp_foursquare_EDA notebook to process station names and identifiers