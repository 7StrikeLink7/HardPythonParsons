---
layout: default
title: Nested If statements Number Guessing Game 2
---
![image](https://user-images.githubusercontent.com/68385109/226178896-5753063b-067a-4172-b295-537718182b1e.png)
![image](https://user-images.githubusercontent.com/68385109/226179002-a2609f91-90e5-40a1-8e41-37d491d64932.png)
![image](https://user-images.githubusercontent.com/68385109/226178977-7d107e04-4681-4ab3-84ad-acbd43063d24.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#The order of the code has been mixed up. Rearrange it so that it makes sense.\n" +
    "import random\n" +
    "luckyNumber = random.randint(1,10)\n" +
    "play = input(&quot;Want to play a game? y/n &quot;)\n" +
    "if (play == &quot;y&quot;):\n" +
    "  guess = int(input(&quot;Guess my number which is between 1 and 10. If you get it right, I will give you £10. &quot;))\n" +
    " \n" +
    "  if (guess == luckyNumber):\n" +
    "    print(&quot;Well done! You guessed my number.&quot;)\n" +
    "    \n" +
    "  else:\n" +
    "     print(&quot;Unlucky. Now you have to pay me £1! The number I was thinking of was&quot;, luckyNumber)\n" +
    "IF play = &quot;y&quot;: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 1,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "0-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#0-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#0-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Topics:
[Outputs](./Outputs.html)
[Variables and Outputs](./Variables.html)
[Variables, Outputs, and Inputs](./Inputs.html)
[Maths Operators (input integers)](./Maths.html)
[Random numbers](./Random.html)
[Strings and Casting](./Casting.html)
[Booleans](./Booleans.html)
[If](./If.html)
[If/Else](./Else.html)
[If/Elif/Else](./Elif.html)
[Nested Ifs](./NestedIf.html)
[For loops](./For.html)
[While loops](./While.html)
[Nested loops](./NestedLoops.html)
[Arrays/Lists](./Arrays.html)
[2D Lists](./2D.html)
[File handling](./Files.html)
[Subprograms(functions/procedures)](./Subprograms.html)
