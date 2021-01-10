


Качаем исходный код и распаковываем архив.
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3.orig.tar.gz
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3-0ubuntu6.dsc

Переходим в папку и туда качаем распаковваем архив для ubuntu
https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/docker.io/1.10.3-0ubuntu6/docker.io_1.10.3-0ubuntu6.debian.tar.xz


применяем заплатку и оповещаем систему сборки об этом 
patch -p1 < func_ppc.patch
patch -p1 < limit_powerpc.patch
dpkg-source --commit

Запускаем сборек debuild -uc -us
