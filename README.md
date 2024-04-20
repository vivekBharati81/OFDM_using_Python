# OFDM using Python
In this project, I have explained OFDM and implemented it in Python

## OFDM 
Orthogonal Frequency Division Multiplexing(OFDM) is a multi-carrier modulation technique. It is the key technology used in the 4G/5G wireless communication system. OFDM divides a broadband channel into multiple parallel narrowband subchannels, where each subchannel carries a low data rate stream, which sums up to a high data rate transmission. In an OFDM transceiver, a set of QAM encoders initially maps the bits into complex symbols. 

These symbols are then fed into an inverse fast Fourier transform (IFFT) to maintain the orthogonality of the subchannels. The resulting output is then converted from parallel to serial and modulated onto a carrier for transmission over the wireless channel.
