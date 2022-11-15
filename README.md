# lead acid battery charger

## **A Study of Charging Control of Lead-Acid Battery for Electric Vehicles**

### Battery Charging Control iMethods

Constant current charging

charging currents for the series connected batteries are equal. However, battery overcharging will result in the degradation of battery life. Small charging current will prolong the charging time.

In this method of charging the batteries are connected in series so as to form groups and each group charges from the DC supply mains through loading rheostats. The number of charging in each group depends on the charging circuit voltage which should not be less than the 2.7 V per cell.

The charging current is kept constant throughout the charging period by reducing the resistance in the circuit as the battery voltage goes up. In order of avoiding excessive gassing or overheating, the charging may be carried out in two steps. An initial charging of approximately higher current and a finishing rate of low current.

In this method, the charge current is approximately one-eighth of its ampere ratings. The excess voltage of the supply circuit is absorbed in the series [resistance.](https://circuitglobe.com/what-is-a-resistance.html) The groups of the battery to be charged should be so connected that the series resistance consumes as little energy as possible.

The current carrying capacity of series resistance should be greater than or equal to the required charging current otherwise, the resistance will overheat and burn out.

The group of batteries which is to be selected should have the same capacity. If the battery has a different capacity, then they will have to be set according to the least capacity.

Constant voltage charging

During the initial stage of charging the possible large charging currents need to be limited to protect devices. When the battery voltage reaches the default value. charging voltage is hold and charging current decreases with time. The charging will cause temperature rise and degradation of the battery life

Two-step charging

combines the constant current and constant voltage charging. In the first stage of charging, the batteries are charged by a constant current until the battery voltage reaches a preset voltage. In the second stage, a constant voltage is applied for battery charging

Pulse charging

pulse current is applied to the battery periodically, this provides the battery a relax time in charging process. The electrochemical reaction and neutralization of battery internal electrolyte are helpful to enhance the life cycle of battery Using a large pulse current will shorten the battery charging time.

12V Battery Charger

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled.png)

Use of RS allows low charging rates with fully charged battery.
**The 1000 μF is recommended to filter out input transients

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%201.png)

Precision Current Limiter

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%202.png)

4A Switching Regulator with Overload Protection

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%203.png)

Low Cost 3A Switching Regulator

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%204.png)

1.2V–20V Regulator with Minimum Program Current

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%205.png)

Minimum load current ≈ 4 mA

5A Constant Voltage/Constant Current Regulator

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%206.png)

https://electronics.stackexchange.com/questions/473609/[5a](https://electronics.stackexchange.com/questions/473609/5a-constant-current-constant-voltage-using-lm350)-constant-current-constant-voltage-using-lm350

Integrator with Bias Current Compensation

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%207.png)

High Current Adjustable Regulator

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%208.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%209.png)

Minimum load current = 30 mA
‡Optional—improves ripple rejection

Adjustable Regulator with Improved Ripple Rejection

5V Logic Regulator with Electronic Shutdown

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2010.png)

Regulator with Protection Diodes

PROTECTION DIODES
When external capacitors are used with any IC regulator it is sometimes necessary to add protection diodes to prevent the capacitors from discharging through low current points into the regulator. Most 10 μF capacitors have low enough internal series resistance to deliver 20A spikes when shorted. Although the surge is short, there is enough energy to damage parts of the IC. When an output capacitor is connected to a regulator and the input is shorted, the output capacitor will discharge into the output of the regulator. The discharge current depends on the value of the capacitor, the output voltage of the regulator, and the rate of decrease of VIN. In the LM117HV, this discharge path is through a large junction that is able to sustain 15A surge with no problem. This is not true of other types of positive regulators. For output capacitors of 25 μF or less, there is no need to use diodes. The bypass capacitor on the adjustment terminal can discharge through a low current junction. Discharge occurs when either the input or output is shorted. Internal to the LM117HV is a 50Ω resistor which limits the peak discharge current. No protection is needed for output voltages of 25V or less and 10 μF capacitance. Figure 22 shows an LM117HV with protection diodes included for use with outputs greater than 25V and high values of output capacitance.

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2011.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2012.png)

D1 protects against C1
D2 protects against C2

LOAD REGULATION
The LM117HV is capable of providing extremely good load regulation but a few precautions are needed to obtain maximum performance. The current set resistor connected between the adjustment terminal and the output terminal (usually 240Ω) should be tied directly to the output of the regulator rather than near the load. This eliminates line drops from appearing effectively in series with the reference and degrading regulation. For example, a 15V regulator with 0.05Ω resistance between the regulator and load will have a load regulation due to line resistance of 0.05Ω × IL. If the set resistor is connected near the load the effective line resistance will be 0.05Ω (1 + R2/R1) or in this case, 11.5 times worse.

EXTERNAL CAPACITORS
An input bypass capacitor is recommended. A 0.1 μF disc or 1 μF solid tantalum on the input is suitable input bypassing for almost all applications. The device is more sensitive to the absence of input bypassing when adjustment or output capacitors are used but the above values will eliminate the possibility of problems. The adjustment terminal can be bypassed to ground on the LM117HV to improve ripple rejection. This bypass capacitor prevents ripple from being amplified as the output voltage is increased. With a 10 μF bypass capacitor 80 dB ripple rejection is obtainable at any output level. Increases over 10 μF do not appreciably improve the ripple rejection at requencies above 120 Hz. If the bypass capacitor is used, it is sometimes necessary to include protection diodes to prevent the capacitor from discharging through internal low current paths and
damaging the device. In general, the best type of capacitors to use are solid tantalum. Solid tantalum capacitors have low impedance even at high frequencies. Depending upon capacitor construction, it takes about 25 μF in aluminum electrolytic to equal 1 μF solid tantalum at high frequencies. Ceramic capacitors are also good at high frequencies; but some types have a large decrease in capacitance at frequencies around 0.5 MHz. For this reason, 0.01 μF disc may
seem to work better than a 0.1 μF disc as a bypass. Although the LM117HV is stable with no output capacitors, like any feedback circuit, certain values of external capacitance can cause excessive ringing. This occurs with values between 500 pF and 5000 pF. A 1 μF solid tantalum (or 25 μF aluminum electrolytic) on the output swamps this effect and insures stability. Any increase of
load capacitance larger than 10 μF will merely improve the loop stability and output impedance.

CHARGING PROCESS OF BATTERIES
Charging a lead acid battery is a matter of replenishing the depleted supply of energy
that the battery had lost during use. This replenishing process can be accomplished with
several different charger implementations: “constant voltage charger” , “ constant
current charger” or a “ "multistage" constant voltage/current charger”. Each of these
approaches has its advantages and disadvantages that need to be compared and weighed
to see which one would be the most practical and realistic to fit with our requirements.
Constant Voltage charger:-
Constant voltage charging is one of the most common charging methods for lead acid
batteries. The idea behind this approach is to keep a constant voltage across the
terminals of the battery at all times. Initially, a large current will be drawn from the
voltage source, but as the battery charges and increases its internal voltage, the current
will slowly fold and decays exponentially. When the battery is brought up to a potential
full charge, which is usually considered around 13.8V, the charging voltage is dropped
down to a lower value that will provide a trickle

charge to maintain the battery as long as it is plugged into the charger. The best
characteristic of this method is that it provides a way to return a large bulk of the
charge into the battery very fast. The draw back, ofcourse, is that to complete a full
charge would take a much longer time since the current is exponentially decreased as
the battery charges. A prolonged charging time must be considered as one of the issues
to this design.
Solar cells are one of our main portable power sources. Inherently, they provide a
constant current which is dependent on light intensity and other uncontrollable
variability in the environment. This characteristic fits well with a constant voltage
charge design, which does not depend on the current provided by the input source,
which in turn eliminates the dependence of the charger on external variations like the
time of day, weather conditions or temperature. The effects of the changing voltage are
also minimized since the voltage is being regulated.

Constant Current Source:-
Constant current charging is another simple yet effective method for charging leadacid
batteries. A current source is used to drive a uniform current through the
battery in a direction opposite of discharge.
This can be analogous to pouring water into a bucket with a constant water flow, no
matter how full the bucket is. Constant current sources are not very hard to
implement; therefore, the final solution would require a very simple design.
There is a major drawback to this approach. Since the battery is always being
pushed at a constant rate, when it is close to being fully charged, the charger would
force extra current into the battery, causing overcharge. The ability to harness this
current is the key to a successful charger. By monitoring the voltage on the battery,
the charge level can be determined, and at a certain point, the current source would
need to be folded back to only maintain a trickle charge and prevent overcharging.

Multi-stage Constant Voltage/Current Charging Solutions:
Both constant voltage and current approaches have their advantages; that is the
reason multistage chargers have been developed which combine the two methods to
achieve maximum charge time, with minimum damage to the charging cell.
Stage 1: Deep Discharge Charging Pulse Mode
The Charger starts charging at 0.5V and give pulse current up to 5V.
This has effect of removing loose sulphation formed during deep
discharge state of the battery.
Stage 2: Constant Current Mode (CC)
The charger changes to constant current 2.5A. When the battery voltage
reaches up to 14.4V, the charging stage changes from (CC) Constant
Current to CV (Constant Voltage) mode.
Stage 3: Constant Voltage Mode (CV)
The charger holds the battery at 14.4V and the current slowly reduces.
When the current reaches at 0.5 C (C= Battery Capacity), this point
called the Switching Point. The Switching Point is one of the great
features of this battery charger that it can adjust the current
automatically according to the battery capacity. Other chargers without
microprocessors are not capable to adjust the current.

Stage 4: Standby Voltage Mode
The charger maintains the battery voltage at 13.8V and current slowly
reduces to zero. Charger can be left connected indefinitely without
harming the battery.
Recharging:
If the battery voltage drops to 13.8V, the charger changes from any
mode to Constant Current mode and restart charging. The charging cycle
will go through Stage 2 to Stage 4.
As much as multi-stage chargers are enticing in terms of their features, for our
purposes, the complexity and the control logic needed to implement this kind
of solution would make our project unrealistic given the time constraints.

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2013.png)

Charging Circuit
General Description
The full charger feedback control circuit can be seen in Figure below. This circuit
implements a three stage charger algorithm: constant current state, constant voltage
full charge state, and constant voltage float charges state. This circuit will require an
input voltage of at least 17 volts to output the 14.7V for charging because of the 2V
drop across the regulator.
The comparator is used to provide feedback of the current that the battery is
drawing from the circuit: as the battery charges, the current drawn decreases. The
current sensing resistor is used to convert that current into voltage, which can be used
to compare to a reference within the circuit. This will be the logic needed for the state
switching mechanism. The full charge state will provide 14.7V or 2.45V/Cell on the
battery and float charge will provide 13.8V or 2.3V/Cell. The battery will try to draw
maximum current, in this case:
(14.7V-10.5V)/.1Ohm= 42A (assuming the battery is completely dead)
The current limiting of the voltage regulator will force the current to 3A. The
charger will continuously pump this 3A until the battery current falls below the limit
of 500 mA. This will bring the voltage of the battery above the reference point,
therefore causing the comparator to turn on the transistor switch, pulling the output
voltage to the float charging level.

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2014.png)

Step 4: Providing feedback through the current sensing resistor
This final step was to build the complete circuit. It proved to be a challenging task.
Even though logically the circuit made sense and did not vary significantly from the
previous one , we were unable to get the expected output. After trying to appease the
simulator for long hours, we came to the conclusion that our analysis is probably
correct and that feedback loop through the current sensing resistor R6, added enough
complexity to the circuit that the simulator did not provide an accurate answer

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2015.png)

market suvey

![Snag_247bf358.png](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Snag_247bf358.png)

[https://www.electroschematics.com/lead-acid-battery-charger/](https://www.electroschematics.com/lead-acid-battery-charger/)

![lead-acid-battery-charger.gif](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/lead-acid-battery-charger.gif)

![EN1979070721.pdf.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/EN1979070721.pdf.jpg)

![EN1979070501.pdf.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/EN1979070501.pdf.jpg)

over voltage protection

![Over-voltage-protection-using-Zener-Diode.png](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Over-voltage-protection-using-Zener-Diode.png)

![overvoltage_protection_circuit_ec71317048018fcb7b271a26d24f5806bf55e1ee.webp](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/overvoltage_protection_circuit_ec71317048018fcb7b271a26d24f5806bf55e1ee.webp)

heat protection circuit

![images.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/images.jpg)

under/over volatge protection

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2016.png)

![over-voltage-and-low-voltage-protection-circuit.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/over-voltage-and-low-voltage-protection-circuit.jpg)

reverse connection protection

![download.png](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/download.png)

short circuit protection/over current protetcion

![Short-Circuit-and-Over-Current-Protection-Using-LM358-OP-AMP-.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Short-Circuit-and-Over-Current-Protection-Using-LM358-OP-AMP-.jpg)

![Short-Circuit-Protection-Using-Relay-For-Batteries-.jpg](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Short-Circuit-Protection-Using-Relay-For-Batteries-.jpg)

market

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2017.png)

[HT66F0182v110.pdf](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/HT66F0182v110.pdf)

[LM324-D.pdf](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/LM324-D.pdf)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2018.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2019.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2020.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2021.png)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2022.png)

[https://www.youtube.com/watch?v=1MMejVScW2A](https://www.youtube.com/watch?v=1MMejVScW2A)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2023.png)

[sn74hc595.pdf](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/sn74hc595.pdf)

[sihg20n5.pdf](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/sihg20n5.pdf)

[https://www.youtube.com/watch?v=zhmVrEevhtU](https://www.youtube.com/watch?v=zhmVrEevhtU)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2024.png)

[https://www.youtube.com/watch?v=0xxKQozjNI0](https://www.youtube.com/watch?v=0xxKQozjNI0)

[https://www.chargingchargers.com/tutorials/charging.html](https://www.chargingchargers.com/tutorials/charging.html)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2025.png)

inspired design

[https://www.youtube.com/watch?v=ycT-PItAzNk](https://www.youtube.com/watch?v=ycT-PItAzNk)

![Untitled](lead%20acid%20battery%20charger%2017d50d468b444d2d940d83cfe3717b67/Untitled%2026.png)

- Switch mode power supply
    
    fuse (small)one inch 
    
    emc filtering circuit - high volatge capacitor and 1:1 choke(high frequency noise removal)
    
    rectifier- primary filter (integrated full bridge rectifier)
    
    high volateg capacitors
    
    switching transisiotrs usually two or one (heat sink) controllerd by pwm controller
    
    transformer to half bridge rectifier(double shotkey)
    
    secondary filter
    
    optocoupler for feedback
    
    shunt resisitor
    
    [https://www.youtube.com/watch?v=cK5WLMFSGnw](https://www.youtube.com/watch?v=cK5WLMFSGnw)
    

[https://www.youtube.com/watch?v=2N_T7VFymFg](https://www.youtube.com/watch?v=2N_T7VFymFg)
