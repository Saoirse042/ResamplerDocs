# tn_fnds.exe
> tn_fnds.exe is made by Zteer and based off the EFB-GW and world4utau. Morise and Ameya/Ayame are both thanked in the readme.


=== "Standard flags"
	| Flag | Name             | Range       | Default | Description                                                                    |
	|:----:|------------------|-------------|:-------:|--------------------------------------------------------------------------------|
	| g    | Gender           |`[-100, 100]`| 0       | Positive values will deepen the voice, while negative ones will make it higher.|
	| t    | Pitch            |             | 0       | Shifts the pitch by a number of cents. 1 cent = 1/100th of a semitone.         |
	| b    | Breath           |             |         | This flag is different from the original, and emphasises consonants (voiceless part). b10 increases the emphasis by 5%, and b100 by 500%. |
	| B    | BRE              |`[50, 100]`  | 50      | The breath component increases when the value is set to 50 or more; it does not change when the value is set to less than 50. |
	| W    | Death Growl      |`[-1]`<br>`[50, 1000]`|| Works differently from the original W flag. Overwrites the result of F0 analysis with the specified frequency. If -1 is specified, the sound is treated as a silent. Adjust the value of 'freq avg' in the original sound profile as a basis. |
	
	
=== "Unique flags"
	| Flag | Name           | Range       | Default | Description                                                                    |
	|:----:|----------------|-------------|:-------:|--------------------------------------------------------------------------------|
	| A    | Amplitude      |`[0, 100]`   | 0       | Changes the volume in accordance with pitch fluctuations. Recommended for careful use on vibrato parts. |
	| O    |                |`[-100, 100]`| 0       | Changes the strength (brightness) of the voice. Positive values suppress low frequencies and amplify the high frequencies. Does not affect unvoiced parts. |
	| e    | Stretch method |             |         | Toggles the combined stretch+loop or stretch method.<br>By default, tn_fnds stretches AND loops the stretched section of a note. If this flag is invoked, the interval is instead stretched as-is with no looping - the behaviour of is most resamplers.<br>Normally the default tn_fnds behaviour sounds more natural, but if the loop cuts strangely using this flag may be easier than re-configuring a voice bank.|

	*[the stretched section of a note]: The white section defined in the oto.ini labelling.
	