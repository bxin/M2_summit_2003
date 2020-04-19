# M2_summit_2003

This repository contains notebooks used for analyzing data from the March 2020 M2 testing on the summit.

### a01_OL_B1_stroke.ipynb            
We commanded actuator B1 by stroke (position) in open loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a02_check_telemetry.ipynb 
We look through the telemetry topics (44 of them in the binary file). Data we use are same as a01_OL_stroke.ipynb, taken on Thursday night (3/4/20)
    
### a03_LUT_0.ipynb 
In this notebook, we compare binary file LUT with Harris csv files, for zenith angle = 0 only (M2 facing down).
    We use the same data as in a01_OL_stroke.ipynb
    
### a04_FB.ipynb
We examine how the FB responds when we impose a force offset on one of the actuators.
    We use the same data as in a01_OL_stroke.ipynb. This test was done on Thursday night (3/4/20)

### a05_OL_B1_steps.ipynb
We commanded actuator B1 by steps in open loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a06_CL_B1_F.ipynb
We commanded actuator B1 by force in closed loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a07_log_events.ipynb
We look at the state transitions during the testing.

### a08_OL_A1_stroke.ipynb 
We commanded tangent link A1 by stroke (position) in open loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a09_Kdc.ipynb
The notebook studies the decoupling matrix Kdc.

### a10_OL_A1_steps.ipynb
We commanded tangent link A1 by steps in open loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a11_CL_A1_F.ipynb 
We commanded tangent link A1 by force in closed loop. Data were taken on Thursday night (3/4/20). Here we examine the relations between forces, encoder counts, steps, and positions.

### a12_temperature.ipynb  
Check temperature sensor readings. We use data that were taken for a01_OL_stroke.ipynb, taken on Thursday night (3/4/20), and also thermal data from each morning.

### a13_position_calib.ipynb 
We wanted to measure the net force and moments, and move the mirror around to find the best position where the force balance load is minimized.

### a14_back_drive.ipynb 
This notebook checks to make sure M2 position and forces did not change after actuator de-energization

### a15_bump_test.ipynb 
This is standard bump test, where we put positive and negative forces on each actuator in turn.
This was performed on 3/6/20, and repeated 3 times. The bump test verifies that all actuators are alive and responds to force commands properly.

### a16_bending_modes.ipynb
This is for bending mode test, where we put positive and negative bending for each bending mode in turn (up to 20).
This was performed on 3/6/20, and repeated 3 times. We check the force accuracy and repeatability.

### a17_LUT_cart_rotation.ipynb
In this test we rotated the M2 on its cart from 0 to 180 degrees then back. We paused at various elevation angles.
Here we check the LUT operations at random elevation angles between 0 and 180 degrees.

### a18_motion_limit.ipynb
This test was about M2 motion limits. Note that we run into actuator actuator limit switches long before we run into the safety stops.

### a19_position_repeatability.ipynb
We moved M2 to various positions along +/-x, +/-y, +/-z, and tilt and rotation angles. We examine the position repeatability and hysterisis.

### a20_force_limit.ipynb
This test verifies that the maximum forces output by the actuators are large enough to meet the force range requirements, but small enough to stay within the maximum force limit.

### a21_strokes.ipynb
This test was about the M2 actuator strokes. Note that with the surrogate mirror (or glass mirror) attached to the mirror cell, we run into limit switches long before we reach the full actuator strokes.

### a22_aos_duration.ipynb
In this notebook we look at the data from the AOS duration test. In that test, we picked 5 low order bending modes (one astigatism, trifoil, focus, coma, and quadrafoil),
and applied them in turn. Each time we apply a bending mode, we hold it for 37s. We examine the force accuracy and repeatibility.

### a23_bandwidth.ipynb
Check statistics of the EFD data from M2 functional tests in Mar 2020. Confirm that the M2 data stream has bandwidth of 20Hz.
We also check the EFD latency and data loss rate.

### a24_position_sensors.ipynb
We use the readings from the 12 displacement sensors to calculate the 6 DOFs of M2. The data used are the same as those used in a19_position_repeatability.ipynb. The 6x12 matrix used to convert the 12 displacement sensor readings into 6 M2 DOFs is saved in disp2dof.txt

