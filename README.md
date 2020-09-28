# rooster_challenge
Given a wav file that contains crows for different roosters, we wanna find the longest rooster crow and rank all the rooster per crow time. 

# Approach
1- Signal is resampled and denoised using https://audiodenoise.com/ (for some reason it provided me with the best denoising approach)   
2- Signal autocorrelation is calculated.   
3- A median filter is applied to the calculated autocorrelation signal to smooth out the spikes.   
4- Voice activity detection is applied to detect voice segments.   
5- Sorting the roosters according to their crow times.   

