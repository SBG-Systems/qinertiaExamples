# Qinertia CLI Examples
Qinertia is a professional GNSS/INS post processing software.
This modern GNSS/INS Post Processing Software can be used with any RTK capable GNSS receivers to deliver centimeter-level Post Processed Kinematic solution (PPK).
Qinertia can also accepts Inertial Measurement Unit (IMU) data to provide a highly accurate and robust tightly coupled GNSS/INS solution.

Qinertia offers an intuitive and powerful Graphical User Interface as well as an easy to use and full-featured Command Line Interface (CLI).

Please visit the official Qinertia web page to get more details: https://www.sbg-systems.com/products/qinertia-ins-gnss-post-processing-software/

The full Qinertia documentation can be found here: https://support.sbg-systems.com/sc/qd/latest

# GNSS modes
Qinertia has been designed from the ground up to support latest GNSS technologies and signals to deliver the most reliable, robust and accurate solution on the market.

It offers unique features such as Precise Point Positioning and Virtual Base Station (VBS) GNSS augmentation.
Qinertia comes with a built in world-wide CORS (Continuously Operated Reference Stations) GNSS reference stations to offer centimeter-level accuracy.

# Photogrammetry & DJI
Qinertia includes a dedicated module for photogrammetry. Qinertia can post process GNSS and, if available, IMU data to output a highly accurate orientation and position of each picture.
Qinertia can also update pictures EXIF/XMP metadata with this highly accurate camera orientation (roll, pitch, yaw) and position to enable high quality and reliable 3D photogrammetry reconstructions.

Qinertia has a specific support for DJI UAV such as the Phantom 4 RTK, the Matrice 300 RTK with Zenmuse P1 payloads.
Qinertia directly reads DJI acquisitions data to compute an accurate Post Processed Kinematic solution (PPK).
The GNSS antenna to CMS lever arm offsets  are taken into account to update each picture with an accurate position.

With Qinertia, you get a turnkey solution to enable professional and reliable photogrammetry workflow for any platform and ideal for DJI solutions.

# Qinertia Version
Qinertia is being improved continuously and new features are added to Qinertia CLI.
Qinertia CLI has been designed to be backward compatible.
A project working with Qinertia 3.0 should thus still work with future Qinertia releases.

In this repository, you can find demo data for each Qinertia versions to showcase new features.
Please select the right tag version according to the Qinertia version you are using.

# Demo Projets
Qinertia offers a Command Line Interface (CLI) to automate processing and integrate PPK in a more complex workflow.
This repository hosts demonstration projects to showcase how to use the Qinertia CLI.

## Simple CLI
This is a simple NAVSIGHT acquisition used to demonstrate basic Qinertia CLI usage.
This log uses a single base station to compute a post processed tightly coupled INS solution.
The log has been acquired in a car with a NAVSIGHT-S connected to an APOGEE-I.
The mechanical configuration has been entered in the NAVSIGHT unit itself and is read by Qinertia automatically.

## Lever Arm Estimation CLI
Demonstrates how to leverage on Qinertia to estimate GNSS primary and secondary lever arms.
High Performance SBG Systems INS come with and automatic real time lever arm estimation tools.
Estimating lever arms require some specific maneuvers and some dynamics.

Qinertia post processing software also offers mechanical installation parameter estimation and has several advantages over a real time estimation.
The estimation process is more stable and accurate especially in low dynamic environments such as large vessels or planes.
It can also be used for products such as ELLIPSE that don't have a built in lever arm estimation module.

This example, simply process a calibration acquisition using loosely coupling to compute and export estimated lever arms.
If you use loosely coupling to estimate mechanical installation parameters, you have to make sure the real time GNSS is providing valid RTK or PPP (Precise Point Positioning) positions.
Otherwise, please consider using Qinertia Tightly Coupled computations to access centimeter-level accuracy.

Please contact the support team support@sbg-systems.com if you have any question.