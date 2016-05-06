INKSCAPE = inkscape

REFFIGS =					\
	hexahedron_edges			\
	hexahedron				\
	prism_edges				\
	prism					\
	pyramid_edges				\
	pyramid					\
	quadrilateral				\
	tetrahedron_edges			\
	tetrahedron				\
	triangle

all: $(addsuffix .pdf, $(REFFIGS))

%.pdf: %.svg
	$(INKSCAPE) --export-pdf=$*.tmp.pdf $<
	mv $*.tmp.pdf $@
