transcript on
if ![file isdirectory verilog_libs] {
	file mkdir verilog_libs
}

vlib verilog_libs/altera_ver
vmap altera_ver ./verilog_libs/altera_ver
vlog -vlog01compat -work altera_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/altera_primitives.v}

vlib verilog_libs/lpm_ver
vmap lpm_ver ./verilog_libs/lpm_ver
vlog -vlog01compat -work lpm_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/220model.v}

vlib verilog_libs/sgate_ver
vmap sgate_ver ./verilog_libs/sgate_ver
vlog -vlog01compat -work sgate_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/sgate.v}

vlib verilog_libs/altera_mf_ver
vmap altera_mf_ver ./verilog_libs/altera_mf_ver
vlog -vlog01compat -work altera_mf_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/altera_mf.v}

vlib verilog_libs/altera_lnsim_ver
vmap altera_lnsim_ver ./verilog_libs/altera_lnsim_ver
vlog -sv -work altera_lnsim_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/altera_lnsim.sv}

vlib verilog_libs/arriaii_hssi_ver
vmap arriaii_hssi_ver ./verilog_libs/arriaii_hssi_ver
vlog -vlog01compat -work arriaii_hssi_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/arriaii_hssi_atoms.v}

vlib verilog_libs/arriaii_pcie_hip_ver
vmap arriaii_pcie_hip_ver ./verilog_libs/arriaii_pcie_hip_ver
vlog -vlog01compat -work arriaii_pcie_hip_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/arriaii_pcie_hip_atoms.v}

vlib verilog_libs/arriaii_ver
vmap arriaii_ver ./verilog_libs/arriaii_ver
vlog -vlog01compat -work arriaii_ver {c:/intelfpga_lite/23.1std/quartus/eda/sim_lib/arriaii_atoms.v}

if {[file exists rtl_work]} {
	vdel -lib rtl_work -all
}
vlib rtl_work
vmap work rtl_work

vlog -sv -work work +incdir+C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer {C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer/sender_fsm.sv}
vlog -sv -work work +incdir+C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer {C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer/receiver_fsm.sv}
vlog -sv -work work +incdir+C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer {C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer/handshake_synchronizer.sv}
vlog -sv -work work +incdir+C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer {C:/projects/systemverilog/ECE11/ProjectPart1/handshake_synchronizer/flipflop_synchronizer.sv}

