# Beta-Burst-Detection
Algorithms used to detect beta-bursting activity in EG data

# Description of bursts
Beta bursting activity occurs all across the brain as transient burst-like events.
Detection can be performed by extracting beta band power, then thresholding.
Bursts are considered maxima of beta power over short time intervals (30-150 ms)

# Algorithms used
This repository contains 2 different algorithms to detect such events:

1) Based on
   Apply a Morlet wavelet across the beta band
   Average obtained beta burst means across all frequencies [15-35] Hz
   Use a threshold (FOM) to extract maxima in the processed data

3) Based on ...
   Bandpass data from beta band [15-35] Hz
   Apply a Hillbert filter across the bandpassed data
   Use a threshold (SD) to extract maxima in the processed data
