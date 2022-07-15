# Introduction
This is a simple NAVSIGHT acquisition used to demonstrate basic Qinertia CLI usage.

This log uses a single base station to compute a post processed tightly coupled INS solution.\
The log has been acquired in a car with a NAVSIGHT-S connected to an APOGEE-I.\
The mechanical configuration has been entered in the NAVSIGHT unit itself and is read by Qinertia automatically.

# Launching the Processing
To start the processing, simple go to the Qinertia CLI directory and type the following command line:

```console
qinertia-cli.exe process --license ########## --process-file "pathToData\simpleDemo.json"
```

# Qinertia Version
This CLI example has been designed and tested for Qinertia 3.1 versions and above.

# Legal Notices
Copyright (C) 2022 SBG Systems - All Rights Reserved

You can ONLY use the provided data and information to evaluate Qinertia CLI.\
You should NOT distribute the processed data to anyone.\
You should NOT use the provided data with an other software.

Please contact the support team support@sbg-systems.com if you have any question.