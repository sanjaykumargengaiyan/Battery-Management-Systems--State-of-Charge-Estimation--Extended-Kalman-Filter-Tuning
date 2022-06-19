# Battery-Management-Systems-State-of-Charge-Estiimation--Extended-Kalman-Filter-Tuning

The goal of Part 1 of the capstone project is to hand-tune an EKF by selecting values for the covariances of process noise, 
sensor noise, and for the error of the initial SOC estimate. You will do this by trial-and-error to get the best result you are able to find.

When tuning an EKF for a real application, these covariances are tuned so that the filter gives good and robust performance 
over a wide variety of operating conditions. However, for this project you will tune the filter to operate well for 
only a single operating scenario (otherwise, the project would take too long to complete).

The scenario that you will be working with exercises a battery cell with an urban dynamometer driving cycle (UDDS). 
The cell is at an initial SOC of 95%. However, the EKF will assume an initial SOC estimate of 90%. 
So, part of the challenge in tuning the filter is to find covariance values that allow the filter to operate 
even with this initial error in the SOC estimate (which might be caused in practice by a poor initial voltage measurement, for example).
