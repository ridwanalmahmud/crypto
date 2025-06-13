CC      := clang
CFALGS  := -Wall -Wextra -pedantic -02

INCDIRS := -I../include -Iutils
UTILDIR := utils
SRCDIR  := ../src

all: chacha20/test_chacha20

chacha20/test_chacha20:
	$(CC) $(CFLAGS) $(INCDIRS) \
	$(SRCDIR)/symmetric/chacha20.c $(UTILDIR)/test_utils.c \
	chacha20/test_chacha20.c -o chacha20/test_chacha20 \

test:
	chacha20/test_chacha20

clean:
	rm chacha20/test_chacha20
