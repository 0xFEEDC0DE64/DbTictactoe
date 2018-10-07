# DbTictactoe
Tool to create thousands of html documents to host a static version of tictactoe. Every possible field gets its own html file with hyperlinks to others.

[![Build Status](https://travis-ci.org/0xFEEDC0DE64/DbTictactoe.svg?branch=master)](https://travis-ci.org/0xFEEDC0DE64/DbTictactoe) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/afe85fb2422445e79445978b88aab5a8)](https://www.codacy.com/app/0xFEEDC0DE64/DbTictactoe?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=0xFEEDC0DE64/DbTictactoe&amp;utm_campaign=Badge_Grade)

## Building from source
This project can only be built as part of the project structure [DbSoftware](https://github.com/0xFEEDC0DE64/DbSoftware)

```Shell
git clone https://github.com/0xFEEDC0DE64/DbSoftware.git
cd DbSoftware
git submodule update --init --recursive DbTictactoe
cd ..
mkdir build_DbSoftware
cd build_DbSoftware
qmake CONFIG+=ccache ../DbSoftware
make -j$(nproc) sub-DbTictactoe
make sub-DbTictactoe-install_subtargets
./bin/serialserver
```
