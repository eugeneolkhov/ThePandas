# ThePandas
Repo for School of AI Hackathon 2019

The Pandas
Team Members: Andrew Armstrong, Irina Nedelcu, Eugene Olkhov
 
Respiratory Rate Predictive Model
PPG (Photoplethysmographic) Signal is used to predict Respiratory Rate of patients in intensive care.
 
Summary
All intensive-care patients need to have respiratory rate measured every few hours in order to detect if any deteriorations in health are occurring. Most of the times, the respiratory rate is manually measured, though it can be prone to inaccurate results. Another way to measure it is to use a respiratory signal device. Still, both options are costly, require resources (which are limited) and can be difficult to use in low tech environments.
To overcome these, we have tested how well ECG and PPG can predict respiratory rate. Both ECG and PPG variables were transformed using Continuous Wavelet Transformation for localization of time-frequency, which is otherwise lost in the frequency domain. When comparing the transformed variables, it was determined that PPG is better at identifying the trend of the respiratory rate signal. The newly transformed PPG variable was then used as an input to an LSTM model, which identifies patterns in sequential data. As a result, peaks in predicted respiratory rate coincide with actual recorded respiratory rate fairly well on both train and testing data.

Data
Data csv files are located on Dropbox, on this location: https://www.dropbox.com/s/5j0r1c8phl4891e/bidmc_csv_zip.zip?dl=0&fbclid=IwAR3kmfbef-NHAcG1c64l6pE5sL3uTE_pdIjPgz3k5-LZkOCBe1vD3MOvW8E

