# GNURadioThresholdingDemonstration
Demonstrates the signal strength threshold required for a signal to be reliably received over another signal on the same channel.

The purpose of this code is to simulate the reception of multiple RF signals on a single channel and compare the reception for different modulation schemes. The two modes used for this example are Double Sideband Full Carrier (AM) and Wideband Frequency Modulation (FM). The modes are compared in terms of a minimum ratio of signal strengths required for the stronger signal to be received over the weaker signal. This threshold ratio can be measured either in terms of being able to detect the desired signal between the two signals or in terms of being able to adequately reject the undesired signal.

# Installation

In order to run the `AM_Threshold.grc` demo, the `AM-Modulator.grc` block must first be run to initialize the custom AM Modulator block. After that, both the `AM_Threshold.grc` and the `FM_Threshold.grc` demos should function as desired.

# Running

A set of sliders shall be used to control the relative amplitudes of the AM and FM signals being transmitted through the common channel.

The expected result of the demonstration is to show the linear superposition of AM signals, but a thresholding capture effect for FM signals.
When the AM signals have similar gains, both should be heard over each other. A threshold of around 10-13dB is required to adequately suppress the undesired signal.
When the FM signals have similar gains, only the stronger signal properly demodulates. The weaker signal is not properly demodulated and instead only distorts and adds noise to the stronger demodulated signal. With only a 0.1dB threshold, the stronger signal can be distinctly heard over the weaker signal. With a threshold of around 3-6dB, the distortion from the weaker signal is suppressed to an acceptable level.
