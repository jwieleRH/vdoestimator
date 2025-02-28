# vdoestimator

This is a tool to estimate space savings that can be achieved by the deduplication and
compression of the dm-vdo device mapper device.

## DEPENDENCIES

This project depends on the indexer from the VDO source and the LZ4 compression
library. The VDO development source and the LZ4 source will be retrieved as subprojects.

## BUILDING

Clone the repository:

~~~
git clone --recurse-submodules https://github.com/dm-vdo/vdoestimator.git
~~~

If you don't provide the `--recurse-submodules` option, the submodules will be retrieved
by the Makefile.

Build vdoestimator with the submodules on which it depends:

~~~
make
~~~

## TESTING

To run a smoke test:

~~~
make test
~~~

## INSTALLING

To install vdoestimator automatically into /usr/bin, run:

~~~
sudo make install
~~~
