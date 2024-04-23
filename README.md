
ArcGIS Configurable Apps will be retired in 2025. The ArcGIS Configurable Apps source code repro is deprecated and will not receive further updates. In addition, this repository will be removed in October 2025, along with the October 2025 ArcGIS Online update.


Deprecated: legend-template
===============

[View it live](http://www.arcgis.com/apps/PanelsLegend/index.html?webmap=c959f521c02f4f64abf4d39019c5ccd5)

#Features
**Legend** is a configurable application template that enables you to display an ArcGIS web map with a legend, description, and basic map tools. The template can be configured using the following options:
 - **Map:** Choose the web map used in the application. 
 - **Color Scheme:** Choose between four application color schemes (Chrome, Gray, Seaside, Pavement).
 - **Header:** Choose to add a header displaying a title and subtitle.
 - **Title:** The application title. The default title is the web map name.
 - **Subtitle:** Text appearing below the title used to further describe the application. The default subtitle is the web map summary.
 - **Footer:**  Choose to include a footer to display additional information about the application.
 - **Description** Display application details. The default description is the web map item description.
 - **Legend** Display a legend for map layers on the left or right side.*
 - **Optional Widgets** Toggle optional tools and buttons - Full Extent, Location, Search.
 
*These options will appear in the application when the web map has properties or layers that support them.

#Instructions
## Instructions

1. Download and unzip the .zip file or clone the repository.
2. Web-enable the directory.
3. Access the .html page.
4. See the [Configuration Options] (https://github.com/Esri/legend-template/wiki/Configuration-Options) section of the wiki for details on configuring the application. 
5. Start writing your template!

[New to Github? Get started here.](https://github.com/)

## Deploying

1. To deploy this application, download the template from Portal/ArcGIS Online and unzip it.
2. Copy the unzipped folder containing the web app template files, such as index.html, to your web server. You can rename the folder to change the URL through which users will access the application. By default the URL to the app will be `http://<Your Web Server>/<app folder name>/index.html`
3. Change the sharing host, found in defaults.js inside the config folder for the application, to the sharing URL for ArcGIS Online or Portal. For ArcGIS Online users, keep the default value of www.arcgis.com or specify the name of your organization.
  - ArcGIS Online Example:  `"sharinghost": location.protocol + "//" + “<your organization name>.maps.arcgis.com`
  - Portal Example where `arcgis` is the name of the Web Adaptor: `"sharinghost": location.protocol + "//" + "webadaptor.domain.com/arcgis"`
4. If you are using Portal or a local install of the ArcGIS API for JavaScript, change all references to the ArcGIS API for JavaScript in index.html to refer to your local copy of the API. Search for the references containing `"//js.arcgis.com/3.13"` and replace this portion of the reference with the url to your local install.
  - For example: `"//webadaptor.domain.com/arcgis/jsapi/jsapi"` where `arcgis` is the name of your Web Adaptor.
5. Copy a map or group ID from Portal/ArcGIS Online and replace the default web map ID in the application’s default.js file. You can now run the application on your web server or customize the application further.

> **Note:** If your application edits features in a feature service, contains secure services or web maps that aren't shared publicly, or generate requests that exceed 200 characters, you may need to set up and use a proxy page. Common situations where you may exceed the URL length are using complex polygons as input to a task or specifying a spatial reference using well-known text (WKT). For details on installing and configuring a proxy page see [Using the proxy](https://developers.arcgis.com/javascript/jshelp/ags_proxy.html). If you do not have an Internet connection, you will need to access and deploy the ArcGIS API for JavaScript documentation from [developers.arcgis.com](https://developers.arcgis.com/).



#Requirements

- Notepad or HTML editor
- Some background with HTML, CSS and JavaScript
- Experience with the ArcGIS API for JavaScript is helpful. 

#Resources

- [ArcGIS API for JavaScript Resource Center](http://help.arcgis.com/en/webapi/javascript/arcgis/index.html)
- [ArcGIS Online] (http://www.arcgis.com)
- Want to create your own template? View the [Application Boilerplate](https://github.com/Esri/application-boilerplate-js) to get started. 

#Issues
Found a bug or want to request a new feature? Please let us know by submitting an issue. 

#Contributing
Anyone and everyone is welcome to contribute. 

#Licensing 

Copyright 2012 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's license.txt file.
