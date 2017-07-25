a warning from the windows firewall; be sure
to check both boxes(" private networks" and" public networks") and click
" allow access." you can now run `siac`(in a separate command prompt) or sia-
ui to interact with siad. from here, you can send money, upload and download
files, and advertise yourself as a host.

building from source
---------------------

please use the intellij settings checked in under settings/ nem_project_settings. jar packages will be created on unix systems in docker image at- time.

### manual quality assurance(qa) testing

changes should be tested by somebody other than the developer who wrote the
code. this is especially important for large or high- risk changes. it is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

translations
------------

changes to translations as well as new translations can be submitted to
[ dash core' s transifex page](https:// www. transifex. com/ projects/ p/ dash/).

translations are periodically pulled from transifex and merged into the git repository. see the
[ translation process](doc/ translation_process. md) for details on how this works.

** important** : we do not accept translation changes as github pull requests because the next
pull from transifex would automatically overwrite them again.

translators should also subscribe to the[ mailing list](https:// groups. google. com/ forum/#! forum/ bitcoin- translators).

litecoin core integration/ staging tree
=============================

[![ build status](https:// travis- ci. org/ litecoin- project/ litecoin- project/ litecoin)
https:// bitcoincore. org

what is bitcoin?
----------------

dash is an experimental new digital currency that enables anonymous, instant
payments to anyone, anywhere in the world. dash uses peer- to- peer technology
to operate with no central authority: managing transactions and issuing money
are carried out collectively by the network. dash core is the name of the open
source software which enables the use of this currency.

for more information, as well as an immediately useable, binary version of
the dash core software, see https:// bitcoin.


license
--------


testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. please be patient and help out, and
remember this is a security- critical project where any mistake might cost people
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
and the process lists.

#### conf. bwantnewpeers

whether your node wants to learn about new peers from its current peers(`true`, the default) or not(`false`). set it to `false` to run your node in stealth mode so that only trusted peers can see its ip address(e. g. if you have online wallets on your server and don' t want potential attackers to learn its ip).

#### conf. sockshost, conf. socksport, and conf. sockslocaldns

settings for connecting through optional socks5 proxy. use them to connect through tor and hide your ip address from peers even when making outgoing connections. this is useful and highly recommended when you are running an online wallet on your server and want to make it harder for potential attackers to learn the ip address of the target to attack. set `sockslocaldns` to `false` to route dns queries through tor as in a config file. it may be used to execute factomd.

the first and second number together identify the kind of thing you' re talking about.

### supporting the project

monero development can be supported directly through donations.

both monero and bitcoin donations can be made to donate. getmonero. org
