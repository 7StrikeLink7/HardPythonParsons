---
layout: default
title: Selection – IF Else statements - Test Score

---

![image](https://user-images.githubusercontent.com/68385109/226179172-6a12eaf0-bebf-44f3-a481-286f0932626e.png)
![image](https://user-images.githubusercontent.com/68385109/226179328-a28fc6b1-74d2-48e6-89c5-210cfe3f893c.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "testScore = int(input(&quot;You just had a test. What did you score out of a hundred? &quot;))\n" +
    "if (testScore == 0):\n" +
    "  print(&quot;I am sure there is a good reason for this.&quot;)\n" +
    "elif (testScore &lt; 0 or testScore &gt; 100):\n" +
    "  print(&quot;That\&#039;s not right...&quot;)\n" +
    "elif (testScore &lt; 50):\n" +
    "  print(&quot;Well done. It was a hard test.&quot;)\n" +
    "    \n" +
    "elif (testScore &gt;= 50):\n" +
    "  print(&quot;Congrats! You have done very well!&quot;)\n" +
    "else: \n" +
    "  print(&quot;Sorry. I wanted a number.&quot;)\n" +
    "  \n" +
    "IF play = &quot;y&quot;: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
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
