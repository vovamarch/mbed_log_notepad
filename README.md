# mbed_log_notepad

View colored mbed serial logs in Notepad++ and easily isolate debug, error, warning and info messages.

## Overview
[Notepad++ source code editor](https://notepad-plus-plus.org/) allows creation of user-defined languages and styles. This project contains .xml files that can be directly imported into Notepad and used straight away for viewing mbed serial logs with color-coded lines.

In contrast to standard languages (C, Java, PHP,..) Notepad++ doesn't allow much flexibility in styles for user-defined languages. In particular background color can't be set and hence it is recommended to rely on the Global Style. That is why the mbed log language in this project is provided in two styles: darkStyle (for dark/black background)  and lightStyle (for light/white background).

Verified with Notepad++ v7.1. 

###Step 1: Import user defined languages in Notepad++
Import both .xml files (_mbed_log_notepad_lightStyle.xml_ and _mbed_log_notepad_lightStyle.xml_) one after the other using Notepad++ Menu _Language=>Define your language..._ and then clicking on _Import..._ button.

###Step 2: Restart the Notepad++
This step is required to get the imported .xml files correctly listed among supported user defined languages.

###Step 3: Configure Default Global Style
This step specifies the background for the default global style that is applied to all non-standard languages including user defined ones. 

* Open Style Configurator dialog via Notepad++ Menu _Settings=>Style Configurator..._ 
* Select the target theme via _Select Theme_ dropdown menu
* Select _Global Styles_ in the **Languages:** area and _Global override_ in the **Style:** area. Configure the background color and check the _Enable global background color_ item.

###Step 4: View mbed logs in color
Open an mbed log in Notepad++. Then click on Menu item _Language_ and in the dropdown list select _mbed_log_darkStyle_ if you use dark background or m_bed_log_lightStyle_ if you use light background. The view shall be as shown below.


## Customization
It is possible to further customize the styles for the language. This can be done via Notepad++ Menu item Language=>Define your language... dialog and selection of corresponding language in _User language_ item. The main styles are defined in _Operators &Delimiters_ Tab.


