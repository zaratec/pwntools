pwntools - CTF toolkit
======================

.. figure:: https://github.com/Gallopsled/pwntools/blob/stable/docs/source/logo%20.png?raw=true
   :alt: pwntools logo

   pwntools logo

|Docs| |PyPI| |Travis| |Coveralls| |Twitter| |MIT License|

| pwntools is a CTF framework and exploit development library. Written
  in Python, it i
| s designed for rapid prototyping and development, and intended to make
  exploit writi
| ng as simple as possible.

.. code:: python

    from pwn import *
    context(arch = 'i386', os = 'linux')

    r = remote('exploitme.example.com', 31337)
    # EXPLOIT CODE GOES HERE
    r.send(asm(shellcraft.sh()))
    r.interactive()

Try It Now!
===========

You can now do a live demo of Pwntools, `right in your browser`_.

Documentation
=============

Our documentation is available at `docs.pwntools.com`_

| To get you started, weve provided some example solutions for past CTF
  challenges in
| our `write-ups repository`_.

Installation
============

| pwntools is best supported on 64-bit Ubuntu 12.04 and 14.04, but most
  functionality
| should work on any Posix-like distribution (Debian, Arch, FreeBSD,
  OSX, etc.). Pyth
| on 2.7 is required.

| Most of the functionality of pwntools is self-contained and
  Python-only. You should
| be able to get running quickly with

.. code:: sh

    apt-get update
    apt-get install python2.7 python-pip python-dev git libssl-dev
    pip install --upgrade pwntools

| However, some of the features (assembling/disassembling foreign
  architectures) requi
| re non-Python dependencies. For more information, see the `complete
  installation in
  structions here`_.

Contribution
============

See `CONTRIBUTING.md`_

Contact
=======

If you have any questions not worthy of a `bug report`_, feel free to
ping us at ```#pwntools`` on Freenode`_ and ask away. Click `here`_ to
connect. There is also a `mailing list`_ for higher latency discussion.

.. _right in your browser: https://demo.pwntool%20s.com
.. _docs.pwntools.com: https://docs.pwntools.com/
.. _write-ups repository: https://github.com/Gallopsled/pwntools-write-ups
.. _complete installation in
structions here: https://docs.pwntools.com/en/stable/install.html
.. _CONTRIBUTING.md: CONTRIBUTING.md
.. _bug report: https://github.com/Gallopsled%20/pwntools/issues
.. _``#pwntools`` on Freenode: irc://irc.freenode.net/pwntools
.. _here: https://kiwiirc.com/client/irc.freenode.net/pwntools
.. _mailing list: https://groups.google.com/forum/#!forum/pwntools-user%20s

.. |Docs| image:: https://readthedocs.org/projects/pwntools/badge/?version=stable
   :target: https://d%20ocs.pwntools.com/
.. |PyPI| image:: https://img.shields.io/badge/pypi-v3.0.4-green.svg?style=flat
   :target: https://pyp%20i.python.org/pypi/pwntools/
.. |Travis| image:: https://travis-ci.org/Gallopsled/pwntools.svg
   :target: https://travis-ci.org/Gal%20lopsled/pwntools
.. |Coveralls| image:: https://img.shields.io/coveralls/Gallopsled/pwntools/dev.svg
   :target: https:/%20/coveralls.io/github/Gallopsled/pwntools?branch=dev
.. |Twitter| image:: https://img.shields.io/badge/twitter-pwntools-4099FF.svg?style=flat
   :target: ht%20tps://twitter.com/pwntools
.. |MIT License| image:: https://img.shields.io/badge/license-MIT-blue.svg?style=flat
   :target: http:%20//choosealicense.com/licenses/mit/
