# Home IOT Irrigation System
#### A "fun" home IOT project featuring an M5stack microcontroller with environment sensors and irrigation pump. The microcontroller also sends a Push Notification update on a mobile application stating the current temperature and humidity using Cloud Messaging via HTTP protocol through the microcontroller.


---

## [Table of contents](#table-of-contents)
1. [Project Context](#project-context)
3. [Project Requirements](#project-requirements)
4. [Planning](#planning)
5. [Project Stack](#project-stack)
6. [Results](#results)
7. [Showcase](#showcase)

---

## [Project Context](#projectcontext)
Like every plant parent that shares and suffers that great deal of stress of leaving their plant babies alone at home while they are overseas, I have decided a DIY method using IOT to customise and solve my problem. I mean what could go wrong.......right? 
<br></br>
`*Insert nervous laughter*`

TL;DR
<br> </br>
~~My project worked! All my plants survived~~ A Plant got hosed to death

---
## [Project Requirements](#projectrequirements) 
Given that I am a helicopter plant parent, I had a few self-imposed requirements to the project. Hence the birth of the commandments to the project.

4 Commandments to this project.
1. Thou shall receive information about the ambient temperature and humidity of the area via push notification.
2. Thy plants shall each be dosed with their own quantity amount of water.
3. Thou shall have vision to check in on thine plants. (Done using Home Security Camera)
4. If thy microcontroller was to be plagued with a network error, thy watering shall still be done locally.

---

## [Planning](#planning) 

### Serial Irrigation System
Intially I designed a serial pump system however with each outlet, the pressure of the water will drop as the water flows through it. This will result in very minimal water output for the terminal plant.

<img width="851" alt="Screenshot 2022-12-12 at 11 28 05 PM" src="https://user-images.githubusercontent.com/47912781/207085870-d014154e-8dab-4f8f-95c5-af4260c34821.png">
<br></br>


### Parallel Irrigation System
With Parallel system, water flow is split amongst X number of plants. Although each plant may receive less amount of water, this method will resolve with the drop of pressure flow which is found in serial method.

<img width="852" alt="Screenshot 2022-12-12 at 11 28 13 PM" src="https://user-images.githubusercontent.com/47912781/207085857-b6b6255b-9211-4fdd-b199-d775bedd1816.png">

### Equipments

#### Watering Unit
<img width="350" alt="Watering Unit" src="https://user-images.githubusercontent.com/47912781/207115884-59485805-be84-48ea-81fe-49382950e536.png">

#### M5stack(Microcontroller) with Env Sensor
<img width="350" alt="M5stack with Env Sensor" src="https://user-images.githubusercontent.com/47912781/207116238-38cad341-cbb6-4826-9d59-c1cb0c51dd14.png">

#### Bucket for reservoir
<img width="330" alt="Bucket for reservoir" src="https://user-images.githubusercontent.com/47912781/207116693-df8dc4d0-b5d2-4d89-8fc3-c59043656329.png">

#### Temp Water Catchment
<img width="350" alt="Temp Water Catchment" src="https://user-images.githubusercontent.com/47912781/207117279-8b7f455f-9f2f-4a2b-9cf9-6f83758d2ff3.png">

#### Roller Clamp to titrate water flow
<img width="350" alt="Roller Clamp" src="https://user-images.githubusercontent.com/47912781/207122032-1866d0b9-8e61-4520-b620-352432777b68.png">


---

## [Project Stack](#projectstack) 
The project was made using Flutter with Firebase as a Backend as a Service and M5stack.

<pre>
Cloud Message: Firebase Cloud Messaging HTTP protocol
Microcontroller: Miro-Python
</pre>

<img src="https://user-images.githubusercontent.com/47912781/206226953-a00dd140-a476-4995-b254-86527b792906.png"  height="150" >

<div align="right">[ <a href="#table-of-contents">↑ to top ↑</a> ]</div>

## [Results](#results)
I came home to witness one my plants drowned. I've forgotten that the medium the plant was in had excellent water retention capacity and I probably shouldn't have watered the plants too fast.

On a sunnier note, I learnt a lot from this project.

- Serial vs Parallel Irrigation System
- Timing of watering was based on a timer which will periodically fetch the datetime from an API.
- Writing of code using Micro-python without standard libraries.


<div align="right">[ <a href="#table-of-contents">↑ to top ↑</a> ]</div>


## [Showcase](#showcase)

# Parallel Irrigation System
![Plant shot](https://user-images.githubusercontent.com/47912781/207088447-09b9d9de-d504-4313-adfd-9d5906f5ae7a.jpg)

# Biopsy result: Drowned to death
![Dead Plants](https://user-images.githubusercontent.com/47912781/207088578-33aca788-78b2-42e2-8380-0001deb29465.jpeg)

# Push Notification Example
<img width="361" alt="Screenshot 2022-12-13 at 1 26 00 AM" src="https://user-images.githubusercontent.com/47912781/207112484-a6fee70b-3bd9-4380-97d6-4da4b0148467.png">

<div align="right">[ <a href="#table-of-contents">↑ to top ↑</a> ]</div>


