# Readers

This section will be covering general aspects and explanation on the various settings found in Readers so as to further facilitate and enhance the understanding towards Reader control. This guide is referenced from N5400 series Control Panel while there may be features discussed here that may not be applicable to other models.

## Reader \(Image\)

![](../.gitbook/assets/untitled3a%20%285%29.png)

## List of Parameters

### 1. Name 

This parameter highlights the name of the Readers that had been assigned earlier during Adding New Control Panel \(refer to 3.1.1.2\). The name of the readers assigned should be unique and identifiable.

### 2. Description 

This parameter will highlight the description that you have set up during Adding New Control Panel \(refer to 3.1.1.2\).

### 3. Reader Type 

This parameter will set the reader type \(type of device\) manufacturers. By default, the Reader Type is ‘Standard Wiegand’ and the Control Panel \(N5400\) is able to support other type of reader manufactured by HID, Suprema, Rosslare, Standard Magnetic Stripe Card Readers \(ABA Track II\) and Standard Wiegand Readers.

### 4. In / Out 

This parameter will allow you to set the reader to either be an IN reader OR OUT reader.

### 5. Bind to Door \(Use Diagram\) 

This parameter will allow you to set to bind a door to a particular reader. By default, Readers 1 & 2 will bind to Door 1 while Readers 3 & 4 will bind to Door 2. Saying that, the system do allow for different readers to be bound to different doors by manually changing the settings.

### 6. HID AGK 

This parameter will allow you to set the AGK format for ‘HID Integrated Keypad’ readers. This setting is required in order to allow proper communication between the Control Panel and HID readers.

{% hint style="info" %}
\(NOTE: For item vii to x, to have a better understanding of the topic please refer to EntryPass Platform1 Server Help File \(F1 Button\).
{% endhint %}

### 7. Wiegand Option 

This parameter will allow you to select "Single" if the controller is non multi-Wiegand type \(e.g.: HCB Batch 1,2,3\), select "Multiple" if the controller is multi-Wiegand type \(e.g.: HCB Batch 4 and above\).

### 8. Wiegand Format

For more information \(please refer to EntryPass Platform1 Server Help File \(F1 button\) 

* i. Wiegand 26-Bits 
* ii. Wiegand 32-Bits 
* iii. Wiegand 34-Bits 
* iv. Wiegand 35-Bits 
* v. Wiegand 37-Bits 
* vi. Custom

### 9. Wiegand Group

Select the Wiegand format created in the Wiegand Group \(For Custom Wiegand Format Only\)

### 10. Wiegand Group Selection

This parameter will allow you to select a maximum of 10 Wiegand formats for the multi-Wiegand controller.

### 11. Activated Time Zone

This parameter will allow you to set the operation time of the reader. By default, this setting will be 1 – 24 hours active i.e., the reader will be active every day for 24 hours. If different Time Zone is applied to this setting, the reader will follow the respective Time Zone while the time outside of that particular time zone, the reader will be rendered ‘inactive’ hence, the reader will not open the required door.

### 12. Enable Access Limit

This parameter will enable you to set Access Limit \(counter\) to the reader. To further understand on what Access Limit is, please refer to 5.7 How to Configure Access Limit Feature.

### 13. Bind To Zone 

This parameter will enable the reader to be bound to a zone for the purpose of Access Limit feature.

### 14. Enable Loop Detector

This parameter will enable the reader to be a loop detector \(CAR PARK FEATURE ONLY\).

### 15. Bypass Access Limit

This parameter will enable the reader to bypass Access Limit feature without resetting the counter.

