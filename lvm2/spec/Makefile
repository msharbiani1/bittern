NAME=$(shell rpm -q --qf '%{name}\n' --specfile *.spec | head -1)
VERSION=$(shell rpm -q --qf '%{version}\n' --specfile *.spec | head -1)

.PHONY: sources
sources:
	cd .. ; git archive --prefix $(NAME)-$(VERSION)/ -o $(CURDIR)/$(NAME)-$(VERSION).tar.gz HEAD
