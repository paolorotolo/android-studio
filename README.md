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

`/opt/intellij-idea-community/bin/idea.vmoptions`

`/opt/intellij-idea-community/bin/idea64.vmoptions`

![screenshot from 2014-11-22 17 28 23](https://cloud.githubusercontent.com/assets/5623301/5154769/fbb162a8-726c-11e4-81ce-503a2622bfba.png)

## Changelog
* v. 4.8.3
  *  New upstream release (1.2 Stable);

* v. 4.8.2
  *  Fixed broken dependencies on i386;

* v. 4.8.1
  *  New upstream release (1.2 Beta 3);

*  v. 4.8
  *  New upstream release (1.1);

*  v. 4.7
  *  New upstream release (1.1 Beta 3);
  *  Adds unzip to Depends;
  *  New Material Icon;

*  v. 4.6
  *  New upstream release (1.1 Preview 1);
  *  Fixes bug with dependencies on 32bit;

*  v. 4.4
  *  New upstream release (1.0.1);

*  v. 4.3
  *  New upstream release (1.0 RC 2);

*  v. 4.2
  *  New upstream release (1.0 RC 1);

*  v. 4.1
  *  New upstream release (0.9.1);

*  v. 4.0
  *  New upstream release (0.9.0);

*  v. 3.0
  *  New upstream release (0.8.13);
  *  Fixed permission issue with built-in update tool.

*  v. 2.0
  *  New install location (from '/usr/share/android-studio' to '/opt/android-studio');
  *  New upstream release (0.8.12);
  *  Android Studio isn't included in packaging anymore. It will be automatically downloaded through the installation process.

*  v. 1.0
  *  First release.

Upsteam changelog [here](http://tools.android.com/recent).
