# Lab 1: Counter
## Task 1: Simulating 8-bit binary counter

### Aim: Simulate a basic 8-bit binary counter

![image](https://github.com/user-attachments/assets/bb57fb2f-cdaf-4d3f-8ed3-bd9ffc0cb0df)

Code above is counter.sv. The counter starts at the positive edge when enable is set to 1. The reset is triggered during the 15th clock cycle, which is displayed at the positive edge of cycle 16. The counter then experiences the reset during Cycle 16, which is displayed at the positive edge of clock cycle 17. 

Below is the testbench.cpp file (which is a template for all other testbench files). The structure is always the same.

![image](https://github.com/user-attachments/assets/2c73185f-cc95-436c-9931-fdc143d08599)

The steps followed from here were:

1) Compiled the System Verilog model with the testbench - this causes Verilator to translate counter.sv into C++ code
2) This then merges with counter_tb.cpp and produces a number of files in a new folder: obj_dir. It also automatically generates a .mk file called Vcounter.mk, which then produces the final simulation model Vcounter.
3) Vcounter is the executable version of the counter. We can run this model and it will generate waves on GTKwave.

The waves are shown below:

![image](https://github.com/user-attachments/assets/be6af5a3-9fb0-4ee2-bb45-4b90e038405b)





## Task 2: Linking Verilator simulation with Vbuddy

### Aim: Modify testbench to interface with Vbuddy board, so the counter runs on the Vbuddy (vbdSetMode(0))

![Uploading image.png…]()





## Task 3: Vbuddy parameter & flag in one-shot mode

### Aim: Making the counter increment only when the encoder is pressed



## Task 4



# Lab 2



# Lab 3 



# Lab 4
