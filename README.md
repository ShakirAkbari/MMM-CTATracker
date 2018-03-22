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

## Configuration options

The following properties can be configured:


<table width="100%">
		<tr>
			<th>Option</th>
			<th width="100%">Description</th>
		</tr>
		<tr>
			<td><code>url</code></td>
			<td>the URL in the iFrame<br>
				<br><b>Example:</b><code>"http:http://example.com/" </code>
				<br><b>Default value:</b> <code>''</code>
			</td>
		</tr>
		<tr>
			<td><code>width</code></td>
			<td>the width of the iFrame<br>
				<br><b>Example:</b><code>"100%"</code>
				<br><b>Example:</b><code>"200px"</code>
				<br><b>Default value:</b> <code>"100%"</code>
			</td>
		</tr>
		<tr>
			<td><code>height</code></td>
			<td>the width of the iFrame<br>
				<br><b>Example:</b><code>"100%"</code>
				<br><b>Example:</b><code>"300px"</code>
				<br><b>Default value:</b> <code>"100px"</code>
			</td>
		</tr>
</table>
