# Govee H6127 w/ HA
This project is based on the following page: https://github.com/BeauJBurroughs/Govee-H6127-Reverse-Engineering, my main goal was to integrate my ble led strip into HA.
I used the 'custom:button-card' to show the devices state (on/ off). 

![image](https://user-images.githubusercontent.com/79994912/126362530-12b2ba39-12b7-4a47-be31-951d74842bc5.png)

Since I'm not very experienced in coding this code will probably not be the most optimal solution, however it works. For the dropdown menus I used an input_selector (see configuration.yaml) as well as a Node-Red flow, which checks for any updates from the input_selector. When detected it triggers a 'call service' node which triggers a script, which then sends a shell_command.

![image](https://user-images.githubusercontent.com/79994912/126362501-a80c9b92-0362-4fb0-95da-46adfdfe2f36.png)

To do:
- Add all effects 
- Add working brightness slider to ui
- Add more color options to ui
- Redesign ui card
