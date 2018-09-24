---
description: >-
  This section will explain the concepts covering the basic Access Control
  Features found within Platform1 Server.
---

# Access Control Features

## Access Level

**The function of Access level is to group together various barriers \(Barrier can be defined as a gate, turnstile, doors, lifts\) to form an Access Control protocol.** 

'Access Level' can be seen as a configuration \(group\) where different types of the barriers being grouped together creating a unique set of access control protocols within an area that only individuals assigned with the proper rights \(access level\) can have access to.In Access Level, there is a maximum limit of 255 'levels' \(groups\) that can be created within the system. 

 For example:

| Access Level 1 | Access Level 2 |
| :--- | :--- |
| Ground Floor Entry, Office Door \(level 5\), Lift \(No.3\), Pantry Door \(level 5\) | Ground Floor Entry, Office Door \(level 10\), Lift \(No. 2\), Pantry Door \(level 10\) |

When Access Level is active, staffs can only access barriers which had been grouped under the Access Level assigned to them. In the above example, when a staff is assigned with Access Level 1, he will then have the 'rights' to access doors and lift listed within Access Level 1 while, he will not be able to access any doors listed under Access Level 2. 

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

**Further consideration on Antipassback:** The Antipassback feature can be enabled for **both entry and exit readers.** By default, ONLY the entry reader is enforced while to enforce the same feature for exit reader, you would need to set the 'Security Mode' in door setting to 'High'. 

## Interlock

Interlock is a feature where:

{% hint style="info" %}
When one of the doors within an Interlock Group is opened, the group's remaining doors cannot be opened until that particular opened door is closed. 
{% endhint %}

To illustrate the above, consider the scenario below:

{% hint style="info" %}
John Doe and Jane Doe is heading to a room where there are two doors \(door 1 and door 2\). John will be passing through door 1 and Jane will be passing through door 2. When both of them reached the room, both flashed their access card at the respective door's reader.

**When Interlock is DISABLED:** John and Jane **will be able** unlock their respective doors \(door 1 and door 2\) simultaneously. 

**When Interlock is ENABLED:** John and Jane **will not be able** to unlock the doors \(door 1 and door 2\) simultaneously. If John flashes his access card first and open door 1, then Jane would need to wait until door 1 is closed before she can flash her card again to unlock door 2 and open that door.
{% endhint %}

There are two modes available for Interlock:

* **Single Board Interlock:** This would bind doors that is listed within a single control panel only.
* **Cross Board Interlock:** This would bind doors that is listed on other control panels as well.

## Fire Release Group

Fire Release Group is a feature where:

{% hint style="info" %}
All doors listed within the Fire Release Group will be 'released' \(UNLOCKED\) automatically when fire sensors are being triggered. 
{% endhint %}

When Fire Release Group is activated, it will be an 'always on' feature and will not be affected by Time Set or Time Zone. 

## Access Limit

Access Limit is a feature where:

{% hint style="info" %}
The system monitors the **number of individuals** permitted to remain within a zone / area.
{% endhint %}

The feature above relies on Entry and Exit readers where it registers the number of staffs entering and exiting a zone / area. For example, when a zone / area is configured to permit only 5 staffs to be within that area at any one time, that entry reader will keep track of the number of staffs entering that zone / area. Once the maximum number is reached \(in this case 5\), then the reader will not allow the 6th person to enter that zone / area. The only time when that 6th person can enter that zone / area is when 1 or more staffs exit that zone / area \(thereby reducing the number of persons in that zone / area\). 

## Buddy Mode

Buddy mode is a feature where:

{% hint style="info" %}
A staff is paired with another staff to enter OR exit a door.
{% endhint %}

This process would involve both staffs flashing their cards at the entry or exit readers to access an area. Without their respective buddies, they would not be able to enter / exit doors where buddy mode is active. 

This feature would require a **minimum of two staffs to be assigned with the same group Buddy Number** while the maximum number of staffs being assigned with the same buddy number is up to the maximum number of cards within the Entrypass Platform1 Server's database. Buddies are paired according to a 'group number' that is assigned to them \(2 - 255\). For example, when a staff is assigned with group Buddy No. 2, that staff would require another staff \(buddy\) that holds Buddy No. 2 to flash their cards at readers to access an area. 

For card holders assigned with **Buddy No.1**, this number is reserved for **'ADMIN'.** Buddy No.1 card holders have **NO REQUIREMENT to be paired with another Buddy No. 1** card holder to flash their cards at the reader to access an area. Instead, any other Buddy Numbers \(e.g. 2, 3, 4 etc.\) can be designated as a Buddy for Buddy No.1 card holders. 

{% page-ref page="how-to-configure-buddy-mode.md" %}

## Roll Call

This feature will enable you to:

{% hint style="info" %}
Monitor staffs' location within designated zones.
{% endhint %}

This feature will display the staffs' information and also it's latest location at zones which had been designated to be monitored. Any staff whom flashes their access card at these zones, will have their information displayed on the Roll Call Tab. 

