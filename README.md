---
title: custom_card_imswel_person
hide:
  - toc
---
<!-- markdownlint-disable MD046 -->

# Custom-card "Person"

This is a `custom-card` that improves the original person card (`card_person`) by adding a pop-up window inspired by  the theme of [@matt8707](https://github.com/matt8707/hass-config)

![Generic](/docs/img/popup.gif)

## Credits

Author: imswel - 2021
Version: 1.0.0

## Changelog

<details>
	<summary>1.0.0</summary>
	Initial release
</details>

## Requirements

This card needs the following to function correctly:
<table>
	<tr>
		<th>Component / card</th>
		<th>required</th>
	</tr>
	<tr>
		<td><a href="https://github.com/thomasloven/lovelace-card-mod">lovelace-card-mod</a></td>
		<td>yes</td>
	</tr>
</table>

## Usage

```yaml
- type: "custom:button-card"
  template: custom_card_imswel_person
  variables:
    ulm_card_imswel_person_entity: person.username
    ulm_card_imswel_person_wifi_tracker: device_tracker.wifi_oneplus_6t
    ulm_card_imswel_person_gps_tracker: device_tracker.oneplus_6t
    ulm_card_imswel_person_findmy_script: script.find_my_oneplus_6t
    ulm_card_imswel_person_use_entity_picture: true
    ulm_card_imswel_person_zone1: Work
    ulm_card_imswel_person_zone2: School
```

#### Variables

<table>
	<tr>
		<th>Variable</th>
		<th>Example</th>
		<th>Required</th>
		<th>Default</th>
		<th>Explanation</th>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_entity</td>
		<td> person.username</td>
		<td>yes</td>
		<td></td>
		<td>The person entity</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_wifi_tracker</td>
		<td>device_tracker.wifi_oneplus_6t</td>
		<td>yes</td>
		<td></td>
		<td>A device_tracker entity of the person based on wifi</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_gps_tracker</td>
		<td>device_tracker.oneplus_6t</td>
		<td>yes</td>
		<td></td>
		<td>A device_tracker entity of the person based on location</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_findmy_script</td>
		<td>script.find_my_oneplus_6t</td>
		<td>yes</td>
		<td></td>
		<td>A script entity that make ring your phone</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_use_entity_picture</td>
		<td>true or false</td>
		<td>no</td>
		<td>false</td>
		<td>If true, shows the entity picture from your user instead of the icon</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_zone1</td>
		<td>Work</td>
		<td>no</td>
		<td></td>
		<td>Set another zone (beside "home") to use for the card. You can set up two zones besides "home".</td>
	</tr>
	<tr>
		<td>ulm_card_imswel_person_zone2</td>
		<td>School</td>
		<td>no</td>
		<td></td>
		<td>Set another zone (beside "home") to use for the card. You can set up two zones besides "home".</td>
	</tr>
</table>