---
layout: default
title: File Handling 
---

<p1>File Creation</p1>
![image](https://user-images.githubusercontent.com/68385109/226173011-67168e26-44b5-45cc-a5ce-9db6e1c58384.png)
![image](https://user-images.githubusercontent.com/68385109/226174212-aa065120-f9af-4920-be34-ad34b43744f4.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "file = open(&#039;newTextFile.txt&#039;,&#039;w&#039;)\n" +
    "story = &quot;Once apon a time...&quot;\n" +
    "story += (&quot;There lived a princess.&quot;)\n" +
    "file.write(story)\n" +
    "file.close()";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 10,
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



<h1>Append and Reading Basic:</h1>
![image](https://user-images.githubusercontent.com/68385109/216831359-834578ab-7336-4f96-a933-568387c2ebd4.png)
![image](https://user-images.githubusercontent.com/68385109/216831445-9fe8a4ae-fc24-4009-a317-7ee7ed8a3ba3.png)

<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "# Append to File\n" +
    "file = open(&#039;newTextFile.txt&#039;,&#039;a&#039;)\n" +
    "file.write(&quot;\nThis will be added to the end of the existing file.&quot;)\n" +
    "file.close()\n" +
    "#Read File\n" +
    "file = open(&quot;newTextFile.txt&quot;, &quot;r&quot;)\n" +
    "print (file.read())\n" +
    "file.close()";
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


<h1>Append and Reading 2:</h1>
![image](https://user-images.githubusercontent.com/68385109/226175413-eb89d1df-903e-40dc-8bc2-de484eda93b1.png)

![image](https://user-images.githubusercontent.com/68385109/226175407-07af0f0d-d890-44ee-b87c-2d0860eb883c.png)

<div id="3-sortableTrash" class="sortable-code"></div> 
<div id="3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "guardian = input(&quot;Enter a scary monster: &quot;)\n" +
    "file = open(&#039;newTextFile.txt&#039;,&#039;a&#039;)\n" +
    "file.write(&quot;Who lived in a castle which was guarded by a terrifying &quot;+ guardian+&quot;.....\n\n&quot;)\n" +
    "file.write(&quot;Some time has passed after the intro.... \n\n ...after the rescue. The handsome programmer was kissed by the Princess. They were to be married, but the handsome programmer has anoter love... their computer. \n&quot;)\n" +
    "file.write(&quot;We put an close to this file for now. Maybe the programmer can open the file up again in another chapter.&quot;)\n" +
    "file.close() # file close for appending\n" +
    "file = open(&quot;newTextFile.txt&quot;, &quot;r&quot;)\n" +
    "print (file.read())\n" +
    "file.close()# file close for reading\n" +
    "magicSpells = (&quot;Fireball&quot;, &quot;Thunderbolt&quot;, &quot;Water Ball&quot;) #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "3-sortable",
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
  $("#3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#3-feedbackLink").click(function(event){ 
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
