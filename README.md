# JqueryCountryCodePickerPlugin
A simple jquery plugin that displays a beautiful list of all the countries allowing the user to pick the country he wishes and provide details like country code and flag.

### Prerequisites
* jQuery

## Installation steps
Follow the below steps to install and set up the plugin.

**Step 1: Clone the Repository**<br>
You can download the ZIP file or git clone from my repo into your project directory.

**Step 2: Configure the Plugin**<br>
After you clone the repo in to your project folder the project need to be set up by following

- Include jQuery library and also ccpplugin at the end of your html page.

```
<script src="http://code.jquery.com/jquery-2.2.3.min.js" type="text/javascript"/>
<script src="ccpplugin.js" type="text/javascript"/>

```

- Initialise plugin and specify the target phonenumber input field.

```
<script>
    	$(document).ready(function(){
    		$('.listCountries').phonecode({
                        setClass:'phonecode'
    		});
    	});
</script>

<div class="form-group">
        <label>Country:</label>
        <select class="listCountries form-control"/>
        <label>Phone Code:</label>
        <input type="tel" class="phonecode form-control"/>
</div>
```
## For more config options with default values.

#### setClass - Class of input field
* Type: String
* Default: null

#### setBgColor - background color of setClass
* Type: String
* Default: white

#### setFontColor - font color of setClass
* Type: String
* Default: black

#### setPrefix - show phonecode prefix
* Type: Boolean
* Default: true

#### Usage example

```
<script>
    	$(document).ready(function(){
    		$('.listCountries').phonecode({
                        setClass:'phonecode'
                        setBgColor:'white',
                        setFontColor:'black',
                        setPrefix:true
            });
    	});
</script>
```

### Credits
* Built on top of [jQuery Plugin To Auto Set Country Calling Codes - phonecode](https://www.jqueryscript.net/form/jQuery-Plugin-To-Auto-Set-Country-Calling-Codes-phonecode.html)
* Original country api from [CountryCodePickerApi](https://github.com/adenuga558/CountryCodePickerApi)


### License
The JqueryCountryCodePickerPlugin is open-sourced software licensed under the [GNU General Public License](http://www.gnu.org/licenses)

