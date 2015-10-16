Building and installing a Debian package of metrics-lib
=======================================================

```
sudo apt-get install build-essential devscripts debhelper javahelper openjdk-6-jdk ant libcommons-compress-java
git clone https://git.torproject.org/metrics-lib.git descriptor-1.0
tar czf descriptor_1.0.orig.tar.gz descriptor-1.0
cd descriptor-1.0
mkdir classes
git clone https://github.com/kloesing/metrics-lib-debian.git debian
debuild -us -uc
sudo dpkg -i ../descriptor_1.0-1_amd64.deb
```

