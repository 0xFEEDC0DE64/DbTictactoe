# DbTictactoe
Tool to create thousands of html documents to host a static version of tictactoe. Every possible field gets its own html file with hyperlinks to others.

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
