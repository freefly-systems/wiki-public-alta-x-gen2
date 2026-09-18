# Interfaces

Alta X Gen2 was designed to be easy to integrate custom payloads with a variety of electrical and communications interfaces.

### **USB-C** <a href="#usb-c" id="usb-c"></a>

<figure><img src="../.gitbook/assets/image (4).png" alt="" width="563"><figcaption></figcaption></figure>

The USB-C connector is located on the top side chassis next to the battery connectors.&#x20;

By default it is configured as an ethernet adapter.

Functionality:

* connection to payload
* mass storage (e.g. flash drive)
* firmware updates

It is not possible to power Alta X Gen2 via this port.

### IO Panel

The IO panel is located in the forward bay door underneath the aircraft.

<figure><img src="../.gitbook/assets/Screenshot from 2026-01-23 10-06-17.png" alt="" width="563"><figcaption></figcaption></figure>



#### Payload <a href="#payload" id="payload"></a>

Connector type: JST-ZPD 26-pin

<img src="https://docs.freeflysystems.com/~gitbook/image?url=https%3A%2F%2F2177404587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F8dwrGJhxGd9cIvsStziq%252Fuploads%252FoghmzxVQ6TylbwpFXAEs%252FScreenshot%25202023-10-26%2520170726.png%3Falt%3Dmedia%26token%3D982c4c82-f7d3-4dc2-94d2-127d7e09d822&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=56923bb2b8b2438316eda766453c6300&#x26;sv=3" alt="" width="563">

This connector can be accessed directly or to pass connections to the [Smart Dovetail](https://docs.freeflysystems.com/astro/other-user-manuals/ecosystem/development-tools/payload-mounting-interfaces#smart-dovetail) connector.

The mating connector to build a payload cable is [ZPDR-26V-S](https://www.digikey.com/en/products/detail/jst-sales-america-inc/ZPDR-26V-S/2472569).

PAYLOAD\_VBAT is 24V DC regulated, and is electronically fused at 6A. If the e-fuse trips, it will reset when the aircraft is power cycled. The e-fuse includes soft start protection for use with loads with high inrush current.&#x20;

#### TELEM3  <a href="#telem3" id="telem3"></a>

Connector: JST GH 6-pin

<img src="https://docs.freeflysystems.com/~gitbook/image?url=https%3A%2F%2F2177404587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F8dwrGJhxGd9cIvsStziq%252Fuploads%252FgaZdw4SHanYhxntihbqU%252Ftelem3.png%3Falt%3Dmedia%26token%3D14bf6f40-38cc-490b-a1f6-0ac045d72c16&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=5004655c5732a45627a4ab3253d9d0d7&#x26;sv=3" alt="" width="563">

#### **AUX UART** <a href="#aux-uart" id="aux-uart"></a>

Connector: JST GH 6-pin

<img src="https://docs.freeflysystems.com/~gitbook/image?url=https%3A%2F%2F2177404587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F8dwrGJhxGd9cIvsStziq%252Fuploads%252FBuwsHnbNJoCk7GL4t0UQ%252Faux%2520uart.png%3Falt%3Dmedia%26token%3Db1c70606-847e-4833-874b-ce5b11ebe838&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=cc221224167075888a1da3390715fcd3&#x26;sv=3" alt="" width="563">

#### **PWM** <a href="#pwm" id="pwm"></a>

Connector: pin headers, 0.1 inch spacing

<img src="https://docs.freeflysystems.com/~gitbook/image?url=https%3A%2F%2F2177404587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F8dwrGJhxGd9cIvsStziq%252Fuploads%252FhP7ydhl78FVGOmiELR8R%252Faux%2520io%2520pwm.png%3Falt%3Dmedia%26token%3D0c51c737-e095-4dbd-b19c-47567646263a&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=7dd4addc8c6144374b5fef6aa30f222e&#x26;sv=3" alt="" width="563">

PWM outputs are active when the aircraft is powered on.

The PWM outputs on the Alta X Gen2 are controlled with the PWM\_AUX\_FUNC parameter where FUNC1-4 are the 4 PWM outputs. To assign a PWM output to a mapping, just find the number of the PWM output, and the associated PWM\_AUX\_FUNC and assign it to the desired mapping. ie, if you use RC AUX 1, it should use Dial 2 to control the PWM output.PWM output values (e.g. 1100 us) are controlled by these parameters (read more in the [PX4 Parameter Reference](https://docs.px4.io/main/en/advanced_config/parameter_reference#parameter-reference)).

| Parameter       | Function                                                                                                                                                    |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| PWM\_AUX\_DIS1  | PWM output when autopilot is not armed. When set to -1 the value for PWM\_AUX\_DISARMED will be used. a similar parameter is available for each channel     |
| PWM\_AUX\_MIN1  | Minimum PWM pulse for this output. When set to -1 the value for PWM\_AUX\_MIN will be used.                                                                 |
| PWM\_AUX\_MAX1  | Maximum PWM pulse for this output. When set to -1 the value for PWM\_AUX\_MAX will be used.                                                                 |
| PWM\_AUX\_REV1  | Invert direction.                                                                                                                                           |
| PWM\_AUX\_FAIL1 | PWM output if autopilot is in failsafe mode. When set to -1 the value is set automatically depending if the actuator is a motor (900us) or a servo (1500us) |

#### Ethernet

Connector: JST GH 6-pin

<figure><img src="../.gitbook/assets/image (2).png" alt="" width="563"><figcaption></figcaption></figure>

This Ethernet port is connected to the Ethernet switch on the IO panel and connects to the payload and Skynode.

A secondary RJ45 jack is also available inside the tub on the IO panel PCBA. This is connected to the same Ethernet switch as the ENET GH connector.&#x20;

<figure><img src="../.gitbook/assets/image (3).png" alt="" width="563"><figcaption></figcaption></figure>



#### XT30 Power

The XT30 connector supplies regulated 24V DC power. It's electronically fused at 6A. If tripped, it will reset when the aircraft is power cycled.  This 24V source is shared with the other 24V connection points on the aircraft. The e-fuse includes soft start protection for use with loads with high inrush current.&#x20;



### External Power Connectors

In the rear bay of the aircraft, there are external facing power connectors.&#x20;

Both of these are regulated from the battery voltage.&#x20;

* 12V is available up to 120W or 10A.&#x20;
* 24V is available up to 240W or 10A.&#x20;



### Rear Power Connections

Alta X Gen2 provides power connections inside and outside the aircraft tub. This is useful for integrations that sit in the payload bay, or for devices that are attached outside of the tub.&#x20;

<figure><img src="../.gitbook/assets/image.png" alt="" width="563"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1).png" alt="" width="563"><figcaption></figcaption></figure>

#### 12V power

12V power is available on XT60 connectors, one internal and one external.&#x20;

Max current draw is 10A/120W

#### 24V power

24V power is available on the XT30 connectors on the DC-DC regulator, one internal and one external. This source is shared with the payload ZPD connector and the IO panel XT30 connector.

Max current draw is 10A/240W

{% hint style="warning" %}
VBAT (\~44V) is also available on an XT30 connector, always double check the voltage on the connector before plugging something in.
{% endhint %}

{% hint style="warning" %}
Keep in mind, when drawing power from the 12V or 24V regulators on the ground, the heatsink may become warm to the touch. Once in flight, airflow around the aircraft helps keep it cool.
{% endhint %}

#### VBAT power

The battery breakout board includes 4x XT30 connectors fused at 10A each. One of these feeds the 12/24V DC-DC regulator, but the remaining connectors are available for use.&#x20;

These are electrically connected directly to the battery bus, nominally 44.4V (12S LiPo).

### Onboard Network Connectivity

The Ethernet switch on Alta X Gen2 provides connectivity to attach payloads or custom devices to the aircraft's onboard network. Any device on the switch can access any other devices connected to the switch, including the Skynode and Payload.&#x20;

The internal network is setup with the subnet 192.168.144.0/24, with subnet mask 255.255.255.0.&#x20;

IP addresses are statically allocated. The reserved addresses include:

| IP             | Endpoint      |
| -------------- | ------------- |
| 192.168.144.10 | Airside Radio |
| 192.168.144.11 | Pilot Pro     |
| 192.168.144.12 | Ground Radio  |
| 192.168.144.20 | Skynode       |

Ethernet based payloads generally have reserved IP addresses that vary per payload.

To connect a custom device, we recommend using an IP address in the range of

&#x20;`192.168.144.200` -  `192.168.144.255`.

{% hint style="info" %}
The radio link to the ground has limited bandwidth, and the internal network is 10/100mb Ethernet. Be mindful of the bandwidth needs of custom devices when connecting them to the aircraft to not overload the network.
{% endhint %}
