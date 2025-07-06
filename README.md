# COMPUTER VISION CAPABILITIES FOR AQUATIC NAVIGATION

## Software vision team:
- [Salvador Cantuarias](https://www.linkedin.com/in/salvador-cantuarias-bb5715268/)
- [Nouhaila Elmalouli](https://www.linkedin.com/in/nouhaila-elmalouli-46517a208/)

This project is in the frame of Njord Autonomous Ship Challenge 2025, a unique, international student competition that will be held onsite from the 4th of August through the 9th of August 2025, where participants are tasked with designing and building an autonomous ship and competing in a series of challenges and events.  

🚤 Our boat is learning to see—and steer!
Here’s a quick look at how we’re teaching our ASV to detect objects and make decisions in real-time.

The system scans the water, spots buoys, and figures out how to navigate between them—adjusting course when needed, just like a smart captain.
It’s all thanks to a combo of tools we’ve been experimenting with:
🎨 Color detection
📐 Edge detection
🌄 SIFT (Scale-Invariant Feature Transform)
🧠 YOLO (yes, the object detection one)

All stitched together in a custom Python class we’ve been building from scratch.

## Tasks:
>**2025-04-11:** <br>
>>>Create a class that uses computer vision's color recognition to detect elements in the video feed and make the boat respond accordingly.<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Nouhaila<br>
>>
>>**observations:** <br>
>>- The script is able to take pre recorded video inputs. now its time to test live feed.<br>
>>- We need to change the mathematical approach to identifing the postion of the buoys. Right now it is just related to which forizontal half of the frame is being used. this ould be changed by measuring the delta space between the buoys, if said delta space has a postive or negative value and how close is the center of that delta space to the center of the frame for color correction.<br>
>>- More cases need to be tested: when theres more than two buoys, when a buoy is partially obstrucuted, etc...<br>
>>- Cardinal buoys need to be integrated into the class.

>**2025-04-22:** <br>
>>>reworking the mathematical system for making desisions (delta distance between buoys)<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Salvador<br>
>>
>>**Observations:** <br>
>>- Now the program is able to give more precise orders to control movement and define the center point of direction between the buoys.
>>- further tunning needs to be done to take into account the the difference in postion of the buoys and how that should affect the center point between them and the direction the boat should take in relation to it.
>>
>>>generate or record more cases of buoys position.<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Salvador <br>
>>
>>**Observations:** <br>
>>- The race path was reconstucted in rhinoceros to the exact specifications given by the competitons handbook and a video was recorded to be used as input. This new footage shed more light on what are the elements to take into consideration and where the script's weakpoints are.<br> [A video of the current performance (2025-04-20) is provided](https://youtu.be/pIJFHZwhgWk)
>>
>>>tap into real time video feed.<br>
>>>**status:** `STARTED`<br>
>>>**assigned to:** Salvador<br>
>>
>>**Observations:** <br>
>>
>>>get some ideas of how to detect the OTTER (unknown obstacle).<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Nouhaila, Salvador<br>
>>
>>**Observations:** <br>

>**2025-04-29:** <br>
>>>use the given dataset and try object detection to get better segmentation of the buoys.<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Nouhaila, Salvador<br>
>>
>>**Observations:** <br>
>>- [link to new updates in performance](https://youtu.be/HbUlDyNRyM8)

>**2025-05-06:** <br>
>>>add cardinal buoys.<br>
>>>**status:** `DONE`<br>
>>>**assigned to:** Nouhaila <br>
>>
>>**Observations:** <br>
>>
>>>Link current detection script with software_gps_path current software development for coordination between object segmentation and gps navigation.<br>
>>**status:** `NOT STARTED`<br>
>>>**assigned to:** Salvador<br>
>>
>>**Observations:** <br>
>>
>>>Link detection script with hardware motor movement system. Start to incorporate hardware functions into script.<br>
>>**status:** `NOT STARTED`<br>
>>>**assigned to:** Salvador<br>
>>
>>**Observations:** <br>
>>
