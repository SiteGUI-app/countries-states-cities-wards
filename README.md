# countries-states-cities-wards
Inaccurate addresses entered by your customers cost your online store money. This repo aims to be the most accurate source for country, state, city and ward lookup through simple API to an edge CDN server near whoever utilizing it. 

Each country has its own folder (country's ISO short name) which contains an index.json file to list all of its states. Each state has a state ID and a state_id.json file containing all of its cities and wards (if wards are available)

The initial database is taken from https://github.com/dr5hn/countries-states-cities-database 

Demo https://sitegui-platform.github.io/countries-states-cities-wards/demo.html

How to use?

Include the following script in your page:

```<script src="https://sitegui-platform.github.io/countries-states-cities-wards/sgaddress.js?v=15" id="sg-js-address" data-source="https://raw.githubusercontent.com/SiteGUI-platform/countries-states-cities-wards/main/"></script>```

Add a wrapper around your address input fields and change data-selector-* to relevant input's ID/class:

```<div class="sg-js-address" data-addr-add="1" data-default-country="VN" data-selector-country="select.billing-country" data-selector-state=".sg-address-state" data-selector-zip=".sg-address-zip" data-selector-city=".sg-address-city-input" data-selector-street2=".sg-address-street2">```
