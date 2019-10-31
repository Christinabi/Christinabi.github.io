---
layout: default
mathjax: true
permalink: /governingEquation/
---

## Governing equations of lithium-ion battery model

### Governing equations

When we talked about electrochemical model of a battery, five governing equations will be mentioned, those are

1. The solid phase mass conservation equation

$$
\frac{\partial c_s}{\partial t}=\frac{1}{r} \frac{\partial}{\partial r} \left( D_sr^2 \frac{\partial c_s}{\partial r}\right)
$$

2. The electrolyte phase mass conservation equation

$$\frac{\partial \varepsilon_e c_e}{\partial t} = \nabla \cdot \left( D_{e,eff}\nabla c_e \right)+a_s\left(1-t_+^0\right)j$$

3. The Solid phase charge conservation equation

$$\nabla\cdot\left(\sigma_{eff}\nabla\phi_s\right)=a_sFj$$

4. The electrolyte phase charge conservation equation

$$\nabla\cdot\left(\kappa_{eff}\nabla\phi_e+\kappa_{D,eff}\nabla\ln c_e\right)+a_sFj=0$$

5. Butler-Volmer kinetics relationship

$$j=j\left(\right)$$

### Mass conservation in the solid

Inside a composite electrode, there are particles with various shapes and sizes. However, it is overwhelming when we are trying model it. Therefore, we assume that spherical particles centered at grid location in the electrode, and that the concentration distribution within the particle is spherically symmetric. This way we can model the concentration inside a particle using a radius dimension, which is what we called a `pseudo-dimension`.  

Now let's look at the equation

$$\frac{\partial c_s}{\partial t}=\frac{1}{r} \frac{\partial}{\partial r} \left( D_sr^2 \frac{\partial c_s}{\partial r}\right)$$

The left-hand side describes how the solid concentration changes over time. The-right hand side is actually the divergence of the concentration flux density

$$\mathbf{N}=-D\nabla c$$ 

where the minus sign shows that the flux density has opposite direction to the gradient, implying that the ions move from a high concentration to a low concentration. 
