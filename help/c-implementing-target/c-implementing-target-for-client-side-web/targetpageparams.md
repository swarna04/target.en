---
keywords: targetPageParams;targetpageparams;pageParams;pageparams;page params;page parameters;at.js;functions;function
description: Information about the targetPageParams() function for the Adobe Target at.js JavaScript library.
title: targetPageParams()
feature: at.js
---

# targetPageParams() {#reference_B235C9F6DA79449ABE3E23F914FEABAE}

This method allows you to attach parameters to the global mbox from outside of the request code.

This function is very useful for including the same set of parameters on multiple mbox calls. The function needs to be defined by the customer. It should return an array of parameters that will be passed only to the global mbox request. This function can be defined before at.js is loaded or in **[!UICONTROL Administration]** > **[!UICONTROL Implementation]** > **[!UICONTROL Edit]** > **[!UICONTROL Library Header]**.

You can pass in parameters to target-global-mbox using the `targetPageParams()` function in any of the following ways:

* An ampersand-delimited list 
* An array 
* A JSON object

## Examples

Ampersand-delimited list (values must be URL encoded):

```javascript
function targetPageParams() { 
    return "param1=value1&param2=value2&p3=hello%20world"; 
}
```

Array (values do not need to be URL encoded):

```javascript
targetPageParams = function() { 
     return ["a=1", "b=2", "c=hello world"]; 
};
```

JSON (values do not need to be URL encoded):

```javascript
targetPageParams = function() { 
  return { 
    "a": 1, 
    "b": 2, 
    "profile": { 
        "age": 26, 
        "country": { 
          "city": "San Francisco" 
        } 
      } 
  }; 
};
``` 
