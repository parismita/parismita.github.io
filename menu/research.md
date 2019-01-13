---
layout: post
title: "Research!"
author: "Parismita Das"
categories: journal
tags: [documentation,sample]
image: Selection_027.png
---

# Reconstruction of EM shower and π0 in ND Ecal

Neutrinos are abundant in nature, but it is very difficult to detect the neutrinos as
they are electrically neutral and they interact only via weak interactions. We aim
to observe the neutrino oscillation from muon type neutrino to electron type neutrino 
as it travels through matter.

We want to distinguish between a gamma shower due to neutral pion decay and an electron 
shower to determine the percentage of electron type neutrinos which already exist in the
source beam and which are formed by neutrino oscillations. There are two major parts of 
this project. 
* Optimisation of the Detector geometry. 
* The reconstruction of EM showers and neutral pion decay.

The aim of this project is to investigate new methods based on statistics and machine
learning to determine the basic characteristics of π0 like its mass, position, separation
angle between both gamma particles, momentum, kinetic energy etc.

## The Detector 

The detector that we are using to study neutral pion decay is an electromagnetic calorimeter.
This detector, used in this project, is proposed to be used in DUNE near detector. 
DUNE will consist of two neutrino detectors placed in the world’s most intense neutrino beam. One detector will record particle interactions near the source of the beam, at the Fermi National Accelerator Laboratory in Batavia, Illinois. A second, much larger, detector will be installed more than a kilometer underground at the Sanford Underground Research Laboratory in Lead, South Dakota — 1,300 kilometers downstream of the source.

We aim to detect the muon type neutrinos content in the beam in the near detector which interacts with the detector nucleus to give neutral pion. To study the characteristics of the particles, the simulation of the real detector is
done using Geant4 software. The detector that we are using to study neutral pion
decay is made of consecutive alternating horizontaland vertical bars of plastic scintillator with lead plates in between them.

<img src="../assets/img/detector.png">

The simulated detector is made according to the known standard Electromagnetic
calorimeter which shows maximum efficiency in detection of particle’s hits data
(hits data is the data containing information about position, momentum, kinetic
energy etc of the particle). Each plate consists of 160 bars aligned in a particular 
direction with dimensions as 4m × 2.5cm × 1cm. Each lead plate is of dimension
4m × 4m × 1.75mm. Hence the overall dimension of Detector is 4m × 4m × 0.7m
The Scintillator material is used for detection of the pion as it absorbs the incoming
particles energy and re-emits as light which we measure and use for further analysis.
Lead Sheet is used for slowing down the particles so that it doesn’t escape the
detector.

## Reconstruction

The reconstruction algorithm is based on machine learning and pattern recognition. We have used various methods like hough transform, PCA, DBScan etc for reconstruction of the neutral pion decay. We are trying to get the vertex and angle of seperation between the two gamma showers.

<img src="../assets/img/pion.png">

This Image shows the two gamma showers after reconstruction and the line intersecting is the vertex.

## Results

Here are results for a 500MeV pion. The seperation angle plot between the two gamma showers.

The Theoritical Seperation Angle plot
<img src="../assets/img/th.png">

The Reconstructed Seperation Angle plot.
<img src="../assets/img/ex.png">

The Pion Mass plot.
<img src="../assets/img/mass.png">

