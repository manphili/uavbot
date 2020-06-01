** This Package Contains 1 main task, 1 sub task, xml config file, access db file and an interactive form**

ID : mp3minu
Created by : Manuel Varghese Philip

Zero Contact - Essentials Delivery UAV Bot
The Bot creates and executes an Autonomous Flight Plan for a UAV / Drone based on Guidelines for Contact less Delivery of Essential commodities during the pandemic.

Theme : Essential Delivery during COVID - Logistics and Supply 

Bringing the true sense of "Anywhere" in the name Automation Anywhere !
 

Inspiration
The Novel Corona-virus has affected humanity in various ways, be it our economy, our freedom of movement, and the loss of loved ones. Something that struck me was elderly people having to wait in a queue for medicines at an outlet. Even though there are home delivery services the risk of infection extremely high as this job requires you to move around places at a higher rate and I recollected news of people infected by pizza delivery agents / Swiggy agents throughout India on multiple occasions. The Lockdown definitely has slowed down the infection rates but we were forgetting that all essential services are not contactless. That's when I decided to create a solution to this by using a Drone / UAV to Deliver essentials and medicines primarily for the vulnerable among us so that we ensure they are safe, Drones are usually manually remote-controlled by a pilot. Me myself being an aerospace engineer with focus on Avionics and with Automation Anywhere. I decided to use an AutoPilot Mission Planner to write coded commands to the Flight controller in order to make the Flight Autonomous and deliver the essential package and return home.

From the News
Bengaluru on superspreader alert after delivery boy tests positive - Click here to read

83-year-old man collapses while waiting in New World queue in New Lynn - Click here to read

Features in a nutshell
Interactive User input
Database Logging
Autonomous UAV Flight
Automated Pre Flight Checks
Address to Geo Coordinates conversion
Distance, Payload release altitude Calculation
AutoPilot Command creation (Flight Plan)
Payload Delivery (Essential package Delivery)
Scalability
What it does
The Bot collects the delivery address and input data using Interactive forms and converts the address string into location coordinates using Geocoding API and uses Python Script to calculate the Flight Distance using Haversine Formula based on the range of the UAV and Performs Pre-Flight Checks such as Wind speed, Temperature, Precipitation Probability, Cloud Cover, Visibility and more. It also checks for any nearby airport and logs the Aeronautical charts for the way-points using Sky Vector web service. It then Sends Flight information to the DGCA for Flying permission via API. It then calculates the payload release altitude based on logic using the Indian regulatory guidelines for construction. Finally, the bot compiles this information to create a flight plan command and uses the Mission Planner which is Ground Control Software to write the code into the Flight controller AutoPilot using a wireless transmitter and launches the UAV on its mission. While doing this each flight is tracked by a unique flight control number and logged to a database for future audit and compliance purposes and folder is created with Logs, charts, and autopilot code. Hence this Bot enables users to completely automate the Pre-Flight processes and automate the creation of code for Autonomous UAV Flight which will Deliver the payload (Essential Package) at the desired location and return back home and complete the mission. This makes the complete process contactless and safe hence serving the essential needs of the most vulnerable and reducing the infection rate.

How I built it
This RPA Solution is Built on Automation Anywhere A2019 and integrates with various technology as mentioned below, which is the real beauty of RPA.

Microsoft Bing Geocoding API
Python 3.8.3
Ardu Pilot Mission Planner ( with wireless transmitter hardware)
Interactive Forms
UAV Forecast Service
Sky Vector Chart Service
DGCA API
Microsoft Access Database
UAV / Drone & Payload release mechanism
Challenges I ran into
One of the challenges was to use complex mathematical formulae using Python to derive certain parameters. However, the Python Package on A2019 made it really easy to call Python functions inside and code and get the output. Also creating a waypoint plan for the Autopilot was initially a challenge however using the product documentation I was able to create the flight plans using Log to file package making all the values dynamic.

Accomplishments that I'm proud of
I am happy that I was able to use my academic knowledge in Aerospace, my work expertise in Robotic Process Automation, and my curiosity to explore new possibilities in creating this solution which can help the world in this traumatic situation. I am also happy that I was able to bring out the true sense of Anywhere in the name "Automation Anywhere".

What I learned
It was indeed a great experience to develop this bot with a lot of research, trial & error and new learnings. I was able to start off with Python and I'm looking forward to trying out further possibilities.

What's next for Zero Contact UAV Bot
The RPA solution can be scaled up for usage with Queue (WLM) and to further improvise and add on more features. To make the solution more independent we can have a "Raspberry Pi" attached to the drone and connected to the Flight controller and the Internet. We can install AA Bot agent on the Raspberry Pi running windows and we can remotely deploy the automation considering the Drone as a bot runner with wings ;). This drone will be a fully automated solution for an Autonomous Flight using Robotic Process Automation as the base Technolgy.

Other areas of usage
Delivery Services
Search and Rescue Facilities
Climbers and Firefighters
Mine and Oil Industry
Military and Gaurd Services


Built With
api
ardupilot
automationanywhere
autonomousuav
flightcontroller
geocodingapi
missionplanner
payloadreleasemechanism
python
skyvector
uavforcast