# Signal background discrimination using CNN
## __Overview__
The aim of this project is to develop a Convolutional Neural Network which does a signal-background discrimination. Here Gamma is the signal and proton is the background. We are using air shower data initiated by Gamma and protons. The data has been simulated using 2 softwares CORSIKA and Sim_telarry which generates air showers and telescopes respectively. From the telescope images, I have seen that most of the proton images have muon rings of different radius. So the idea was to develop a CNN which seperates protons(background) from Gamma(signal). <br>
## __Data Structure__
The data used here are telescope pixel data in Numpy format (.npy). Signal images are the air shower images generated from Gamma primary and the background images are the ones generated from Proton primary. Signal and background images are located in 2 folders locally: 1) Signal-Photon and 2) Background-Proton. After several trials I have come up with 2 CNN, one after another to increase the quality of separation. First CNN (gamma/Proton) seperates protons from Protons, second CNN (Ring/no-ring) separates images with rings (Usually Proton) from images without ring (Usually Gamma). Quality of separation is calculated using Quality factor using individual signal/background efficiencies. <br>
- The data preprocessing has been done using Pandas before importing the data here in the notebooks. 
# __Settings__
Setting up the virtual environment:<br>
- Install latest version of Pytorch using Anaconda
