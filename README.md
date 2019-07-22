# Kernels and modules:

- linux-aufs

- linux-bfq

- linux-lqx

- linux-next-git

- linux-uksm

###### linux-aufs incorporates:

* [AUFS](https://github.com/sfjro/aufs5-standalone) / [AUFS](http://aufs.sourceforge.net) - advanced multi-layered unification filesystem

###### linux-lqx incorporates:

* [liquorix patchset](https://github.com/damentz/liquorix-package) - authored by Steven Barrett

###### linux-bfq incorporates:

* [bfq improvements](https://groups.google.com/forum/#!forum/bfq-iosched) - latest fixes authored by Paolo Valente and BFQ Team

* [bfq-dev](https://github.com/Algodev-github/bfq-mq/commits/dev-bfq-on-5.2) - latest fixes authored by Paolo Valente and BFQ Team

* [LL-patches](https://github.com/sirlucjan/kernel-patches/tree/master/5.1/ll-patches) / [LL-patches](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.1/ll-patches) - specific patches authored by Piotr Gorski

* [bfq-lucjan-dev](https://github.com/sirlucjan/bfq-mq-lucjan/commits/dev-bfq-on-5.2-lucjan) - latest fixes authored by Paolo Valente and BFQ Team and forked by Piotr Gorski

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
