TPRG II - PROJECT2

Project Overview
In this project, we've built a system that consists of a server and a client. This system enables data to be collected in one program and presented in a user-friendly graphical format through another program. The client program, known as "ClientAWB.py," runs on a Raspberry Pi and collects data, while the server program, "ServerAWB.py," can operate on both Raspberry Pi and PC platforms. The collected data is formatted using JSON, and the server extracts and displays the relevant information through a graphical interface.

Project Structure

Client Program
ClientAWB.py: This Python script is tailored to run exclusively on a Raspberry Pi and is responsible for data collection and formatting. It includes features like gracefully exiting when running on a PC, sampling data at 2-second intervals, and sending 50 iterations of data to the server. The client also collects data from the Raspberry Pi using "vcgencmd" commands and sends it to the server. A simple GUI illustrates the connection status, featuring a Unicode LED symbol and an Exit button. The code is well-documented and includes error-handling mechanisms.

Server Program
ServerAWB.py: The server program is versatile and can run seamlessly on both Raspberry Pi and PC environments. It incorporates a Main guard clause and is executed on the Pi using Thonny. The server creates a user-friendly GUI that displays six values obtained from the JSON data sent by the client. The GUI also includes a Unicode LED that toggles with incoming data and an Exit button for user interaction. Similar to the client, the server code is well-documented and includes error handling.

Client Marking:
Runs on Pi only __/2
2 second intervals for vcgen data __/2
50 iterations of data before exiting gracefully __/2
Used 5 Pi vcgencmd’s __/3
Simple GUI with working Unicode LED __/2
Use of own 'Def' function and achieving float value __/2
No collated data other than system shell __/1
Use of meaningful comments __/3

Server Marking:
Runs on Pi or PC __/2
Use Main Guard clause __/2
Use on Pi as well __/ 1
GUI to show all 6 values __/4
GUI has Unicode LED that toggles with new data __/4
Use of meaningful comments __/3
