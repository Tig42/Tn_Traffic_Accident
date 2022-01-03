
# Tn_Traffic_Accident
Motivation
Reducing traffic accidents, especially serious accidents, is nevertheless always an important challenge. The proactive approach, one of the two main approaches for dealing with traffic safety problems, focuses on preventing potential unsafe road conditions from occurring in the first place. For the effective implementation of this approach, accident prediction and severity prediction are critical. If we can identify the patterns of how these serious accidents happen and the key factors.
Objectives
The objective of this project is to recognize key factors affecting the accident severity
Process
Data cleaning was first performed to detect and handle corrupt or missing records. EDA (Exploratory Data Analysis) and feature engineering were then done over most features. Finally, Logistic regression, Random Forest Classifier, and EasyEnsemble were used to develop the predictive model.
Traffic Attributes
ID: This is a unique identifier of the accident record.
Source: Indicates source of the accident report (i.e. the API which reported the accident.).
TMC: A traffic accident may have a Traffic Message Channel (TMC) code which provides more detailed description of the event.
Severity: Shows the severity of the accident, a number between 1 and 4, where 1 indicates the least impact on traffic (i.e., short delay as a result of the accident) and 4 indicates a significant impact on traffic (i.e., long delay).
Start_Time: Shows start time of the accident in local time zone.
End_Time: Shows end time of the accident in local time zone.
Start_Lat: Shows latitude in GPS coordinate of the start point.
Start_Lng: Shows longitude in GPS coordinate of the start point.
End_Lat: Shows latitude in GPS coordinate of the end point.
End_Lng: Shows longitude in GPS coordinate of the end point.
Distance(mi): The length of the road extent affected by the accident.
Description: Shows natural language description of the accident.
Address Attributes:
Number: Shows the street number in address field.
Street: Shows the street name in address field.
Side: Shows the relative side of the street (Right/Left) in address field.
City: Shows the city in address field.
County: Shows the county in address field.
State: Shows the state in address field.
Zipcode: Shows the zipcode in address field.
Country: Shows the country in address field.
Timezone: Shows timezone based on the location of the accident (eastern, central, etc.).
Weather Attributes (11):
Airport_Code: Denotes an airport-based weather station which is the closest one to location of the accident.
Weather_Timestamp: Shows the time-stamp of weather observation record (in local time).
Temperature(F): Shows the temperature (in Fahrenheit).
Wind_Chill(F): Shows the wind chill (in Fahrenheit).
Humidity(%): Shows the humidity (in percentage).
Pressure(in): Shows the air pressure (in inches).
Visibility(mi): Shows visibility (in miles).
Wind_Direction: Shows wind direction.
Wind_Speed(mph): Shows wind speed (in miles per hour).
Precipitation(in): Shows precipitation amount in inches, if there is any.
Weather_Condition: Shows the weather condition (rain, snow, thunderstorm, fog, etc.).
POI Attributes:
Amenity: A Point-Of-Interest (POI) annotation which indicates presence of amenity in a nearby location.
Bump: A POI annotation which indicates presence of speed bump or hump in a nearby location.
Crossing: A POI annotation which indicates presence of crossing in a nearby location.
Give_Way: A POI annotation which indicates presence of give_way sign in a nearby location.
Junction: A POI annotation which indicates presence of junction in a nearby location.
No_Exit: A POI annotation which indicates presence of no_exit sign in a nearby location.
Railway: A POI annotation which indicates presence of railway in a nearby location.
Roundabout: A POI annotation which indicates presence of roundabout in a nearby location.
Station: A POI annotation which indicates presence of station (bus, train, etc.) in a nearby location.
Stop: A POI annotation which indicates presence of stop sign in a nearby location.
Traffic_Calming: A POI annotation which indicates presence of traffic_calming means in a nearby location.
Traffic_Signal: A POI annotation which indicates presence of traffic_signal in a nearby location.
Turning_Loop: A POI annotation which indicates presence of turning_loop in a nearby location.
Period-of-Day:
Sunrise_Sunset: Shows the period of day (i.e. day or night) based on sunrise/sunset.
Civil_Twilight: Shows the period of day(i.e. day or night) based on civil twilight.
Nautical_Twilight: Shows the period of day (i.e. day or night) based on nautical twilight.
Astronomical_Twilight: Shows the period of day (i.e. day or night) based on astronomical twilight.

Contents
Exploratory Data Analysis
Q1: Where do most accidents happen?
      1.1 Accident visualization: accident severity distribution for each City
      1.2 Top Cities Accident Rate Per 100,000 population
      1.3 Accident visualization: accident map
Q 2: When do most accidents happen?
       2.1 Accident visualization : time series analysis
      2.2 Daytime versus nighttime
      2.3 Weekday versus weekend
Q3: With what weather condition do most accidents happen?
        3.1    Top weather conditions with accidents  
Q5 What relates to accident severity?   
Q6 what is the conclusion from the analysis of datasets?


Source
 https://cdan.dot.gov/query 
