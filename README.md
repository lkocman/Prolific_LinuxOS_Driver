## Updated Profilic driver for newer kernels



```
sudo zypper in kernel-source kernel-devel gcc make flex bison libdw-devel
# sudo zypper in -t pattern devel_kernel  # in case you're still missing some basic packages
cd Prolific_LinuxOS_Driver/6.19.2_ok
make all
sudo make install
sudo modprove pl2303
```

Please note that kernel-devel version absolutely have to match the running kernel version see `uname -r`.
Make sure to apply 

