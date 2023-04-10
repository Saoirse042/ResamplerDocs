# Resampler Flags

> resampler.exe is the default resampler made by Ameya that comes with UTAU.

```
- Taken directly from https://utau-bowl.tumblr.com/post/647016314853097472/utau-flag-guide .
- Need to check how accurate this is (range values for t?) and word better (explain filters).
- Also find whatever names people use most for each flag to explain what they are.
```

| Flag | Name             | Range      | Default | Description                                                                                                                                                                                   |
|:----:|------------------|------------|:-------:|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| a    |                  |            | 100     | Stretches or compresses the consonant part of a sample.                                                                                                                    |
| b    |                  |`[0-100]`   | 0       | Applies breathiness after synthesis. Is not affected by other flags (such as F)                                                                                                              |
| B    |                  |`[0-100]`   | 50      | Applies breathiness before synthesis, and is affected by other flags.                                                                                                                         |
| c    |                  |`[0-100]`   | 50      | Sets value of C flag before formant filter adaptation.                                                                                                                                     |
| C    |                  |`[0-100]`   | 0       | High pass filter                                                                                                                                                                              |
| D    |                  |`[0-100]`   | 0       | Mid pass filter                                                                                                                                                                               |
| E    |                  |`[0-100]`   | 0       | Low pass filter                                                                                                                                                                               |
| F    | Formant strength |            | 3       | I think it can go up to 5 or so, beyond that it all starts to give similar results                                                                                                            |
| g    | Gender           |`[-100-100]`| 0       | Positive values will deepen the voice, while negative ones will make it higher.                                                                                                               |
| G    |                  |            |         | Forces resampler to render .frq files before playing. This makes the synthesis process slower, but gives you new frqs.                                                                        |
| H    |                  |`[0-99]`    | 0       | Emphasizes low tones, and cuts higher ones.                                                                                                                                                   |
| h    |                  |`[0-99]`    | 0       | Emphasizes higher tones, and cuts low ones.                                                                                                                                                   |
| L    |                  |            |         | Sets a fixed frequency for F flag. Has no default value. Probably has the same limits as F flag.                                                                                              |
| N    | Formant on/off   |            |         | Turns the formant filter off.                                                                                                                                                                 |
| P    | Peak compressor  |`[0-100]`   | 86      | Compresses the voice to make the volume more consistent.                                                                                                                                      |
| t    | Pitch            |            | 0       | Shifts the pitch by a number of cents. 1 cent = 1/100th of a semitone.                                                                                                                                           |
| W    |                  |            |         | Produces a sharper and more metallic sounding voice. Flag is used by itself without a number added.                                                                                           |
| x    |                  |`[-100-100]`| 0       | Affects a note depending on how the sample it takes from was recorded. Higher notes make the voice brighter, while low notes make the voice more muffled. Negative values affect the formant. |
| Y    |                  |`[0-100]`   | 100     | Controls the breathiness for the “vowel” part of a note.                                                                                                                                      |

