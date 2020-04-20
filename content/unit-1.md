# Charge Distributions
## Density
- Charge density describes the amount a charge per unit length, area, or volume. Linear (length) charge density is represented by $\lambda$, surface (area) charge density is represented by \(\sigma\), and volume charge density is denoted as $$\rho$$
- The different types of density follow the equations: 
\\[\lambda=\frac Ql \;\;\;\;\;\;\; 
\sigma=\frac Q A    \;\;\;\;\;\;\;
\rho=\frac Q V \\]
	where $$Q$$ is the charge in a region, $$l$$ is the region's length, $$A$$ is surface area, and $$V$$ is volume
- To find the total charge in a region, you have to evaluate the integral
\\[Q=\int\rho dV\\]
where $$\rho$$ and $$V$$ can be replaced with the corresponding density and area/length variables needed.

## Symmetry
- A charge distribution is spherically symmetric if you can draw a spherical shell around the center and the surface density is the same at any point on its surface.
- A charge distribution is cylindrically symmetric if you can draw a cylindrical shell around central line of charge and the surface density is the same at any point on its surface.
- A charge distribution has planar symmetry if it is a large, flat plane.

# Electrostatic Forces and Energy
## Coulomb's Law
- The magnitude of the electrostatic force between two charges is described by Coulomb's Law:
\\[F=k\frac{q_1q_2}{r^2}=\frac1{4\pi\epsilon_0}\frac{q_1q_2}{r^2}\\]
where $$F$$ is the magnitude of the force, $$q_1$$ and $$q_2$$ are the charges on each particle, and r is the distance between the particles.
- $$k$$ denotes Coulomb's constant, and $$\epsilon_0$$ denotes a closely related constant called the vacuum permitivity. The values $$k$$ and $$\frac1{4\pi\epsilon_0}$$ are used interchangeably in Coulomb's law.

## Electric Field
- Electic field is the force that acts on a particle per unit charge on each particle. Force and electric field are related by the formula
\\[\overrightarrow F=\overrightarrow Eq\\]
where $$\overrightarrow E$$ is the eletric field vector, $$\overrightarrow F$$ is the electric force vector, and $$q$$ is the charge of the particle being acted upon.
- The strength of the electric field at a distance from a point charge follows the formula
\\[E=k\frac{q}{r^2}\\]
where $$k$$ is Coulomb's constant, $$q$$ is the charge, and $$r$$ is the distance from the charge.

## Electric Potential
- The electric force is associated with electric potential energy just as gravitational force is associated with gravitational potential energy. The electric potential energy of a system of two point charges follows the formula
\\[U=-k\frac{q_1q_2}{r}\\]
- Electric potential is defined as the energy per unit charge on an object. Electric potential and energy are both scalar and are related by the formula
\\[U=Vq\\]
- From this equation, you can derive the expression for the electric potential around a point charge:
\\[V=k\frac{q}{r}\\]
- The electric field strength is the derivative of electric potential:
\\[E=\frac{dV}{dr}\\]
- The electric potential difference between two points can be found by integrating the electric field any the path between them:
\\[\Delta V=\int_b^a\overrightarrow E\cdot d\overrightarrow r\\]
where a and b refer to the starting and ending coordinates
<div class="callout callout--info">
Note the dot product here. $$\overrightarrow E\cdot d\overrightarrow r$$ is equivalent to $$Er\cos \theta$$. In AP, you will almost always be integrating over a straight line parallel to the electric field, so you usually don't have to worry about $$\cos\theta$$.
</div>

# Gauss's Law
## The Formula
- Electric flux ($$\Phi$$) is defined as the total electric field passing through a surface. It follows the formula
\\[\Phi=\oint \overrightarrow E\cdot d\overrightarrow A\\]
where $$\overrightarrow E$$ is the electric field vector and $$\overrightarrow A$$ is the area vector. $$\oint$$ denotes a surface integral. You will never need to evaluate this integral in AP. You will almost always use the algebraic form of the rule:
\\[\Phi=EA\cos\theta\\]
(TODO: insert an image that makes the concept clearer)

- Gauss's Law states:
\\[\oint E\cdot dA=\frac Q{\epsilon_0}\\]
The left side of the equation represents electric flux through a closed surface. In AP Physics, this will usually be a sphere, cylinder, or plane. On the right side, $$Q$$ denotes the total charge encolsed within that surface epsilon_0 is the vacuum permitivity.
	
## Applications
- If no charge is enclosed by a closed surface, the net flux through that surface will be 0. The electric flux entering the surface will be equal to the electric flux leaving the surface.
- For a spherically symmetric charge distribution, you can imagine a sphere enclosing it. The surface area of this sphere is $$4\pi r^2$$, so the total electric flux passing through the sphere is $$\Phi=4\pi r^2E=\frac Q{\epsilon_0}$$. From here, you can use Gauss's law to solve for the electric field strength at any point on the sphere's surface.

- If you draw a cylinder if radius $$r$$ and length $$h$$ around a cylindrical charge distribution, the flux through that cylinder will be $$\Phi=2\pi rhE=\frac Q{\epsilon_0}$$ (the cylinder's surface area times electric flux). Then you can use Gauss's law to solve for $$E$$ at any point on the cylinder's surface.

- Planar charge distributions are typically described by a surface charge density ($$\sigma$$). Remember that $$\sigma=\frac QA$$.
The total flux through a plane of area $$A$$ is $$2EA$$ because the plane has two sides; the flux leaving one side is $$EA$$, so the flux leaving through both sides is $$2EA$$.
Gauss's law now becomes $$2EA=\frac{\sigma A}{\epsilon_0}$$. The areas cancel out and you can solve for $$E$$ on the plane's surface.
