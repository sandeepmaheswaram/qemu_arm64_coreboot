# qemu_arm64_coreboot

# Building coreboot

$ git clone https://review.coreboot.org/coreboot

$ cd coreboot

$ git submodule update --init --checkout

$ make menuconfig

$ make crossgcc-aarch64

$ make






# Running corebooot on QEMU

qemu-system-aarch64 -bios coreboot.rom -M virt -machine secure=on,virtualization=on -cpu cortex-a53 -nographic -m 8192M
