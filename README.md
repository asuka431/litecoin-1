SCPFoundation Core integration/staging tree
=====================================


What is SCPFoundation?
SCPFoundationCoinとは何でしょう？
----------------
Special Containment Procedures:
SCPFoundation is a symple cryptcuurency which is forked Litecoin.
It is unofficial but allowed from scpfoundation-jp site to deverop.
For more information, as well as an immediately useable, binary version of
the SCPFoundation Core software, see [http://scp-jp-sandbox3.wikidot.com/draft:6861450-3-a538](http://scp-jp-sandbox3.wikidot.com/draft:6861450-3-a538).
But it is written in japanese, so i hope someone to help us with trancelate in english.
特別収容プロトコル：
SCP財団コインはシンプルな文字置換を使って製作されたLitecoinのForkです。
財団非公式ですが、SCP財団日本支部から開発の許可を得ています。
さらに情報が必要な場合は、バイナリーバージョンのこちら
[http://scp-jp-sandbox3.wikidot.com/draft:6861450-3-a538](http://scp-jp-sandbox3.wikidot.com/draft:6861450-3-a538)
を見ていただけるとありがたいです。
しかしながら説明文は日本語しか用意できてないです。誰か翻訳手伝って...

License
-------

SCPFoundation Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/scpfoundation-project/scpfoundation/tags) are created
regularly to indicate new official, stable release versions of SCPFoundation Core.
「master」タグのブランチは一通りの動作が確認されていますが、バグもあります。
新しいステーブル版の完成にご協力お願いします。

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/scpfoundation-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #scpfoundation-dev.

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

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to SCPFoundation periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
