include ../../Makefile.top

PROJECT_LIST  := FOL_Test

all install clean spotless:
	for d in $(PROJECT_LIST); do \
		$(MAKE) -f Makefile.$$d $@ ; \
	done

$(PROJECT_LIST):
	$(MAKE) -f Makefile.$@

include ../../Makefile.dep
