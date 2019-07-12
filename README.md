# Kernels and modules:

- linux-aufs

- linux-lqx

- linux-next-git

- linux-uksm

###### linux-aufs incorporates:

* [AUFS](https://github.com/sfjro/aufs5-standalone) / [AUFS](http://aufs.sourceforge.net) - advanced multi-layered unification filesystem

###### linux-lqx incorporates:

* [liquorix patchset](https://github.com/damentz/liquorix-package) - authored by Steven Barrett

###### linux-uksm incorporates:

* [UKSM (sources)](https://github.com/dolohow/uksm) / [UKSM (sources)](https://github.com/zaza42/uksm) / [UKSM (patches)](https://github.com/sirlucjan/kernel-patches) / [UKSM (patches)](https://gitlab.com/sirlucjan/kernel-patches) / [UKSM (info)](https://www.usenix.org/sites/default/files/conference/protected-files/fast18_slides_xia.pdf) - resync from dolohow’s / zaza42's github or patches from sirlucjan's github/gitlab (resync from pfkernel)

***
# Download:

```
git clone https://github.com/sirlucjan/aur.git

```

or

```
git clone https://gitlab.com/sirlucjan/aur.git

```
# Install:


```
cd /some_path/aur/package_name
makepkg -srci

```
