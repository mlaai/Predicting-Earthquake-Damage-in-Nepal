# Predicting Earthquake Damage in Nepal
# Executive Summary 
This document presents an analysis of the damage to buildings in Nepal due to a 7.8 magnitude earthquake that hit the region in April of 2015. The analysis was based on 10000 observations of buildings with various attributes. Key characteristics of the buildings were presented in the data and relevant feature set was created for training a model to predict the outcome of the severity of the damage caused based on key characteristics of the buildings. 

After exploring the data by calculating summary and descriptive statistics, and by creating visualizations of the data, several potential relationships between building characteristics and damage grade were identified. After exploring the data, a predictive model to classify damage grade from its features was created. 

While many factors can help indicate the damage grade of a building, significant features found in this analysis were:

• geo_level_1_id, geo_level_2_id, geo_level_3_id geographic region in which building exists, from largest (level 1) to most specific sub-region (level 3). – buildings with less id values are most likely to get damaged than the buildings with greater id values 

• age (type: int): age of the building in years. – new buildings were mostly damaged than older ones 

• area (type: int): plinth area of the building in m2m2. – buildings with less area were more likely to be damaged than larger area 

• height (type: int): height of the building in mm.  

• has_superstructure_mud_mortar_stone (type: binary): flag variable that indicates if the superstructure was made of Mud Mortar - Stone. 

• has_superstructure_cement_mortar_brick (type: binary): flag variable that indicates if the superstructure was made of Cement Mortar - Brick. 

• has_secondary_use (type: binary): flag variable that indicates if the building was used for any secondary purpose. – buildings with secondary use are more likely to get damaged 

• has_secondary_use_agriculture (type: binary): flag variable that indicates if the building was used for agricultural purposes. – buildings used for agriculture are more likely to get damaged 

• has_superstructure_rc_non_engineered (type: binary): flag variable that indicates if the superstructure was made of nonengineered reinforced concrete. 

• has_superstructure_rc_engineered (type: binary): flag variable that indicates if the superstructure was made of engineered reinforced concrete. 

• plan_configuration (type: categorical): building plan configuration. Possible values: a779, 84cf, 8e3f, d2d9, 3fee, 6e81, 0448, 1442, cb88. – Plan configuration play a significant role in determining high risk buildings 

• foundation_type (type: categorical): type of foundation used while building. Possible values: 337f, 858b, 6c3e, 467b, bb5f. - Foundation types play a significant role in determining high risk buildings 

• ground_floor_type (type: categorical): type of the ground floor. Possible values: b1b4, b440, 467b, e26c, bb5f. Ground floor types play a significant role in determining high risk buildings 

• other_floor_type (type: categorical): type of constructions used in higher than the ground floors (except of roof). Possible values: f962, 9eb0, 441a, 67f9. – Other floor types play a significant role in determining high risk buildings 

• position (type: categorical): position of the building. Possible values: 3356, bfba, bcab, 1787. – Position plays a significant role in determining high risk buildings 
