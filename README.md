# CKEditor 5 Balloon Editor for React & NextJS

# Usage

> npm install @ckeditor/ckeditor5-react ckeditor5-custom-build-with-balloon-editor

    import CKEditor from ('@ckeditor/ckeditor5-react')

    import CustomBalloonEditor from ('ckeditor5-custom-build-with-balloon-editor')

# Component Usage

More details please refer https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/frameworks/react.html#component-properties

```javascript


<CKEditor

editor={CustomBalloonEditor}

data="<p>Type Your Text</p>"

onInit={(editor)  =>  {

// You can store the "editor" and use when it is needed.

}}

onChange={(event, editor)  =>  {

const  data  = editor.getData();

setEditData(data);

}}

config={{  toolbar: {

items: [

'heading',

'|',

'bold',

'italic',

'link',

'bulletedList',

'numberedList',

'|',

'|',

'imageUpload',

'blockQuote',

'insertTable',

'mediaEmbed',

'undo',

'redo',

'alignment',

'fontSize',

'highlight'

]

},

language: 'en',

image: {

toolbar: [

'imageTextAlternative',

'imageStyle:full',

'imageStyle:side'

]

},

table: {

contentToolbar: [

'tableColumn',

'tableRow',

'mergeTableCells'

]

}}

/>
```

# Result

![Result Image](https://i.ibb.co/09CzdGV/npm.png)
