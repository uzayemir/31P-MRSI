# Ultra-Short Echo Time 31P 3D MRSI at 3T with Novel Rosette k-space Trajectory
#

Our group proposes a 31-P MRSI sequence utilizing Rosette-Petal shaped 3D k-space 
acquisition to achieve 1 mL isotropic resolution (10x10x10mm^3) over a FOV of 480x480x480mm^3 
with a total scanning duration of 6.7 minutes using a Siemens Prisma 3T scanner.

## Method

A custom rosette trajectory (Shen et al. 2022) was used with an isotropic FOV = (480mm)^3 and an imaging 
matrix grid of 48x48x48 voxels.  The spectral bandwidth was 2083 Hz, a TE = 50 us, a TR = 350 ms, and a total of 1444 Petals.  Total scan duration = 8.4 minutes. Anatomical data was acquired through an Ultrashort Echo Time Magnetization Transfer (UTE-MT)  sequence which uses a pair of adiabatic hyperbolic secant (sech) 180-degree pulses with a pulse duration  of 24ms, a pulse bandwidth of 1kHz, an offset frequency of ~1300 Hz from water. Image reconstruction and post-processing steps were performed in MATLAB (MathWorks, USA). Nonuniform fast Fourier transform (NUFFT) was used to calculate the forward encoding transform of the acquired k-space data. A compressed sensing approach was used for image reconstruction, using total generalized variation (TGV) as the sparsifying penalty. The complex-valued coil sensitivity maps were first extracted from the center of k-space using ESPIRIT for coil combination. We used  LCModel for the quantificatio of in vivo 31P NMR Brain Spectra using LCModel. 


**K-SPACE**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0001-m.jpg?raw=true)

**PSF**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0003-m.png?raw=true)

**SNR**

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/mrm29451-fig-0005-m.png?raw=true)


In order to achieve the acceptable acquisition timing in clinical settings (reconstructed images with accelaration factor = 2 and 4 were tested for further acceleration purpose. 

## Results 

### Lcmodel findings of accelaration factor = 1 

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc1_23_27_24.jpg?raw=true)


### Lcmodel findings of accelaration factor = 2

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc2_23_27_24.jpg?raw=true)


### Lcmodel findings of accelaration factor = 4

![alt text](https://github.com/uzayemir/31P-MRSI/blob/main/acc4_23_27_24.jpg?raw=true)




Shen, Xin, et al. "Ultra-short T2 components imaging of the whole brain using 3D dual-echo UTE MRI 
with rosette k-space pattern." Magnetic Resonance in Medicine (2022).
