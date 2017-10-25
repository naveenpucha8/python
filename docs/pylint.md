To Install Pylint
Windows, Mac OS X & Debian:
```bash
   pip install pylint
```
Fedora:
```bash
   sudo yum install pylint
```
Ubuntu:
```bash
   sudo apt-get install pylint
```
To Run Pylint
Change the directory to where the file is located on command prompt

Get Full Report

Run the command pylint with the file name as shown below:
```bash
   pylint fileName.py
```

Get Errors & Warnings

To return all the errors within the file, run pylint -rn and the file name
```bash
   pylint -rn fileName.py
```

To Get Errors

To return all the errors within the file, run pylint -E (capital E) and the file name
```bash
   pylint -E fileName.py
```

To Disable Warning

To generate errors and warning with a disabled violation, use `-d` along with disable code or comment as shown below:
```bash
   pylint -rn -d unused-variable fileName.py
```
# or
```bash
   pylint -rn -d W06012 fileName.py
```
To Use Configuration File

The configuration file that is being used on jenkins pylint can be found in the following directory inside the mantid folder :

  mantid\tools\Pylint\pylint.cfg
To generate the exact same errors and warning as displayed on jenkins pylint, run the following command:

  pylint --rcfile ..mantid\tools\Pylint\pylint.cfg fileName.py
  # note: provide the full path of the configuration file
To Run GUI

Run the following command to get Pylint GUI

  pylint-gui
