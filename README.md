# CalgaryR Presentation

CalgaryR: The Fall season is on

https://www.meetup.com/calgaryr/events/303153313/

# From Math to App
This presentation explains the journey from formulating a mathematical problem to its formal analytical and then numerical solution and finally to creating a visualization to show the output for ranges of input values.

The formulation is an ordinary differential equation (ODE) of second order. The Shiny app uses the numerical solution to produce the interactive output in response to changes in the input variables made through the UI.

## Simulation: Math formulation

The solution to the ODE has two parts. The complementary solution is the system response without the intervention of external forces.
The particular solution originates in the presence of external forces.
Both superimpose over the full system response, so they can be added to produce the solution.

There are three cases to consider for the complementary solution: two distinct real roots, two identical real roots, or two complex conjugate roots for the characteristic polynomial of the ODE. Each one is addressed separately and the code correspondingly identifies each case.

The product of the analytical solution is a series of formulas. They are used to formulate a numerical solution in several R functions that use vectorized code to mimic the math as closely as possible.

After a reliable numerical solution is achieved and some base plotting has confirmed its consistency with the expected physical reality, the final step is to write a visualization UI as a Shiny app. 

## Project and code 

All the  code can be found in this Github project. Some R project setup is required, the RStudio IDE helps by asking the user to download the missing packages. 

## Visualizations

For the app visit https://padames.github.io/spring_dynamics_presentation/
