# Troubleshooting

### Only one battery detected

If you have two batteries connected to Alta X Gen2 but are only seeing one battery in AMC:

* Check that both batteries are on. If one of the batteries doesn't have any LEDs lit up, try pressing the button on the battery to wake it.&#x20;
* Verify that you are in smart battery mode. See the [Battery page](batteries-and-charging.md#switching-battery-modes) for instructions on changing battery mode.
  * Dual battery display in AMC is only supported when smart battery mode is enabled.



### LTE not connecting

If you’re having trouble with LTE connectivity, here’s a few things to check:

* With Alta X Gen2 powered on and connected to AMC via Pilot Pro or a computer, check the LTE status in the dropdown.&#x20;
* Ensure you’ve installed the SIM card properly.
* Check the APN and roaming settings under the Vehicle Overview -> Connectivity -> LTE menu in AMC.
* If you’re in an area with spotty coverage, try moving outside and away from large buildings.&#x20;



### WiFi not connecting

* With Alta X Gen2 powered on and connected to AMC via Pilot Pro or a computer, check the WiFi status in the vehicle connectivity -> Connectivity -> Wi-Fi menu.&#x20;
* Verify in the Wi-Fi tab that the button is on.
* Press the scan icon to search for network.
* Try moving Alta X Gen2 closer to the router or access point.
* Note that when RemoteID is enabled, WiFi's mode switches to serve RemoteID. It is a manual process for the pilot to switch the WiFi's mode to internet connectivity when not flying.

{% hint style="info" %}
5.8GHz WiFi networks have better performance due to less radio interference from the onboard RF
{% endhint %}



### Pilot Pro not connecting (rebind controller)

**For Alta X Gen2 with Herelink radio:**

* Prepare tweezers or paperclip.
* Power on Alta X Gen2 with one battery and the fused cable.
* Turn on Pilot Pro.
*   Wait 30 seconds for the drone to power on, then press the pairing button on the IO panel five times quickly. (The IO panel is located on the bottom side of the aircraft near the nose).

    <figure><img src="../.gitbook/assets/image (14).png" alt="" width="563"><figcaption></figcaption></figure>
* On the Pilot Pro side, locate the pairing button on the Herelink radio. Using tweezers, press and hold the Herelink Air Unit's "Pair/Reset" button until LED blinks (hold approximately 3 seconds).

<figure><img src="../.gitbook/assets/image (22).png" alt="" width="563"><figcaption></figcaption></figure>

* Wait for Pilot Pro and Alta X Gen2 to pair. Once paired, Pilot Pro's power button LED should turn green.



**For Alta X Gen2 with Doodle Labs radio:**

* Make sure Alta X Gen2 and Pilot Pro are at least 6-10’ apart. The Doodle Labs radios are powerful and may interfere with each other at close range.
* Power on Alta X Gen2 with one battery and the fused cable.
* Power on Pilot Pro.
* Give it time. Each radio takes about 60 seconds from power-up to fully boot its system. Ensure both the air and ground radios have been powered on for at least 60 seconds before checking connectivity.
* Open the Pilot Pro App and open the side menu. Navigate to "Radio Settings". Then open "Pairing Manager".

<figure><img src="../.gitbook/assets/image (24).png" alt="" width="563"><figcaption></figcaption></figure>

*   Locate and press the binding button on the IO panel five times quickly. (The IO panel is located on the bottom side of the aircraft near the nose).

    <figure><img src="../.gitbook/assets/image (13).png" alt="" width="563"><figcaption></figcaption></figure>
* Wait for 30 seconds for the radio to go into pairing mode, then press “Scan” on Pilot Pro App.&#x20;
* From the list of results, find the one that matches Alta X Gen2's serial number. Then press pair.
*   Wait 60 seconds for process to complete.

    [<br>](https://freefly.gitbook.io/pilot-pro-public/operating-handbook/radio-modules/doodle-labs-radio-module/doodle-rj45-ethernet-port)
