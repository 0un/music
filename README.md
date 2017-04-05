# music
Computer music programs, mostly involving the PDP-8

wav_creator directory contains time2wav, a program which generates music from a PDP-8. It requires a simple patch to SimH to generate the total elapsed cycle count every time a CAF instruction is executed. The program takes the values (treated as elapsed time) and generates a WAV file with pulses at each value. The WAV file is low-passed as it would be if an AM radio were playing the music. This is very much a beta program and will likely crash given certain input files. The only dependency is libsamplerate used to sample down the series of pulses.
