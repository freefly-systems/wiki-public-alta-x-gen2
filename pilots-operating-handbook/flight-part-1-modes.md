---
description: Understand the Flight Modes available on Alta X Gen2
---

# Flight Part 1 - Modes

Alta X Gen2 offers several flight modes with varying levels of pilot assistance.

Flight mode can be changed via the buttons on Pilot Pro or the AMC app.

<figure><img src="../.gitbook/assets/image (26).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="success" %}
Manual Mode may be necessary to react to emergency situations. Pilots should be proficient in Manual Mode. Position, Altitude, and Return Mode are assistive only and are not a replacement for pilot skill and preparedness.
{% endhint %}

{% hint style="warning" %}
Always neutralize the control input sticks on the pilot handset when switching between control modes to prevent unexpected aircraft movement.
{% endhint %}



***



## Pilot-Controlled Modes

{% tabs %}
{% tab title="Position" %}
<figure><img src="../.gitbook/assets/Pilot position Buttons.png" alt=""><figcaption><p>Position Mode Button on Pilot Pro</p></figcaption></figure>

In Position Mode, when sticks are centered, the aircraft maintains its position over a point on the ground and holds altitude, correcting for disturbances.

**Controls:**

* Pitch/Roll stick → commands ground speed (forward, backward, left, right)
* Throttle stick up/down → commands vertical speed
* Throttle stick left/right → commands yaw rate



{% hint style="info" %}
Position Mode requires a strong GPS signal. If signal deteriorates (near buildings, under tree cover), the aircraft will automatically revert to Altitude Mode.
{% endhint %}

{% hint style="danger" %}
Flight in areas of degraded GPS is not recommended. Automatic reversion to Altitude Mode can cause unexpected changes in flight behavior.
{% endhint %}
{% endtab %}

{% tab title="Altitude" %}
<figure><img src="../.gitbook/assets/Pilot Pro Altitude Button.png" alt=""><figcaption><p>Altitude Mode Button on Pilot Pro</p></figcaption></figure>

Similar to Position Mode, but the aircraft only holds altitude—not lateral position. Alta X Gen2 will drift with the wind and will not hold a fixed point without pilot input.



{% hint style="info" %}
The aircraft holds altitude above Mean Sea Level (MSL) by default. It is not aware of terrain height changes without additional configuration.
{% endhint %}
{% endtab %}

{% tab title="Manual" %}
<figure><img src="../.gitbook/assets/Pilot Pro Manual Button.jpg" alt=""><figcaption><p>Manual Mode Button on Pilot Pro</p></figcaption></figure>

In Manual Mode, the aircraft attempts to remain level when sticks are centered but will drift with wind. Constant throttle adjustment is required to hold altitude.

**Controls:**

* Pitch/Roll stick → commands aircraft angle (tilt)
* Throttle stick → controls motor speed directly
* Throttle left/right → commands yaw rate

**Manual Mode Settings**

The hover throttle setting controls thrust produced when the throttle stick is centered.

* Default: \[TBD]% will hover with no payload
* Approximately \[TBD]% will hover with \[TBD] grams of payload

Adjust hover throttle setting in AMC:&#x20;

* Switch to Advanced Mode by repeatedly tapping on the AMC icon <img src="https://freefly.gitbook.io/astro-public/~gitbook/image?url=https%3A%2F%2F2177404587-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252F8dwrGJhxGd9cIvsStziq%252Fuploads%252FcIXsEaCuTON0v3R1b0cb%252FAMC_icon.jpg%3Falt%3Dmedia%26token%3De5f082e7-eae0-4bf7-9326-fdca0ee01eef&#x26;width=68&#x26;dpr=4&#x26;quality=100&#x26;sign=179222a7&#x26;sv=2" alt="" data-size="line">in the top-left-hand corner of the app.
* Go to Vehicle Setup → Tuning → Hover Throttle<br>
{% endtab %}

{% tab title="Position Slow" %}
<figure><img src="../.gitbook/assets/Pilot Pro pos slow Button.png" alt=""><figcaption><p>Position Slow Mode Button on Pilot Pro</p></figcaption></figure>

Position Slow acts like Position Mode but allows finer control over movement speed using the dials on Pilot Pro. Useful for tower inspections or cinematic shots.

{% hint style="info" %}
The gimbal's dial (left) is always active regardless of mode
{% endhint %}
{% endtab %}
{% endtabs %}



***



## Autonomous Modes

{% tabs %}
{% tab title="Return" %}
<figure><img src="../.gitbook/assets/Pilot Pro return Buttons.png" alt=""><figcaption><p>Return Mode Button on Pilot Pro</p></figcaption></figure>

Return Mode commands Alta X Gen2 to:

1. Climb to the Return Altitude
2. Fly back to the Home Point in a straight line
3. Land



**Key settings:**

* **Return Altitude:** Set it in AMC → Vehicle Setup → Safety. If already above Return Altitude, aircraft maintains current altitude.
* **Home Point:** Automatically set to GPS coordinates where aircraft was armed. Resets every arm.



By default, Return Mode is activated automatically by some Failsafes.

{% hint style="warning" %}
Before every flight, think through the path the aircraft will take if Return Mode activates. Activating Return Mode while under an obstacle lower than Return Altitude will cause a collision.
{% endhint %}

{% hint style="info" %}
You can exit Return Mode by pressing another flight mode button.
{% endhint %}



### **Return behavior based on position:**

In most cases, RTL mode will travel to the predetermined RTL altitude, travel over the home point, and automatically descend to land. However, if the aircraft is close to the home point, the behavior will be slightly different in order to save time and reduce the amount of distance Astro will need to move.

<figure><img src="../.gitbook/assets/Generated Image January 23, 2026 - 3_02PM.jpeg" alt="" width="375"><figcaption></figcaption></figure>

| Position                          | Behavior                                       |
| --------------------------------- | ---------------------------------------------- |
| Directly over home point          | Land without gaining altitude                  |
| Within a few meters of home       | Move over home point, land                     |
| <20m altitude AND <20m distance   | Climb to 20m, move over home, land             |
| 20-35m altitude AND <20m distance | Maintain altitude, move over home, land        |
| >35m altitude OR >20m distance    | Climb to Return Altitude, move over home, land |

&#x20;
{% endtab %}

{% tab title="Takeoff" %}
Takeoff Mode arms the aircraft, climbs to the Takeoff Altitude, and enters Hold Mode (hover in place).

Can be engaged via AMC Fly view button or as the first command in a mission.

{% hint style="info" %}
Takeoff Mode requires a GPS lock.
{% endhint %}
{% endtab %}

{% tab title="Landing" %}
### Landing Mode

Landing Mode descends and lands directly below current position. Aircraft disarms after touchdown.

Engage via AMC Fly view button (hold to confirm).&#x20;

Also used as the last command in missions or triggered by some failsafes.

{% hint style="warning" %}
Land Mode requires GPS when engaged manually. If engaged by failsafe without GPS, aircraft descends like Altitude Mode and may drift.
{% endhint %}
{% endtab %}

{% tab title="Mission" %}
Mission Mode executes a predefined autonomous waypoint mission uploaded via AMC.

See AMC documentation for:

* [Planning a mission](https://freefly.gitbook.io/astro-public/astro/pilots-operating-handbook/software/auterion-mission-control/amc-plan#example-mission)
* [Flying a mission](https://docs.auterion.com/auterion-mission-control/fly/flying-a-mission)
* [Remove a mission from the aircraft](https://docs.auterion.com/auterion-mission-control/plan/plan-ui-overview#file-sync-tools)

{% hint style="danger" %}
Starting a mission can cause the aircraft to arm and take off without further input. Ensure area is clear.
{% endhint %}

{% hint style="info" %}
If a mission is interrupted (e.g., pilot switches to Position), AMC will prompt to resume. If no prompt, use Action Menu → Resume Mission.
{% endhint %}

<figure><img src="../.gitbook/assets/image (27).png" alt="" width="180"><figcaption></figcaption></figure>

{% hint style="info" %}
Aircraft must have GPS lock before takeoff to start a mission. If armed without GPS lock, Mission Mode will be unavailable until landing and rearming with GPS.
{% endhint %}
{% endtab %}
{% endtabs %}





