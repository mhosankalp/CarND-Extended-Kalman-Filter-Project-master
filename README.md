# Extended Kalman Filter implementation in C++

This is the C++ code to implement extended kalman filter.
1. main.cpp file is to communicates with the Term 2 Simulator receiving data measurements, calls a function to run the Kalman filter, calls a function to calculate RMSE. It reads in the data and sends a sensor measurement to FusionEKF.cpp. 
2. FusionEKF.cpp file is to initializes the filter, calls the predict function, calls the update function.It takes the sensor data and initializes variables and updates variables. FusionEKF.cpp has a variable called ekf_, which is an instance of a KalmanFilter class. The ekf_ will hold the matrix and vector values. You will also use the ekf_ instance to call the predict and update equations.
3. kalman_filter.cpp is to defines the predict function, the update function for lidar, and the update function for radar
4. tools.cpp is to function to calculate RMSE and the Jacobian matrix.

The final RMSE for dataset 1 is [0.0973, 0.0855, 0.4513, 0.4399]. See figure below in the simulator

  <img width="632" alt="screen shot 2017-11-16 at 2 09 29 pm" src="https://user-images.githubusercontent.com/22051168/32910667-df2983d8-cad7-11e7-9df5-2af73d473e27.png">


The final RMSE for dataset 2 is [0.0726, 0.0965, 0.4216, 0.4932]. See figure below in the simulator

  <img width="633" alt="screen shot 2017-11-16 at 2 09 13 pm" src="https://user-images.githubusercontent.com/22051168/32910676-e718646a-cad7-11e7-9014-c3474435c827.png">





