# Dexter script

Dexter is a script that can help in reducing the method count of a Unity android project.
The script parses the Unity project and looks for android libraries that can be refactored to reduce the overall method count via the process mentioned here : https://developers.helpshift.com/unity/troubleshooting-android/#dex-issues

NOTE : 
This script refactors the folder strtucture as well as the AndroidManifest.xml files of the android libraries in your project. The app needs to be thoroughly tested after executing the script.


The script accepts the following arguments : 
'-v', '--verbose'         Enables logging
'-p', '--project-dir'     Path to the project directory. Default is the present working directory.
'-b', '--backup-suffix'   Suffix to add to dir where backup is taken. Default is '.bkp'
'-a', '--android-target'  Android target version to be added in the project.properties file of refactored android                                 libraries.



Setup :
This is a Python script and needs the folloewing modules to be installed:
1. yaml
2. json
3. requests
4. shutil
5. xml.dom.minidom
6. urllib2
7. logging
8. argparse
9. zipfile
10. contextlib

If any of the above is not installed on your system you can install with the following command :

pip install <module-name>
 
