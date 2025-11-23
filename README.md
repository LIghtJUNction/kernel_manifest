# ace2

# 安装repo
- pacman -S repo

- mkdir KERNEL_WORKSPACE

- cd KERNEL_WORKSPACE

- repo init -u https://github.com/LIghtJUNction/kernel_manifest

- repo sync -c -j8

# how to build
./kernel_platform/oplus/build/oplus_build_kernel.sh waipio gki  
./kernel_platform/oplus/build/oplus_rebuild_img.sh waipio gki
