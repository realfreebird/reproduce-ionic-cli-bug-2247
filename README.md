# Use this repository to reproduce ionic-cli bug #2247
https://github.com/driftyco/ionic-cli/issues/2247


Search for "reproduce_ionic_cli_bug_2247" here:<br>
https://github.com/realfreebird/reproduce-ionic-cli-bug-2247/commit/d0da52655a701ad004fcf11a44761fe01d65c70e

The problem is related to watching non-existing files. <br>
Just comment out the following code, and everything works just fine. <br>
<br>
<pre>
  reproduce_ionic_cli_bug_2247: {
     src: ['{{ROOT}}/node_modules/non_exiting_file.txt'],
     dest: '{{BUILD}}'
   }
 </pre>
