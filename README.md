# Kernels and modules:

- linux-aufs

- linux-bfq

[![Packaging status](https://repology.org/badge/vertical-allrepos/linux-bfq.svg)](https://repology.org/project/linux-bfq/versions)

- linux-lqx

[![Packaging status](https://repology.org/badge/vertical-allrepos/linux-lqx.svg)](https://repology.org/project/linux-lqx/versions)

- linux-next-git

- linux-uksm

###### linux-aufs incorporates:

* [AUFS](https://github.com/sfjro/aufs5-standalone) / [AUFS](http://aufs.sourceforge.net) - advanced multi-layered unification filesystem

###### linux-bfq incorporates:

* [bfq improvements](https://groups.google.com/forum/#!forum/bfq-iosched) - latest fixes authored by Paolo Valente and BFQ Team

* [bfq-dev](https://github.com/Algodev-github/bfq-mq/commits/dev-bfq-on-5.2) - latest fixes authored by Paolo Valente and BFQ Team

* [LL-patches](https://github.com/sirlucjan/kernel-patches/tree/master/5.1/ll-patches) / [LL-patches](https://gitlab.com/sirlucjan/kernel-patches/tree/master/5.1/ll-patches) - specific patches authored by Piotr Gorski

* [bfq-lucjan-dev](https://github.com/sirlucjan/bfq-mq-lucjan/commits/dev-bfq-on-5.2-lucjan) - latest fixes authored by Paolo Valente and BFQ Team and forked by Piotr Gorski

[![latest packaged version(s)](https://repology.org/badge/latest-versions/linux-bfq.svg)](https://repology.org/project/linux-bfq/versions)

###### linux-lqx incorporates:

* [liquorix patchset](https://github.com/damentz/liquorix-package) - authored by Steven Barrett

[![latest packaged version(s)](https://repology.org/badge/latest-versions/linux-lqx.svg)](https://repology.org/project/linux-lqx/versions)

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
