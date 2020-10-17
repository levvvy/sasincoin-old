Sasincoin (c) 2020
================================

![Alt text](/share/pixmaps/bitcoincoin256.png?raw=true)

Copyright (c) 2009-2014 Bitcoin Developers  
Copyright (c) 2011-2014 Litecoin Developers  
Copyright (c) 2020 Sasincoincoin Developers 

---

### :mag: **Block Explorer** - http://18.197.190.51:3001/ :mag_right:
![wykop](https://www.wykop.pl/cdn/c3201142/comment_R1x9oiehIKf69fMicte6mGoYXVphyIbF.gif) **Tag na wykopie** - https://www.wykop.pl/tag/sasincoin/  

---

# :warning: Przy próbie uruchomienia programu dla windows, antywirusy, przeglądarka oraz windows defender powinny zgłaszać zagrożenie   
**Jest to nic innego jak bitcoin-miner, czyli program, który chemy otworzyć,** ****nie stanowi on zagrożenia.****  
https://www.virustotal.com/gui/file/23db0a504b7c4fc2dcda371c63ba1d5790f5da8558e6c61b73817c5f00882bef/detection  
### Jeśli masz dalsze wątpliwości, samodzielnie skompiluj portfel na windows lub linux!  
----------------



Co to jest Sasincoin?
----------------

Sasincoin to lite wersja Bitcoina wykorzystująca scrypt jako algorytm proof-of-work.
  - 1-minutowe cele blokowe
  - dotacja zmniejsza się o połowę w blokach 10000 tys.
  - łącznie ~ 70 milionów monet

Inne
  - 7 monet na blok
  - 2016 bloków, aby zmienić poziom trudności

Aby uzyskać więcej informacji, a także natychmiast użyć binarnej wersji programu
oprogramowanie klienta Sasincoin, patrz https://github.com/levvvy/sasincoin

License
-------

Sasincoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Sasincoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/sasincoin-project/sasincoin/tags) are created
regularly to indicate new official, stable release versions of Sasincoin.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./sasincoin-qt_test

