# SimpleMDE - Markdown Editor (With Mentions)

Based on [sparksuite/simplemde-markdown-editor](https://github.com/sparksuite/simplemde-markdown-editor)

```JavaScript
var md = new SimpleMDE(
{ 
    element: document.getElementById("MyID"),
    autoSuggest: 
    {
        mode: 'markdown',
        triggers: {
            '@': function(stringToTest) {
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
            },
            '#': function(stringToTest) {
                return [
                    {
                        text: 'Two Sum ',
                        displayText: 'Two Sum'
                    },
                    {
                        text: '3Sum ',
                        displayText: '3Sum'
                    },
                    {
                        text: '4Sum ',
                        displayText: '4Sum'
                    }
                ];
            }
        },
    },
});
```