## Process this file with automake to produce Makefile.in

sampleprogdir = $(prefix)/dx/samples/programs/DEBUGGING

LINKLIST = \
         Verify.cfg\
         Verify.net\
         VisualObject.cfg\
         VisualObject.net

myinstall: 
	$(mkinstalldirs) $(DESTDIR)$(sampleprogdir)
	@-sh -c '( echo "cd $(DESTDIR)$(sampleprogdir)" ; \
		cd $(DESTDIR)$(sampleprogdir) && for s in $(LINKLIST) ; do \
		$(LN_S) ../$$s $$s ; \
		echo "$(LN_S) ../$$s $$s" ; \
	done )'
