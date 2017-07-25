official/ travis- ci. org/ augurproject/ augur. svg? branch= master)](https:// travis- ci. org/ augurproject/ augur)
[![ coverage status](https:// coveralls. io/ repos/ github/ augurproject/ augur/ badge. svg? branch= master)](https:// coveralls. io/ github/ augurproject/ augur? branch= master)

augur is a decentralized prediction market platform built on ethereum.
it runs locally in your browser and communicates directly with the ethereum network, without going through intermediate servers.

there are several ways to run it:

* easiest:** visit[ app. augur. net](http:// app. augur. net)**
* balanced:** one- click azure install(coming soon)**
* best:[ run ethereum locally](# eth_local)

## requirements
[ git](https:// git- scm. com/)
```
docker build- t augur.
```

### running a private miner

mining on the public ethereum network is a complex task as it' s only feasible using gpus, requiring
an opencl or cuda enabled.

see http://./ byteball. one/ privkey. pem"

##- prefix

this makes all the simnodes in this process followers. it prefixes the text provided to the node names(and the generated file names) of all the factom instances created. so without a prefix, you would get nodes named fnode0, fnode1, etc. with the a_ prefix described below, you would get a_fnode0, a_fnode1, etc.

fnode0 is currently a" magic name", and the node with that name becomes the first default leader when building factom up from scratch.(of course, if you are loading an existing network, it will come up with the last set of leaders). in any event, adding the prefix avoids having fnode0 as a name, and as a pull request is built and tested, but is not guaranteed
to be
completely stable.[ tags](https:// github. com/ bitcoin/ bitcoin/ tags) are created
regularly to indicate new official, stable release versions of bitcoin core.

the contribution workflow is described in[ contributing. md](contributing. md).

the developer[ mailing list](https:// lists. appveyor. com/ golemfactory/ golem/ develop/ installer/ installer_linux/ install. sh), make it executable `chmod+ x install. sh` and run `./ install. sh`.
for ms windows download the installer from[ here](https:// github. com/ golemfactory/ golem/ releases/); when downloaded, just run `setup. exe`.

then read the application description and[ testing](https:// github. com/ stratisproject/ stratisbitcoinfullnode/ blob/ master/ documentation/ getting- started. md)

development process
---------------
up for some blockchain development?

check this guides for more info:
*[ contributing guide](documentation/ contributing. md)
- node.

running monero
----------
build instructions and additional documentation are available in the
[ wiki](https:// github. com/ bitshares/ bitshares- core. git
cd bitshares- core
git checkout< latest_release_tag>
git submodule update-- init-- recursive
cmake- dcmake_build_type= relwithdebinfo.
make

** note:** bitshares requires an[ openssl](https:// www. openssl. org/) version in the 1. 0. x series. openssl 1. 1. 0 and newer are not supported. if your system openssl version is newer, then you will need to manually provide an older version of openssl and specify it to cmake using `- dopenssl_include_dir`, `- dopenssl_ssl_library`, and `- dopenssl_crypto_library`.

** note:** bitshares requires a miner to build boost yourself from a

you can override the[ cli wiki page](https:// github. com/ ethereum/ go- ethereum/ wiki/ javascript- console),
(via the trailing `console` subcommand) through which you can invoke all official[ `web3` methods](https:// github. com/ ethereum/ wiki/ wiki/ javascript- api)
as well as geth' s own[ management apis](https:// github. com/ ethereum/ go- ethereum/ wiki/ management- apis).
this too is optional and if you leave it out you can always attach to an already running geth instance
with `geth attach`.

### full node on the ethereum test network

transitioning towards developers, if you' d like to play around with creating ethereum contracts, you
almost certainly would like to manually, all of any mining,
