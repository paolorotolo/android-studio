Android Studio for Ubuntu
=====================

Android Studio by Google packaged for Ubuntu.
Visit the official website [here](http://paolorotolo.github.io/android-studio/).

##FAQ
###### 32-bit compatibility libraries
**Q:** *I can't build correctly my project on Ubuntu amd64. Even if using a sample project with all default settings.*

**A:** You probably need to install 32-bit compatibility libraries. Open a terminal and run:

``` sudo apt-get install libc6-i386 lib32stdc++6 lib32gcc1 lib32ncurses5 lib32z1 lib32z1-dev ```

![screenshot from 2014-11-22 17 28 23](https://cloud.githubusercontent.com/assets/5623301/5154769/fbb162a8-726c-11e4-81ce-503a2622bfba.png)

## Changelog
 * Android Studio **main** changelog [here](http://tools.android.com/recent);
 * **Packaging** changelog [here](http://paolorotolo.github.io/android-studio/changelog.html);
