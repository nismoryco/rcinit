PREFIX ?= /usr
DESTDIR ?=
SBINDIR ?= $(PREFIX)/sbin
CFLAGS ?= -O2 -pipe

CFLAGS += -Wall -Wextra -pedantic

start-stop-daemon: start-stop-daemon.c

install: start-stop-daemon
	install -v -D -m 0755 start-stop-daemon "$(DESTDIR)$(SBINDIR)/start-stop-daemon"

clean:
	rm -f start-stop-daemon

.PHONY: clean
