### The way to copy text from https://loigiaihay.com/vocabulary-phan-tu-vung-unit-3-tieng-anh-9-moi-c141a28696.html

1. Right-click and select `Inspect`

![image](https://github.com/johnhf804/emily-tricks/assets/141122408/851d89b7-4d82-478b-ba84-a3c34dae8bf5)

2. Select tab `Console`, copy and paste below code then press `Enter`

```javascript
var jqry = document.createElement('script');
jqry.src = "https://code.jquery.com/jquery-3.3.1.min.js";
document.getElementsByTagName('head')[0].appendChild(jqry);
jQuery.noConflict()

const data = []
$('.block-vocabulary').each(function () {
	const no = this.innerText.split('.')[0]
	let txt = `${no}. `
	const yellowBlock = $(this).find('.voca-left')[0]
	const firstBlock = $(this).find('.voca-word')[0]

	const keyWord = $(firstBlock).children()[0].innerText
	const fullText = firstBlock.innerText
	const s2 = fullText.substr(keyWord.length).trim()

	txt += `<b>${keyWord}</b> ${s2}`

	const ls = $(yellowBlock).find('p')
	txt += `\n<br\>${ls[1].innerText}`
	txt += `\n<br\>${ls[2].innerText}`
	txt += `\n<br\>${ls[3].innerText}`

	data.push(txt)
})
console.log(data.join('\n\n <br\><br\>'))
```

![image](https://github.com/johnhf804/emily-tricks/assets/141122408/c6810fae-aff4-4874-a83a-0d7a4067ba37)

3. Copy output text (when text is too long, you can click `copy`)
![image](https://github.com/johnhf804/emily-tricks/assets/141122408/4c2dffc4-c336-456c-b697-ed6148354e2e)

4. Go to https://codebeautify.org/htmlviewer
- patse this text to left cell and press `Run/View`

![image](https://github.com/johnhf804/emily-tricks/assets/141122408/19fc617e-f930-4fa1-9262-0a910c000f7a)


5. Copy text in right cell and paste it to Word
