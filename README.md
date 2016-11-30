# Data-Science-Final-Project--NIST

## NIST Eval: Data & Exploratory

### Part I: Data Overview
#### 1.  detector_lane_inventory.csv:
* lane_id: uniquely identify a detector (totally 2,139).
* zone_id: identifier of a zone in a road (around 1,000).
* road: on which road, e.g. I-66.
* location_description: e.g. I-66 NEAR Sudley Rd @ MM 49.02
* Geographical coordinate: (latitude, longitude)  

There are 11 other less important fields.

#### 2.  events_train.csv:
* event_id: uniquely identify an event, e.g. “MDOT_CHART_4aff02b300110095003f0be8b3035daa”
* event_description: a text description about an event, e.g. “Disabled Vehicle Event @ I-495 AT MD 187”
* Timestamps: times the event was created, confirmed, and closed (some are missing).
* event_type: the type of an event, e.g. “accidentsAndIncidents”.
* geographical location: (latitude, longitude)

There are 9 other less important fields.

#### 3.  lane_measurement/*.tsv:
* trial_id:
* lane_id: identifier of a detector that this record is collected from.
* measurement_start: timestamp when measurement starts, e.g. 2007-04-09 14:04:12-04
* flow: measured average flow of the last interval, e.g. 13.
* speed: measured average speed (mph) of the last interval, e.g. 70.
* occupancy: measured occupancy of the last interval, e.g. 7.





### Part II: Final Project Tasks Preview
#### Cleaning Task
* clean traffic lane detector measurements containing incorrect flow values, providing correct traffic flow values for the erroneous traffic flow measurements.  

#### Alignment Task
* analyze video from camera feeds to detect an event and match it to a separate inventory of traffic events (disabled car, accidents, etc).  

#### Prediction Task
* develop a system that can predict the number and types of traffic events by type for a given (geographical bounding, interval of time) pair.  

#### Forecasting Task
* leverage past traffic information and current conditions (weather, maps) to forecast vehicle flows on major roads.  

*We only participate in task #1 and #3.
