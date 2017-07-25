bitcoin core integration/ staging tree
============================================================================================================================================================================================================================

[![ build status](https:// travis- ci. org/ bitcoin/ bitcoin. svg? branch= master)](https:// travis- ci. org/ nemproject/ nemcommunityclient)

ncc is the initial client provided with nem. it provides a web interface for managing transactions.
| folder | contents | and | allow |
| doxygen | any | no | `doxygen` | `doxygen` | yes | documentation |
| graphviz | any | no | `graphviz` | `graphviz` | yes | documentation |

[ ^] on debian/ ubuntu `libgtest- dev` only includes sources and headers. you must
build the library binary manually. this can be done with the following command ```sudo apt- get install libgtest- dev&& cd/ usr/ src/ gtest&& sudo cmake.&& sudo make&& sudo mv libg*/ usr/ lib/ ```

### build instructions

monero uses the cmake build system and a top- level[ makefile](makefile) that
invokes cmake commands as needed.

#### on linux and os x

* install the dependencies
* change to the root of the source code directory and build:

cd monero
make

* optional* : if your machine has several cores and enough memory, enable
parallel build by running `make- j< number of threads> ` instead of `make`. for
this to be worthwhile, the machine should have one core and about 2gb of ram
available per thread.

* the resulting executables can be found in `build/ release/ bin`

* add `path="$ path:$ home/ monero/ build/ release/ bin" ` to `. profile`

* run monero with `monerod-- detach`

** you may wish to reduce the size of the swap file after the build has finished, and delete the boost directory from your home directory

#### on windows:

binaries for windows are built on windows using the mingw toolchain within
[ msys2 environment](http:// msys2. github. io). the msys2 environment emulates a
posix system. the toolchain runs within the environment and* cross- compiles*
binaries that can run outside of the environment as a regular windows
application.

** preparing the build environment**

* download and install[ geth specific apis](https:// github. com/ ethereum/ go- ethereum/ wiki/ management- apis)). these can be
exposed via http, websockets and ipc(unix sockets on unix based platforms, and named pipes on windows).

the ipc interface is enabled by default and exposes all the apis supported by geth, whereas the http
and ws interfaces need to manually be enabled and only expose a subset of apis due to security reasons.
these can be turned on/ off and configured as you' ll be running the same testnet node before changes

```
git remote set- url origin https:// github. com/ bitshares/ bitshares- core. git
git checkout master
git remote set- head origin-- auto
git pull
git submodule sync-- recursive
git submodule update-- init-- recursive

getting started
-------------------

to build from source,[ go 1. 8 must be installed](https:// golang. org/ doc/ install)
on the system. then simply use `go get`:

```
go get- u github. com/ nebulouslabs/ sia/....
```

this will download the sia repo to your `$ gopath/ src` folder, and install the
`siad` and `siac` binaries in your `$ gopath/ bin` folder.

to stay
