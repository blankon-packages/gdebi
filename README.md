# gdebi for BlankOn

gdebi is a simple to tool install local deb files or install the
build-dependencies of .dsc files.

It will use apt to figure if the dependencies can be satified and
what additonal software is required. 

It needs a vte and recent python-apt to work. vte needs a patch to
make it not close file descriptors, python-apt needs some new features.

It will need root to install the deb, and it has a non-root non-root
bit to view the deb and a "non-interactive" bit that is exec()ed with
gksudo.
