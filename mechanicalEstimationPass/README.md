# Introduction
This project demonstrates the `mechanicalEstimationPass` parameter for Qinertia CLI.

Qinertia can automatically post process INS data to estimate mechanical parameters such as lever arms and alignments.\
Once this estimation is completed, a second post processing run is executed using the estimated parameters to achieve the best accuracy.

The log has been acquired in a car with a NAVSIGHT-S connected to an APOGEE-I.\
A user supplied Septentrio base station is used to compute the tightly coupled INS solution.\
The base station position frame is overridden to 'RGF93' datum.

# Launching the Processing
To start the processing, simple go to the Qinertia CLI directory and type the following command line:

```console
qinertia-cli.exe process --license ########## --process-file "pathToData\mechanicalEstimationPass.json"
```

# Qinertia Version
This CLI example has been designed and tested for Qinertia 3.2 versions and above.

# Legal Notices
Copyright (C) 2022 SBG Systems - All Rights Reserved

You can ONLY use the provided data and information to evaluate Qinertia CLI.
You should NOT distribute the processed data to anyone.
You should NOT use the provided data with an other software.

Please contact the support team support@sbg-systems.com if you have any question.