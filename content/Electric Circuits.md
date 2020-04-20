<style>
body {
    color: #333;
    font-family: "Noto Sans",sans-serif;
    font-size: 1em;
    line-height: 1.8em;
}
h1 {
    font-family: "Montserrat",sans-serif;
    font-weight: 400;
    line-height: 1.5em;
    margin: 2.5rem 0 .9375rem 0;
}

.callout {
    border: 2px solid #efefef;
    background-color: #f9f9f9;
    padding: .9375rem 1.25rem .625rem 1.25rem;
    margin: 0 0 1.25rem 0;
}
.callout--info {
    background-color: #f2f8ff;
    border-color: #deedff;
}
</style>
#Electric Current
##Current
- Electric current is defined as the amount of charge that passes through a region every second. It follows the formula:
\\[I=\frac{dQ}{dt}\\]
where $$I$$ is electric current, $$Q$$ is the amount of charge that has passed through a point in a circuit, and $$t$$ is time
- Conventional current: The direction of the current is defined as the direction that positive charge flows. Technically, only negative charges (electrons) ever move through a circuit, but an electron moving in one direction can be treated as a proton moving in the opposite direction, and all of the math will work out.
- Current density is defined as the current flowing per unit area of the wire's cross section. It follows the formula:
\\[I=\overrightarrow J\cdot\overrightarrow A\\]
where $$I$$ is current, $$\overrightarrow J$$ is current density, and $$\overrightarrow A$$ is the cross-sectional area vector (remember that the direction of $$\overrightarrow A$$ is perpendicular to the cross-section). In AP, it's usually safe to ignore the $$\cos\theta$$ from the dot product, so the equation becomes $$I=JA$$.
- Current also has a microscopic definition:
\\[I=Nev_dA\\]
where $$N$$ is the number of charge carriers per unit volume, $$e$$ is the elementary charge, $$A$$ is cross-sectional area, and $$v_d$$ is drift velocity: the average velocity that charge carriers move in the wire. $$v_d$$ is usually extremely slow.

##Resistance
- The motion of charge is driven by a potential difference, or voltage ($$V$$), which creates an electric field in the wire (remember $$E=\frac{dV}{dr}$$), pushing charge through it. Additionally, resistance ($$R$$) is a property of a conductor which resists the motion of charge. Ohm's Law relates voltage, current, and resistance:
\\[V=IR\\]
- The resistance of a conductor can be calculated with the equation:
\\[R=\frac{\rho l}{A}\\]
where $$R$$ is resistance, $$l$$ is the length of the conductor, and $$A$$ is the cross-sectional area of the conductor. $$\rho$$ denotes resistivity, which has a value specific to the type of material the conductor is made of.
- Current density relates to resistivity and the electric field strength in a wire by the following formula:
\\[\overrightarrow E=\rho \overrightarrow J\\]
where $$\rho$$ is the wire's resistivity and $$\overrightarrow J$$ is the current density.
- The definition of resistance can be derived from the microscopic current definition:  
Start with $$I=Nev_dA$$  
You can find current density: $$J=\frac IA=Nev_d$$  
You can then calculate voltage: $$V=El=\rho J l=\rho Nev_d l$$  
Then you can find resistance: $$R=\frac VI=\frac{\rho Nev_dl}{Nev_dA}=\frac{\rho l}A$$
 
##Power
- When current flows through a resistor, the kinetic energy of moving charge carriers is converted to heat.
- Power ($$P$$) in a circuit is the amount of energy converted to heat per second. It follows the formula:
\\[P=IV=I^2R=\frac{V^2}R\\]

#Circuits with resistors and batteries
##Series and Parallel Circuits
- Series circuits have resistors arranged like this:  
<center>![](series.png)</center>
- The total resistance of a series circuit is equal to the sum of the resistances of all the individual resistors. This is expressed mathematically as:
\\[R_s=\sum _i R_i\\]
- In a series circuit, the current is the same at all points.
- Parallel circuits look like this:
<center>![](parallel.png)</center>
- The total resistance of a parallel circuit follows the formula:
\\[\frac 1{R_p}=\sum_i\frac1{R_i}\\]
- In a parallel circuit, the voltage across each branch is the same.

##Kirchoff's Rules
- Current rule: the total current entering a junction must be equal to the total current leaving that junction.
- Loop rule: If you add up the voltage differences across any closed loop in a circuit, the result will be zero.

##Other Circuit Components
- Ammeters measure current. An ideal ammeter has negligible resistance and must be placed in series with a circuit to determine the current flowing through it.
- Voltmeters measure voltage. An ideal voltmeter has very large or infinite resistance and must be placed in parallel with a circuit.
- Batteries may have internal resistance.

#RC Circuits
##Capacitance
- Remember the formula for capacitance:
\\[C=\frac QV\\]
- If you have multiple capacitors wired in parallel, they will behave as a single capacitor with a capacitance following the formula
\\[C_p=\sum_iC_i\\]
- If you have multiple capacitors wired in series, they will behave as a single capacitor with a capacitance following the formula
\\[\frac 1{C_s}=\sum_i\frac1{C_i}\\]
- When capacitors are wired in parallel, the total charge stored in the circuit is equal to the sum of the charges stored on each capacitor.
- When capacitors are wired in series, each has the same charge $$Q$$, and the total charge stored in the circuit is equal to $$Q$$

##Behavior
- RC circuits contain resistors and capacitors. $$R$$ denotes the equivalent resistance of all the resistors, and $$C$$ denotes the equivalent resistance of all the capacitors.
- Capacitors take time to charge and dicharge.
- When a capacitor charges, the voltage, charge, and current in the capcitor as a function of time can be found by solving a differential equation. You don't need to solve this equation on the exam; you should just know that the equation will always contain a factor of $$e^{-\frac t{RC}}$$
- $$RC$$ is called the time constant and is sometimes denoted as $$\tau$$
- At time $$t=0$$, an uncharged capacitor will behave as a bare wire with no voltage difference across it, and the current through the circuit can be found using Ohm's law for the resistor.
- As $$t$$ approaches infinity, the capacitor will become fully charged and act as a break in the circuit (there will be no current flow through it).
