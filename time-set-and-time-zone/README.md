---
description: >-
  This section will describe the concept of Time Set and Time Zone as well as
  how to go about configuring it.
---

# Time Set & Time Zone

This section will cover the aspects of setting up Time Set and Time Zone. System Users should take particular note on the importance of having proper settings for Time Set and Time Zone as it will affect operational timing for HARDWARE and FEATURES. 

## Time Set

Time Set defines a **'Time Interval'** **\(Operational Hours\)** for the system expressed in **‘Hours’ and ‘Minutes’**. To further incorporate flexibility requirements on operational hours for Hardware and Features, there are 3 time ‘Intervals’ available for setting purposes. Time Set comes with two default settings:

{% hint style="info" %}
* Time Set 0 = Not Active \(default and non-editable within the system\)
* Time Set 1 = 24 Hours Active \(default and non-editable within the system\)
* Time Set 2 and above = User configurable
{% endhint %}

## Time Zone

Time Zone defines a **'Time Interval'** **\(‘Operational Hours’\)** for the system, **grouped together daily** on a **‘Week’** basis. To put this into a simpler perspective, Time Zone defines **'daily operational hours within a week'** for the system. EntryPass Platform1 Server comes with two default Time Zone settings and System User configurable Time Zone settings:

{% hint style="info" %}
* Time Zone 0 = Not Active \(default and non-editable within the system\)
* Time Zone 1 = 24 Hours Active \(default and non-editable within the system\)
* Time Zone 2 & above = User configurable
{% endhint %}

## Infographic Illustration

![Time Set within Time Zone](../.gitbook/assets/untitled1a%20%283%29.png)

From the above illustration, we can clearly see that Time Zone contain subset\(s\) of Time Set. All hardware and features will point to Time Zone for operational day and time instruction.

It is important for you to note that:

{% hint style="warning" %}
"Whenever any **hardware** Time Zone setting is in INACTIVE state, all **features** will not be functional despite its setting is ACTIVE"
{% endhint %}

To illustrate the above concept, we shall take a look at some of the setting scenarios below.

## Setting Scenarios

### Scenario 1 \(Hardware Setting only\)

Consider the Time Set \(TS\) & Time Zone \(TZ\) settings below:

{% tabs %}
{% tab title="Time Set" %}
![](../.gitbook/assets/untitled3%20%2834%29.png)
{% endtab %}

{% tab title="Time Zone" %}
![](../.gitbook/assets/untitled4%20%2828%29.png)
{% endtab %}

{% tab title="Reader \(Time Zone 2\)" %}
![](../.gitbook/assets/untitled5%20%2821%29.png)
{% endtab %}
{% endtabs %}

#### Infographic:

![Time Zone for Reader](../.gitbook/assets/untitled2%20%2811%29.png)

#### When the above setting is applied to a hardware \(eg. a reader\), any staff using assigned access card would experience the following:

* **Between 9.00am - 5.00pm:** 

  * Reader: Active
  * Result: all staff can pass through the door.

* **Between 5.01pm - 8.59am next day:**

  * Reader: Inactive
  * Result: all staff cannot pass through the door.

* **Saturdays, Sundays and Holidays**
  * Reader: Inactive
  * Result: all staff cannot pass through the door.

{% hint style="info" %}
**Conclusion: Staff's will not have any access to doors when the reader \(hardware\) is INACTIVE.**
{% endhint %}



### Scenario 2 \(Hardware with Feature Setting\)

Consider the Time Set & Time Zone settings below:

{% tabs %}
{% tab title="Time Set" %}
![](../.gitbook/assets/untitled6%20%288%29.png)
{% endtab %}

{% tab title="Time Zone" %}
![](../.gitbook/assets/untitled7%20%2823%29.png)
{% endtab %}

{% tab title="Reader \(Time Zone 2\)" %}
![](../.gitbook/assets/untitled5%20%2828%29.png)
{% endtab %}

{% tab title="Feature \(Antipassback\) \(Time Zone 3\)" %}
![](../.gitbook/assets/untitled8%20%2816%29.png)
{% endtab %}
{% endtabs %}

#### Infographic

![Time Zone applied to Reader \(hardware\)](../.gitbook/assets/untitled2%20%283%29.png)

![Time Zone applied to Antipassback \(Feature\)](../.gitbook/assets/untitled3%20%2836%29.png)

#### When the above setting is applied to a hardware \(eg. a reader\) and feature \(Antipassback\), any staff using the access card would experience the following:

* **Between 9.00am - 3.00pm:**

  * Reader: Active
  * Feature \(Antipassback\): Active
  * Result: door is active and staff can pass through.
  * Staffs cannot pass through \(enter\) the same door without performing 'flashing' out first \(Antipassback feature\). 

* **Between 3.01pm - 5.00pm:** 

  * Reader: Active
  * Feature \(Antipassback\): Inactive
  * Result: door is active and staff can pass through.
  * Staffs can pass through \(enter\) the same door without performing 'flashing' out first \(Antipassback feature turned off\). 

* **Between 5.01pm - 8:59am \(Next Day\):**

  * Reader: Inactive
  * Feature \(Antipassback\): Inactive
  * Result: reader is inactive.
  * Staffs cannot pass through the door.

* **Saturdays, Sundays and Holidays:**
  * Reader: Inactive
  * Feature \(Antipassback\): Inactive
  * Result: reader is inactive.staffs cannot pass through the door.

{% hint style="info" %}
**Conclusion:** 

1. As long as the hardware \(e.g. reader\) stays ACTIVE, any features will be active as long as its Time Zone setting is similar to hardware \(e.g. reader\). 
2. If the feature Time Zone is 'shorter' \(shorter operating hours\) compared to hardware, the feature will be INACTIVE \(turned off\) like Scenario 2. 
3. If the feature Time Zone setting is 'longer' compared to the hardware \(e.g. reader\), the feature will not work beyond the hardware's Time Zone because the hardware is in INACTIVE state like Scenario 2.
{% endhint %}

## Quick Notes

**Antipassback Feature:** A system where the card holder would need to perform a complete process by flashing IN and OUT when entering and exiting the door. Refer to the chapter Antipassback for more information.

{% page-ref page="../access-control-features/how-to-configure-local-antipassback.md" %}

