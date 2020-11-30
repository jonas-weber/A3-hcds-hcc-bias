# A3-hcds-hcc-bias

## Goal of the project
Collecting the amount and quality of articles of politicians from different countries and calculating the articles written per population, the quaity per population and other relations.

## Data acquisition
### Source
* [Wikipedia article names of politicians with countries](https://figshare.com/articles/Untitled_Item/5513449)
Published by Os Keyes under CC-BY-SA 4.0 license. 

* [Countries with population and region](https://www.prb.org/international/indicator/population/table/)
Published by Population Reference Bureau. No license found.

* [ORES endpoint doc](https://ores.wikimedia.org/v3/#!/scoring/get_v3_scores_context_revid_model), [About ORES](https://www.mediawiki.org/wiki/ORES)
Developed by Wikimedia Scoring Platform team. No license found.

## Description of data fields
* **page** - The name of the article
* **country** - The name of the country associated with the article
* **rev_id** - The article ID
* **prediction** - The predicted article quality by the ORES API. [Quality Range](https://www.mediawiki.org/wiki/ORES#Article_quality)
* **population** - The population of the country, given in millions (see *Considerations*)
* **region** - The region associated with the country
  
## Considerations
* The population data was preprocessed and contains errors in some countries using 'thousands' instead of 'millions'