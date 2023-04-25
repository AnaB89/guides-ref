#  spellcheck

## **Return Types**
[LANGUAGES](./LANGUAGES.md),
## **Supported Clients**

    SmartClient

## Methods Summary

| Type                                                  | Name                    | Summary                                                                                                           |
| ----------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------------------------------- |
|void | [checkTextComponent(textComponent)](spellcheck.md#checktextcomponent-textcomponent)                   | Spellcheck the form element/component..                                    |
|void | [checkTextComponent(textComponent, language)](spellcheck.md#checktextcomponent-textcomponent-language)                   | Spellcheck the form element/component..                                    |

## Methods Details

### checkTextComponent(textComponent)

Spellcheck the form element/component.

**Parameters**\
[Object](../../JSLib/Object.md) textComponent  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// The desired spellcheck provider and language are set via the SpellCheck Preference Page, in the Client Preferences.
// Spellchecking currently works in SmartClient only.
plugins.spellcheck.checkTextComponent(forms.actionDetails.elements.actionText);
// Optionally, the language can be sent as an argument to the function.
// The language string is provided from the language constants class, as in the sample below
// NOTE: the optional language, if provided, overrides the Preference Panel page setting, of the current SpellCheck provider (RapidSpell/Google).
// plugins.spellcheck.checkTextComponent(textInDutch, SpellCheck_Languages.DUTCH);
```
### checkTextComponent(textComponent, language)

Spellcheck the form element/component.

**Parameters**\
[Object](../../JSLib/Object.md) textComponent  ;\
[String](../../JSLib/String.md) language  ;

**Returns**\
void 

**Supported Clients**\
SmartClient

**Sample**

```javascript
// The desired spellcheck provider and language are set via the SpellCheck Preference Page, in the Client Preferences.
// Spellchecking currently works in SmartClient only.
plugins.spellcheck.checkTextComponent(forms.actionDetails.elements.actionText);
// Optionally, the language can be sent as an argument to the function.
// The language string is provided from the language constants class, as in the sample below
// NOTE: the optional language, if provided, overrides the Preference Panel page setting, of the current SpellCheck provider (RapidSpell/Google).
// plugins.spellcheck.checkTextComponent(textInDutch, SpellCheck_Languages.DUTCH);
```

