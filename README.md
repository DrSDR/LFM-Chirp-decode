decode text message
message has 216 bits  , 8 bit char
27 char total

fs = 48khz

bits are defined by chirps

chirp details:
pw = 200msec
bw = 12khz
slope = bw/pw

dt = 1/fs

t = [dt:dt:pw]

t = t - pw/2


bit1 = exp(1i * pi *slope *t.^2)


bit0 = exp(-1i *pi *slope *t.^2)



need to find start of signal

the first 8 bits are:  01100011


the signal is in noise, matched filter will be needed

first part of the text message is:
code is:



