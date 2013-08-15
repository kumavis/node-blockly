#Node-Blockly
###The Blockly Core, ready to Browserify in the Node.js style.

see the [original repo on google code](https://code.google.com/p/blockly/) for more information

First just install:

    npm install blockly

Then you can require it in your project:

    var Blockly = require('blockly');

Now you're ready to call functions like you normally would to Blockly:

      Blockly.Language.text_length = {
      category: 'Text',
      helpUrl: 'http://www.w3schools.com/jsref/jsref_length_string.asp',
      init: function() {
        this.setColour(160);
        this.appendValueInput('VALUE')
            .setCheck('String')
            .appendTitle('length');
        this.setOutput(true, 'Number');
        this.setTooltip('Returns number of letters in the provided text.');
      }
    };  