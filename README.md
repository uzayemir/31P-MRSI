# Ultra-Short Echo Time 31P 3D MRSI at 3T with Novel Rosette k-space Trajectory

Use the following link to download post-processing and sequence files 
https://purr.purdue.edu/projects/ismrm31pmrsi

# REPORT: 2022-23 ISMRM Challenge Repeat It With Me: Reproducibility Team Challenge
## Ultra-Short Echo Time 31P 3D MRSI at 3Twith Novel Rosette k-space Trajectory
## Original Authors: Uzay E Emir
## Reproducers: Ulrich Pilatus, Goethe University Frankfurt
## Seyma Alcicek, Goethe University Frankfurt
## Alexander Richard Craig-Craven, University of Bergen

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/k-fSdqBT_9o/0.jpg)](https://www.youtube.com/watch?v=k-fSdqBT_9o)

https://youtu.be/qQSBB_Lwarc
# Comparison of Compressed Sensing Accelerated Rosette UTE and Conventional 31P 3D MRSI at 3T in Leg Muscle

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/qQSBB_Lwarc/0.jpg)](https://youtu.be/qQSBB_Lwarc)

### Cardiac 31P MRSI 
### PCr map
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/31PRAPIDSurfaceCoilLiver.png?raw=true)

# ATP/PCr Accelaration x4 
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/accelaration_UTE_MRSI2.png?raw=true)



# ATP/PCr Accelaration x2 
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/31PMRSIx2.png?raw=true)



# AUTHORS
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/authors.jpg?raw=true)

## SUMMARY
Our group proposes a 31-P MRSI sequence utilizing Rosette-Petal shaped 3D k-space 
acquisition to achieve 1 mL isotropic resolution (10x10x10mm^3) over a FOV of 480x480x480mm^3 
with a total scanning duration of 6.7 minutes using a Siemens Prisma 3T scanner.

## Method

A custom rosette trajectory (Shen et al. 2022) was used with an isotropic FOV = (480mm)^3 and an imaging 
matrix grid of 48x48x48 voxels.  The spectral bandwidth was 2083 Hz, a TE = 50 us, a TR = 350 ms, and a total of 1444 Petals.  Total scan duration = 8.4 minutes. Anatomical data was acquired through an Ultrashort Echo Time Magnetization Transfer (UTE-MT)  sequence which uses a pair of adiabatic hyperbolic secant (sech) 180-degree pulses with a pulse duration  of 24ms, a pulse bandwidth of 1kHz, an offset frequency of ~1300 Hz from water. Image reconstruction and post-processing steps were performed in MATLAB (MathWorks, USA). Nonuniform fast Fourier transform (NUFFT) was used to calculate the forward encoding transform of the acquired k-space data. A compressed sensing approach was used for image reconstruction, using total generalized variation (TGV) as the sparsifying penalty. The complex-valued coil sensitivity maps were first extracted from the center of k-space using ESPIRIT for coil combination. We used  LCModel for the quantificatio of in vivo 31P NMR Brain Spectra using LCModel. 

## Pulse diagram with a delay of 10 us between RF pulse and the ADC  
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/31pmrsi.png?raw=true)


## Acquisition Protocol

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/IMG_4390.jpg?raw=true)


**K-SPACE**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0001-m.jpg?raw=true)

**PSF**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0003-m.png?raw=true)

**SNR**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0005-m.png?raw=true)


In order to achieve the acceptable acquisition timing in clinical settings (reconstructed images with accelaration factor = 2 and 4 were tested for further acceleration purpose. 

## Results 

 (α-ATP+β-ATP+γ-ATP)/phosphocreatine (PCr) and inorganic phosphate (Pi)/PCr
 
 

### Lcmodel findings of accelaration factor = 1 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc1_23_27_24.jpg?raw=true)

#### (α-ATP+β-ATP+γ-ATP)/phosphocreatine (PCr) 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex1atps.png?raw=true)

#### inorganic phosphate (Pi)/PCr

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex1pi.png?raw=true)

### Lcmodel findings of accelaration factor = 2

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc2_23_27_24.jpg?raw=true)


#### (α-ATP+β-ATP+γ-ATP)/phosphocreatine (PCr) 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex2atps.png?raw=true)

#### inorganic phosphate (Pi)/PCr

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex2pi.png?raw=true)


### Lcmodel findings of accelaration factor = 4

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc4_23_27_24.jpg?raw=true)

#### (α-ATP+β-ATP+γ-ATP)/phosphocreatine (PCr) 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex4atps.png?raw=true)

#### inorganic phosphate (Pi)/PCr

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/imagex4pi.png?raw=true)

[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/ujU8WiZdrcM/0.jpg)](https://www.youtube.com/watch?v=ujU8WiZdrcM)




### Cardiac 31P MRSI 
### PCr map
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/Fkmyq9mXEAE410X.jpg?raw=true)
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/CARDIAC.png?raw=true)



## Spatial Response Function Analysis

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure6.svg?raw=true)

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure1.svg?raw=true)
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure2.svg?raw=true)
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure3.svg?raw=true)
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure4.svg?raw=true)
![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/figure5.svg?raw=true)


Courtesy of Alex Craig-Craven

Whole Brain 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/FonduVwXEAAdmjn.jpg?raw=true)

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/lcmodel.png?raw=true)

Courtesy of Seyma Alcicek

Whole Brain 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/FqEJ81xWYAQbTXL.jpg?raw=true)


https://www.researchgate.net/publication/358462656_Ultra-Short_Echo_Time_31P_3D_MRSI_at_3T_with_Novel_Rosette_k-space_Trajectory

https://www.researchgate.net/publication/368259219_Comparison_of_Compressed_Sensing_Accelerated_Rosette_UTE_and_Conventional_31P_3D_MRSI_at_3T_in_Leg_Muscle
https://www.researchgate.net/publication/368258393_Fast_3D_31P_MRSI_Using_Novel_Rosette_Petal_Trajectory_at_3T_with_x4_Accelerated_Compressed_Sensing

Shen, Xin, et al. "Ultra-short T2 components imaging of the whole brain using 3D dual-echo UTE MRI 
with rosette k-space pattern." Magnetic Resonance in Medicine (2022).
