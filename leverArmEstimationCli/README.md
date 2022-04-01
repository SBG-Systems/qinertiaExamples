# Introduction
Demonstrates how to leverage on Qinertia to estimate GNSS primary and secondary lever arms.
High Performance SBG Systems INS come with and automatic real time lever arm estimation tools.
Estimating lever arms require some specific maneuvers and some dynamics.

Qinertia post processing software also offers mechanical installation parameter estimation and has several advantages over a real time estimation.
The estimation process is more stable and accurate especially in low dynamic environments such as large vessels or planes.
It can also be used for products such as ELLIPSE that don't have a built in lever arm estimation module.

This example, simply process a calibration acquisition using loosely coupling to compute and export estimated lever arms.
If you use loosely coupling to estimate mechanical installation parameters, you have to make sure the real time GNSS is providing valid RTK or PPP (Precise Point Positioning) positions.
Otherwise, please consider using Qinertia Tightly Coupled computations to access centimeter-level accuracy.

# Launching the Processing
To start the processing, simple go to the Qinertia CLI directory and type the following command line:

  qinertia-cli.exe process --license ########## --process-file "pathToData\leverArmEstimationCli.json"

# Extracting Estimated Lever Arms
Once the process is successfully done, Qinertia generates a PDF and a JSON processing report.
The PDF report is used for human QC assessment and to review the estimated lever arms.

The JSON report can be used to automatically extract the estimated lever arms.
You can find the results and status in the `reports/json/reportMinimal.json` file.
In the JSON file, you should look at the JSON node: `processing:mechanicalParametersEstimation`

# Qinertia Version
This CLI example has been designed and tested for Qinertia 3.1 versions.

# Legal Notices
Copyright (C) 2022 SBG Systems - All Rights Reserved

You can ONLY use the provided data and information to evaluate Qinertia CLI.
You should NOT distribute the processed data to anyone.
You should NOT use the provided data with an other software.

Please contact the support team support@sbg-systems.com if you have any question.