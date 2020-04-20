#Conductors
##Properties of Conductors
- Charge moves freely in a conductor. Technically, only electrons move freely, but you are allowed to assume that both positive and negative charges move around, and all the math works out the same.
- All the charges in a conductor repel each other until all charge lies on its surface.
- Since no charge exists in the conductor's interior, Gauss's law states that there is no electric field inside a conductor.
- Electrostatic shielding is a method of removing an external electric field from an area by enclosing it with a conductive shell.
- The electric field just outside the surface of a conductor is perpendicular to the conductor's surface.
- Conducting surfaces are equipotential surfaces, even if there is an external electric field.

##Induction and Movement of Charge
- A ground is something that can give and receive charge to and from a conductor until it reaches equilibirum. A conductor is said to be grounded if it is connected to a ground.
- If a conductor is grounded and placed on an external electric field, charge will move in or out of the conductor, giving it a net charge.
- When a charged object is placed next to a neutral, not-grounded conductor, it will create an induced charge, causing one side of the conductor to be positive and the other negative. This causes the charged object to attract the conductor.

##Dielectrics
- Dielectrics are insulating materials that contain atoms which polarize in an electric field, causing the electric field to decrease in strength. The exact physics behind this is not covered in AP.
- All you need to know is that dielectrics are characterized by a dielectric constant \\(\kappa\\).
- The electric permitivity \\(\epsilon\\) is defined by the formula:
\\[\epsilon=\kappa\epsilon_0\\]
- \\(\epsilon_0\\) is the electric permitivity of a vacuum. Most situations in AP use \\)\epsilon_0\\), But when the vacuum is replaced by a dielectric material, you must use \\(\epsilon\\) instead.
- The dielectric constant of a vacuum is 1, so in a vacuum, \\)\epsilon=\epsilon_0\\).

#Capacitors
##General
- A capacitor consists of two conductors, usually referred to as plates, which can hold charge and are close enough to influence each other.
- The plates hold equal and opposite charges (the charge on one plate is equal to the negative charge on the other plate)
- Every capacitor has a capacitance defined by the formula:
\\[C=\frac Q{\Delta V}\\]
where \\(Q\\) is the charge on each plate and \\(\Delta V\\) is the potential difference between the plates
- The electric potential energy stored in a capacitor is:
\\[U=\frac12 C(\Delta V)^2=\frac12 Q\Delta V=\frac12\frac{Q^2}C\\]
 
##Parallel Plate Capacitors
The capacitance of a parallel plate capacitor follows the formula:
\\[C=\frac{\epsilon A}d\\]
where epsilon is the electric permitivity, A is the area of each plate, and d is the distance between the plates. The thickness of each plate does not matter, since all charge resides on the conductor's surface.
<div class="callout callout--info">
Parallel plate capacitors dominate this section of the AP exam. If you're short on time, you can get away without knowledge of spherical or cylindrical capacitors.
</div>

##Spherical Capacitors
In a spherical capacitor, one of the plates is a sphere, and the other is a shell enclosing the sphere. Generally you will be asked to find the capacitance given r1, the radius of the inner sphere, and r2, the radius of the outer sphere.
Capacitance Calculation:
The electric field between the sphere and the shell can be calculated with Gauss's law:
\\[E=\frac Q{4\pi r^2 \epsilon}\\]
The voltage between the plates can then be calculated with the integral:
\\[\Delta V=\int_{r_1}^{r_2}Edr=\int_{r_1}^{r_2}\frac Q{4\pi r^2 \epsilon}dr=\frac Q{4\pi \epsilon}(\frac1{r_1}-\frac1{r_2})\\]
Therefore,
\\[C=\frac Q{\Delta V}=\frac{4\pi\epsilon}{\frac1{r_1}-\frac1{r_2}}\\]

##Cylindrical Capacitors
In a cylindrical capacitor, one of the plates is a cylinder, and the other is a shell enclosing the cylinder. Generally you will be asked to find the capacitance given a, the radius of the inner cylinder, and b, the radius of the outer cylinder.
Capacitance Calculation:
The electric field between the shells can be calculated using Gauss's law:
\\[E=\frac Q{\epsilon2\pi rh}\\]
The voltage across the capacitor can be calculated with the integral:
\\[\Delta V=\int_a^bEdr=\int_a^b\frac Q{\epsilon2\pi rh}dr=\frac Q{\epsilon2\pi h}(\ln b-\ln a)=\frac Q{\epsilon2\pi h}\ln\frac ba\\]
Therefore, the capacitance is:
\\[C=\frac Q{\Delta V}=\frac {\epsilon2\pi h}{\ln\frac ba}\\]
