manifest
========

manifest

添加project 添加到default.xml

然后:

mkdir source
cd source

repo init -u git@github.com:lshain-android-source/manifest.git

repo sync
repo start --all master
cd script
source git_remote_set_url.sh

#提取 flo 驱动
cd ..
./extract-asus-flo.sh
./extract-broadcom-flo.sh
./extract-qcom-flo.sh

source build/envsetup.sh
lunch aosp_flo-eng
make -j32
