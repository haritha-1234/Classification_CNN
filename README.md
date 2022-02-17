# Classification_CNN
Signal-Background descriminator using CNN. 
Here the data used are telescope pixel data in Numpy format. 
Signal and background images are located in 2 folders: Signal-Photon and Background-Proton.
Used 2 CNN one after another to increase the quality of separation. 
First CNN (gamma/Proton) seperates gammas from protons. 
Second CNN (Ring/no-ring) separates images with rings (Usually Proton) from images without ring (Usually Gamma).
Quality of separation is calculated using Quality factor with the help of individual signal/background efficiencies. 
