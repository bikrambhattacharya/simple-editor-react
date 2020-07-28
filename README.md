# simple-text-editor-react

> A simple text editor with image upload functionality.
> Working on the documentation.

[![JavaScript Style Guide](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)

## Install

```bash
npm install --save simple-text-editor-react
```

## Usage

```jsx
import React, { Component } from 'react'

import SimpleEditor from 'simple-text-editor-react'

class Example extends Component {
  render() {
    return (
      <SimpleEditor 
      onChange={(value)=>{
        // value contains the html value and all keystroke events 
      }}
      onImageUpload={(image, callback)=>{
        //upload image then return the url in callback
        //callback(url)
      }}
      containerStyle={{
                      width: '100%',
                      height: '100%',
                      border: '1px solid #cec7c7',
                      position: 'relative' // position relative is required if showWordCharCount !== false
      }}
      value={value} //pass initial value
      id={id} // not required but can be useful in some usecases
      showWordCharCount // if true word and character count will be shown. Default value is true
      />
    )
  }
}
```

## License

MIT © [bikrambhattacharya](https://github.com/bikrambhattacharya)
