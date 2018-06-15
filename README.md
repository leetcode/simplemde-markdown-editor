# SimpleMDE - Markdown Editor (With Mentions)

Based on [sparksuite/simplemde-markdown-editor](https://github.com/sparksuite/simplemde-markdown-editor)

```JavaScript
var md = new SimpleMDE(
{ 
    element: document.getElementById("MyID"),
    autoSuggest: 
    {
        mode: 'markdown',
        startChars: ['@', '#'],
        listCallback: function(stringToTest)
        {
            return [
                    {
                        text: 'Thomas ',
                        displayText: 'Thomas'
                    },
                    {
                        text: 'Maria ',
                        displayText: 'Maria'
                    },
                    {
                        text: 'Peter ',
                        displayText: 'Peter'
                    }
                ];
        }
    }
});
```