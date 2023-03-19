---
layout: default
title: Selection – If statements - New Password 
---


![image](https://user-images.githubusercontent.com/68385109/226180749-f01b4b38-8889-4bb5-95c7-26b6abcd5ed6.png)
![image](https://user-images.githubusercontent.com/68385109/226180861-817e2057-64fe-407d-9201-b866f127e66d.png)
![image](https://user-images.githubusercontent.com/68385109/226180893-cf825cc3-c0e1-48d3-80ee-625e8e79b6c7.png)
![image](https://user-images.githubusercontent.com/68385109/226180916-8c274c49-4b7d-4add-add9-209c1e67cec7.png)

<h2> Beware, 2 lines do not belong. You do not need to use all the lines.</h2>
<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "newPassword = input(&quot;Enter your new password: &quot;)\n" +
    "if (len(newPassword) &lt; 7):\n" +
    "  print(&quot;That is too short! &quot;)\n" +
    "if (len(newPassword) &gt; 15):\n" +
    "    print(&quot;That is too long! &quot;)\n" +
    "iF (newPassword &lt; 7): #distractor\n" +
    "if {len[newPassword} &gt; 15]: #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 2,
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
