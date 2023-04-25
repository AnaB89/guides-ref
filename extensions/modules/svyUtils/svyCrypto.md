# API Documemtation
**svyCrypto** is a set of utility methods that can easily enable encryption to any Servoy project.  It uses a combination of AES/DES algorithms for this purpose.  

**Example**


    //Create your own internal AES key to be used:

    var INTERNAL_KEY_AES_128 = "Your Unique Key";

    // First create options to initialize and set the internal key if you haven't done so already.
    var options = scopes.svyCrypto.createOptions();
    options.setKey(INTERNAL_KEY_AES_128);

    // ENCRYPT DATA:
    //execute the encrypt function and pass in your desired raw value to be encrypted. 
    //This will return a new encrypted string.
    scopes.svyCrypto.encrypt(rawValue, options);

    // DECRYPT DATA:
    
    //or execute the decrypt function and pass in your encrypted value to be deciphered. 
    //This will return a decrypted string.
    scopes.svyCrypto.decrypt(encryptedString, options);

***

# svyCrypto
A single scope that contains all the functionality

## Method Summary
### encrypt 
**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | value | value to be encrypted | Required
EncryptionOptions | options | encryption options | optional
String | secretPassPhrase | Secret Pass Phrase | optional



**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

## Method Summary
### decrypt 
**Params**

Type | Name | Summary | Required
--- | --- | --- | ---
String | value | encrypted value | Required
EncryptionOptions | options | encryption options | optional
String | secretPassPhrase | Secret Pass Phrase | optional


**Returns** [String](https://wiki.servoy.com/display/DOCS/String)

## Method Summary
### createOptions 

**Returns** EncryptionOptions
