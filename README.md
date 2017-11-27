# Tadarida-D
COPY OF TADARIDA FOR TESTING: A Toolbox for Animal Detection on Acoustic Recordings Integrating Discriminant Analysis - Detection and Feature extraction part

How to build on CentOS 6
========================
Original code downloaded from https://github.com/YvesBas/Tadarida-D

Assumptions
-----------
It is assumed that you have a working QT project file (in this case Tadarida-D.pro) from which qmake can generate the Makefile, note that this project file is not included in the code from the above URL, instead it was generated from running "qmake -project" and then tweaked to include the other required libraries.

Prerequisites
-------------
Run the following as root on the CentOS server you're compiling this on
<pre><code>yum -y install fftw3-devel libsndfile-devel qt5-qtbase-devel.x86_64
yum -y groupinstall 'Development Tools'
</code></pre>

Compile
-------
<pre><code>qmake-qt5 -r
make</code></pre>

Use
---
The compiled program file is called "tadaridaD", to process a directory full of "wav" files called "waves" run the program with
<pre><code>tadaridaD waves</code></pre>

General
-------
See the test script for usage examples.
