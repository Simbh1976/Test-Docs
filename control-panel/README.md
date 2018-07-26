---
description: >-
  This chapter will cover aspects of managing Control Panels for Entrypass
  Platform1 Server
---

# Control Panel

This section will highlight some of the basic settings that you may find useful to an organisations' security protocols. 

## Add New Control Panel

Before proceeding further into the next section, it is important for you to take note that you would need to obtain the **network address** and **port number** of the control panel that you're going to add into the server. To obtain the network address, you can either:

1. get the network address and port number from your System Installer \(SI\) OR
2. follow the method outlined in the manual 'QUICK START-UP GUIDE' in page 3.

The network address and port number is needed for setting up purposes as it is an important piece of information that will resolve the addressing needs of the server. 

## Enabling AES Encryption and changing AES User Key

The Advanced Encryption Standard \(AES\), also known by its original name Rijndael \(Dutch pronunciation: \[ˈrɛindaːl\]\), is a specification for the encryption of electronic data established by the U.S. National Institute of Standards and Technology \(NIST\) in 2001 and is widely adopted by the U.S. Government and worldwide. Within the Control Panel, you can choose to have the data stored to be encrypted with this encryption system so as to secure your data from other third party view. 

Due to the nature of the system where the algorithm is based upon symmetric-key algorithm, meaning the same key is used for both encrypting and decrypting the data, **it is IMPORTANT that you need to take note and have proper safe keeping of User Keys**. If this feature is to be enabled, it is strongly advised that you change the default AES key to a unique number. 

{% hint style="warning" %}
**Default AES Key Number: 123456.** 
{% endhint %}

{% hint style="danger" %}
As highlighted previously, it is important not to lose the AES Key number and the consequence of losing the key number would render the control panel not being able to connect to the P1 Server when Platform1 Server software is reinstalled or undergoing a data migration process. In the event that the User Key is missing and you would like to reconnect the Control Panel back to P1 Server, a ‘Hard Reset’ is required to be performed on Control Panel. During this process, the control panel will delete all data and history stored within.
{% endhint %}



