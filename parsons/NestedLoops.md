---
layout: default
title: Nested Loops: Reversing strings
---


![image](https://user-images.githubusercontent.com/68385109/226176381-ce385f00-26d0-4e7f-8cc4-561104227159.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "run = &quot;True&quot;\n" +
    "while (run != &quot;&quot;):\n" +
    "  run = input(&quot;I can reverse any word you enter: &quot;)\n" +
    "  reverseWord = &quot;&quot; \n" +
    "  for i in range(len(run), 0, -1):\n" +
    "   reverseWord += run[i-1]\n" +
    "  print(reverseWord)";
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

![image](https://user-images.githubusercontent.com/68385109/216830541-e6e4b465-7eab-4705-8750-339fec0948bd.png)

![image](https://user-images.githubusercontent.com/68385109/216830477-526c1c28-bb21-4ed4-a693-9a61724f719a.png)
<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#These are arrays that can hold more than one value. If a variable is like a box, an array is a row of boxes.\n" +
    "students = [ &quot;John&quot;, &quot;Bill&quot;, &quot;Pete&quot;, &quot;Dave&quot; ]\n" +
    "subjects = [ &quot;English&quot;, &quot;Music&quot;, &quot;Computer Science&quot;, &quot;Art&quot; ]\n" +
    "#Output all students with all subjects. x student is good at x subject\n" +
    "for student in students:\n" +
    "  for subject in subjects:\n" +
    "        print(student + &quot; is good at &quot; + subject)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#1-feedbackLink").click(function(event){ 
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
