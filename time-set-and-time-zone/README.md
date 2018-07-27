---
description: >-
  This section will describe the concept of Time Set and Time Zone as well as
  how to go about configuring it.
---

# Time Set & Time Zone

This section will cover the aspects of setting up Time Set and Time Zone. System Users should take particular note on the importance of having proper settings for Time Set and Time Zone as it will affect operational timing for HARDWARE and FEATURES. 

## Time Set

Time Set defines a **'Time Interval'** **\(Operational Hours\)** for the system expressed in **‘Hours’ and ‘Minutes’**. To further incorporate flexibility requirements on operational hours for Hardware and Features, there are 3 ‘Intervals’ available for System Administrators to set the Time Period within each interval while Entrypass Platform1 Server comes with two default Time Set settings and System User configurable Time Set settings:

{% hint style="info" %}
* Time Set 0 = Not Active \(non editable within the system\)
* Time Set 1 = 24 Hours Active \(non editable within the system\)
* Time Set 2 and above = System User configurable
{% endhint %}

## Time Zone

Time Zone defines a **'Time Interval'** **\(‘Operational Hours’\)** for the system, **grouped together** on a **‘Weekly’** basis. To put this into a simpler perspective, Time Zone defines **'Day + Time Interval' \(Operational Day + Operational Hours\)** for the system. EntryPass Platform1 Server comes with two default Time Zone settings and System User configurable Time Zone settings:

{% hint style="info" %}
* Time Zone 0 = Not Active \(non editable within the system\)
* Time Zone 1 = 24 Hours Active \(non editable within the system\)
* Time Zone 2 & above = System User configurable
{% endhint %}

## Infographic Illustration

![Time Set within Time Zone](../.gitbook/assets/untitled1a%20%282%29.png)

From the above illustration, we can clearly see that Time Zone contain subset\(s\) of Time Set. All hardware and features will point to Time Zone for operational day and time instruction.

It is important for you to note that:

{% hint style="warning" %}
"Whenever any hardware Time Zone setting is in INACTIVE state, all features will not be functional despite its setting is ACTIVE"
{% endhint %}

To illustrate the above concept, we shall take a look at some of the setting scenarios below.

## Setting Scenarios

### Scenario 1 \(Hardware Setting only\)

{% hint style="info" %}
**Time Set Setting \(TS\)**

* Time Set 0: Inactive \(TS 0\)
* Time Set 2: 9.00 - 17.00 \(TS 2\)
{% endhint %}

| Time Zone | Mon | Tue | Wed | Thu | Fri | Sat | Sun |
| --- | --- |
| Time Set | **TS 2** | **TS 2** | **TS 2** | **TS 2** | **TS 2** | **TS 0** | **TS 0** |

When the above setting is applied to a hardware \(eg. a reader\), any staff using the access card would experience the following:

1. Between 9.00am to 5.00pm \(Mon to Fri\), all staff would have full access through the door \(reader ACTIVE\).
2. Anytime beyond 5.00pm to 8.59am next day \(Mon to Fri\), all staff do not have access through the door \(reader INACTIVE\).
3. All staff do not have access through the door on Saturday and Sundays \(reader INACTIVE\).
4. **Conclusion:** Staff's will not have any access to doors when the reader \(hardware\) is INACTIVE.

### Scenario 2 \(Hardware with Feature Setting\)

{% hint style="info" %}
**Time Set Setting \(TS\)**

* Time Set 0: Inactive \(TS 0\)
* Time Set 2: 9.00 - 17.00 \(TS 2\)
* Time Set 3: 9.00 - 15.00 \(TS 3\)
{% endhint %}

| **Hardware** Time Zone | Mon | Tue | Wed | Thu | Fri | Sat | Sun |
| --- | --- |
| Time Set | **TS 2** | **TS 2** | **TS 2** | **TS 2** | **TS 2** | **TS 0** | **TS 0** |

| **Feature** Time Zone | Mon | Tue | Wed | Thu | Fri | Sat | Sun |
| --- | --- |
| Time Set | **TS 3** | **TS 3** | **TS 3** | **TS 3** | **TS 3** | **TS 0** | **TS 0** |

When the above setting is applied to a hardware \(eg. a reader\) and feature \(Antipassback\), any staff using the access card would experience the following:

{% hint style="info" %}
Antipassback Feature: A system where the card holder would need to perform a complete process by flashing IN and OUT when entering and exiting the door. Refer to the chapter Antipassback for more information.
{% endhint %}

1. Between 8.00am - 3.00pm, staffs _will not be able_ to pass through the door TWICE \(Antipassback feature\). During this period, the reader and feature is **ACTIVE**.
2. Between 3.01pm - 5.00pm, staffs _will be able_ to pass through the same door TWICE. This is because, the reader is **ACTIVE** during this time while the Antipassback feature is **INACTIVE**.
3. Between 5.01pm - 8:59am \(Next Day\), staffs cannot pass through the same door as the hardware reader is **INACTIVE** during this time.
4. Conclusion: As long as the hardware \(e.g. reader\) stays ACTIVE, any features will be active as long as its Time Zone setting is similar to hardware \(e.g. reader\). If the feature Time Zone is 'shorter' \(shorter operating hours\) as compared to hardware, the feature will be **INACTIVE** \(turned off\) like the case above. Conversely, if the feature Time Zone setting is 'longer' compared to the hardware \(e.g. reader\), the feature will not work beyond the hardware's Time Zone because the hardware is in **INACTIVE** state.

