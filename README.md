BitcoinTK Core integration/staging tree
=====================================

https://bitcoin.tk

https://bitcointk.org

What is BitcoinTK?
----------------

Bitcoin TK exchanges for the Time as valued unit: 1 BITK = 60 sec.
For Time is intended the time needed to complete a task.

Our Mission is to establish an equal financial retribution model for Global workers. 
We keep records and proof of working and social time and local tax payments 
on the Blockchain for an United Welfare and Pension system. 

BitcoinTK is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. BitcoinTK uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. 

Bitcoin TK stands for Bitcoin Time Kit
Bitcoin TK (BITK) is a peer-to-peer cryptocurrency and open-source software project released 
under the MIT/X11 license. Litecoin was an early bitcoin spinoff or altcoin, starting in 
October 2011. In technical details, Litecoin is nearly identical to Bitcoin.

It is the first Cryptocurrency to be exchanged for the Time as valued unit: 1 BITK = 60 sec.
For Time is intended your time - the time you need to compete a task.

BitcoinTK is released via an open-source client on GitHub.
It is a source code fork of the Bitcoin Core client, differing primarily by having a decreased 
block generation time (1 minute), increased maximum number of coins, different hashing algorithm 
(scrypt, instead of SHA-256), and a slightly modified GUI.

BitcoinTK is different in some ways from Bitcoin.
* The BitcoinTK Network aims to process a block every 60 seconds, rather than Bitcoin's 10 minutes. 
This allows BitxoinTK to confirm transactions much faster than Bitcoin.
* BitcoinTK uses scrypt in its proof-of-work algorithm, a sequential memory-hard function requiring 
asymptotically more memory than an algorithm which is not memory-hard.
Due to BitcoinTK’s use of the scrypt algorithm, FPGA and ASIC devices made for mining BitcoinTK 
are more complicated to create and more expensive to produce than they are for Bitcoin, which uses SHA-256.

In cryptography, scrypt is a password-based key derivation function created by Colin Percival, 
originally for the Tarsnap online backup service. The algorithm was specifically designed to make it 
costly to perform large-scale custom hardware attacks by requiring large amounts of memory. 
In 2016, the scrypt algorithm was published by IETF as RFC 7914. A simplified version of scrypt is used 
as a proof-of-work scheme by a number of cryptocurrencies, first implemented by an anonymous programmer 
called ArtForz in Tenebrix and followed by Fairbrix and Litecoin soon after and now BicoinTK.
Scrypt is used in many cryptocurrencies as a proof-of-work algorithm. 
It was first implemented for Tenebrix (released in September 2011) and served as the basis for 
Litecoin and Dogecoin and BitcoinTK, which also adopted its scrypt algorithm. 
Specialized ASIC mining hardware is available for scrypt-based cryptocurrencies.

BitcoinTK Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the BitcoinTK Core software, see [https://bitcoin.tk](https://bitcoin.tk).

License
-------

BitcoinTK Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/atixi/BITK/tags) are created
regularly to indicate new official, stable release versions of BitcoinTK Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md)
and useful hints for developers can be found in [doc/developer-notes.md](doc/developer-notes.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/bitcointk-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #bitcointk-dev.

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

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and macOS, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to BitcoinTK periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
