## Process this file with automake to produce Makefile.in

sampleprogdir = $(prefix)/dx/samples/programs/PROBES

LINKLIST = \
         PlotLine2.cfg\
         PlotLine2.net\
         ProbeText.cfg\
         ProbeText.net\
         UsingProbes.cfg\
         UsingProbes.net\
         UsingStreakline.cfg\
         UsingStreakline.net

myinstall: 
	$(mkinstalldirs) $(DESTDIR)$(sampleprogdir)
	@-sh -c '( echo "cd $(DESTDIR)$(sampleprogdir)" ; \
		cd $(DESTDIR)$(sampleprogdir) && for s in $(LINKLIST) ; do \
		$(LN_S) ../$$s $$s ; \
		echo "$(LN_S) ../$$s $$s" ; \
	done )'
