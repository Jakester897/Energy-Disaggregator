# Energy-Disaggregator
Website/GUI for Energy Disaggregation

The objective of this project is to provide a way for end users to visualize the data that is disaggregated via our neural network.

App menu structure

Upon startup, goes to Dashboard if devices are set up, else goes to Setup.
(Devices are saved locally - no login or account needed)

Top menu buttons - accessible from anywhere
-Dashboard --- Data --- Settings-

******
Setup
******
Walks through process of synchronizing device to the app

This section needs to be fleshed out more

**********
Dashboard
**********
Displays graphs with selector buttons as in Andrew's sketch
+ button below selectors to display new quantity -> shortcuts to appropraite Data menu section
+ button below graphs to add a new graph to the dashboard
	-Line graph and pie chart option
		-Pie chart is based on per-device estimates from data. Line graphs can have custom quantities
Press and hold a selector or graph to switch to delete mode.
	-Red X appears in corner of elements.
	-Back button replaces top menu buttons.

*****
Data
*****
Displays last n seconds of data obtained every p period
	-n and p have a reasonable default. Can be changed from settings menu.
First two rows are raw total voltage and current measurements
Next rows are per-device estimates
New rows can be added for new quanitities that are functions of existing ones (spreadsheet style with some limitations?)
Hold cells in first column of each row to add a quanitity to a graph on the dashboard

*********
Settings
*********
-Manage devices
	-Set up a new devices -> Setup screen
	-Switch devices (app will only pay attention to one at a time, but save tensors for each)
-Tweaks and appearance
	-changes color scheme (e.g. dark mode) and font
-Data settings
	-Change displayed number of data points and data period
	-Toggle advanced mode (displays raw data)
		-Advanced setting: Machine learning parameters
-Dashboard
	-Change length of press needed for delete mode
	-Change method of toggling delete mode
	-Toggle multiple selections for line graphs (to display multiple quantities on the same graph)
-About
	-Display information about the app
