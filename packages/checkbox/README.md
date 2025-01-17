# Checkbox

![npm (scoped)](https://img.shields.io/npm/v/@leafygreen-ui/checkbox.svg)

## Example

```Javascript
import Checkbox from '@leafygreen-ui/checkbox';

<Checkbox
	className='my-checkbox'
	onChange={(event) => {/* Something to handle the click event */}}
	label='This is how you enable a thing'
	checked={true}
	bold={false}
/>
```

**Output HTML**

```HTML
  <label class="css-1rgbgdt my-checkbox" title="Create an item" for="checkbox-14827892">
		<input
		  checked
			type="checkbox"
			role="checkbox"
			class="css-32kjhsdaf"
			id="checkbox-14827892"
			name="checkbox-14827892"
			aria-disabled="false"
			aria-checked="true"
			aria-labeledby="checkbox-14827892-label"
		/>

		<div class="css-34kjkdfg">
			<div class="css-98sdfjsad"></div>
		</div>

		<span class="css-8xdsjfh9" id="checkbox-14827892-label">
			This is how you enable a thing
		</span>
  </label>
```

## Properties

### variant

**Type:** `string`

**Default:** `'default'`

Sets the style variant of the checkbox. Valid variants for checkboxes are `'default'` and `'light'`.

### checked

**Type:** `boolean`

**Default:** `false`

Checks the checkbox.

### label

**Type:** `node`

**Default:** `null`

The label for the checkbox.

### disabled

**Type:** `boolean`

**Default:** `false`

Disables the checkbox.

### indeterminate

**Type:** `boolean`

**Default:** `false`

Sets the checkbox as indeterminate. **NOTE:** the checkbox will become out of sync with the indeterminate prop when it's clicked. Make sure to unset the `indeterminate` prop on change where you're controlling your input.

### className

**Type:** `string`

**Default:** `''`

Adds a className to the outermost element.

### bold

**Type:** `boolean`

**Default:** `false`

Determines whether the text will be bold or not.

### id

**Type:** `string` || `number`

**Default:** randomly generated string

Adds an ID only to the input, and it's used elsewhere for accessibility props.

### onChange

**Type:** `function`

**Default:** `() => {}`

The event handler function for the 'onchange' event. Receives the associated `event` object as the first argument.

#### Any other properties will be spread on the `input` element.
