installcheck-local:
	$(PYTHON) $(srcdir)/roundTripNCLTest.py -x $(bindir)/NEXUSnormalizer $(srcdir)/funkyValidIn $(srcdir)/funkyValidOut
	$(PYTHON) $(srcdir)/roundTripNCLTest.py -e $(bindir)/NEXUSnormalizer $(srcdir)/ExternalValidIn $(srcdir)/ExternalValidOut
	$(PYTHON) $(srcdir)/roundTripNCLTest.py -i -e $(bindir)/NEXUSnormalizer $(srcdir)/ExternalInvalidIn
	$(PYTHON) $(srcdir)/roundTripNCLTest.py -a $(bindir)/NEXUSnormalizer
	$(PYTHON) $(srcdir)/roundTripNCLTest.py $(bindir)/NEXUSnormalizer $(top_srcdir)/data/characters.nex $(srcdir)/data
	$(PYTHON) $(srcdir)/roundTripNCLTest.py $(bindir)/NEXUSnormalizer $(top_srcdir)/data/sample.tre $(srcdir)/data
	$(PYTHON) $(srcdir)/roundTripNCLTest.py $(bindir)/NEXUSnormalizer $(srcdir)/NTSValidIn $(srcdir)/NTSValidOut
	$(PYTHON) $(srcdir)/roundTripNCLTest.py -o -y -e $(bindir)/NCLconverter $(srcdir)/2NexmlIn $(srcdir)/2NexmlOut
