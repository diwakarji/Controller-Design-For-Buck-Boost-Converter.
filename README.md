###Controller-Design-For-Buck-Boost-Converter.
#Introduction
A power electronics converter's output voltage may fluctuate in response to changes in the load, the input voltage, or the switching device's duty cycle. A controller is essential to achieving a steady output voltage. The input voltage of PV solar plants varies greatly in many real-world situations, which also causes the output DC voltage to rise, which is highly undesirable.
##Software required
Go to https://in.mathworks.com/products/matlab.html to install the MATLAB software. When installing Matlab software, don't forget to include the Simscape Electricals toolbox.
##Design of PID and Instruction
Vo = (D*Vin)/(1-D);

where Vo=Output voltage, D=duty cycle, Vin=Input Voltage.
By altering the duty cycle of the converter, a buck-boost converter's output voltage can be adjusted. The buck-boost converter's PID controller design makes use of this idea. I've assumed that the reference voltage for this project is -13 volts. Double-clicking the V_ref block of the Buck_boost_coverter_with_PID_controller.slx file will allow you to adjust the reference voltage. Buck_Boost_converter_without_controller.slx contains a buck-boost converter without PID controller tuning. The given parameters are given. Double-click the PID block in the Buck_boost_converter_with_PID_controller.slx file to adjust the PID controller. In the PID dialogue box, click the tune button.
##Reference
https://www.saranathan.ac.in/emagazine/eee/sj/vol1_1/sjeee9.pdf https://in.mathworks.com/help/slcontrol/gs/automated-tuning-of-simulink-pid-controller-block.html
