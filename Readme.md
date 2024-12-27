# Working with Sensor Data
These examples show methods for simple manipulations of raw data for more advanced interactions. They are designed specifically for the [Arduino Nano33 IOT](https://docs.arduino.cc/hardware/nano-33-iot/), but the methods are applicable to other microcontrollers.

- **6 DOF IMU (Inertial Measurement Unit):**
   - **Basic Acceleration:** Measures acceleration in X, Y, and Z axes and calculates total movement magnitude. ([imu_accelerationData.ino](Sensors/IMU/imu_accelerationData/imu_accelerationData.ino))
   - **Orientation Data:** Uses SensorFusion to calculate Roll, Pitch, and Yaw in degrees. ([imu_orientationData.ino](Sensors/IMU/imu_orientationData/imu_orientationData.ino))

- **Distance Sensor:**
   - **Raw and Smoothed Distance:** Calculates both the basic distance value and a smoothed value using a rolling average. ([distance_raw_smoothed.ino](Sensors/Distance/distance_raw_smoothed/distance_raw_smoothed.ino))
   - **Motion Detection:** Calculates the total motion and 1D direction (Toward/Away). ([distance_motionDetection.ino](Sensors/Distance/distance_motionDetection/distance_motionDetection.ino))

- **Light Sensor:**
   - **Basic Light Reading:** Reads the immediate value as well as a smoothed value calculated with a rolling average. Compares the current value to the calibrated value read at startup. ([ligh_raw_smoothed.ino](Sensors/Light/ligh_raw_smoothed/ligh_raw_smoothed.ino))
   - **Compare Sensors:** Reads and compares values from two light sensors to determine which sensor is darker. ([light_compareSensors.ino](Sensors/Light/light_compareSensors/light_compareSensors.ino))

- **Potentiometer:**
   - **Basic Reading:** Reads the immediate value as well as a smoothed value calculated with a rolling average. ([potentio_smoothed.ino](Sensors/Potentiometer/potentio_smoothed/potentio_smoothed.ino))
   - **Direction and Velocity:** Calculates the velocity and direction of the turning motion. ([potentio_direction_velocity.ino](Sensors/Potentiometer/potentio_direction_velocity/potentio_direction_velocity.ino))

- **Capacitive Touch 5:**
   - **Basic Touch Reading:** Reads touch inputs. ([touch5.ino](Sensors/Capacitive/touch5/touch5.ino))
   - **Touch Timing:** Calculates the speed of touch/release on Input 1. ([touch5_tapTime_tapSpeed.ino](Sensors/Capacitive/touch5_tapTime_tapSpeed/touch5_tapTime_tapSpeed.ino))

- **Capacitive Touch 8:**
   - **Basic Reading:** Reads and unpacks all 8 values. ([touch8.ino](Sensors/Capacitive/touch8/touch8.ino))
   - **Compare Touch Speed:** Reads touch data on inputs 0 and 1, calculates the touch/release speed for both, and compares them. ([touch8_tapSpeedComparison.ino](Sensors/Capacitive/touch8_tapSpeedComparison/touch8_tapSpeedComparison.ino))
