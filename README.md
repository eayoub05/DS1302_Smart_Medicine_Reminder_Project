 

Smart Medication Reminder System


CTE 558 – Embedded Systems
Students:
Hayek Mary
Ayoub Elie
Instructor:
Prof. ZAITER CLARA

Date:
09-01-2025

 
I.	Abstract
The Smart Medication Reminder System is an embedded solution designed to streamline medication management by providing timely alerts. Using a DS1302 Real-Time Clock (RTC) module for accurate timekeeping, the system integrates an Arduino UNO, an LCD for display, LEDs, and a buzzer to deliver visual and audible notifications. Users can set and adjust up to four medication schedules through an intuitive interface of push buttons. The project showcases a robust design leveraging I2C communication for RTC operation, reliable alert mechanisms, and user-friendly features, ensuring an efficient and practical healthcare assistance tool. 
Table of Contents
I.	Abstract	2
II.	Introduction	4
III.	Objectives	4
IV.	System Overview	4
V.	Components Description	4
1.	Hardware Components	4
2.	Software Components	5
VI.	Circuit Design	5
VII.	Software Implementation	6
3.	Key Functions in Code	6
VIII.	Flowchart Explanation	6
4.	Flowchart	7
IX.	Features and Functionalities	8
X.	Testing and Results	8
5.	Testing	8
6.	Results	8
XI.	Future Enhancements	8
XII.	Conclusion	8
XIII.	References	9





Table of Figures:	
Figure 1: Circuit Description	6
Figure 2: Flowchart Diagram	8

 
II.	Introduction  
The Smart Medication Reminder System is designed to assist users in managing their medication schedules effectively. By integrating real-time clock (RTC) functionality, visual and audible alerts, and user-friendly controls, the system ensures timely reminders for up to four daily medications.

III.	 Objectives  
-	Track and display real-time information.  
-	Enable users to set and adjust current time through push buttons.  
-	Allow scheduling of up to four medication times for four distinct containers.  
-	Provide both visual (LED) and audible (buzzer) alerts for medication reminders.  

IV.	System Overview  
The system uses an RTC module to keep accurate time, an Arduino UNO to process user inputs and control outputs, and an LCD to display schedules. Push buttons serve as the interface for configuring time and medication schedules. LEDs and a buzzer provide reminders when it's time to take medication.

V.	Components Description  
1.	Hardware Components  
-	RTC - DS1302: Keeps accurate time for reminders.  
-	Arduino UNO: Central processing unit for the system.  
-	LCD Display: Shows real-time and scheduled data.  
-	Push Buttons (4):  
-	Set/adjust time.  
-	Schedule medication times.  
-	Buzzer: Sounds alerts.  
-	LEDs (4): Indicate which medication slot is active.  
-	Resistors and Jumper Wires: For circuit stability and connections.  
 
2.	Software Components  
-	Arduino IDE for coding.  
-	Libraries: DS1302 for RTC functionality, LiquidCrystal for LCD control.  

VI.	Circuit Design  
The circuit connects the RTC module to the Arduino UNO for timekeeping, the LCD for displaying information, and LEDs and a buzzer for alerts. Push buttons are used for input, interfacing with the Arduino via GPIO pins.
 
Figure 1: Circuit Description
 
VII.	Software Implementation  
3.	Key Functions in Code  
1.	Initialization:  
Configure LCD, RTC, and pins for buttons, LEDs, and buzzer.  

2.	Time Reading:  
Retrieve current time from the RTC module.  

3.	Modes of Operation:  
-	Normal Mode: Displays the current time.  
-	Time Setting Mode: Adjusts time values using buttons.  
-	Config Mode: Schedules medication times for up to four slots.  

4.	Alerts:  
-	Compare current time with scheduled times.  
-	Activate corresponding LED and buzzer for the medication slot.  

VIII.	Flowchart Explanation  
The system’s operation follows this flow:  
o	Start: Initialize all components (RTC, LCD, pins).  
o	RTC Check: Verify and retrieve the current time.  
o	Modes of Operation:  
-	Normal Mode: Default display of real-time.  
-	Time Set Mode:  
-	Adjust hours, minutes, and seconds.  
-	Save and return to Normal Mode.  
-	Config Mode:  
-	Set schedules for up to four medication slots.  
-	Activate buzzer and LED for notifications.  
o	Alert Activation: When the current time matches a scheduled time, activate the corresponding LED and buzzer.
 
4.	Flowchart  
  
  
Figure 2: Flowchart Diagram

IX.	Features and Functionalities  
-	Time Tracking: Continuous tracking of real-time using RTC.  
-	Time Adjustment: Easy-to-use interface for setting time.  
-	Medication Scheduling: Configures up to four medication schedules.  
-	Alert Mechanism: Combines visual (LEDs) and audible (buzzer) notifications.  

X.	Testing and Results  
5.	Testing  
o	RTC tested for accurate time tracking.  
o	Buttons tested for smooth operation in all modes.  
o	Buzzer and LEDs tested for appropriate responses at scheduled times.  

6.	Results  
o	Accurate time display and scheduling.  
o	Reliable alerts at specified times.  
o	User-friendly interface for setup and operation. 

XI.	Future Enhancements  
-	Expand support for additional medication slots and timings.  
-	Integrate mobile application for remote scheduling and control.  
-	Add voice reminders for improved accessibility.  
XII.	Conclusion  
The Smart Medication Reminder System successfully achieves its objectives of providing real-time tracking, medication scheduling, and timely reminders. The project demonstrates the potential for expanding its functionality to meet diverse user needs in healthcare assistance.   
XIII.	References
1.	Course Notes: "CTE558 Embedded Systems"
2.	Datasheet: DS1307 Real-Time Clock Module
3.	"I2C Communication Protocol" - Philips Semiconductors Documentation
4.	Arduino IDE Documentation
5.	"UART Communication Basics" - Microchip Technology

