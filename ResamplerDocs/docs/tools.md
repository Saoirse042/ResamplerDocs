# Dependencies
>Everything on this page is optional! Most resamplers don't need any of these tools.
## Encoders
Some resamplers need additional libraries for full functionality. This isn't normally a problem as UTAU banks and resamplers use WAV files, but for the sake of file sizes, some authors release samples in different formats.

[LAME](https://lame.sourceforge.io/index.php) is an MP3 decoder. As the distribution license has changed recently, you may already have it installed.<br>
[FLAC](https://xiph.org/flac/) is a lossless audio decoder and compressor that can be used to create much smaller file sizes than WAV at equal audio quality output.<br>
[Ogg Vorbis](https://xiph.org/vorbis) is a compressed and lossy audio format which normally results in similar filesize and quality to MP3.<br>
[FFmpeg](https://ffmpeg.org/) is a package that normally includes LAME, Ogg and a number of video encoders, and may sometimes provide an easier install option.

### Prebuilt Libraries
Even if they're essential to a program working, these can't normally be bundled with installs due to conflicting types of open source license and patent restrictions.<br>
Additionally, LAME is still only distributed by the developers as source code.

=== "For Windows"
	All three libraries for additional formats Doppeltler can use are hosted at RareWares.org:
	
	- LAME: [RareWares](https://rarewares.org/mp3-lame-bundle.php), [AegisCorp builds](http://aegiscorp.free.fr/lame/)
	- FLAC: [RareWares](https://rarewares.org/lossless.php#flac-bundle), [Xiph](https://xiph.org/flac/download.html)
	- Ogg Vorbis: [oggdec.exe](https://rarewares.org/ogg-oggdec.php) from RareWares

=== "For macOS"
	- LAME: [AegisCorp builds](http://aegiscorp.free.fr/lame/)
	- FLAC: [Xiph](https://xiph.org/flac/download.html)

=== "For Linux"
	!!! info "You might already have FLAC at least..?"
		It's quite likely there'll be a package with one or all of these for your specific distribution. It's worth checking your documentation!

!!! help "Wait, these are familiar. It isn't the first time I've had to install these! Maybe I don't need it...?"
	You might have downloaded something like [FFmpeg for Audacity](https://manual.audacityteam.org/man/faq_opening_and_saving_files.html#foreign) at some point, but unless you manually set environment variables to point to the files, you're going to have to install them again. Sorry!
	
## System Envrionment Variables
[Here](https://superuser.com/a/284351) is a detailed explanation on setting system environment variables on both Windows and Unix based systems.<br>
For using Doppeltler, follow the instructions in the readme:

 * Set `lame.exe` at `lamepath`
 * Set `flac.exe` at `flacpath`
 * Set `oggdec.exe` at `oggpath`

## FFTW	
Some older resamplers based off WORLD need the [Fastest Fourier Transform in the West](http://www.fftw.org/download.html) package.




## Editors
- [Audacity](https://www.audacityteam.org/) is free, cross platform and open source. It's fast and it works.

- [Reaper](https://www.reaper.fm/) is WinRAR free, cross platform and has a learning curve, but is extremely powerful and has more functionality than Audacity.


