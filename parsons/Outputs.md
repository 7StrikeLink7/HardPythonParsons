---
layout: default
title: Outputs
---
<h1> Cup of Tea </h1>
![image](https://user-images.githubusercontent.com/68385109/226185060-b6ef37b3-cc57-42a6-95b5-b215153d4438.png)
![image](https://user-images.githubusercontent.com/68385109/226185187-36611b34-b432-47e4-a4ee-6f1b599c3d9c.png)
<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;First, boil the water.&quot;)\n" +
    "print(&quot;Secondly, grab your favourite cup, a teabag, and some sugar.&quot;)\n" +
    "print(&quot;Put the teabag in the cup, and two teaspoons of sugar.&quot;)\n" +
    "print(&quot;After the water has boiled, pour the water into the cup until it is almost full. Leaving space for milk.&quot;)\n" +
    "print(&quot;Squeeze and take out the teabag, and pour in milk, and stir.&quot;)\n" +
    "print(&quot;Lastly, enjoy your cup of tea.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 0,
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
