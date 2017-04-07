
FC=ifort

OBJS= force_verticale.f

.PHONY:
	make all

force_verticale:force_verticale.f
	$(FC) $< -o xforce
	rm -f force_verticale.o *.trace

bicouche:bicouche.f
	$(FC) $< -o xbicouche
	rm -f bicouche.o *.trace

explosion:explosion.f
	$(FC) $< -o xexplosion
	rm -f explosion.o *.trace

all: 
	rm -f *.o *.trace
	make force_verticale
	make bicouche
	make explosion

clean: 
	rm -f *.o *.trace
