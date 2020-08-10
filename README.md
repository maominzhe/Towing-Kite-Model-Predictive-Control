# Towing-Kite-Model-Predictive-Control
Wind energy is considered as one of the clean energy. As an alternative of facilitating the wind energy, towing kite is adopted as the new propulsion system for ship design to reduce fuel comsuption. In this paper we extract the towing kite as a mathematical model and apply nonlinear model predict control.
The aim of the project is to apply model predictive control on twoing kite and analyze the performance of the different discretization approaches Explicit euler, Multiple shooting, Orthogonal collocation and compare them in terms of the accuracy and computational cost.
In order to facilitate cross-sectional comparison of the results initial states, testing and sampling time will be set the same in each discretization methods.

![towing-kite](https://user-images.githubusercontent.com/51397883/89793667-6bad9680-db26-11ea-9da2-42e351e17500.jpg)

<img width="203" alt="mathematical-model" src="https://user-images.githubusercontent.com/51397883/89793720-7a944900-db26-11ea-9c9e-66974e39a063.png">

## Euler_Kite.ipynb
This file execute MPC with explicit euler mathod. Key parameter here is the sampling time dt, in order to reach a better performance dt should be set ralatively small under the consideration of computational cost.
<img width="700" alt="eo" src="https://user-images.githubusercontent.com/51397883/89795082-3f931500-db28-11ea-8620-0bf0354842f3.png">

## MS_Kite.ipynb
In this file the multiple shooting method is used. The uncertain parameters are set the same as the other two methods.
<img width="700" alt="eo" src="https://user-images.githubusercontent.com/51397883/89795021-29855480-db28-11ea-9a1e-96f9c1697312.png">

## OC_Kite.ipynb
When the model is discretized with orthogonal collocation it achieves the best acurracy.
<img width="740" alt="oc" src="https://user-images.githubusercontent.com/51397883/89795055-373ada00-db28-11ea-97a3-7175eb277ee1.png">
