# Smart-Water-Management-System
SMART WATER MANAGEMENT SYSTEM PROPOSAL

i
ACKNOWLEDGEMENT

First and foremost, We praise and thank God, the Almighty, for His showers of blessings throughout our research work to complete the research successfully.
We would like to express our deep and sincere gratitude to our research supervisor Rahul Naidu sir, Ram sir, Dilip sir, Anupam sir, for giving us the opportunity to do research and providing valuable guidance throughout this research. Their dynamism, vision, sincerity and motivation have deeply inspired us. They have taught us the methodology to carry out the research and to present the research works as clearly as possible. It was a great privilege and honor to work and study under their guidance. We are extremely grateful for what they have offered us. We would also like to thank them for their friendship, empathy, and great sense of humor during the discussion we had with them on research work and thesis preparation.
We would like to say thanks to Dilip sir and Anupam sir for their constant encouragement and express our special thanks for their genuine support throughout this research work.
Finally, our thanks go to our parents and colleagues who have supported us to complete the research work directly or indirectly.












ii
TABLE OF CONTENTS

MEMORANDUM OF UNDERSTANDING (MOU)	1-2
INTRODUCTION TO PROBLEM STATEMENTS	3-9
Abstract	3
Need for Smart Water Management System	3
Problem Statements	3
Solutions	4-5
Working of smart water management system	6
Sensors used	7-9
SYSTEM ARCHITECTURE DEVELOPMENT	10-12
Complete Architecture of Society	10
Building View Architecture	11
Network Architecture	12
BUDGETING AND PROPOSAL OF PROJECT	13-22
Devices Price Comparison	13-16
Hardware Cost (Package distribution)	17-21
Primary Package	17
Simple Package	18
Basic Package	18
Regular Package	19
Premium Package	20
Luxury Package	21
Total Project Cost	22
CONCLUSION	23
REFERENCES	24
iii
LIST OF FIGURES
Fig. 1.1 Workflow of water pump automation								       6
Fig. 1.2 Overflow and leakage detection workflow								       6
Fig. 2.1 Complete architecture of society									     10
Fig. 2.2 Building View Architecture										     11
Fig  2.3 Network architecture											     12
LIST OF TABLES
Table 3.1     Flow sensor price comparison									     13
Table 3.2     Turbidity sensor price comparison								     13
Table 3.3     pH sensor price comparison	     								     14
Table 3.4     Relay module price comparison									     14
Table 3.5     Ultrasonic sensor price comparison								     15
Table 3.6     ESP price comparison										     15
Table 3.7     Data usage											     16
Table 3.8     Power consumption										     16
Table 3.9     Primary Package											     17
Table 3.10   Simple Package											     17
Table 3.11   Basic Package											     18
Table 3.12   Regular Package											     19
Table 3.13   Premium Package										     20
Table 3.14   Luxury Package											     21
Table 3.15   Total Project Cost										     22






iv
MEMORANDUM OF UNDERSTANDING (MOU)

Dear dcs faculty,
	As per the series of discussions we have had till date regarding your workflow automation requirement, the following are the major action points and deliverables.
Workflow:

Salient features:
Water pumps respond automatically.
Leakage detection in pipes.
Water wastage detection.
Water consumption analysis.
Automatic water billing system.
Assurance of good quality water.
Visualization on mobile app.
Reuse of overflow water.
Milestones:
1
25% Advance with PO - Day ‘0’
25% After 40% installation - Day ‘8’
25% After 75% installation - Day ‘14’
25% After complete installation - Day ‘20’
Commercial:  
I. The Contract/Licence fee is Rs 1,500/- (One-time Charge). 
ii. All prices with GST exclusive. 
iii. Payment schedule as follows:
a. Advance with PO - Rs 9,250/- 
b. First milestone (40% installation completion) – Rs. 9,250/- 
c. Second milestone (75% installation completion) – Rs 9,250/- 
d. Third milestone (complete installation) – Rs 9,250/- 
iv. All costs towards 3rd party service providers like Hosting, SMS gateway, IVRS, etc will be at actuals and payable directly to the respective vendor. We can render advice on various options, however we are willing to work with any vendor of your choice
v. 6 months support/maintenance free from the date the third milestone goes live.
vi. Subsequent support/AMC charges will be Rs 1500/- per month
vii. All data ownership will vest with you. Our access will be limited to the technical support required by you during the period of active AMC.
viii. This contract will be governed by standard NDA practices.
Company info: 
Name
XYZ
GST no.
XXXXXXXXXXXXXX
Bank details
HDFC Bank A/c no. – IFSC Code

We now look forward to receiving your confirmation along with the work order. 
Warm Regards,
G-1, sec-5													      
2
Chapter - 1
INTRODUCTION TO PROBLEM STATEMENTS
Abstract 
This paper presents an IoT device which helps to manage and plan the usage of water. This system can be easily installed and maintained for a long run. The Waterproof Ultrasonic sensor is placed on the tank which continuously monitors the water level in real time. This information will be updated in the cloud and users can analyze the amount of water. According to the level of water in the tank, the motor functioning is automatically controlled. When the water level falls below the threshold level the motor will be again turned on automatically.
Need for Smart Water Management System 
This system is needed to reduce wastage, detect leakage and quality of water, analyze water consumption, and make the whole process automatic and managed centrally and effectively.
Problem Statements
Measure the water level in water tanks in each building.
Making water pumps to respond automatically.                  
Detection of water level in a storage tank.
Detecting contamination of water coming from a storage tank.
Detecting water leakage.
Analyzing water consumption.         
Detecting and handling wastage of water.
Detecting and utilizing overflow water.   
Visualization and control of the complete system in one place.
Designing proper interconnectivity.
Solutions
Measure the water level in water tanks
													     3
To make the water pumps respond automatically, we have to first detect the water level in the tank by using a water level detection sensor. We will also check for no. of peoples present in the building and predicting usage depending on earlier consumptions to fill water tanks, so that if less water will be needed for that building then instead of filling that tank we will use that water for other buildings.
Making water pumps to respond automatically
          When the water level will be less than a certain height then a signal will be sent to the water pumps to be turned off using a relay module. Then before turning the water pump on, it sends a signal to the water level detection sensor fitted in the storage tank to check the water level status of that tank.
Detection of water level in storage tank
          If the storage tank has sufficient water to supply then on receiving signal back the motor will be turned on, otherwise, it will generate an alert to fill up the storage tank first, after filling the storage tank, it will supply water to the building tanks. 
Detecting contamination of water coming from a storage tank
At the outlet of the storage tank from where the water is to be supplied to consumers, a water quality detection sensor will be fitted. To detect the quality of water to be supplied, if that water quality will be too poor then it sends an alert and will not supply water to the buildings. i.e. deny the permission to turn off water pumps until the quality of water will not be improved. If anyhow, the water present in the building tanks gets contaminated then also it sends an alert for that building.
Detecting water leakage
To detect water leakages in pipes, we can add a water flow sensor to detect the rate and amount of water incoming and outgoing in a pipe at its inlet and outlet respectively, for every pipe, then if the amount of water exiting the pipe is less than at inlet, possibly it will be a water leakage and sends an alert for water leakage in that pipe.
Analyzing water consumption
We have used sensors to detect the amount of water at the outlet of each pipe. so, using the data from flow rate sensors at outlets of pipes providing water to individual flats i.e. sensors in the main pipeline of each flat, we can get the total consumption of water per day per flat of each building on our server database.
4
Detecting and Handling Wastage of Water
While detecting the water leakage in pipes, if any leakage is found then the difference in the amount of water at the inlet and outlet will be considered as wastage and handled with the leakage alert. While analyzing the consumption of water in each flat, we also take data of members in the flat daily to analyze the average consumption according to the no. of members. So, if there will be a vast increase in consumption of water having the same no. of members as in the previous data, then it is considered as wastage and a message will be sent to the owner to check for any wastage in that building.
Detecting and utilizing overflow water from the tank
If while filling a water tank, any of the sensor used for automatic turn on/off water pump got failed or damaged then the water might flow out through the tank and will be wasted, so for this, we have to connect the pipe through which the water is overflowing to the storage tank to utilize that water and when the water flow through that pipe then a sensor damage alert will be sent to the server.
Visualization and control of the complete system at one place
For visualizing data in one place, we will send data to cloud storage from sensors in realtime and then the data is analyzed and data usage will be displayed per flat on a daily basis as well as on a monthly and weekly basis. The alert for water leakage and wastage will  be notified as the notification on the app provided to the customer.  Status of all motors will be shown on the app. Water level in all tanks including storage tanks will be visualized. The app will show the whole water management status to the secretary of the society, but the society members will have the data of only their own flats on the app based on the id provided to the users. 
Designing proper interconnectivity
For proper connectivity, all sensors inside a building are connected using ESP12F i.e. using WiFi for proper data transfer without loss to the ESP at storage tank separately. All ESPs except one at storage tank will work as station point (WiFi) mode and ESP at storage tank will work as Access Point(hotspot) mode for proper ESP to ESP direct connection using Antenna at storage tank ESP.  Then the required data is transferred to the cloud through that access point ESP at the storage tank.


5
Working of smart water management system

Fig. 1.1 Workflow of water pump automation

Fig. 1.2 Overflow and leakage detection workflow
6
Sensors used
Waterproof Ultrasonic distance Sensor (JSN-SR04T)
Use:  This sensor will be used to detect the level of water in tanks.
Unit Price:  INR 312
Average Lifetime:  6 months.
Link:https://www.alibaba.com/product-detail/Waterproof-Ultrasonic-sensor-Module-JSN-SR04T_60664900606.html?spm=a2700.galleryofferlist.0.0.188b6513V5qmsL
Analog PH Sensor (RKI-2237)
Use:  This sensor will be used to detect the pH of water present in the storage tank.
Unit Price:  INR 550.
Average Lifetime:  1-1.5 years.
Link: https://www.indiamart.com/proddetail/universal-ph-electrode-20212202433.html
Turbidity Sensor (TS-300B)
Use:  This sensor will be used to measure the turbidity level of water present in the storage tank.
Unit Price:  INR 100.
Average Lifetime:  1 year.
Link:https://ruizeinc.en.alibaba.com/product/62030210497-810213828/TS_300B_High_Quality_Turbidity_Sensor_Detection_Module_Water_Quality_Test_Washing_Machine_Turbidity_Transducer_for.html
Water Flow Sensor (YF-S201)
Use:  This sensor will be used to check for proper supply of water, analyzing water consumption, and to detect leakage in pipes.
Unit Price:  INR 190.
Average Lifetime:  3 months.
Link:https://www.indiamart.com/proddetail/super-debug-yf-s201-water-flow-measurement-sensor-22008021230.html
7
Relay Module (KY-019)
Use:  This module will be used to switch on/off our water motors in each building.
Unit Price:  INR 25.
Average Lifetime:  3 months.
Link:https://www.alibaba.com/product-detail/Explosive-sales-JQC-3FF-S-Z_62327391124.html?spm=a2700.galleryofferlist.0.0.6e5d21d8hiGuOx&bypass=true
ESP8266 (ESP12F)
Use:  This module will be used for controlling all sensors used and sending data to the firebase.
Unit Price:  INR 85.
Average Lifetime:  2 years.
Link:https://www.alibaba.com/product-detail/ESP12-F-ESP12F-ESP12-F-ESP_60611209447.html?spm=a2700.galleryofferlist.0.0.5c6e1660w6pgcq
Battery
Use:  This module will be used to supply power to sensors and charged by the solar panels.
Unit Price:  INR 600.
Average Lifetime:  2 years.
Link:https://www.alibaba.com/product-detail/Factory-direct-supply-lithium-battery-for_60839675076.html?spm=a2700.galleryofferlist.0.0.2ece73f3a9p58w
Battery Charger
Use: This module will be used to charge batteries.
Unit Price: INR 100.
Average Lifetime: 2 years.
Link:https://www.alibaba.com/product-detail/18650-lithium-battery-8-4v-1a_62234887318.html?spm=a2700.galleryofferlist.0.0.70266789X2jqD3
Solar Panel
Use: Solar panels will be used for power supply to the sensors through batteries.
8
Price: INR 217/Watt.
Average Lifetime: 20-30 years.
Link:https://news.energysage.com/how-much-does-the-average-solar-panel-installation-cost-in-the-u-s/
Antenna
Use: Antenna is used to increase the range of ESP12F to get proper connectivity between ESPs.
Unit Price: INR 100.
Average Lifetime:  6 months.
Link:https://www.alibaba.com/product-detail/4g-lte-external-antenna-screw-mount_62263015584.html?spm=a2700.galleryofferlist.0.0.2231605fXr0lj5




















9
Chapter - 2
SYSTEM ARCHITECTURE DEVELOPMENT
Complete Architecture of Society

Fig. 2.1 Complete architecture of society

In Fig. 2.1, we provide a brief view of our complete network (about how our smart water management system communication works).
Assuming 5 floored 8 building system, each building has 1 relay module near the water pump to switch motor each with one ESP, an ultrasonic sensor in building tank to detect water level, a flow sensor at the inlet of overflow pipe to detect overflow water for any possible sensor damage, a flow sensor at outlet of building tank and 1 flow sensor at each flat’s main pipeline to analyze water consumption of each flat and to detect leakage in pipes. 
We have a ph sensor, turbidity sensor, and ultrasonic sensor at storage tank connected through wired connection with a single esp having antenna attached to it and internet access for proper communication with firebase cloud server.

10
Building View Architecture

Fig. 2.2 Building View Architecture

Fig 2.2 shows how our flow sensors, relay, and other sensors will be connected in each building and their position. Flow sensors at inlet of overflow pipe and pipe supplying water to each flat and the ultrasonic sensor in the building tank, these three sensors will be connected with a single ESP. The other flow sensors at each flat and relay module all will be connected with seperate ESP’s. All sensors in a building will be connected with a li-ion rechargeable battery which will be charged through the solar panels installed in each building via a battery charger. If the water level in building tanks is less than a required level then it sends that 
data to access point ESP and to switch on the motor, then that ESP will check for the data from pH , turbidity, and ultrasonic sensor, if water is enough and clean for supply then it sends data to relay to turn on the motor. Similarly, in  case of completely filling the building tank, Station point ESP will send data to access point ESP and then it turns off the motor through relay.






11
Network Architecture 

Fig 2.3: Network architecture

In network architecture as shown in Fig 2.3 above, all of the sensors and modules are connected with ESP’s through wired medium and respond to them. Each of that ESP will interface that sensor and transfer data from the sensor to the ESP at the storage tank and vice versa for actuators i.e. relays. All ESPs except one at storage tank will work as station point (WiFi) mode and ESP at storage tank will work as Access Point (hotspot) mode for proper ESP to ESP direct connection using Antenna at storage tank ESP. That access point ESP has internet access and will send data to the firebase cloud server and then data will be analyzed and visualized on the application provided to all members of society. 







12
Chapter - 3
BUDGETING AND PROPOSAL OF PROJECT
Devices Price Comparison
S. No.
Model
Company/Seller
Price
Specifications
1.
YF-S201
Robokits
Rs.448
Working Voltage: 5-18v DC
Working Flow rate: 1-30 L/min.
Max. Current : 15mA
2.
YF-S201
Robokart_26(amazon)
Rs.737
3.
YF-S201
Indiamart
Rs.190
4.
YF-S201
Alibaba
Rs.196
Best Price :
Rs.190
Table 3.1: Flow sensor price comparison

S. No.
Model
Company/Seller
Price
Specifications
1.
TS-300B
Banggood
Rs.395
Analog Output
Output Voltage:0-5V
Response time<500ms
2.
TS-300B
Robokits
Rs.392
3.
TS-300B
Indiamart
Rs.1484
4.
TS-300B
Alibaba
Rs.100
Best Price :
Rs.100
Table 3.2: Turbidity sensor price comparison
13

S. No.
Model
Company/Seller
Price
Specifications
1.
pH sensor with BNC connector
Analab scientific  instruments  private limited.
INR 633
Temp.:0-70 deg C
Dimension:120mm long
connection:BNC type
2.
Labman PE-4
Double junction ph electrode
Spectrum technology
INR 700
Temp.:0-70 deg C
Pressure:0-87 PSI
connection:BNC type
3.
RKI-2237
indiamart
INR 550
Temp.:0-60 deg C
Response time <=1 min
connection:BNC type
Best Price :                   
INR 550
Table 3.3: pH sensor price comparison

S. No.
Model
Company/Seller
Price
Specifications
1.
KY-019
Indiamart
Rs.75
operating voltage: 5v
Max current: 20mA
Relay contact current capacity: 250V/10A 
2.
KY-019
Electronicscomp.com
Rs.85
3.
KY-019
Robu.in
Rs.99
4.
KY-019
alibaba.com
Rs.26
Best Price :
Rs.26
Table 3.4: Relay module price comparison

14
S. No.
Model
Company/Seller
Price
Specifications
1.
RKI-1055
Banggood
Rs. 575
Range:0.25-5m
2.
JSN-SR04T
alibaba
Rs. 312.13
Range:0.2~8m, Voltage:5v+_ 0.1v, Data Interface:UART/I2C
3.
RKI-1055
ROBOKITS INDIA
Rs. 1152
voltage:DC 5v, Current:40mA, Range:6m, Temp:-10*~70*
Best Price :
RS.312.13
Table 3.5: Ultrasonic sensor price comparison

S. No.
Model
Company/Seller
Price
Specifications
1.
ESP12E
Electronicscomp.com
Rs.150
 single core; Integrated TCP/IP protocol stack;Operating voltage : 3.0v~3.6v
2.
ESP12F
alibaba.com
Rs.85.27
Optimized antenna + all features of ESP12E
3.
ESP32- D0WDQ6
robu.in
Rs.189
Dual  core, 2.4GHz, supports bluetooth 4.2 & bluetooth low energy, 
4.
ESP32- WROOM-32
robokits.co.in
Rs.531
Bluetooth, WiFi  Transceiver Module 2.4GHz ~ 2.5GHz  Surface Mount
Best Price :
Rs.85.27
Table 3.6: ESP price comparison
15
S. No.
Data 
Per day(Bytes)
Per month(Bytes)
1.
Level of tanks
3110400 
93312000
2.
Relay (Motor Status)
86400 
259200
3.
Ph Sensor data
345600  
10368000
4.
Turbidity Sensor data
345600
10368000
5.
Flow sensor data
19353600
580608000
Total
23241600(0.02324 GB)
697248000(0.69 GB)
Table 3.7: Data usage
Note : - Here data size calculated from the data packets size (base is the size of datatypes). Assuming that all sensors send data continuously.
S.No.
Device Name
Power Consumption 
Per building consumption 
Consumption at storage tank
Total
1.
Relay
450mW
450mW
--
3,600mW
2.
Ultrasonic Level Sensor 
44mW
44mW
44mW
88mW
3.
Flow sensor
75mW
525mW
--
4,200mW
4.
pH sensor 
500mW
--
500mW
500 mW
5.
Turbidity Sensor
200mW
--
200mW
200mW
6.
ESP12F
231mW
1,617mW
231mW
12,936mW
Total


2,636mW 
975mW
3W*8+1W = 25W
Table 3.8: Power consumption
Approximate power consumption is 3W per building and 1W at storage tank.
16
Hardware Cost (Package distribution)
Why Packages?
We have Made some packages based on customer requirements, because different customers want   different features or have different requirements and budgets.
Primary Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price
Total Price
Resources
Lifespan 
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
RS.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months
3.
ESP8266
ESP12F
17
Rs.85.26
Rs.1,450
alibaba.com
1.9 years
Total
Rs.4,466
Table 3.9: Primary Package
Features:
Automatic Water level detection.
Automatic water tank filling.
Simple Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price
Total Price
Resources
Lifespan 
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
RS.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months

17
3.
Ph Sensor
RKI-2237
1
Rs.550
Rs.550
indiamart.com
1 year
4.
Turbidity Sensor
TS-300B
1
Rs.100
Rs.100
alibaba.com
1 year
5.
Flow Sensor
YF-S201
8
Rs.190
Rs.1,520
indiamart.com
3 months
6.
ESP8266
ESP12F
17
Rs.85.26
Rs.1,450
alibaba.com
1.9 years
Total
Rs.6,636
Table 3.10: Simple Package
Features:
Water level detection.
Water quality check.
Consumption analysis per building
Basic Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price
Total Price
Resources
Lifespan 
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
Rs.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months
3.
Ph Sensor
RKI-2237
1
Rs.550
Rs.550
indiamart.com
1 year
4.
Turbidity Sensor
TS-300B
1
Rs.100
Rs.100
alibaba.com
1 year
5.
Flow Sensor
YF-S201
48
Rs.190
Rs.9,120
indiamart.com
3 months
6.
ESP8266
ESP12F
57
Rs.85.26
Rs.4,860
alibaba.com
1.9 years
Total
Rs.17,646
Table 3.11: Basic Package
Features:
18
Water level detection.
Water quality check.
Consumption analysis per flat(Easy Billing System).
Leakage Detection.
 Regular Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price 
Total Price
Resources
Lifespan 
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
Rs.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months
3.
Ph Sensor
RKI-2237
1
Rs.550
Rs.550
indiamart.com
1 year
4.
Turbidity Sensor
TS-300B
1
Rs.100
Rs.100
alibaba.com
1 year
5.
Flow Sensor
YF-S201
56
Rs.190
Rs.10,640
indiamart.com
3 months
6.
ESP8266
ESP12F
57
Rs.85.26
Rs.4,860
alibaba.com
1.9 years
Total
Rs.19,166
Table 3.12: Regular Package
Features:
Water level detection.
Water quality check.
Consumption analysis per flat.
Leakage Detection.
Sensor damage detection.(Overflow Detection)



19
Premium Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price
Total Price
Resources
Lifespan 
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
Rs.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months
3.
Ph Sensor
RKI-2237
1
Rs.550
Rs.550
indiamart.com
1 year
4.
Turbidity Sensor
TS-300B
1
Rs.100
Rs.100
alibaba.com
1 year
5.
Flow Sensor
YF-S201
56
Rs.190
Rs.10,640
indiamart.com
3 months
6.
ESP8266
ESP12F
57
Rs.85.26
Rs.4,860
alibaba.com
1.9 years
7.
ESP12F Antenna
7 dbi 4g lte
1
Rs.100
Rs. 100
alibaba.com
6 months
Total
Rs. 19,266
Table 3.13: Premium Package
Features:
Water level detection.
Water quality check.
Consumption analysis per flat.
Leakage Detection.
Sensor damage detection.(Overflow Detection).
Internet connection only at storage tank.(No internet usage from society).


20
Luxury Package
S.no
Device Name
Device Model / Brand
Quantity
Unit Price 
Total Price
Resources
Lifespan
1.
Waterproof ultrasonic distance sensor
JSN-SR04T
9
Rs.312.13
RS.2,810
alibaba.com
3 months
2.
Relay 
KY-019
8
Rs.25.82
Rs.206
alibaba.com
3 months
3.
Ph Sensor
RKI-2237
1
Rs.550
Rs.550
indiamart.com
1 year
4.
Turbidity Sensor
TS-300B
1
Rs.100
Rs.100
alibaba.com
1 year
5.
Flow Sensor
YF-S201
56
Rs.190
Rs.10,640
indiamart.com
3 months
6.
ESP8266
ESP12F
57
Rs.85.26
Rs.4,860
alibaba.com
1.9 years
7.
ESP  Antenna
7 dbi 4g lte
1
Rs.100
Rs.100
alibaba.com
6 months
8.
Solar Panel
--
8(3W)+ 1(1W)
Rs. 217.5/W
Rs.5437
Price per watt
20-30 years
9.
Battery Charger
2500 mA dc power adapter
9
Rs. 100
Rs. 900
alibaba.com
4 years
10.
Battery
6.4v, 4.5ah li-ion
9
Rs.600
Rs. 5,400
alibaba.com
2 years
Total
Rs.31,000
Table 3.14: Luxury Package
Features:
Water level detection.
Water quality check.
Consumption analysis per flat.
Leakage detection.
Water wastage detection.
21
Sensor damage detection.(Overflow detection)
Internet connection only at storage tank.(No internet usage from society)
Power Supply from solar Panel using rechargeable batteries.
Total Project Cost
S.No.
Requirements
First time
Monthly
Yearly
Remarks
1.
Hardware Cost
Rs.31,000
--
--
One time cost
2.
Software Cost *
--
According to usage by users.
According to  usage by users.
--
3.
Internet Usage
--
1.5 GB * INR 19.5 = INR 29.25
18 GB*INR 19.5= INR 351
Price per gb
4.
Electricity Usage
--
3W*24*30=2.16kW per building+710W=18kW 
18kW * 12 = 216 kW
Using Solar panel
216kW * 6 = Rs.1296 per year(Rs.108 per month) will be saved using solar panels.
5.
Installation Charges
Rs.6000
--
--
One time cost 
6.
Maintenance Charges 
--
INR 1500 (avg.)
INR 18000
This cost will be applied for any sensor damage.
Total
Rs.37,000
INR 1530 + software cost.
INR 18350 + software cost.
--
Table 3.15: Total Project Cost

22
Benefits
Easy water usage monitoring on a daily basis as well as monthly basis per flat.
Water leakage identification.
Water wastage identification, if any.
Automation of the water management system.
Visualization of complete data to every user on their mobile app.
Automatic water billing system.
Reduced water wastage. 
Water tank will never be empty..
Pipe leakage detection alert.
Six months free maintenance services.
Easy switching of pumps through the app, in case of sensor damage.
Reuse of overflowed water from tanks.
Motor on/off status on app.


Conclusion
Our intention of this research work was to establish a flexible, economical, easily configurable and most importantly, a portable system which can solve our water wastage problem. It is a robust system and small in size. Our proposed system for water level monitoring comes under the field of Internet of Things (IoT). Our main objective was to design a smart system for approximating the water level in the tank and prevent overflow or analyse the water usage. This analysing feature can also help us in finding whether there is any leakage in the tank or not. Nowadays liquid level monitoring is vital in every society, industries, etc. Using our smart system we can analyse the usage and also detect the leakage in the tanks of the societies, and also for overflow and reduce wastage of water.




23
References
https://www.alibaba.com/
https://robokits.co.in/
https://www.indiamart.com/
https://news.energysage.com/how-much-does-the-average-solar-panel-installation-cost-in-the-u-s/
https://economictimes.indiatimes.com/tech/internet/india-has-the-cheapest-mobile-data-in-world-study/articleshow/68285820.cms#:~:text=The%20average%20price%20of%20USD,was%20USD%208.53%20for%201GB.
https://www.maximintegrated.com/en/design/technical-documents/app-notes/9/956.html#:~:text=Power%20consumed%20by%20the%20relay,normal%20operating%20voltage%20of%205V.&text=The%20relay%20shown%20has%20a,supply%20voltage%20of%202.5V.
https://scidle.com/how-to-use-a-ph-sensor-with-arduino/


	















24
