# LPC21ISP

ISP Programmer for LPC Controllers.
** This version is as branch of the original LPC21ISP code and is modified to use with LNLS' BPM electronics, be careful when using for other purposes **

## Usage

Connect an USB cable to the controller serial port (use an external USB-Serial converter if not available in hardware)

Program a binary file:

    ./lpc21isp -control -bin <Path to Bin> <Serial Port> <Serial Speed> <Controller clock frequency in KHz>

Example:

    ./lpc21isp -control -bin rffe-uc-fw.bin /dev/ttyUSB0 230400 12000

If a memory wipe is needed before programming, add the `-wipe` flag to the command
