EXPLANATION OF THE FILTERING PROCESS
--
#**Loading the Audio**<br>
We first of all clone the repository and navigate to the folder containing our audio.<br>
#**Conducting an FFT Analysis**<br>
In this analysis we convert a time domain signal into a frequency domain signsl<br>
It deconstructs the wave into its sine and cosine parts. We check from the graph of fft the highest amplitude(the peak amplitude) frequency.And create a bandpass filter that only allows the frequency between these two frequencies known as carrier frequencies.<br>
#**Demodulation**<br>
I dont really understand this part in detail but this is what internet says : The Demodulation is the process of extracting the original information from a modulated carrier wave. 

We multiply the modulated signal with a cosine wave of the carrier frequency.

This shifts the signal’s frequency content back to the baseband (original message).

This method is called coherent demodulation (used in AM signals).
#**Filtering**<br>
I first paqssed it through a band pass filter to remove all the junk frequencies (my bandpass filter allowed only the frequencies- 9830 to 10560 HZ). It removed most of the noise though i doubt it could have been better cuz i can still hear some noise.
#**GRAPHS**<br>
I plotted several graphs during the process including one of filter vs unfiltered (which i guess looks pretty accurate to me since my filtered wave is a very straight line, wondering if i actually did a pretty accurate job and that maybe the audio cant be filtered further).

![fft](https://github.com/user-attachments/assets/f7186e8f-9263-432a-a338-fc533de307c8)
![demodulated wave](https://github.com/user-attachments/assets/5c72dfbd-cfe2-4ee0-a0f0-8b4444230a6f)
![filtered vs unfiltered](https://github.com/user-attachments/assets/b553cfad-8622-43e5-adf1-fb6266566231)
