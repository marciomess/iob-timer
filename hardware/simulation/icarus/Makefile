TIMER_DIR:=../../..
incdir:=-I
defmacro:=-D
include ../simulation.mk

#icarus verilog simulator
VLOG:=iverilog -W all -g2005-sv

run: a.out
	./$<

a.out: $(VSRC) $(VHDR)
	$(VLOG) $(INCLUDE) $(DEFINE) $(VSRC)

clean: clean_hw
	@rm -f a.out *~ *.vcd

.PHONY: all clean

