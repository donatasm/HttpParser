CC= gcc
CFLAGS= -arch i386 -Wall -ansi -pedantic -O3 -std=c99
HTTP_PARSER= HttpParser_x32.dylib

HttpParser: http_parser.h http_parser.c Makefile
	$(CC) $(CFLAGS) \
	-dynamiclib -o $(HTTP_PARSER) \
	http_parser.c \
	-framework CoreFoundation \
	-framework CoreServices

clean:
	rm -f $(HTTP_PARSER)