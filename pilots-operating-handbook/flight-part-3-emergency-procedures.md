# Flight Part 3 - Emergency Procedures

## General Guidance

**Human safety must be the top priority. Aircraft can be replaced. People cannot. Always prioritize the safety of yourself and others over the preservation of aircraft or equipment.**

Emergency situations are dynamic events, that will not often conform perfectly to the categories listed below. A thorough understanding of aircraft systems, proficiency in piloting the aircraft, and sound judgment will allow you to bring about the best possible outcome in an emergency.

The likelihood of an emergency can be reduced substantially through proper aircraft maintenance, the use of [checklists for normal procedures](flight-part-2-operation.md#flight-checklists), and careful pre-flight planning. The likelihood of a safe flight often depends on the diligence of the pilot, both before taking off and during operation.

In general, if an emergency occurs, three basic actions can be applied to most situations:

1. Maintain aircraft control — Small emergencies can quickly escalate if the pilot is distracted attempting to troubleshoot the problem. Always maintain visual contact with the aircraft during an emergency to reduce the likelihood of losing orientation.
2. Analyze the situation — Once the aircraft is stabilized, assess the cause of the emergency.
3. Take appropriate action — In many cases, the appropriate action will be to land the aircraft as soon as possible. Aircraft can be replaced.&#x20;

### Return Mode

Do not be over-reliant on [Return Mode](flight-part-3-emergency-procedures.md#return-mode) in emergencies. The cause of the emergency may degrade or disable Return Mode (e.g., GPS loss disables Return Mode).

By default, stick movements do not interrupt Return Mode. Press a flight mode button to exit Return Mode.



***



## Emergency Checklists

The flight [checklists](flight-part-2-operation.md#flight-checklists) contain concise instructions to follow to mitigate risk in the event of an in-flight emergency. Some of these situations are discussed in more detail below.

{% tabs %}
{% tab title="Orientation Loss" %}
### Loss of Orientation

If orientation is lost, neutralize inputs and activate position mode. Then work to identify the front of the aircraft.

We recommend identifying the front of the aircraft via a "guess and check" method of small roll right inputs alternating with yawing the aircraft 90 degrees at a time. We recommend a roll input rather than pitch because at a distance it is easier to see lateral motion than fore/aft motion.

If it is not possible to identify orientation, and it is safe to activate Return Mode, do so. By default in Return Mode, after climbing, the aircraft will yaw to put the front toward the direction of flight.

Resume flying or land as necessary.
{% endtab %}

{% tab title="Unexpected Behavior" %}
### Unexpected Aircraft Behavior

If aircraft behaves unexpectedly, do the following: neutralize inputs, activate Position Mode, and observe the aircraft. If it is still flying in an uncommanded manner in Position or Altitude Mode, switch to Manual Mode.&#x20;

In some cases, unexpected behavior is due to degraded GPS signal or erroneous sensor readings (e.g. compass error). In such cases, Return Mode may not behave reliably. Manual Mode does not rely on these sensors.

Land as soon as possible.
{% endtab %}

{% tab title="Landing Detector Failure" %}
### Landing Detector Failure

If the aircraft touches down, but hops back up into the air several times, or sits on the ground with the props continuing to spin, the autopilot may not have detected a landing. Climb and retry landing with a greater downward velocity.

{% hint style="info" %}
Landing the aircraft firmly will give the accelerometers and gyroscopes a sufficient contrast between flight and landing.
{% endhint %}

If an attempted landing is unsuccessful in Position and Altitude mode, land in Manual Mode.

If an attempted landing is unsuccessful in Manual Mode, perform an Emergency Stop (see below) with the aircraft on the ground or as close as possible.
{% endtab %}

{% tab title="GPS Loss" %}
### Loss of GPS

If GPS is lost, flight modes that rely on GPS (Position, Return, Mission, etc) will not be available. If the aircraft is in Position mode when GPS is lost, the autopilot will switch to Altitude Mode. If the aircraft is in Return or Mission modes when GPS is lost, it will automatically start landing. Landing can be overridden by the pilot by changing modes to Altitude or Manual modes.

{% hint style="info" %}
It is the pilot's responsibility to be proficient with Altitude and Manual Mode and to have the aircraft configured to behave safely if GPS is lost.
{% endhint %}

Examples of behavior without GPS:

* If GPS is not available upon arming, no Home Point is set, and Return Mode is not available. Even if GPS becomes available while flying, Return Mode will not be available.
* If the pilot commands Return Mode, the aircraft will remain in Altitude or Manual Mode, and an error will be displayed on the pilot handset.
* If Land Mode is activated (e.g. by a failsafe), the aircraft will descend as though in Altitude mode, maintaining a consistent descent but drifting with the wind.
* If GPS is lost in Position, the aircraft will display a warning and switch flight mode to either Altitude Mode or Manual Mode, depending on the degradation of the signal and other sensors
* If GPS is providing altitude information (e.g. while using RTK GPS), and GPS is lost, the ability of Altitude Mode to accurately maintain altitude may be affected.
{% endtab %}

{% tab title="RC Loss of Signal (LOS)" %}
### RC Loss of Signal (LOS)

RC Loss of Signal (LOS) can occur if the pilot handset signal is degraded or stops, or if aircraft does not receive the signal due to distance or interference (e.g. from obstacles or other radio signals).

If the signal is lost longer than the RC Timeout, a failsafe action will be triggered. The RC Timeout is quite short by default: 0.5 seconds. The pilot may not have time to react before the failsafe action is activated. By default, the failsafe action is Return Mode.

If the signal is lost, check the pilot's handset power and [antenna orientation](pro-tips-and-limitations.md#antenna-positioning). Antenna orientation is especially important when Astro is far from the pilot.

If the signal is recovered, the pilot will be able to take control by pressing a flight mode button.
{% endtab %}

{% tab title="Video Loss" %}
### Loss of Video Signal

Loss of Video Signal can occur if the aircraft flies out of range or if it flies behind an object that interrupts the signal. Maintaining visual contact is the preferred method to re-establish control of the aircraft, either with the pilot seeing the aircraft or by the use of a visual observer.

Yawing the aircraft can help signal reception if the body of the aircraft is blocking the line of sight between the transmitter and receiver antennas.

If video signal or visual contact cannot be re-established, enable Return Mode to bring the aircraft back to signal reception range.

{% hint style="danger" %}
It is the responsibility of the pilot to see and avoid other aircraft, people, or obstacles. Always maintain a direct line of sight with Astro during flight, use visual observers as operations require, and follow local regulations regarding see-and-avoid requirements.
{% endhint %}
{% endtab %}
{% endtabs %}



***



## Emergency Stop

{% hint style="danger" %}
#### As a last resort, if it is not possible to land or control the aircraft, perform an Emergency Stop. If performed while flying, this will cause the aircraft to crash. Perform the Emergency Stop as far away from people as possible.
{% endhint %}

There are three ways to initiate emergency stop:

* Pilot Pro: Flip open the red Kill Switch cover and pull the Kill Switch down
* Pilot Pro: In Manual Mode, hold the throttle stick down and left for 10 seconds.
* AMC: Tap "Armed" button (top center of screen) and swipe/hold to shut down. This will work even when the aircraft is airborne.



***



## Failsafes

Failsafe behavior and settings are configured in AMC. The [AMC documentation ](https://docs.auterion.com/vehicle-operation/settings-and-maintenance/safety)covers each failsafe and related settings in detail.

{% hint style="warning" %}
We strongly recommend using the default settings, changing only Return Altitude, unless you are an expert user and have tested the effect of changes thoroughly.
{% endhint %}

#### Low Battery Failsafe

As the battery level becomes low, the autopilot can take action. The default settings do not interfere until the battery becomes quite low. Additionally, low battery failsafes are only able to estimate how long it will take the aircraft to return to the home point. This means it is the pilot's responsibility to be aware of the battery level and ensure the aircraft is on the ground.

Autopilot uses a variety of inputs to warn or take action.&#x20;

* State of Charge (SoC) of the batteries.&#x20;
* Onboard voltage measurement.
* Complex time to home estimation based on flight characteristics

| State     | Triggered By                | Action       |
| --------- | --------------------------- | ------------ |
| Warning   | 30% SoC                     | Warning only |
| Critical  | 20% SoC                     | Return Mode  |
| Critical  | Distance to home estimation | Return Mode  |
| Emergency | 10% SoC                     | Warning only |
| Emergency | 43.5 Volts                  | Warning only |

{% hint style="info" %}
When activated by a low battery failsafe, Return and Land Mode cannot be overridden by stick movement. They can be overridden by pressing a flight mode button (e.g. Position).
{% endhint %}



***



## Error and Warning Indication&#x20;

The aircraft communicates the presence of errors and warnings primarily through Auterion Mission Control (AMC) [status indicators](https://docs.auterion.com/auterion-mission-control/fly/fly-view-ui-overview#vehicle-status-indicators-top-bar) on the pilot handset or PC. Many messages are accompanied by an audible message (e.g. "Return Flight Mode"). Additionally, Alta X Gen2 boom LEDs will flash when the battery level is critical.&#x20;

Status messages, including errors and warnings, are stored in Flight Logs. After any emergency, review the log to determine the source of the problem.

If the meaning of an error or warning is not clear, please [contact Freefly Support](https://freeflysystems.com/contact). Share as much detail as possible, including sharing the flight log.

