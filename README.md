# OFDM using Python
In this project, I have explained OFDM and implemented it in Python

## OFDM 
Orthogonal Frequency Division Multiplexing(OFDM) is a multi-carrier modulation technique. It is the key technology used in the 4G/5G wireless communication system. OFDM divides a broadband channel into multiple parallel narrowband subchannels, where each subchannel carries a low data rate stream, which sums up to a high data rate transmission. In an OFDM transceiver, a set of QAM encoders initially maps the bits into complex symbols. 

These symbols are then fed into an inverse fast Fourier transform (IFFT) to maintain the orthogonality of the subchannels. The resulting output is then converted from parallel to serial and modulated onto a carrier for transmission over the wireless channel.

## Steps involved in OFDM transmission and reception
### At Transmitter
1) Generate random bits
2) Use serial to parallel converter to map the bits into complex symbols
3) Take IFFT
4) Convert parallel data stream to serial data
5) Add cyclic prefix and transmit it through the air
### Wireless Channel
The channel is noisy, so the received signal at the receiver is a convolution of the transmitted signal and channel impulse response added with noise.

### At Receiver
1) Remove the cyclic prefix
2) Pass the signal to serial to parallel converter
3) Take FFT to transfrom the signal into the frequency domain
4) Estimate the channel using pilot symbols
5) Equalize the channel and remap the complex symbols back to bits
6) Use parallel to serial converter to get the transmitted bits

## Conclusion
I implemented simple OFDM transmission and reception, and after receiver processing obtained the data bits and calculated the BER for a given SNR. 
Vary the SNR to see the BER.
