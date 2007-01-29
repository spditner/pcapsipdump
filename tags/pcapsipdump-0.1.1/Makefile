all: pcapsipdump

pcapsipdump: pcapsipdump.cpp calltable.cpp calltable.h
	c++ -s -Wall -O2 -fomit-frame-pointer pcapsipdump.cpp calltable.cpp -o pcapsipdump -lpcap

pcapsipdump-debug: pcapsipdump.cpp calltable.cpp calltable.h
	c++ -ggdb -Wall pcapsipdump.cpp calltable.cpp -o pcapsipdump-debug -lpcap

clean:
	rm -f pcapsipdump
