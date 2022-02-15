# Doppelter

>Ameya has been building the original UTAU resampler from scratch.

>Doppleter is multi-thread and 64-bit compatible, and even utilises system PATH variables for audio decoders such as Ogg Vorbis or MP3.


=== "Standard flags"
	g, B, N, P, t  flags are supported,


=== "Unique flags"
	| Flag |  Description |        
	|:----:|-----------------------------------------------------------------------------------------|
	|   A  | High frequency emphasis rate of the noise component (default setting a100)|
	|   R  | Backwards. reverse front and back|
	|   S  | Number of threads By default, the number of threads corresponds to the number of logical cores on the computer.|
	|   i  | length of the rear fixed area (ms)|
	|   v  | consonant velocity of the rear fixed area |

	
### Others
    
* Input files are not required to be sampled at 44100Hz
* You can also specify a consonant velocity of the rear fixed area in the form of "front/back" for the fourth argument. But it makes little sense if UTAU does not support it itself.
* You can also specify the rear fixed length in the form of "front/back" in the fixed length of the eighth argument. But it makes little sense if UTAU does not support it itself.
 
### System PATH variables

* If the path of lame.exe is defined in the environment variable "lamepath", MP3 files can be read.
* If the path of flac.exe is defined in the the environment variable "flacpath", FLAC files can be read.
* If the path of oggdec.exe is defined in the environment variable "oggpath", OGG files can be read.

Previously, if a file format other than ".wav" has been specified in oto.ini, UTAU will append ".wav" to the file name (so aaa.mp3 becomes aaa.mp3.wav) and forward it to the engine.

* Instead, Doppeltter treats ".mp3.wav", ".flac.wav" and ".ogg.wav" as ".mp3", ".flac" and ".ogg".