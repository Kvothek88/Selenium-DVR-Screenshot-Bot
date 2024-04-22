I was working as an electrical engineer for a company that constructed and maintained photovoltaic plants across Greece. In the monitoring department there was a periodic check of all the plants' cctv carried out by an engineer, so I automated this process through a python script using the Selenium library. This script auto-logins to the DVR, hits the play button and captures a Screenshot of the camera grid. All these are done by finding the relevant html element using the XPATH method. Besides capturing the camera grid I wrote a function which understands which cameras aren't working. Additionally the script understands if a plant is offline. The script constructs 3 excel files, one that keeps track of which plants are captured so if you stop the program and run it again it will continue from where it left by converting the excel into a python list, a second excel which archives the offline plants and a third one which archives the cameras' status meaning which cameras don't work properly. The 3 excels along with the screenshots are stored in a file directly under the main.py path which is created at the start of the program (if it doesn't exist) and it has today's date.