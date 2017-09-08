#Spiess - speech analysis for highlighting emotional characteristics based on MFC coefficients
##  Based on: A Simple MFCC Feature Extractor using C++ STL and C++11 (D S Pavan Kumar)
## Main idea
* Useful application which uses spectrum and cepstrum analysis for getting statisics of human's behaviour.
## Features (D S Pavan Kumar)
* Takes PCM Wave input and outputs MFCCs as comma separated floating point values, each line representing a frame.
* Supports batch extraction through list input and output.
* Command line control for window length, frame shift, sampling rate, number of cepstra and filterbank cutoff frequencies.
* Computes MFCCs through pre-emphasis, Hamming window, FFT, power spectrum, equal height log-Mel filterbank followed by discrete cosine transform.

## Compilation
g++ -std=c++11 -O3 compute-mfcc.cc -o compute-mfcc

## Usage Examples
* compute-mfcc --input input.wav --output output.mfc
* compute-mfcc --input input.wav --output output.mfc --samplingrate 8000
* compute-mfcc --inputlist input.list --outputlist output.list
* compute-mfcc --inputlist input.list --outputlist output.list --numcepstra 17 --samplingrate 44100

## License
GNU GPL V3.0

## Contributors
D S Pavan Kumar
