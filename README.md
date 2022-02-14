# CKEditor 5 editor generated with the online builder for React & Next JS

# First add Import
import CKEditor from ('@ckeditor/ckeditor5-react')

Import CustomBalloonEditor from ('ckeditor5-custom-build-with-balloon-editor')

# Add Component like this
```javascript

	<CKEditor
					editor={CustomBalloonEditor}
					data="<p>Type Your Text</p>"
					onInit={(editor) => {
						// You can store the "editor" and use when it is needed.
					}}
					onChange={(event, editor) => {
						const data = editor.getData();
						setEditData(data);
					}}
					config={{	toolbar: {
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