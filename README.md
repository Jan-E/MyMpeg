MyMpeg
======

This helper script lets you cross compile a windows 32 or 64 bit version of ffmpeg including many dependency libraries they use.

It also lets you build FFmpeg with your own patches. volnorm.patch is a good example

To run the script, in a Linux box (VM or native):

download the script (git clone the repo, run it, or do the following in a bash window) $

```bash
wget https://raw.github.com/Jan-E/MyMpeg/master/cross_compile_ffmpeg.sh -O cross_compile_ffmpeg.sh
chmod u+x cross_compile_ffmpeg.sh
./cross_compile_ffmpeg.sh
```

And follow the prompts.  
It should end up with a working static ffmpeg.exe within the sandbox directory.

It works with 32 or 64 bit (host) Linux, and can produce either/or 32 and 64 bit windows ffmpeg.exe's, with lots of dependencies built in. To build more than just FFmpeg, use command line parameters to the script.

Many thanks go to Kyle Schwarz and Roger Pack:
http://ffmpeg.zeranoe.com/blog/
https://github.com/rdp/ffmpeg-windows-build-helpers
