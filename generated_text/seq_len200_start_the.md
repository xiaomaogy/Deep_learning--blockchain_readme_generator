the stratis bitcoin blockchain:
sidechains, private/ permissioned blockchain, compiled smart contracts, ntumblebit/ breeze wallet and more...

running a fullnode
-------------------

our full node is currently in alpha.

```
git clone https:// github. com/ stratisproject/ stratisbitcoinfullnode. git
cd stratisbitcoinfullnode

git submodule init
git submodule update

dotnet restore
dotnet build

```

to run on the bitcoin network: ``` stratis. bitcoind\dotnet run ```
to run on the stratis network: ``` stratis. stratisd\dotnet run ```

see more details[ here](https:// github. com/ stratisproject/ stratisbitcoinfullnode/ blob/ master/ documentation/ getting- started. md)

development
------------

ncc is fully open- sourced and looking for contributors. please take a fork and add a feature :).

# running tests

`sbt test`

# running integration tests

## tl; dr

* make sure you have[ docker](https:// www. docker. com/ get- docker) and sbt.
* `sbt-----------

## prerequisites

1. download[ nodejs](https:// nodejs. org/)
[ info] tagging image e243fa08d496 with name: com. wavesplatform/ root
[ success] total time: 4 s, completed mar 22, 2017 12:36:34 pm
```

in this example, `e243fa08d496` is the image id you need. make sure to re- build the image whenever the node code(not
the tests). to run the test suite after building, run the `chain_test` executable in the `tests` folder.

### creating and launching a single- node testnet
after successfully building the project, the `eosd` binary should be present in the `programs/ eosd` directory. go ahead and run `eosd`-- it will probably exit with an error, but if not, close it immediately with ctrl- c. note that `eosd` will have created a directory named `data- dir` containing the default configuration(`config. ini`) and some other internals. this default data storage path can be overridden by passing `-- data- dir/ path/ to/ data` to `eosd`.

edit the `config. ini` file, adding the following settings to the defaults already in place:

```
# load the testnet genesis state, which creates some initial block producers with the default key
genesis- json=/ path/ to/ eos/ source/ genesis.

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along
