# Flight Part 2 - Operation

{% hint style="warning" %}
Make sure you understand Alta X Gen2's [Emergency Procedures](flight-part-3-emergency-procedures.md) and can operate in [Manual Mode](flight-part-1-modes.md#manual) before taking flight.
{% endhint %}

## Flight Checklists

Below is our recommended checklist and emergency procedures, which covers the main considerations you need to be aware of before, during, and after operation.

{% file src="../.gitbook/assets/Alta X Gen2 Checklists and EPs - V1.pdf" %}

We also offer this checklist as a [Google Sheet template](https://docs.google.com/spreadsheets/d/1JPw9swa9Qgde6kN0BwlyTe5oQbtJ-K0krS4xsyxAoW8/edit?usp=sharing) for customization to your company's procedures, workflow, or region.



***



## Before Flight

#### Powering On Pilot Pro

* Press the power button once to wake it up and to check its charge level. Press a second time to power it on.
* Once the Tablet boots, the Pilot Pro App will open. Switch to AMC app for flight.



#### Powering On Alta X Gen2

* Alta X Gen2 is powered by connecting the Tattu batteries — no power button required.
* **For ground/bench operations:** Connect one battery using the fused cable. This prevents arming as a safety mechanism.
* **For flight:** Connect two batteries directly (no fused cable). Both batteries power on automatically when connected.

{% hint style="warning" %}
Bench mode (single battery + fused cable) is not a substitute for the absolute safety of removing propellers.
{% endhint %}



#### Checking Battery Levels

* Once connected, AMC displays Alta X Gen2 battery level in the status bar. Tap the battery indicator to see more details, such as per-battery values.

<figure><img src="../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The LED indicator on the Tattu battery itself can be inaccurate. For accurate state of charge, check via the Tattu Smart Charger or AMC.
{% endhint %}



***



## Arming and Disarming

Alta X Gen2 has two states:

| State    | Definition                         | Boom LEDs |
| -------- | ---------------------------------- | --------- |
| Disarmed | Safe, propellers will not spin     | Dim       |
| Armed    | Ready to fly, propellers will spin | Bright    |

* Alta X Gen2 can arm with or without GPS.
* Pro Tip: Wait for GPS lock even if you don't plan to use Position Mode because Return Mode relies on GPS.
* Missions with a takeoff command will arm automatically when initiated.

{% hint style="danger" %}
Before arming, ensure people and other obstacles are clear of the propellers.&#x20;
{% endhint %}





#### Arming and Disarming with Sticks (Mode 2)

| Action    | Input                                                             |
| --------- | ----------------------------------------------------------------- |
| Arming    | Hold throttle stick down and right for 2 seconds                  |
| Disarming | After landing, continue holding throttle stick down for 2 seconds |

* You cannot disarm via sticks while in flight. Use Emergency Stop if needed.
* Use only the throttle stick. Alta X Gen2 does not respond to two-stick arming gestures (i.e. DJI arming gesture)
* The pilot's handset default configuration is [Mode 2](https://docs.px4.io/master/en/getting_started/rc_transmitter_receiver.html#types-of-remote-controls).



#### Automatic Disarm

Under these conditions, Alta X Gen2 will automatically disarm.

| Condition           | Behavior                                                 |
| ------------------- | -------------------------------------------------------- |
| Ground timeout      | If armed but idle on ground for 10 seconds, auto-disarms |
| Return or Land mode | After detected landing, disarms after 2 seconds          |



***



## Taking Off

Position Mode is recommended for takeoff in most cases.

For 5 seconds after takeoff, maximum pitch and roll angles are limited to 12 degrees.

> **Tip:** After takeoff, promptly climb above 3 meters (10 feet) to exit ground effect and avoid snagging landing gear.

#### In Position or Altitude Mode

1. After arming, allow throttle stick to return to center—propellers remain at idle
2. When ready, raise throttle stick
3. Propellers spin up and aircraft takes off

#### In Manual Mode

1. After arming, hold throttle stick straight down (no yaw input)
2. Slowly raise throttle—propellers accelerate immediately
3. As throttle approaches mid-point, aircraft will lift off
4. Continue raising throttle for a brisk takeoff



***



## Landing

Position Mode is recommended for landing in most cases.

{% hint style="danger" %}
Do not hand catch Alta X Gen2. Land on hard, flat surfaces only. Hand catching can result in serious injury or death.
{% endhint %}

In Position and Altitude Modes

* Below 7 meters altitude, maximum descent rate is reduced to 0.7 m/s (from 2 m/s).
* Below 2 meters altitude, maximum pitch/roll angle is reduced to 12 degrees to prevent tip-overs.

Alta X Gen2 disarms automatically after detecting landing. Landing detection brings together input from several sensors to determine when it is safe to disarm.

{% hint style="warning" %}
If landing is not detected (props keep spinning after touchdown), see Emergency Procedures for Landing Detector Failure.
{% endhint %}

#### Landing best practices

{% tabs %}
{% tab title="Landing In Position Mode" %}
1. Hover above 2 meters over landing spot
2. Pull throttle straight down—no pitch, roll, or yaw input
3. Landing sensor manages descent speed
4. After touchdown, hold throttle down until disarm

{% hint style="warning" %}
Pitch, Roll, or Yaw commands very near the ground can cause crashes or tip-overs.
{% endhint %}
{% endtab %}

{% tab title="Landing In Altitude Mode" %}
1. Hover above 2 meters over landing spot
2. Use minimal pitch/roll to control lateral drift
3. Pull throttle down—autopilot controls descent rate
4. After touchdown, hold throttle down until disarm
{% endtab %}

{% tab title="Landing In Manual Mode" %}
Landing in Manual Mode is different than Position or Altitude Mode because the pilot is responsible for managing vertical _and_ lateral velocity.

1. Hover above 2 meters over landing spot
2. Use minimal pitch/roll to minimize lateral speed
3. Reduce throttle to descend slowly
4. Near ground (in ground effect), reducing throttle further is often needed to keep the aircraft descending
5. After touchdown, reduce throttle to zero promptly
6. Hold throttle down until disarm and propellers stop completely
{% endtab %}
{% endtabs %}



{% hint style="danger" %}
While Alta X Gen2 will recognize that the battery is low and perform a failsafe action (return to launch by default), the aircraft has no context of situations that might prevent a safe landing before the battery is exhausted. For instance, if the aircraft is several miles away from the RTL point when the failsafe is triggered, there is a chance that there won't be enough battery life to return. \
\
It is the pilot's responsibility to determine the appropriate time for a battery change and to ensure the aircraft is safely grounded.
{% endhint %}







