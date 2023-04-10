# Doppelter
```
-Some of this is translated with DeepL, and needs to be edited for clarity
```
>Ameya has been building the original UTAU resampler from scratch. <br>
>Doppelter is multi-threaded, 64-bit compatible, and can even handle file formats other than `.wav`.



=== "Standard flags"
	| Flag | Name             | Range      | Default | Description                                                                    |
	|:----:|------------------|------------|:-------:|--------------------------------------------------------------------------------|
	| g    | Gender           |`[-100-100]`| 0       | Positive values will deepen the voice, while negative ones will make it higher.|
	| B    |                  |`[0-100]`   | 50      | Applies breathiness before synthesis, and is affected by other flags.          |
	| N    | Formant on/off   |            |         | Toggles the formant filter on or off.                                          |
	| P    | Peak compressor  |`[0-100]`   | 86      | Compresses the voice to make the volume more consistent.                       |
	| t    | Pitch            |            | 0       | Shifts the pitch by a number of cents. 1 cent = 1/100th of a semitone.         |


=== "Unique flags"
	| Flag |  Description |        
	|:----:|-----------------------------------------------------------------------------------------|
	|   A  | High frequency emphasis rate of the noise component (default setting a100)|
	|   R  | Backwards. reverse front and back|
	|   S  | Number of threads By default, the number of threads corresponds to the number of logical cores on the computer.|
	|   i  | length of the rear fixed area (ms)|
	|   v  | consonant velocity of the rear fixed area |
	
### Other Notes
    
* Input files are no longer required to be sampled at 44100Hz
* You can also specify a consonant velocity of the rear fixed area in the form of "front/back" for the fourth argument. UTAU itself does not currently support this.
* You can also specify the rear fixed length in the form of "front/back" in the fixed length of the eighth argument. UTAU itself does not currently support this.

Previously, if a file format other than `.wav` is found in `oto.ini`, UTAU will append `.wav` to the file name like this:
:	`aaa.mp3` → `aaa.mp3.wav`<br>

Now, with environment variables set, Doppelter is able to read files in their original format.

!!! info "I'd like to use Doppelter with other file formats!"
	You need LAME, FLAC and Ogg decoders for this. See [tools](/ResamplerDocs/tools/#encoders) for information on setup.
 
