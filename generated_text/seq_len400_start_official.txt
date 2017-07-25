official go- ethereum project comes with several wrappers/ executables.

### running

the settings for a full web node, sbt need. to compile the system, and ` is
used to login and gain access to additional, restricted api' s
and agree upon. this consists of a small json file(e. g. call it `genesis. json`) :

```json
{
	" port" : 6611,
	" storage" :" mysql",
	" database" : {
		" max_connections" : 30,
		 proxy_set_header x- real- ip$ remote_addr;
		 proxy_set_header x- forwarded- for$ proxy_add_x_forwarded_for;
		 proxy_set_header upgrade$ http_upgrade;
		 proxy_set_header connection" upgrade";
	 }

	 root/ var/ www/ html;
	 server_name _;
}
```

# factom

[![ build status](https:// travis- ci. org/ factomproject/ factomd. svg? branch= develop)](https:// travis- ci. org/ factomproject/ factomd)

factom is an open- source project that provides a way to build applications on the bitcoin blockchain.

factom began by providing proof of existence services, but then move on to provide proof of existence of transforms. a list of such entries can be thought of as a factom chain. factom can be used to implement private tokens, smart contracts, smart properties, and more.

factom leverages the bitcoin blockchain, but in a way that minimizes the amount of data actually inserted in the blockchain. thus it provides a mechanism for creating bitcoin 2. 0 services for the trading of assets.
the contribution workflow is described in[ contributing. md](contributing. md).

the developer[ mailing list](https:// groups. google. com/ forum/#! forum/ litecoin- dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

developer irc can be found on freenode at# litecoin- dev.

testing
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

lisk is a next generation crypto- currency and decentralized application platform, written entirely in javascript. for more information please refer to our website: https:// lisk. io/.

[![ build status](https:// jenkins. lisk. io/ buildstatus/ icon? job= lisk- pipeline/ development)](https:// jenkins. lisk. io/ buildstatus/ icon? job= lisk- pipeline/ development)](https:// jenkins. lisk. io/ buildstatus/ icon? job= lisk- pipeline/ development)](https:// codecov. io/ gh/ golemfactory/ golem)

the aim of the golem project is to create a global prosumer market for computing power, in which
producers may sell spare cpu time of their personal computers and consumers may acquire resources
for computation- intensive tasks. in technical terms, golem is designed as a decentralised peer- to- peer
network established by nodes running the golem client software. for the purpose of this paper we assume
that there are two types of nodes in the golem client. to run the client.
simply copy these files to your web server of choice.
