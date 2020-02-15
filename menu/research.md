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
source beam and the ones that are formed by neutrino oscillations. There are two major parts of 
this project. 
* Optimisation of the Detector geometry. 
* The reconstruction of EM showers and neutral pion decay.

The aim of this project is to investigate new methods based on statistics and machine
learning to determine the basic characteristics of π0 like its mass, position, separation
angle between both gamma particles, momentum, kinetic energy etc.

## Motivation
In 1957, Bruno Pontecorvo postulated neutrino oscillations and in 1960, after discovery of the second type of neutrino, he suggested that there is oscillation of muon type neutrino to electron type neutrino . Finally, oscillations of atmospheric neutrinos were evidently seen at the Super-Kamiokande experiment in 1998, which supported this postulate. It also showed that the deficit in atmospheric muon type neutrino depends on the neutrino path length and energy.
 
 In 2001, oscillations of solar neutrinos were discovered in the SNO experiment. The SNO collaboration published strong evidence for the flavour transformation of electron neutrinos into muon and tau neutrinos.
 
 In 2003, oscillations of reactor neutrinos were discovered in KamLAND with the disappearance of $\bar\nu_e$ for long neutrino path length. 
 
There were many more recent experiments that confirm Bruno's postulate. 
 
Neutral pion plays an important role in the study of neutrino oscillations. The muon type neutrino  oscillates to electron type neutrino as it moves through space. To observe these neutrino oscillations, we use an initial beam of muon type neutrino and observe its conversion to electron type neutrino by calculating the amount of electron and muon detected in the long baseline detector. 

As electromagnetic calorimeter gives information about energy deposition only, the gamma shower and electron shower from muon type neutrino to electron type neutrino oscillation are indistinguishable. Neutral pion decays predominantly into two gamma showers, thus it can be easily mistaken as two electron showers which will result in miscalculation of the neutrino oscillation.

## The Detector 

To study the characteristics of the particles, the simulation of the real detector is done using Geant4 software. The detector that we are using to study neutral pion decay is an electromagnetic calorimeter made of consecutive alternating horizontal and vertical bars of plastic scintillator with lead plates in between them.

Electromagnetic calorimeter detects particles by slowing and stopping them, hence there would be energy deposition during this process which is collected and measured. Electromagnetic calorimeter detects particles that interact via electromagnetic interactions for example charged particles like electrons and positrons.

The simulated detector is made according to the T2K Electromagnetic calorimeter which shows maximum efficiency in detection of particle's hits data (hits data is the data containing information about position, momentum, kinetic energy etc of the particle). Each plate consists of 160 bars aligned in a particular direction with dimensions as 4m × 2.5cm × 1cm. Each lead plate is of dimension 4m × 4m × 1.75mm. Hence the overall dimension of Detector is 4m × 4m × 0.7m

<img src="../assets/img/detector.png">

The Scintillator material is used for detection of the pion as it absorbs the incoming particles energy and re-emits as light which we measure and use for further analysis. Lead Sheet is used for slowing down the particles so that it doesn't escape the detector.

## Reconstruction

The reconstruction algorithm is based on machine learning and pattern recognition. 3D Iterative Hough transform is used to find the most poppulated lines in space, which determines the main path of the 2 gamma particles. After determining the lines, various clustering methods are used to seperate out the gamma particles whose total energy gives us the invariant mass of incoming particle. Hence we can determine if the incoming particle is a pion or not.

<img src="../assets/img/pion.png">

This Image shows the two gamma showers after reconstruction and the line intersecting is the vertex.

## Results

From  the  Reconstruction  algorithm,  we  obtain  the  position  of  vertex,  separation angle between the two gamma showers and the invariant mass of pion. Here are some results for pion of energy 0.2, 0.5, 0.8, 1.2 GeV

Separation Angle of gamma showers for 0.2 GeV pion
<img src="../assets/img/a02.pdf">
Separation Angle of gamma showers for 0.5 GeV pion
<img src="../assets/img/a05.pdf">
Separation Angle of gamma showers for 0.8 GeV pion
<img src="../assets/img/a08.pdf">
Separation Angle of gamma showers for 1.2 GeV pion
<img src="../assets/img/a12.pdf">

Figure 5.2 and 5.3 shows the separation angle we get from the MC truth data for0.2  and  0.5  GeV  respectively.   This  is  calculated  but  considering  the  momentuminformation of the two initial gamma.

The Vertex plot.
<img src="../assets/img/vertex_sim.png">

The Pion Mass plot.
<img src="../assets/img/mass.png">

We calculate the separation angle for 4 energies and compare them with our recon-structed separation angle.  Fig 5.4, 5.5 shows the separation angle we get from theMC truth data for 0.8 and 1.2 GeV respectively.


The mean separation angle for pion kinetic energy as 0.2, 0.5, 0.8, 1.2 GeV is 60, 34,23, 16 degree respectively.
In Fig 5.6 to 5.9, the Reconstructed separation angle is shown for energies 0.2,0.5,0.8,1.2 GeV

The peak of the reconstructed separation angle of the two gamma showers are 29,31, 17, 13 for energies 0.2, 0.5, 0.8, 1.2 GeV. 
This shows that the algorithm fails for pions with very low energy such as 0.2 GeV.Fig 5.10 to 5.13 shows the position of vertex of the pion for energies 0.2,0.5,0.8, 1.2GeV. The pion generated by Mc has position of vertex at 0.0 cm

The Reconstructed position of vertex of the pion peaks near 3cm to 4cm for energyrange from 0.2 to 1.2 GeV. And the maximum deviation from the original vertexposition is around 20cm.The Fig 5.14 to 5.17 shows the invariant mass of the pion while the kinetic energyof the pion is 0.2, 0.5, 0.8, 1.2 GeV.

From figure 5.14 and 5.17 we can say that the algorithm doesn’t work very well forvery low or high energy pions.
