# ME0045
Matlab Apps for ME0045 class
Spectrum Analyzer
The Spectrum_Analyzer is essentially a simple recording MATLAB app with some add-on features.
Upon lauching, the App initializes and calibrates to measure the startup transient of the system. For most windows machines, this startup transient could be turned off in the sound setting. However, for the general user, it is easier to have this feature integrated into the app.
If a custom trim length is wanted for higher accuracy or if the default trimmer isn't working as intended, the user can always add a "custom trim" to the recording process. The default value will be the value observed at the startup of the application.
The default recording length will be 1 second + the trim length, meaning that the user will always be left with 1 second worth of data. This could be manipulated through changing the "Record Length" editfield.
Upon clicking the "plot" button, the app records from the default input device at the selected/default specs.
The time domain signal is plotted on the top of the UI, while the FFT signal is plotted on the bottom side.
