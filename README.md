# CWPINN
CWPINN: The-Constrained-Weight-Physics-Informed-Neural-Network

Physics-Informed Neural Networks (PINNs) have shown considerable promise in solving partial differential equations that describe physical processes. However, their computational efficiency is often limited by the structural complexity of the network and the large number of parameters involved. To address this issue, it is essential to enrich the network architecture with additional physical information. Building on the weight-function formulation of PINNs, this study uncovers a strong physical correlation between the network’s weight layers and the collocation points. This insight leads to the development a Constrained-Weight PINN model (CWPINN), in which the strong enforcement of boundary conditions is shifted from the output layer to the hidden layers. A distance function is computed for each neuron in the hidden layers, simplifying derivative calculations and alleviating gradient pathology. The CWPINN demonstrates outstanding performance across applications in thermodynamics, fluid mechanics, and solid mechanics. For three-dimensional problems, the forward analysis model CWPINN-F achieves a computational speed 667 times faster than conventional PINNs under the Deep Energy Method (DEM) framework. Furthermore, the inverse analysis model CWPINN-I treats labeled data as boundary conditions imposed in strong form at the weight layers, and incorporates additional loss terms that constrain derivatives and function variables. This approach effectively overcomes the convergence challenges commonly associated with the DEM framework.

<img width="865" height="706" alt="image" src="https://github.com/user-attachments/assets/a27eb8e4-31f2-4465-a685-e85f2eb8aeb1" />

 Forward analysis model (CWPINN-F): (a) network topology; (b) computational flowchart.

 
 <img width="865" height="753" alt="image" src="https://github.com/user-attachments/assets/3e86e1db-c517-4ad1-9cda-1ae0f3ab1597" />
 
 Inverse analysis model (CWPINN-I): (a) network topology; (b) computational flowchart.


