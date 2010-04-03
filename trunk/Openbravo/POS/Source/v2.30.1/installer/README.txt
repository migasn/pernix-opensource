ABOUT THE installer.xml and installer-unix.xml files

Is important to note that the installer-unix.xml needs to be a
copy of the installer.xml file, the only difference needs to be
in the Advance options for the "Final Page Actions" where due
to a difference in how platforms execute files we need to change
the value for the run program action parameter "Program" from
"${installdir}/configure.bat" to "${installdir}/configure.sh" this
way the action will execute the proper file in a unix enviroment.

The other change needs to go in the "Packing" option where the
"Build Platform" parameter needs to be changed from Windows to a
Unix like of Operative System