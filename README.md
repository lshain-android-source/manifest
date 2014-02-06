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


