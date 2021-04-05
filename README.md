export HOME=/work
dnf install -y rpm-build dnf-plugins-core

dnf builddep mingw-gcc.spec

rpmbuild --ba mingw-gcc.spec

