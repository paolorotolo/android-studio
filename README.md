Android Studio for Ubuntu
=====================

Android Studio by Google packaged for Ubuntu.
Visit the official website [here](http://paolorotolo.github.io/android-studio/).

##FAQ
###### 32-bit compatibility libraries
**Q:** *I can't build correctly my project on Ubuntu amd64. Even if using a sample project with all default settings.*

**A:** You probably need to install 32-bit compatibility libraries. Open a terminal and run:

``` sudo apt-get install libc6-i386 lib32stdc++6 lib32gcc1 lib32ncurses5 lib32z1 lib32z1-dev ```

###### Unable to launch
**Q:** *Android Studio doesn't appear in Unity's dash / GNOME Overview.*

**A:** I'm [currently working](https://github.com/PaoloRotolo/android-studio/issues/7) on this issue. Meanwhile, you can manually start Android Studio with the following command:

``` /opt/android-studio/bin/studio.sh ```

###### HiDPI support
**Q:** *Android Studio looks strange. Some icons and objects are way to small.*

**A:** To fix some of these problems add

`-Dhidpi=true`

to these files:

`/opt/android-studio/bin/studio.vmoptions`

`/opt/android-studio/bin/studio64.vmoptions`

![screenshot from 2014-11-22 17 28 23](https://cloud.githubusercontent.com/assets/5623301/5154769/fbb162a8-726c-11e4-81ce-503a2622bfba.png)
