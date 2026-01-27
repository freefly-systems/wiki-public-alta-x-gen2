# Batteries and Charging

Alta X Gen2 is designed to fly with two Tattu Plus 1.0 12S 16Ah LiPo batteries. The battery voltage bus runs between 36 and 50.4 volts.&#x20;

In an emergency, the aircraft is capable of flying and landing safely on one battery.

It is not possible to power the aircraft via the USB-C port.

{% hint style="warning" %}
Battery hot swaps are not recommended. Please power off the aircraft by disconnecting both batteries when swapping packs to ensure ideal performance and battery lifespan.
{% endhint %}





## Charger

The Tattu TA3200 smart charger is the recommended charger. It supports dual battery charging, and single connector charging through the AS150U connector.&#x20;

<figure><img src="../.gitbook/assets/AltaXGen2-045.jpg" alt="" width="563"><figcaption></figcaption></figure>

For more information, see the charger's [user manual](https://www.genstattu.com/content/TA3200TA3200HVManual.pdf).





***

## Batteries

Alta X Gen2 is designed to operate with two Tattu Plus 1.0 12S 16Ah smart batteries with AS150U connectors.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>





***

## Installing the Battery Balance Port Stickers

When flying in rain, we have seen some instances where water ingresses to the battery through the balance lead port. This may cause the battery’s BMS to report incorrect information. To prevent this, we include stickers to cover the balance port on the batteries. If you need more stickers, contact [Freefly Support](https://freeflysystems.com/contact). <br>

**You will need:**

* Tattu Plus 1.0 12S 16Ah smart battery
* Balance port sticker
* Alcohol swab (included with the sticker)

<figure><img src="../.gitbook/assets/unknown (24).png" alt="" width="563"><figcaption></figcaption></figure>

1. On the Tattu Plus 1.0 12S 16Ah smart battery, fully seat the rubber cover on the balance port and remove the warning sticker.

<figure><img src="../.gitbook/assets/unknown (25).png" alt="" width="563"><figcaption></figcaption></figure>

<br>

2. Use the included alcohol wipe to clean off any dust, dirt, or residue from the area marked below.&#x20;

<figure><img src="../.gitbook/assets/unknown (26).png" alt="" width="563"><figcaption></figcaption></figure>

3. Once dry, apply the sticker over the cover with the tab poking out through the hole in the sticker. Use firm pressure to ensure adhesion.&#x20;

<figure><img src="../.gitbook/assets/unknown (27).png" alt="" width="563"><figcaption></figcaption></figure>





***

## Switching Battery Modes

{% hint style="danger" %}
This is an advanced feature and not recommended for normal use.&#x20;
{% endhint %}

Alta X Gen2 ships in smart battery mode. This mode enables the aircraft to communicate with the batteries' BMSs for:

* Better flight time estimation
* Battery fault monitoring
* Requires two batteries to arm

We recommend leaving Alta X Gen2 in this default configuration and flying with the recommended smart batteries.

The battery mode can be changed to disable smart battery mode. This enables flying with other batteries (like Alta X Gen1 flight batteries) or non-traditional power systems. To change this, follow the instructions below to change the mode.&#x20;

**To change the mode:**

1. Power on Alta X Gen2 with one battery and the fused cable.&#x20;
2. Power on Pilot Pro or connect a PC with a USB-C cable.
3. Open AMC, then press the upper left icon 7 times to enter Advanced mode.&#x20;
4. Click the icon again to open the side menu, then navigate to Advanced -> Parameters.&#x20;
5. Enter "FF\_AX2\_BAT\_CFG" in the search box, then select the FF\_AX2\_BAT\_CFG parameter.
6. Enter the new value, the click Save.
   1. To enable Smart Battery mode (enabled by default) set this parameter to 2.
   2. To disable Smart Battery mode set this parameter to 0.&#x20;
7. Once saved, reboot the aircraft.





***

## Replacing the fuse in the fused cable

Alta X Gen2 includes an inline power cable with a protective fuse designed for ground operations. Install it between a single battery and the aircraft when performing maintenance, updates, configuration, or other work near the drone. In the event that the fuse blows, it can be replaced with a 5A mini automotive blade fuse.&#x20;

<figure><img src="../.gitbook/assets/unknown (11).png" alt="" width="563"><figcaption></figcaption></figure>

1. Open the rubber cover in the fused cable.

<figure><img src="../.gitbook/assets/unknown (12).png" alt="" width="563"><figcaption></figcaption></figure>

2. Remove the old fuse.

<figure><img src="../.gitbook/assets/unknown (13).png" alt="" width="563"><figcaption></figcaption></figure>

3. Replace with a 5A mini automotive blade fuse. Note: Do not use a higher current rating fuse in this cable.&#x20;

<figure><img src="../.gitbook/assets/unknown (14).png" alt="" width="563"><figcaption></figcaption></figure>

4. Close the rubber cover.

<figure><img src="../.gitbook/assets/unknown (15).png" alt="" width="563"><figcaption></figcaption></figure>

<br>
