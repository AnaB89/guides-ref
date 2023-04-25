#  WEBCONSTANTS

## **Supported Clients**

    WebClient

## Constants Summary

| Type                                                  | Name                                          | Summary                                                          |
| ----------------------------------------------------- | --------------------------------------------- | ---------------------------------------------------------------- |
| [String](../JSLib/String.md) | [WEBCLIENT_TEMPLATES_DIR](WEBCONSTANTS.md#WEBCLIENT_TEMPLATES_DIR)                   | Property that can be set using application..                                    |

## Constants Details

### WEBCLIENT_TEMPLATES_DIR

Property that can be set using application.putClientProperty(), it sets the servoy_web_client_default.css location directory in the templates dir for this client

**Returns**\
[String](../JSLib/String.md) 

**Supported Clients**\
WebClient

**Sample**

```javascript
// set this if you want to set the css path to the servoy_web_client_default.css file that you can specify per client
// by default this file resides in '/servoy-webclient/templates/default/servoy_web_client_default.css'
// and you will override the 'default' in that url so setting it to myclient1 will result in:
// by default this file resides in '/servoy-webclient/templates/myclient1/servoy_web_client_default.css'
application.putClientProperty(APP_WEB_PROPERTY.WEBCLIENT_TEMPLATES_DIR, 'myclient1');
```

