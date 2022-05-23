# [E&E News investigation into FEMA elevation grants](https://www.politico.com/)

To assess how FEMA elevation grants have been distributed nationwide, E&E News analyzed the 18 states that have received at least $5 million from FEMA to elevate homes and calculated the funding that went to individual communities within those states.

The racial and ethnic composition and income level of the communities were recorded using the Census Bureau's American Community Survey figures for 2019, the most recent year for which FEMA elevation spending figures are publicly available.

E&E News then calculated how much elevation money in each state has gone to communities that are overwhelmingly white or wealthy. E&E News defined overwhelmingly white as communities where more than 90 percent of the population was non-Hispanic white, and wealthy communities as those that had a median household income of more than $100,000.

Throughout the story, “community” refers to either a municipality or a distinct part of a municipality that the Census Bureau recognizes and collects data on (known as a census-designated place).

`FEMA_elevation_data.csv` contains the dataset used for this story. The dataset includes analysis of 12 states where more than half of the FEMA residential elevation grant money went to communities that met the wealthy-or-white criteria:

* Connecticut
* Florida
* Georgia
* Kentucky
* Massachusetts
* New Jersey
* New York
* Ohio
* Oregon
* Pennsylvania
* Washington
* West Virginia

### Data dictionary


`State`: State of grant recipient

`Project ID`: FEMA project ID

`Project title`: FEMA project title, given by local officials in applications to FEMA (This data is no longer available in FEMA's project database. This was archived by E&E News, and individual project addresses were removed to protect privacy.)

`Subgrantee`: Government recipient of the elevation funds

`Community`: Municipality or census designated place where funds were spent

`Rich/white`: A flag indicating if the community was 90%+ non-Hispanic white or had a median household income over $100,000 in the 2019 American Community Survey

`FEMA $`: Amount FEMA spent on residential elevations on the project in the community*

`FEMA share`: Percent of total project cost paid by FEMA

`Elevated homes`: Number of residential properties that received elevation funding. In some projects, the number of elevated properties is 0. That could occur for several reasons, according to FEMA. The project could be incomplete. The project could be complete but no homes were elevated because a homeowner withdrew or homes were found to be unsuitable for elevation. The number 0 could also be erroneous.

`Multi-purpose`: A flag indicating if the project was used for other actions in addition to elevation (i.e. acquisition/demolition of flood-prone homes)

`Multi-community`: A flag indicating if the project funded actions in mutliple communities. In this case, there are multiple rows for the project — one for each community.

`Multi-elevation`: A flag indicating if the project includes elevation actions involving residential as well as non-residential properties. In these cases, the `FEMA $` column shows the total amount of project elevation money in the community, multipled by the percent of elevated properties that were residential 

_*When a project involved both elevating homes and acquiring homes, E&E News calculated the number of homes that were elevated and the number of homes that were acquired and divided the FEMA spending proportionately. In these cases, E&E News also weighted the spending to reflect that acquiring a home typically costs more than elevating a home. E&E News based its weighting on a Government Accountability Office finding in 2020 that FEMA spent an average of $136,000 on each home it acquired and $107,000 on each home it elevated._

### Data sources

[FEMA project data](https://www.fema.gov/openfema-data-page/hazard-mitigation-assistance-projects-v2)

[FEMA properties data](https://www.fema.gov/openfema-data-page/hazard-mitigation-assistance-mitigated-properties-v2)
