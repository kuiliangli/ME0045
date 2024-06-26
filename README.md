# ME0045
Matlab Apps for ME0045\
\
Spectrum Analyzer\
The Spectrum_Analyzer is essentially a simple spectrum analysis MATLAB app with some add-on features.\
Upon lauching, the App initializes and calibrates to measure the startup transient of the system. For most windows machines, this startup transient could be turned off in the sound setting. However, for the general user, it is easier to have this feature integrated into the app.\
If a custom trim length is wanted for higher accuracy or if the default trimmer isn't working as intended, the user can always add a "custom trim" to the recording process. The default value will be the value observed at the startup of the application.\
The default recording length will be 1 second + the trim length, meaning that the user will always be left with 1 second worth of data. This could be manipulated through changing the "Record Length" editfield.\
Upon clicking the "plot" button, the app records from the default input device at the selected/default specs.\
The time domain signal is plotted on the top of the UI, while the FFT signal is plotted on the bottom side.\
\
Waves Filter\
The Waves_Filter app is an app designated to visualize how filter could change a square wave signal.\
Upon lauching the app, the original square wave is generated through the bottom left text boxes.\
Entering numbers in the frequency and duration text box can control the base square wave pre-filtered.\
The "Max Time" and "Max Feq." text boxes are there to control the x limits of the original time-domain signal as well as the FTT'ed frequency-domain signal.\
The filter applied is a Butterworth filter, where the order, normalized cutoff frequency, and filter type (high-pass or low-pass) could be controlled through the respective control interfaces.\
Hitting the "Generate and Plot" shows the two graphs of the filtered signal, while hitting the "Play" button plays the resulting signal.\
\
Wave builder & filter\
This is a MATLAB app based on the previous filter app. The sub-UI enables the user to create custom source waveforms instead of just square waves.\
The main generator is the base UI for this application. The sub-UI is called "generatorApp".\
The main generator is basically the same with the filter application, with only one addition of a button.\
This button prompts the sub-UI which generates a custom waveform function. The generator is used by moving the sliders on underneath each one of the specific wave types.\
The sliders correspond to a coefficient that multiplies the corresponding waveform.
After each change in position of the sliders, the waveform graphs on the left will show a cycle of the result waveform on the top and the FFT graph of the corresponding waveform.\
The frequency text box could be adjusted to change the frequency of the waveform, while the Max freq. changes the x axis limit of the FFT graph.\
After clicking "Done", the sub-UI is closed, and the custom waveform function is saved as the base waveform to be filtered in the main filter app as described in the last app.
