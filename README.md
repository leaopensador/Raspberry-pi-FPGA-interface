# Raspberry-pi-FPGA-interface
In this repository, applications of Raspberry pi (RPi) and FPGA interface are under progress. RPi acts as a web server which taken user inputs and displays outputs via web browser. Towards the FPGA end, the RPi also configures the FPGA using JTAG communication with bit files and opens additional communication channels, eg SPI, I2C, etc. 

As a first application, I am extending my previous FPGA sevquencer git, https://github.com/mdnoaman/fpga_sequencer. In this git, the software side interface is provided on a web server using AJAX and PHP. The RPi runs any basic OS, in this case, headless Raspbian. Using SSH, all the desired controls are accessed. Apache webserver is installed and set. The files in the git are placed in the /var/www/html folder in the RPi.

To get a rough idea, a screenshot "web_app.png" is included in the folder. The different configuration inputs are enterd and uploaded to the server with a set of different options. For example, FPGA configuration file is loaded to the FPGA by assigning the name of the .bit file. The files can be stored on the RPi separately to have faster communication. The other parts shown in the screenshot displays a basic layout of a sequence generator. Complex structures can easily be added. At the moment, the software side interface is completed. By clicking "Load seqeunce" button, the settings are stored in a file named "setting.txt" placed in the RPi.

The progress is ongoing to eshtablish SPI communication with FPGA to transfer all text file data.
