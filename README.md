# [vue-verify](https://www.npmjs.com/package/vue-verify)

> This is a vue component, which is sliding to unlock for login or sign up.
[demo](https://fewbadboy.github.io/vue-verify/)

## Installation

``` bash
npm install vue-verify --save
# or
yarn add vue-verify
```

## Usage
``` xml
<vue-verify :width="width" 
	:height="height" 
	:text="text" 
	:success-text="successText" 
	:background="background" 
	:progress-bar-bg="progressBarBg" 
	:completed-bg="completedBg" 
	:handler-bg="handlerBg" 
	:handler-icon="handlerIcon" 
	:text-size="textSize" 
	:success-icon="successIcon" 
	:circle="getShape"></vue-verify>
```

``` javascript
import Vue from 'vue'
import VueVerify from 'vue-verify'

export default {
  name: 'app',
  components:{
    VueVerify
  }
}
```
## Props

Property|Type|Default|Description
---|---|---|---
width|Number|200|The width of the component
height|Number|60|The height of the component
text|String|swiping to the right side|The text shows on the component
successText|String|success|The text shows when it’s successful
background|String|#ccc|The background color of the component
color|String|#ffffff|The color of the text
progressBarBg|String|#FFFF99|The backgound color of the progress bar
completedBg|String|#66cc66|The backgound color of the component when the button dragged to the right side
circle|Boolean|true|If true, the shape of component is round
handlerIcon|String|-|The icon of handler
successIcon|String|-|The icon of handler when the button dragged to the right side
handlerBg|String|#fff|The background color of the handler
textSize|String|20px|Font size of prompt message


## Event

### success-callback
Emitted when pass verify, the handler dragged to the right side.

