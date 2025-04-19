# GNURadioThresholdingDemonstration
Demonstrates the signal strength threshold required for a signal to be reliably received over another signal on the same channel.

The purpose of this code is to simulate the reception of multiple RF signals on a single channel and compare the reception for different modulation schemes. The two modes used for this example are Double Sideband Full Carrier (AM) and Wideband Frequency Modulation (FM). The modes are compared in terms of a minimum ratio of signal strengths required for the stronger signal to be received over the weaker signal. This threshold ratio can be measured either in terms of being able to detect the desired signal between the two signals or in terms of being able to adequately reject the undesired signal.

A set of sliders shall be used to control the relative amplitudes of the AM and FM signals being transmitted through the common channel.

The expected result of the demonstration is to show the linear superposition of AM signals, but a thresholding capture effect for FM signals.
