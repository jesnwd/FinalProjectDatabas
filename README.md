# FinalProjectDatabas
final project for database 3380

#Team Members:
Jordan Sebacher
Anjay Patel (not in class)

#Application
The application allows skiers/snowboarders to signup and pick their favorite resorts from 100 ski resorts in the USA, and Canada.
The app gives information on both the mountain (peak elevation, vertical, skiable acreage), as well as weather information (chance of snow, temperature, sunrise, sunset, etc).

#schema
The database consists of 4 tables:
###SkiResortInfo
This table hold information on each ski resort the fields are:
RESORT - datatype = varchar(30) holds the name of each resort
ID - datatype = int(11). The Primary key, a unique int associated with each resort.
LOCATION - datatype = varchar(25). The state/province the resort is located in.
PEAK - datatype = int(11). The peak elevation of the resort in feet.
BASE - datatyoe = int(11). The base elevation of the resort in feet.
VERTICAL - datatype = int(11). The vertical drop in feet of the resort.
ACREAGE - datatype = int(11). The skiable acreage of the resort.
TRAILS - datatype = int(11). The number of trails in the resort.
LIFTS - datatype = int(11). The number of lifts at the resort.
SNOWFALL - datatype = int(11). The average annual snowfall in inches.
ZIPCODE - datatype = varchar(7). The zipcode of the resort used to locate the proper weather data through the API. varchar used because canadian sip codes have letters.
LOGO - datatype = varchar(50). holds the file path to the resorts coorsponding logo in the java App
##SkiWeather
Collected from worldweatheronline.com api
ID - datatype = int(11). the resort id
SUNRISE - datatype = varchar(20). The time of sunrise in HH:MM AM/PM format
SUNSET - datatype = varchar(20). the time of sunset in the same format
CHANCEOFSNOW - datatype = int(11). the % chance of snow for the day
FORECASTDATE - datatype = date. the date of the current forecast.
SNOWFALL - datatype = float. the expected snowfall for the day in inches
BOTTOMMAXTMP - datatype = int(11). The expected high at the mountain base.
BOTTOMMINTMP - datatype = int(11). the expected low at the mountain base
MIDMAXTMP - datatype = int(11). the expected high at mid mountain
MIDMINTMP - datatype = int(11). the expect low at mid mountain
TOPMAXTMP - datatype = int(11). the expected high at the summit
TOPMINTMP - datatype = int(11). the expected low at the summit
H0CHANCESNOW - datatype = int(11).the chance of snow at midnight
H0CHANCESUN - datatype = int(11). the chance of sun (no clouds) at midnight
H3CHANCESNOW - datatype = int(11).the chance of snow at 3:00AM 
H3CHANCESUN - datatype = int(11).the chance of sun at 3:00pm
H6CHANCESNOW - datatype = int(11).the chance of snow at 6:00AM
H6CHANCESUN - datatype = int(11).the chance of sun at 6:00pm
H9CHANCESNOW - datatype = int(11).the chance of snow at 9:00AM
H9CHANCESUN - datatype = int(11).the chance of sun at 9:00pm
H12CHANCESNOW - datatype = int(11).the chance of snow at 12:00PM
H12CHANCESUN - datatype = int(11).the chance of sun at 12:00pm
H15CHANCESNOW - datatype = int(11).the chance of snow at 3:00pm
H15CHANCESUN - datatype = int(11).the chance of sun at 3:00pm
H18CHANCESNOW - datatype = int(11).the chance of snow at 6:00pm
H18CHANCESUN - datatype = int(11).the chance of sun at 6:00pm
H21CHANCESNOW - datatype = int(11).the chance of snow at 9:00PM
H21CHANCESUN - datatype = int(11).the chance of sun at 9:00pm
##UserFavorites
app uploads user selected favorites and user id here
USERID - datatype = int(11)
RESORTID -datatype = int(11)
##UserInfo
ID - int(11) auto increments as users are added holds unique user id
USERNAME - varchar(45)
PASSWORD - varchar(45). holds hashed user password

#Video of application
https://youtu.be/KQZuJch3p14

#ERD

