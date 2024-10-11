# Hide Specific Property

[Hide Specific Property](../snippet/hide-specific-property.css) allows you to hide specific ***frontmatter*** properties.

## Usage

To hide properties, you need to add the following to the ***frontmatter***:

```yaml
cssclasses:
  - hide-specific-property
```

## Adding a Property to Hide

To hide the ***frontmatter*** property you need, follow these steps:

1. Copy the following block:
    ```css
    .metadata-property[data-property-key="<property-name>"] {
        display: none;
    } 
    ```
2. Paste it into the `.markdown-reading-view .hide-specific-property` block between the curly braces.
3. Replace `<property-name>` with the name of the property you want to hide.
4. Save the changes.
5. ...
6. Profit

For example, if you have a property named `custom`, after following the steps above, you will get the following code:

```css
.markdown-reading-view .hide-specific-property {

    /* hide cssclasses */
    .metadata-property[data-property-key="cssclasses"] {
        display: none;
    }

    .metadata-property[data-property-key="custom"] {
        display: none;
    }

}
```