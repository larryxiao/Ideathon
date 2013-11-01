*  [How to generate video screencaps of video files via linux commandline - Stack Overflow](http://stackoverflow.com/questions/1150812/how-to-generate-video-screencaps-of-video-files-via-linux-commandline)
 * [Creating video thumbnails using ffmpeg – Prashanth Ellina](http://blog.prashanthellina.com/2008/03/29/creating-video-thumbnails-using-ffmpeg/)
 * [SlickSlice](http://slickslice.sourceforge.net/)
 * <pre>
./slickslice.sh -x video.avi -s 5x3 -e
</pre>
 * <pre>
mplayer -nosound -sstep 15 -vo png video.mkv
montage *.png -tile 3x3 -geometry 300x+0+0 screencaps.png
</pre>
 * <pre>ffmpeg -itsoffset -4 -i test.avi -vcodec mjpeg -vframes 1 -an -f rawvideo -s 320x240 test.jpg</pre>

* [Cinder | The library for professional-quality creative coding in C++](http://libcinder.org/)
* [Bloom: new ways to see and communicate](http://bloom.io/#mission)
  * [Planetary: A Visual Music Player for iPad by Bloom Studio, Inc.](http://planetary.bloom.io/)
  * [Biologic: A Playful Social Network Browser for iPad by Bloom Studio, Inc.](http://biologic.bloom.io/)  

* Audio Related
  * [btr . Cinder KissFFT . Stephen Schieberl's blog about making things and doing stuff](http://www.bantherewind.com/cinder-kissfft)
