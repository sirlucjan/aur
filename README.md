# Kernels and modules:

- linux-aufs

- linux-bfq-dev

[![Packaging status](https://repology.org/badge/vertical-allrepos/linux-bfq-dev.svg)](https://repology.org/project/linux-bfq-dev/versions)

- linux-lqx

[![Packaging status](https://repology.org/badge/vertical-allrepos/linux-lqx.svg)](https://repology.org/project/linux-lqx/versions)

- linux-next-git

- linux-uksm

[![Packaging status](https://repology.org/badge/vertical-allrepos/linux-uksm.svg)](https://repology.org/project/linux-uksm/versions)

###### linux-aufs incorporates:

* [AUFS](https://github.com/sfjro/aufs5-standalone/tree/aufs5.13) / [AUFS](http://aufs.sourceforge.net) - advanced multi-layered unification filesystem

* [graysky's GCC/Clang patch](https://github.com/graysky2/kernel_compiler_patch) - version for gcc v11/clang v12

###### linux-bfq-dev incorporates:

* [bfq improvements](https://groups.google.com/forum/#!forum/bfq-iosched) - latest fixes authored by Paolo Valente and BFQ Team

* ~~[bfq-dev](https://github.com/Algodev-github/bfq-mq/tree/dev-bfq-on-5.6) - latest fixes authored by Paolo Valente and BFQ Team~~

* ~~[bfq-dev-lucjan](https://github.com/sirlucjan/bfq-mq-lucjan/tree/dev-bfq-on-5.6-lucjan) - latest fixes authored by Paolo Valente and BFQ Team and forked by Piotr Gorski~~

* ~~[bfq-dev-lucjan-rc](https://github.com/sirlucjan/kernel-patches/tree/master/5.11/bfq-dev-lucjan) / [bfq-dev-lucjan-rc](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.11/bfq-dev-lucjan) - specific patches authored by Paolo Valente and Piotr Gorski~~

* [bfq-lucjan](https://github.com/sirlucjan/kernel-patches/tree/master/5.13/bfq-lucjan) / [bfq-lucjan](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.13/bfq-lucjan) - specific patches authored by Paolo Valente and Piotr Gorski

* [graysky's GCC/Clang patch](https://github.com/graysky2/kernel_compiler_patch) - version for gcc v11/clang v12

* [LL-patches](https://github.com/sirlucjan/kernel-patches/tree/master/5.13/ll-patches) / [LL-patches](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.13/ll-patches) - specific patches authored by Piotr Gorski

[![latest packaged version(s)](https://repology.org/badge/latest-versions/linux-bfq-dev.svg)](https://repology.org/project/linux-bfq-dev/versions)

###### Some patches for BFQ conflict with patches for BFQ-dev.

###### To use linux-bfq-dev smoothly apply bfq-reverts before bfq-dev patch. Otherwise the kernel will not compile.

* ~~[bfq-reverts](https://github.com/sirlucjan/kernel-patches/tree/master/5.11/bfq-reverts-all) / [bfq-reverts](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.11/bfq-reverts-all) - specific patches authored by Piotr Gorski~~

###### linux-lqx incorporates:

* [liquorix patchset](https://github.com/damentz/liquorix-package/tree/5.12/master) - authored by Steven Barrett

[![latest packaged version(s)](https://repology.org/badge/latest-versions/linux-lqx.svg)](https://repology.org/project/linux-lqx/versions)

###### linux-uksm incorporates:

* [UKSM (sources)](https://github.com/dolohow/uksm) / [UKSM (info)](https://www.usenix.org/sites/default/files/conference/protected-files/fast18_slides_xia.pdf) - resync from dolohow’s github

* [graysky's GCC/Clang patch](https://github.com/graysky2/kernel_compiler_patch) - version for gcc v11/clang v12

[![latest packaged version(s)](https://repology.org/badge/latest-versions/linux-uksm.svg)](https://repology.org/project/linux-uksm/versions)

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

# Enable bfq

~~For now, you can use `sudo tee /sys/block/sda/queue/scheduler <<< bfq` to enable "bfq".~~

~~You can also add this to file `60-schedulers.rules`:~~

```
# Non-rotational disks
ACTION=="add|change", KERNEL=="sd[a-z]", ATTR{queue/rotational}=="0", ATTR{queue/scheduler}="bfq"
# Rotational disks
ACTION=="add|change", KERNEL=="sd[a-z]", ATTR{queue/rotational}=="1", ATTR{queue/scheduler}="bfq"
```

~~and run a command `sudo udevadm control --reload && sudo udevadm trigger`~~

For now, bfq is enabled by default! [(since 5.0-lucjan-ll1-rc1.patch and LL-elevator-set-default-scheduler-to-bfq-for-blk-mq.patch)](https://github.com/sirlucjan/kernel-patches/blob/master/5.0/ll-patches/0002-LL-elevator-set-default-scheduler-to-bfq-for-blk-mq.patch)
