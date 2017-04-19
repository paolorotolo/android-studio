[DEPRECATED] Android Studio for Ubuntu
=====================
**NOTICE: THIS PROJECT IS NO LONGER SUPPORTED.**<br>
Please consider using [ubuntu-make](https://github.com/ubuntu/ubuntu-make) or [mfonville's repo](https://mfonville.github.io/android-studio/) instead.

## Install Android Studio VIA ubuntu-make
```bash
  # Install Ubuntu Make
  sudo apt install ubuntu-make
  
  # Install Android Studio
  umake android
```


Android Studio by Google packaged for Ubuntu.
Visit the official website [here](http://paolorotolo.github.io/android-studio/).

## FAQ
##### 32-bit compatibility libraries
**Q:** *I can't correctly build my project on Ubuntu amd64. Even if using a sample project with all default settings.*

**A:** You probably need to install 32-bit compatibility libraries. Open a terminal and run:

``` sudo apt-get install libc6-i386 lib32stdc++6 lib32gcc1 lib32ncurses5 lib32z1 lib32z1-dev ```

##### Unable to start
**Q:** *When I click on the icon, Android Studio just doesn't start.*
**A:** Did you install Java? Try to install Java 8 from [this PPA](http://www.webupd8.org/2012/09/install-oracle-java-8-in-ubuntu-via-ppa.html).

Also, try:

``` sudo /opt/android-studio/bin/studio.sh ```

If you have this error, you probably have to install the **jdk**:

```
Start Failed: Internal error. Please report to https://code.google.com/p/android/issues

java.lang.NoClassDefFoundError: com.intellij.util.lang.ClassPath
at java.lang.Class.initializeClass(libgcj.so.14)
[...]
```

##### Invisible icon
**Q:** *Android Studio doesn't appear in Unity's dash / GNOME Overview.*

**A:** I'm [currently working](https://github.com/PaoloRotolo/android-studio/issues/7) on this issue. Meanwhile, you can manually start Android Studio with the following command:

``` sudo /opt/android-studio/bin/studio.sh ```

##### HiDPI support
**Q:** *Android Studio looks strange. Some icons and objects are way too small.*

**A:** To fix some of these problems add

`-Dhidpi=true`

to these files:

`/opt/android-studio/bin/studio.vmoptions`

`/opt/android-studio/bin/studio64.vmoptions`

![screenshot from 2014-11-22 17 28 23](https://cloud.githubusercontent.com/assets/5623301/5154769/fbb162a8-726c-11e4-81ce-503a2622bfba.png)
