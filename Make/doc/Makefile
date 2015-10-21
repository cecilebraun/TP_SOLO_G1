DESTDIR  = /usr/local
MAKEINFO = makeinfo
RM       = rm -f

gnuchess.info: gnuchess.texi version.texi fdl.texi
	$(MAKEINFO) $<

install: gnuchess.info
	mkdir -p $(DESTDIR)/share/info
	cp gnuchess.info $(DESDIR)/share/info

clean:
	$(RM) gnuchess.info

.POHNY: clean install
