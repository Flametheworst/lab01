# lab01
wget https://sourceforge.net/projects/boost/files/boost/1...
2. tar -xf boost_1_69_0.tar.gz
3. cd boost_1_69_0; tree -L 1
4. tree
4.1 tree -P *.cpp
5.2 tree -P *.h
5.3 ls -la | grep "^-" | grep -v ".cpp" | grep -v ".h" | wc
6. cd boost; readlink -e any.hpp
7. grep -lR "boost::asio"
8. sudo apt install libicu-dev
./bootstrap.sh —prefix=boost_output
./b2 install
9. mv boost_output ~/boost-libs
10. du -ah boost-libs
11. du -ah ~/boost-libs | sort -rh | head -n 10
