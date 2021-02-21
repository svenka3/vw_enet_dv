
all: clean
	vlib work
	vlog -f tb.f -f dut.f -sv -mfcu -l comp.log
	vsim -c packet_tb_top -do "run 1us;exit"

clean:
	rm -fr work *.log *.wlf


