---
layout: default
title: Variables - Story Time
---
 

![image](https://user-images.githubusercontent.com/68385109/226184677-2732b2c5-bebd-441f-86af-42a084e9d604.png)
![image](https://user-images.githubusercontent.com/68385109/226184805-fbe6951d-e87c-432f-9842-f35b3a39d126.png)

<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "dogName = &quot;Fluffy&quot;\n" +
    "mastersName = &quot;Flan&quot;\n" +
    "print(&quot;There once was a dog called &quot; + dogName + &quot;, who was very loyal to his master called &quot; + mastersName + &quot;.&quot;)\n" +
    "print(mastersName + &quot; goes to work everyday via train.&quot;)\n" +
    "print(dogName + &quot; waited days, weeks, months, and years outside the train station. But his master never came home...&quot;)\n" +
    "print(dogName + &quot; waits outside the trainstation for him everyday.&quot;)\n" +
    "print(&quot;But one day, his Master, &quot; + mastersName +  &quot;, did not come home on time.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 0,
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
