# EFOtech_MLV
EFOtech Multilevel Headphone Virtualization

Basic creation formula:
1. Recorded original in-room BRIRs BRIR-raw.wav (channels: 1. Left speaker to left ear, 2. Left speaker to right ear, 3. Right speaker to left ear, 4. Right speaker to right ear)
2. Cropped all channels to various impulse lengths as stated in version number of final impulse (e.g. MLV-02048 cropped to 2048 samples here)
3. Calculated 1/24th octave smoothed frequency responses for channel 1+3 and channel 2+4, calculated minimum phase correction filters to equalize these "two" channels to same frequency response with 1/24th oct tolerance, applied to channels (i.e. one correction for channels 1 and 3 and another for channels 2 and 4)

Result: balanced and centred output for virtually all listeners with stereo-centred input sound sources

4. Convolved eclectic stereo music test track calibrator.flac with balanced output from (3), compared result with original, calculated 1/24th octave smoothed min-phase "restore FR to original" filter and applied to impulse

Result: FR-neutral headphone virtualizer applying minimal colouration to original headphone sound signature while providing varying levels of virtualization depending on length chosen in (2)
