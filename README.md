# This is a work in progress and does not work at the moment
# 
# 
# 
# 
# 
# 
# 

# MMM-CTATracker
A Magic Mirror module (MMM) whose purpose is to retrieve bus arrival in Chicago using the CTA API

This module has been built off the newfeed module built into Magic Mirror (https://github.com/MichMich/MagicMirror)

To use this module, add it to the modules array in the `config/config.js` file:
````javascript
modules: [
			{
			module: "MMM-CTATracker",
			position: "bottom_bar",
			config: {
				feeds: [
					{
						title: "Bus Number",
						url: "http://www.ctabustracker.com/bustime/api/v1/getpredictions?key=YOUR_CTA_API_KEY_GOES_HERE&stpid=730"
					}
				],
				showSourceTitle: true,
				showPublishDate: true
			}
		},
]
````
