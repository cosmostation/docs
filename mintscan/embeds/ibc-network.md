---
description: To embed ibc-network, simply insert the iframe code. 😊
---

# IBC Network

## 1. Usage&#x20;

{% code lineNumbers="true" %}
```html
<iframe
    src="https://hub.mintscan.io/chains/ibc-network?embed=true&hide-ui=true"
    width="1200px"
    height="600px"
></iframe>
```
{% endcode %}

The embedded ibc-network fills the given iframe area.



## 2. Examples

### 2.1 Without UI

{% code lineNumbers="true" %}
```html
<iframe
    src="https://hub.mintscan.io/chains/ibc-network?embed=true&hide-ui=true"
    width="1200px"
    height="600px"
></iframe>
```
{% endcode %}

<figure><img src="../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

### 2.2 With UI

{% code lineNumbers="true" %}
```html
<iframe
    src="https://hub.mintscan.io/chains/ibc-network?embed=true"
    width="1200px"
    height="600px"
></iframe>
```
{% endcode %}

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>



### 2.3 Focus on a specific chain

{% code lineNumbers="true" %}
```html
<iframe
    src="https://hub.mintscan.io/chains/ibc-network?embed=true&c=cosmos"
    width="1200px"
    height="600px"
></iframe>
```
{% endcode %}



<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>



## 3. Options

| Key     | Value         | Required | Description                                                                                                                              |
| ------- | ------------- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| embed   | true          | yes      | Should be set to true when using iframe.                                                                                                 |
| hide-ui | true \| false | no       | <p>Show or hide the ui <br><em><mark style="color:red;">* If the width of the iframe is 1080px, the ui is not displayed.</mark></em></p> |
| c       | string        | no       | <p>chain name<br><em>ex) cosmos, osmosis</em></p>                                                                                        |



## 4. Codepen Example

{% embed url="https://codepen.io/hyunwoo-the-flexboxer/pen/PoBKgzw" %}











