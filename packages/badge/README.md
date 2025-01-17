# Badge

![npm (scoped)](https://img.shields.io/npm/v/@leafygreen-ui/badge.svg)

## Example

```Javascript
import Badge from '@leafygreen-ui/badge';

<Badge variant='blue' className='my-badge'>
  New
</Badge>
```

**Output HTML**

```HTML
  <div class="leafygreen-ui-rhgfxf my-badge">New</div>
```

## Properties

### variant

**Type:** `string`

**Default:** `'lightgray'`

Sets the style variant of the badge. Valid variants for badges are `'lightgray'`, `'darkgray'`, `'red'`, `'blue'`, `'green'`, and `'yellow'`

### className

**Type:** `string`

**Default:** `''`

Adds a className to the class attribute.

### children

**Type:** `node`

**Default:** `null`

The content that will appear inside of the `<Badge />` component.

#### Any other properties will be spread on the root element.

Note: Specifying the `onClick` attribute will change the cursor style to pointer.
