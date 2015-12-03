---
layout: post
title: "Porting KDE Games: Progress Report"
---

Hello everyone,

As I mentioned in my last blog post, I'm working on porting KDE Games to KF5/Qt5. After porting the libkdegames project, I ported three games - KMines, KNavalBattle and KBounce to test how these build against the new libs. Everything works as expected as of now. Here are the screenshots of the three games:

![KMines](/public/images/kmines.png)
![KNavalBattle](/public/images/navalbattle.png)
![KBounce](/public/images/kbounce.png)

You can build the ported games and libraries from _clones/{project name}/anujpahuja_ hosted on [quickgit](http://quickgit.kde.org) and give your reviews.

I'd also like to add something about how KStandardDirs -> QStandardPaths port works. While porting, I found out that `QStandardPaths::StandardLocation` searches for files in specific locations on Linux. For example, `QStandardPaths::GenericDataLocation` will only look for files/directories in these locations - `~/.local/share`, `/usr/local/share`, `/usr/share`. So be careful when installing files to a custom directory. I explicitly added a `DATA_INSTALL_DIR` variable in the build system to ensure files are being installed in the locations as specified by `QStandardPaths::StandardLocation`. Better fixes to this are most welcomed.

There's still a couple of small things that need to be done to make the games fully ready. Will keep you updated.

Cheers!
