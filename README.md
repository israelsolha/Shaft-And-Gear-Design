# Shaft-And-Gear-Design

This 7000 lines project was the base of my Senior Research Paper for obtaining my Bachelor's Degree in Mechanical Engineering at the Federal University of Paraiba (Brazil). The project consists in a program made on MATLAB's App Designer to help engineers design Shaft and Gear Systems. By only providing basic geometric and material properties, the software gives a full report regarding static and dynamic analyses, demonstrating if the project complies to the safety specifications, and pointing to the possible issuses so that they can be quickly fixed. The results also include all forces acting on every single component of the system, graphs of moment, most likely causes of failure, safety factor, and much more.

This program works with four of the most commonly used types of gears:
* Spur gears
* Helical gears
* Conical gears
* Worm drive

This is an example of an input page for a Spur Gear, defining the properties of the motor gear, the moved gear, and the shafts they are placed on:

<p align="center">
  <img src="https://i.imgur.com/6MhbvAX.png">
</p>

After adding the gears and shafts, the result of the static analysis is presented in a page like this, allowing the user to choose which element to focus on, and get the desired properties:

<p align="center">
  <img src="https://i.imgur.com/1VQpN8I.png">
</p>

Then, a dynamic analysis can be performed, by giving the material properties of the components. The program comes pre-configured with a library of the most important materials and means of fabrication, so that the user can quickly choose some default values. In case of something more specific, the values for these properties can also be inserted manually. The dynamic analysis information page is as follows, depending on which type of gears are used.

<p align="center">
  <img src="https://i.imgur.com/4ZMF1mP.png">
</p>

Finally, a full report of the system can be obtained. An example report to this configuration would be something like:

```
=======================================================
                      RELATÓRIO                      
=======================================================

ANÁLISE ESTÁTICA:

======= Eixo 1 Principal =======

Diâmetro mínimo: 267.00 mm
Torque máximo: 185.68 N.m
Momento máximo: 26.14 N.m

Reação no Mancal 1:

Fx = -1787.891 N
Fy = 4912.190 N
Fz = 0.000 N

Reação no Mancal 2:

Fx = -357.578 N
Fy = 982.438 N
Fz = 0.000 N

Forças nas Engrenagens 1 :

Fx = 2145.469 N
Fy = -5894.628 N
Fz = -0.000 N

======= Eixo 2  =======

Diâmetro mínimo: 287.00 mm
Torque máximo: 371.36 N.m
Momento máximo: 26.14 N.m

Reação no Mancal 1:

Fx = 1787.891 N
Fy = -4912.190 N
Fz = 0.000 N

Reação no Mancal 2:

Fx = 357.578 N
Fy = -982.438 N
Fz = 0.000 N

Forças nas Engrenagens 1 :

Fx = -2145.469 N
Fy = 5894.628 N
Fz = 0.000 N

===================================

ANÁLISE DINÂMICA:

======= Engrenagens 1  =======

Coeficientes de segurança do pinhão

Contra fadiga: 1.17
Contra escoamento: 0.72
Falha no pinhão proveniente de ESCOAMENTO

Coeficientes de segurança da coroa

Contra fadiga: 1.27
Contra escoamento: 0.65
Falha na coroa proveniente de ESCOAMENTO

======= Eixo 1 Principal =======

A análise dinâmica não foi realizada nesse eixo

======= Eixo 2  =======

A análise dinâmica não foi realizada nesse eixo

=======================================================
```

All these calculations are often made by hand, or in many steps, by many engineers. This programs allows a user to solve problems that would literally take days in a matter of minutes. The best part is that after realizing something has to be changed, changing a single line of input can suffice, and a new model will be made instantly, greatly improving an engineering's ability to explore and test their ideas.
