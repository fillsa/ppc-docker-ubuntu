


������ �������� ��� � ������������� �����.
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3.orig.tar.gz
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3-0ubuntu6.dsc

��������� � ����� � ���� ������ ������������ ����� ��� ubuntu
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3-0ubuntu6.debian.tar.xz


��������� �������� � ��������� ������� ������ �� ���� 
patch -p1 < func_ppc.patch
patch -p1 < limit_powerpc.patch
dpkg-source --commit

��������� ������ debuild -uc -us
