# RightMesh Checkstyle Config

From their website:

>"Checkstyle is a development tool to help programmers write Java code that adheres to a coding standard. It automates the process of checking Java code to spare humans of this boring (but important) task. This makes it ideal for projects that want to enforce a coding standard."

This Checkfile config builds off of Checkstyle's [official implementation of the Google coding standard](http://checkstyle.sourceforge.net/google_style.html), adding in features from [this GitHub project](https://github.com/hypest/checkstyle-android) that adhere to [the official Android coding standards](https://source.android.com/source/code-style.html).

## Using This File

These standards are downloaded and referenced automatically in the Gradle tasks for `Left/RightMesh`.

To use these standards right in Android Studio, install the Checkstyle-IDEA plugin. Once installed, go to `File => Settings...`, then to `Other Settings => Checkstyle` in the menu on the left, and click on the green plus sign in the "Configuration File" box. In the new window that pops up, check the `Use a Checkstyle file accessible by HTTP` radio box and provide the URL `https://raw.githubusercontent.com/RightMesh/Checkstyle-Config/master/config/checkstyle.xml`. Fill in the Description and press "Next". You will now be able to select the RightMesh Checkstyle configuration from the "Rules:" dropdown in the Checkstyle plugin tab at the bottom of the screen.

## Updating This File

This repo is actually a branch of the [Checkstyle GitHub repo](https://github.com/checkstyle/checkstyle/) where the Google style config is maintained. One _should_ be able to just rebase this repository from time to time to get their latest additions to the Google style guide. The Android repo has been dormant since 2015, so it is unlikely to change. 

This configuration used Google and the Android project as a starting point, but is entirely our own - feel free to open a merge request to make changes as needed.
