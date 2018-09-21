---
description: >-
  This section will explain the concepts covering the basic Access Control
  Features found within Platform1 Server.
---

# Access Control Features

## Access Level

**Access level can be defined as the 'right to access', of a staff member through a barrier \(Barrier can be defined as a gate, turnstile, doors, lifts\).** When Access Level is active, staffs will only have access to those area whom they had been explicitly given  the permission to. 

Access Level does not limit itself to a single door but rather, it can be grouped together that may contain multiple doors or other form of barriers to create a well integrated network of barriers. 

 For example:

| Access Level 1 | Access Level 2 |
| :--- | :--- |
| Ground Floor Entry, Office Door \(level 5\), Lift \(No.3\), Pantry Door \(level 5\) | Ground Floor Entry, Office Door \(level 10\), Lift \(No. 2\), Pantry Door \(level 10\) |

In the above example, when a staff is allocated with Access Level 1, he then will have the 'rights' to access doors and lift listed within Access Level 1 while, he will not be able to access any doors listed under Access Level 2. 

In Access Level, there is a maximum limit of 255 'levels' \(groups\) that can be created within the system. A single 'Level' can be defined as a configuration \(group\) where different types of the barriers being grouped together creating a unique set of access control protocols within an area that only individuals assigned with the proper rights \(access level\) can have access to. 

## Access Group

**Access Group has the same feature as Access Level** with the exception that, it has **'Unlimited Access Levels'** i.e., it does not limit itself to 255 levels \(configuration\). This feature is supported on the latest group of products. 

## Antipassback

Antipassback is a feature when enabled:

{% hint style="info" %}
**Will not be allow staffs to ENTER a location / zone twice without first EXITING that location / zone.**
{% endhint %}

To illustrate the above, consider the scenario below:

{% hint style="info" %}
John Doe is walking towards the entrance to his office. He takes out his access card and flashed his card at the **entry reader** **\(terminal\)** and the door is **UNLOCKED**. However, he was distracted by a conversation and **DID NOT pass through that unlocked door,** while the door 'Re-lock' itself after a brief period of time. When John finished his conversation, he flashed **his access card at the entry reader \(terminal\) again in an attempt to unlock and pass through that door.** 

**When Antipassback feature is DISABLED**: The door will **UNLOCK** and John _**WILL BE ABLE**_ to pass through that door again.

**When Antipassback feature is ENABLED**: The door will stay **LOCKED** and John _**WILL NOT BE ABLE**_ to pass through that door. As the system had detected that John had flashed his access card at the entry terminal and had not flashed out at the exit reader, the system will refuse to unlock the door as he is deemed to have 'flashed twice' at the entry terminal. When John had flashed in at the entry reader to pass through that door, he must perform 'flash out' on the exit reader so that the next time he 'flashes in' on the entry reader again, the door can be unlocked.
{% endhint %}

For Antipassback feature, there is two modes available:

* Local Antipassback: Limited to the doors listed in a **single Control Panel** only.
* Global Antipassback: Will include all doors from **other Control Panels** listed within the server.

#### Further consideration on Antipassback

1. The Antipassback feature can be enabled for **both entry and exit readers.** By default, ONLY the entry reader is enforced while to enforce the same feature for exit reader, you would need to set the 'Security Mode' in door setting to 'High'. 

## Interlock

Interlock is a feature where:

{% hint style="info" %}
A group of doors being tied to each other. When one of the doors within the group is opened, the remaining doors cannot be opened until that particular door is closed. 
{% endhint %}

To illustrate the above, consider the scenario below:

{% hint style="info" %}
John Doe is heading to his office on level 10 where he needs to pass through a corridor with two doors located at each end \(door 1 & door 2\). To reach his office, he needs to pass through door 1 first and then door 2 before reaching the office entrance. At the same time, Jane Doe had just exited her office entrance and heading towards the opposite direction of John and would need to pass through the same corridor through door 2 and then, door 1.

**When Interlock is DISABLED:** John and Jane **will be able** to flash their access card and unlock the doors \(door 1 and door 2\) simultaneously to proceed through the corridor.

**When Interlock is ENABLED:** John and Jane **will not be able** to flash their access card and unlock the doors \(door 1 and door 2\) simultaneously. If John flashes his access card first and open door 1, then Jane would need to wait until door 1 is closed before she can unlock door 2 and open that door.
{% endhint %}

There are two modes available for Interlock:

* Single Board Interlock: This would tie doors that is listed within a single control panel only.
* Cross Board Interlock: This would tie doors that is listed on other control panels as well.

## Fire Release Group

Fire Release Group is a feature where:

{% hint style="info" %}
All doors listed within a group will be 'released' \(UNLOCKED\) when fire sensors are being triggered. 
{% endhint %}

## Access Limit

Access Limit is a feature where:

{% hint style="info" %}
The system monitors the number of individuals permitted to remain within a zone / area.
{% endhint %}

The feature above relies on Entry and Exit readers where it registers the number of staffs entering and exiting a zone / area. If for example, a room is only permitted to have 5 staffs within it, the entry reader will permit up to 5 staffs entering that zone / area while rejecting the 6th staff. If 1 staff exit the zone / area, then the system will permit up to 1 staff to enter that place.

## Buddy Mode

Buddy mode is where a staff is paired with another staff to enter OR exit a door. The process would involve  both flashing their cards at the entry or exit readers to access an area. Without their respective buddies, they would not be able to enter doors in which the buddy mode is active. This feature would allow a staff to be paired with more than 1 buddies.

## Roll Call

This feature will enable you to:

{% hint style="info" %}
Monitor staffs within a particular area / zone.
{% endhint %}

When a Roll Call group is created staffs will be assigned to that particular group and where ever the staff flashes their access cards, the system will update the staffs' latest location on the **Roll Call Tab**. 

