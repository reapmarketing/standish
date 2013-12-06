---
'layout': 'default'
'title': 'HubSpot'
---

## HubSpot integration

HubSpot is integrated directly into the Theme. To add HubSpot forms to the site, a few changes need to made to the embed code.

[The documentation for hbspt.forms.create()](https://developers.hubspot.com/docs/methods/forms/advanced_form_options)

**Removed**: HubSpot JavaScript

	<script charset="utf-8" src="//js.hsforms.net/forms/current.js"></script>

The forms JavaScript is already included by the template.

**Added**: Option to include no styles

	, css: ''

(Don't forget to fix the commas)

This stops the HubSpot form from importing its own styles, which will mess up our custom styles, the footer form, and any modal forms.

### Example

#### Modified Code

	<script>
		hbspt.forms.create({ 
			portalId: '239485',
			formId: 'e1c82df0-cb33-4f66-8f8c-3f6b78660f60',
			css: ''
		});
	</script>

#### Original Code

	<script charset="utf-8" src="//js.hsforms.net/forms/current.js"></script>
	<script>
		hbspt.forms.create({ 
			portalId: '239485',
			formId: 'e1c82df0-cb33-4f66-8f8c-3f6b78660f60'
		});
	</script>
