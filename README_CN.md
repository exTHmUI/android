# <img src="https://github.com/exTHmUI/android/blob/Tenshi/logo.png" width="400"> #

## [EN](https://github.com/exTHmUI/android) | CN ##

### 这是什么？ ###

``exTHmUI`` 是一个由国内东方众维护的，基于AOSP的东方化系统。

### 如何同步 ###

```bash
# 初始化空的索引仓库
$ repo init -u https://github.com/exTHmUI/android -b Tenshi

# 开始同步仓库
$ repo sync -j4
```

### 如何编译 ###

```bash
# 初始化编译环境
$ . build/envsetup.sh

# 选择编译设备
$ lunch exthm_$device-userdebug

# 开始编译!!
$ make reimu -j$(nproc --all)
