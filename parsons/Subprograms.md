---
layout: default
title: Subprograms (Functions and Procedures)
---

![image](https://user-images.githubusercontent.com/68385109/219981525-65c44a99-4375-4156-98a6-23bb77a62f5c.png)
![image](https://user-images.githubusercontent.com/68385109/219981539-3beae822-41b3-4cc9-ab07-d6c0def68340.png)


<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def cubedNumber(number):\n" +
    "  number = int(number ** 3)\n" +
    "  return $$toggle::number::num::cubedNumber$$\n" +
    "print(&quot;2 cubed + 8 = &quot;, cubedNumber(2) + 8)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.VariableCheckGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "0-sortableTrash",
    "vartests": [
        {
            "message": "",
            "initcode": "",
            "code": "",
            "variables": {}
        }
    ]
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


![image](https://user-images.githubusercontent.com/68385109/219982255-931ac115-b0bb-4e76-a2df-99cee98b942c.png)
![image](https://user-images.githubusercontent.com/68385109/219982289-9aaf9e1d-3fd0-4a6a-a850-d142f2e7077c.png)


<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#Declaring turn, counter, target, player1, and player2 in order.\n" +
    "turn = 0\n" +
    "counter = 0\n" +
    "target = 11\n" +
    "player1 = &quot;Alice&quot;\n" +
    "player2 = &quot;Bob&quot;\n" +
    "#procedure for a player to choose a number between 1 and 3, then adds to running total\n" +
    "def playerGo(player):\n" +
    "  global counter\n" +
    "  goUpBy = int(input(player + &quot; Pick a number from 1-3: &quot;))\n" +
    "  if (goUpBy &gt; 0 and goUpBy &lt; 4):\n" +
    "    counter = counter + goUpBy\n" +
    "    print(&quot;Current counter is&quot;, counter)\n" +
    "    if (counter &gt; 10):\n" +
    "      print(player, &quot;loses!&quot;)\n" +
    "  else: #If the user enters an invalid number, call the procedure again.\n" +
    "    playerGo(player)\n" +
    "#Main Program: Call the subprograms, where player 1 and 2 take turns.\n" +
    "print(&quot;Time to play, unlucky&quot;, target,&quot;! First one to reach the unlucky number loses.&quot;)\n" +
    "while (counter &lt; target):\n" +
    "  if turn % 2 == 0:\n" +
    "    playerGo(player1)\n" +
    "  else: \n" +
    "    playerGo(player2)\n" +
    "  turn = turn + 1";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
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
