  **<h1>Alarm Clock LWC Application ⏰</h1>**
  
A fully functional **Alarm Clock** built with **Salesforce Lightning Web Components (LWC)**. This application allows users to set and manage alarms with a dynamic, real-time clock display and a responsive UI.
<h3>Features</h3>

* Display current time in HH:MM:SS AM/PM format.

* Set alarms with selectable hours, minutes, and AM/PM.

* Trigger alarms with a ringing sound and animated clock image when time matches.

* Clear alarms and reset all selections easily.

* Responsive design using SLDS (Salesforce Lightning Design System).

* Custom dropdown component for reusable hour, minute, and meridiem selection.

<h3>Demo</h3>
Clock shakes and ringtone plays when alarm triggers.

<h3>Components</h3>

**1. alarmClockApp**

* Main component that displays the clock, alarm buttons, and dropdowns.

* **Handles:**

  * Real-time clock updates.

  * Alarm logic and triggering.

  * Communication with child dropdown component via CustomEvent.

**2. clockDropdown**

* Reusable dropdown component for selecting hour, minute, or AM/PM.

* **Props:**

    * label — Label for the dropdown.

    * options — List of selectable options.

    * uniqueId — Unique identifier for the dropdown.

* **Events:**

    * optionhandler — Sends selected value back to the parent component.

* **API Method:**

    * reset(value) — Resets the dropdown to a specified value.
 
**Technologies Used**

* Salesforce Lightning Web Components (LWC)

* SLDS (Salesforce Lightning Design System) for styling

* JavaScript for alarm logic

* HTML & CSS for layout and styling

* Audio API for alarm ringtone

**How It Works**

**1. Clock Display:** alarmClockApp updates every second to show the current time.

**2. Setting Alarm:**
* User selects hour, minute, AM/PM from dropdowns.

* Click Set Alarm to save alarm time.

**3. Triggering Alarm:**

* When the current time matches the alarm, the clock image shakes, and the ringtone plays in a loop.

**4. Clearing Alarm:**

* Click Clear Alarm to stop ringtone and reset all selections.
