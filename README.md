# Qinertia CLI Examples
Qinertia is a professional GNSS/INS post processing software.

This modern GNSS/INS Post Processing Software can be used with any RTK capable GNSS receivers to deliver centimeter-level Post Processed Kinematic solution (PPK).\
Qinertia can also accepts Inertial Measurement Unit (IMU) data to provide a highly accurate and robust tightly coupled GNSS/INS solution.

Qinertia offers an intuitive and powerful Graphical User Interface as well as an easy to use and full-featured Command Line Interface (CLI).

Please visit the official Qinertia web page to get more details: https://www.sbg-systems.com/products/qinertia-ins-gnss-post-processing-software/

The full Qinertia documentation can be found here: https://support.sbg-systems.com/sc/qd/latest

# GNSS modes
Qinertia has been designed from the ground up to support latest GNSS technologies and signals to deliver the most reliable, robust and accurate solution on the market.

It offers unique features such as Precise Point Positioning and Virtual Base Station (VBS) GNSS augmentation.\
Qinertia comes with a built in world-wide CORS (Continuously Operated Reference Stations) GNSS reference stations to offer centimeter-level accuracy.

# Photogrammetry & DJI
Qinertia includes a dedicated module for photogrammetry. Qinertia can post process GNSS and, if available, IMU data to output a highly accurate orientation and position of each picture.

Qinertia can also update pictures EXIF/XMP metadata with this highly accurate camera orientation (roll, pitch, yaw) and position to enable high quality and reliable 3D photogrammetry reconstructions.

Qinertia has a specific support for DJI UAV such as the Phantom 4 RTK, the Matrice 300 RTK with Zenmuse P1 payloads.\
Qinertia directly reads DJI acquisitions data to compute an accurate Post Processed Kinematic solution (PPK).\
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

## Simple Demo
This is a simple NAVSIGHT acquisition used to demonstrate basic Qinertia CLI usage.

This log uses a single base station to compute a post processed tightly coupled INS solution for a NAVSIGHT unit.

## Lever Arm Estimation
Demonstrates how to leverage on Qinertia to estimate GNSS primary and secondary lever arms.

You can use Qinertia to easily estimate mechanical installation parameters such as lever arms and alignments.\
This project shows primary GNSS antenna lever arm and dual antenna alignment estimation using a loosely coupled processing.

## Mechanical Estimation Pass
This project demonstrates the `mechanicalEstimationPass` parameter for Qinertia CLI.

With this parameter, Qinertia can automatically estimate mechanical parameters such as lever arms and then post process the data using the estimated parameters.