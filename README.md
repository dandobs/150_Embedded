# 150_Embedded

This project was made to mimic a laser doorway such that the number of objects entering/leaving a ‘room’ is recorded. 
This is done by reading the number of breaks in a laser’s path, as sensed by a photodiode. 
The project also incorporates debouncing with hysteresis to increase the effectiveness of the 
photodiodes and to not overcome false positives/negatives. 
In addition, the raspberry pi watchdog was implemented to recover in case the system gets stuck in a loop/crashes/etc. 
This system was designed to run without constant monitoring, and as a result, it was configured to run on startup, 
and print log information to a log file and laser breaks information to a statistics file.
