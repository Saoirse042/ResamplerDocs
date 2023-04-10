# Audio Tools
## Encoders
Some resamplers need audio libraries such as [LAME](https://lame.sourceforge.io/index.php) or [FLAC](https://xiph.org/flac/).

!!! help "But this is annoying! If these encoders are so important, why aren't they just bundled with software?"

    The short answer is conflicting types of open license and patent restrictions. Sorry! All anyone can do is link them and explain the installation.

A number of different LAME builds are avaliable, but mine (for Windows or OSX) are from [here](http://aegiscorp.free.fr/lame/). <br>
The FLAC binaries I'm using are from [Xiph](https://xiph.org/flac/download.html).

The Windows [FFmpeg](https://ffmpeg.org/) essentials package from [gyan.dev](https://www.gyan.dev/ffmpeg/builds/#release-builds) includes both `libmp3lame` and `libvorbis` so can make installation easier.
It also has `avisynth+` for video editing, so it's genuinely worth installing and setting these up for future use.

!!! info "But what about Linux?"

    It's quite likely there'll be a package for your specific distribution. You should check that documentation instead of this one :P

## FFTW	
Some older resamplers based off WORLD need the [Fastest Fourier Transform in the West](http://www.fftw.org/download.html) package.



## System Envrionment Variables
[Here](https://superuser.com/questions/284342/what-are-path-and-other-environment-variables-and-how-can-i-set-or-use-them) is a detailed explanation on setting system environment variables on Windows.

 * Set `lame.exe` at `lamepath`
 * Set `flac.exe` at `flacpath`
 * Set `oggdec.exe` at `oggpath`

## Editors
- [Audacity](https://www.audacityteam.org/) is free, cross platform and open source. It's fast and it works.

- [Reaper](https://www.reaper.fm/) is WinRAR free, cross platform and has a learning curve, but is extremely powerful and has more functionality than Audacity.


