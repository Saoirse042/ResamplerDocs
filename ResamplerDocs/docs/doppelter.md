# Doppelter

>Ameya has been building the original UTAU resampler from scratch.

Multi-thread, 64-bit compatible
g, B, N, P, t  flags are supported,
## Unique flags:

| Flag |  Description |        
|:----:|-----------------------------------------------------------------------------------------|
|   A  | High frequency emphasis rate of the noise component (default setting a100)|
|   R  | Backwards. reverse front and back|
|   S  | Number of threads By default, the number of threads corresponds to the number of logical cores on the computer.|
|   i  | length of the rear fixed area (ms)|
|   v  | consonant velocity of the rear fixed area |
	
  Others
    
    A file other than 44100Hz can also be used for the input file.
    You can also specify a consonant velocity of the rear fixed area in the form of "front/back" for the fourth argument. But it makes little sense if UTAU does not support it itself.
    You can also specify the rear fixed length in the form of "front/back" in the fixed length of the eighth argument. But it makes little sense if UTAU does not support it itself.
    If the path of lame.exe is set to the environment variable "lamepath", the MP3 file can also be read.
    If the path of flac.exe is set to the environment variable "flacpath", the FLAC file can also be read.
    If the path of oggdec.exe is defined in the environment variable "oggpath", the OGG file can also be read.
    If a file format other than ".wav" is specified in oto.ini, the current UTAU adds ".wav" to the file name and forwards it to the engine. So this engine treats ".mp3.wav", ".flac.wav" and ".ogg.wav" as ".mp3", ".flac" and ".ogg".