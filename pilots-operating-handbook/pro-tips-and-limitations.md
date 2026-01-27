# Pro-tips and Limitations

It is possible to operate Alta X Gen2 close to the limits of performance by maintaining awareness of the performance envelope, how the aircraft behaves if the limits are exceeded, and best practices for operating in harsh environments.

This page reflects the limitations of the most current version. As the Alta X Gen2 platform matures, limitations are likely to change.&#x20;





***

## Radio Range and Interferences <a href="#radio-range-and-interferences" id="radio-range-and-interferences"></a>

Operating with a weak signal, whether due to interference or long range, can cause loss of link with the aircraft, which will engage failsafes. If you anticipate a weak signal situation, double-check that failsafes are set appropriately.

### Range <a href="#range" id="range"></a>

The range of Herelink and Doodle radios on Alta X Gen2 is approximately 2 km in ideal conditions, assuming there are no interferences and the antennas are positioned correctly.

### Antenna Positioning <a href="#antenna-positioning" id="antenna-positioning"></a>

This is one of the simplest to miss and impact the range of the flight

**Pilot Pro**

Both the Doodle and Herelink radio modules on Pilot Pro use two blade antennas that are omni directional. It is important to follow these basic guidelines:

* Antennas should both point in the same direction.
* Antennas should point towards ground or sky.
* Minimize how much the antennas are getting blocked in close proximity. For instance, if you are using the Pilot Pro with the tablet in the open configuration, then pointing antennas towards ground instead of sky is usually better.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

### Interferences <a href="#interferences" id="interferences"></a>

Range can be reduced by radio interference from other sources like WiFi networks. Obstacles like trees and buildings in close proximity to the controller or Alta X Gen2, as well as directly between the two, can dramatically reduce range.

#### Multiple Aircraft <a href="#multiple-aircraft" id="multiple-aircraft"></a>

* Alta X Gen2's Doodle radio configuration runs on dedicated peer to peer channels. In order to fly multiple Alta X Gen2 or Astro aircraft in the same airspace, make sure to scan channels and then set each Doodle to a different channel.
* Alta X Gen2's Herelink radios are channel hopping by default. 4 aircraft can fly simultaneously in the same airspace in practice. If more aircraft are present, interference can cause loss of radio link and control.





***

## Environment

### Temperature

Alta X Gen2 can operate between -20 and 50 C. Position mode and survey flying are normal throughout the range. However, care is needed to operate at low and high temperatures.

{% tabs %}
{% tab title="Tips for operating in hot environments" %}
At high temperatures, the limiting factor is battery temperatures. AMC will display a warning if the batteries become too hot. Heed the warnings! Alta X Gen2 operates normally in forward flight up to 15 m/s with a full payload.&#x20;

Cooling air is your friend. The system gets much more cooling air in forward flight than in a hover. Overheat errors may occur when hovering because there is less airflow, or when flying aggressively because heating increases with current.

Batteries may require cooling before charging. Bring an extra set of batteries and chargers to enable continuous flying.

Keep the equipment out of prolonged direct sunlight.
{% endtab %}

{% tab title="Tips for operating in cold environments" %}
At low temperatures, the battery cell temperature is the key limiting factor. When the cells themselves are below 10 °C (ambient air can be down to -20 °C), the batteries' performance may be reduced. If this happens, low battery failsafes (RTL and Land) will be triggered, causing the aircraft to climb or descend suddenly.

These failsafes can be overridden by selecting another flight mode. The battery will not cut off power output in the air, however low temperatures generally reduce capacity which will reduce flight time.

If the batteries are 10 °C or warmer at the start of a flight, heating from discharge will keep them warm enough to fly.

To keep batteries warm, charge them in a heated environment and store them in an insulated container (a cooler works well)​.&#x20;

**In rare cases propellers can experience icing, this occurs when ice begins to form on the tips and underside of the blades due to temperature and humidity. This will cause the props to become unbalanced, increasing drag and reducing lift. Flying with iced blades can be dangerous and is not advised.**
{% endtab %}
{% endtabs %}

### Ingress

Alta X Gen2 is designed to withstand light rain ([IP43 rated](../specs/tech-specs.md#environmental)). Ensure the IO panel, voltage regulator, and USB covers are installed when flying in dusty or wet conditions.

When flying in rain, we have seen some instances where water ingresses to the battery through the balance lead port. This may cause the battery’s BMS to report incorrect information. To prevent this, we include stickers to cover the balance port on the batteries. See [here](../maintenance/batteries-and-charging.md#installing-the-battery-balance-port-stickers) for instructions on installing them.
