SEAL_INCLUDE=-I/usr/local/include/SEAL-3.6
SEAL_LIBS=-L/usr/local/lib -lseal-3.6 -lz -Wl,-rpath=/usr/local/lib -lntl

seal_attack: seal_attack.cpp eval.h eval.cpp seal_utils.h seal_utils.cpp
	g++ seal_attack.cpp seal_utils.cpp eval.cpp -o seal_attack  -std=c++17 -O3 -pthread $(SEAL_LIBS) $(SEAL_INCLUDE)

clean:
	rm -f attack seal_attack

.PHONY: all clean

