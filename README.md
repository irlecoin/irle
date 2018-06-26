IrleCoin Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/irlecoin-project/irlecoin.svg?branch=master)](https://travis-ci.org/irlecoin-project/irlecoin)

https://irlecoin.com

Blockchain Properties
----------------

- Algorithm: Scrypt
- Type: PoW 
- Coin Name: Irlecoin
- Coin Abbreviation: IRLE 
- RPC Port: 44421
- Block Reward: 50 Coins 
- Coin Supply: 21,000,000 Coins 
- Premine Amount: 1,000,000 Coins
- Telegram: https://t.me/joinchat/HPt-_Qt-bqghWcv9Vj7AvA

Nodes:

- 77.95.36.184:44421
- 45.76.83.205:44421
- 51.15.162.24:44421
- 173.212.211.156:44421
- 88.198.33.48:44421
- 192.95.33.131:44421
- 212.237.37.46:44421
- 173.249.38.175:44421
- 80.211.53.13:44421
- 5.189.148.168:44421
- 80.211.1.45:44421
- 51.15.185.7:44421
- 85.10.206.105:44421
- 95.165.157.61:44421
- 173.212.235.98:44421
- 180.216.101.138:44421
- 61.68.133.85:44421
- 123.29.69.244:44421

What is IrleCoin?
----------------

IrleCoin is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. IrleCoin uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. IrleCoin Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the IrleCoin Core software, see [https://irlecoin.com](https://irlecoin.com).

License
-------

IrleCoin Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/irlecoin-project/irlecoin/tags) are created
regularly to indicate new official, stable release versions of IrleCoin Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/irlecoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #irlecoin-dev.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to IrleCoin periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
