If you want to create your own templates used for any of the lookup, you can do that by inheriting from one of the base forms provided. The module features a number of base forms in this hierarchy:

* AbstractLookup 
  - AbstractLookupMulti
     - svyLookupTableMulti
     - svyLookupNGTableMulti
  - svyLookupTable
  - svyLookupNGTable

You can extend the Abstract forms for a fully custom implementation of the UI, while you can extend any of the svy* to customize the given template form.

Extend any of the *Multi form is suitable to implement lookup template for multi selection, while other templates are suitable for single selection.
