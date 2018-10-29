# Hummingbird-Simulink
Hummingbird Tailsitter MATLAB Simulink Models

This repository contains the MATLAB simulink models to simulate the Hummingbird's dynamics and motion controllers. You need both models to run simulations.

The entry of the simulation is `Hummingbird_Main.slx`. Within this model, you can specify a simulated position and velocity trajectory for the simulator to start or import log data from the MATLAB workspace.

`Hummingbird_Main.slx` references `Nonlinear_Motor_Tracking`, which is a high-fidelity emulation of the motor dynamics and speed control strategy. We model the dynamics of the BLDC motor as a second-order system (taking the inductance into account) and apply a PI controller to improve speed tracking performance. All dynamic parameters and controller gains used in real experiments are being used in simulation. Refer to the simulink parameters for their values.

For questions, contact Yilun Wu at <yl.wu@robotics.utias.utoronto.ca>.
