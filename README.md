# ace2

# 安装repo
- pacman -S repo

- mkdir KERNEL_WORKSPACE

- cd KERNEL_WORKSPACE

# 同步官方原版内核

- repo init -u https://github.com/LIghtJUNction/kernel_manifest

- repo sync -c -j8

# 同步我的susfs+ksu+bbg的修改版本（可直接构建最新susfsV2+ksu官方版本）
- repo init -u https://github.com/LIghtJUNction/kernel_manifest -m ksu_susfs_bbg.xml

# how to build
./kernel_platform/oplus/build/oplus_build_kernel.sh waipio gki  
./kernel_platform/oplus/build/oplus_rebuild_img.sh waipio gki
