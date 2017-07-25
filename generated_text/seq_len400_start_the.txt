the project

the wasm_llvm_config environment variable is used to find our recently built wasm compiler.
this is needed to compile the example contracts insde eos/ contracts folder and their respective tests.

```
git clone https:// github. com/ eosio/ eos-- recursive`

if a repo is cloned without the `-- recursive` flag, the submodules can be retrieved after the fact by running this command from within the repo:

`git submodule update-- init-- recursive`

### configuring and building
to do an in- source build, simply run `cmake. ` from the top level directory. out- of- source builds are also supported. to override clang' s default choice in compiler, add these flags to the cmake command:

`- dcmake_cxx_compiler=/ path/ to/ c++- dcmake_c_compiler=/ path/ to/ cc`

for a debug build, add `- dcmake_build_type= debug`. other common build types include `release` and.

to run a p2p node(ca. 2gb of memory is required at the moment) :

docker run \
- d- p 2001:2001- p 8090:8090-- name steemd- default \
steemit/ steem

docker logs- f steemd- default# follow along

## dockerized full node

to run a node with* all* the data(e. g. for supporting a content website)
that uses ca. 14gb of memory and growing:

docker run \
-- env use_way_too_much_ram= 1-- env use_full_web_node= 1 \
- d- p 2001:2001- p 8090:8090-- name steemd- full \
steemit/ steem

docker logs- f steemd- full

# environment variables

there are quite a few environment variables that can be set to run steemd in different ways:

* `use_way_too_much_ram`- if set to true, steemd starts a' full node'
* `use_full_web_node`- if set to true, a default config file will be used that enables a full set of api' s and associated plugins.
* `use_nginx_frontend`- if set to true, this will enable an nginx reverse proxy in front of steemd that proxies websocket requests to steemd. this will also enable a custom healtcheck at the path'/ health' that lists how many seconds away from current blockchain time your node is. it will return a' 200' if it' s less than 60 seconds away from synced.
* `use_multicore_readonly`- if set to true, this will enable steemd in multiple reader mode to take advantage of multiple cores(if available). read requests are handled by the
[ wiki page](https:// github. com/ bitshares/ bitshares- core/ blob/ master/ libraries/ wallet/ include/ graphene/ wallet/ wallet. hpp).

support
---------
technical support is available in the[ bitsharestalk technical support subforum](https:// bitsharestalk. org/ index. php? board= 45. 0).

bitshares core bugs can be reported directly to the[ issue tracker](https:// github. com/ bitshares/ bitshares- core/ blob/ master/ libraries/ wallet/ include/ graphene/ wallet/ wallet. hpp).

support
--------

testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. please be patient and help out by testing
other people' s pull requests, and remember this is a security- critical project where any mistake might cost people
lots of money.

### automated testing

developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

unit tests for the core code are in `src/ test/ `. to compile and run them:

cd src; make- f makefile. linux test

unit tests for the gui code are in `src/ qt/ test/ `. to compile and run them:

qmake bytecoin_qt_test= 1- o makefile. test bytecoin- qt. pro
make- f makefile. test
./ bytecoin- qt

every pull request is built for both windows and linux on a dedicated server,
and unit and sanity tests are automatically run. the binaries produced may be
used for manual qa testing-- a link to them will appear in a comment on the
pull request posted by' bytecoinpulltester'. see `https:// github. com/ thebluematt/ test- scripts`
for the build/ test scripts.

### manual quality assurance(qa) testing

large changes should have a test plan, and should be tested by somebody other
than the developer who wrote the code.

see `https:// github. com/ bytecoin/ qa/ ` for how to create a test plan.

# lisk

lisk is a next generation crypto- currency
