# Brackets-en-Debian
con dependencias de libcurl3

    Download the .deb installer file
    In the folder you downloaded the file run:
    dpkg-deb -R ./Brackets.Release.1.12.64-bit.deb Brackets
    Edit file Brackets/DEBIAN/control and replace libcurl3 with libcurl3 | libcurl4
    Rebuild .deb installer running dpkg-deb -b Brackets Brackets-fixed.deb
    Install Brackets using the fixed installer running sudo dpkg -i Brackets-fixed.deb
