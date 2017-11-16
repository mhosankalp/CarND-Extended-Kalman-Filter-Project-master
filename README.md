# Extended Kalman Filter implementation in C++

This is the C++ code to implement extended kalman filter.
main.cpp file is to communicates with the Term 2 Simulator receiving data measurements, calls a function to run the Kalman filter, calls a function to calculate RMSE. It reads in the data and sends a sensor measurement to FusionEKF.cpp. 
FusionEKF.cpp file is to initializes the filter, calls the predict function, calls the update function.It takes the sensor data and initializes variables and updates variables. FusionEKF.cpp has a variable called ekf_, which is an instance of a KalmanFilter class. The ekf_ will hold the matrix and vector values. You will also use the ekf_ instance to call the predict and update equations.
kalman_filter.cpp is to defines the predict function, the update function for lidar, and the update function for radar
tools.cpp is to function to calculate RMSE and the Jacobian matrix.

The final RMSE for dataset 1 is [0.0973, 0.0855, 0.4513, 0.4399]. See figure below in the simulator
