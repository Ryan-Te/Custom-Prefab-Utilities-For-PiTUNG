# Custom-Builder-Tools
Custom Builder Tools
This Is A Set Of Functions That Make Using The Custom Builder In PiTUNG Alot Eaiser!
Functions:

NOTE: Things Inside [] Are Optional

<This Function Is A Modified Version Of Falsepatterns Function.>
  
createCube(X,[Y]Z)

  This Will Create A Cube Of Size X Y Z, Default For Y is 1
  
  
getPegPos(X,[Y],Z,Side,[OffestX],[Offset Y])

  This Will Turn The Given Cube Size(X,Y,Z) 
  And Output The Position Of A Peg On Side Side And Offset The Peg By Offset X TUNG Grid Spaces Left/Right And Offset Y TUNG Grid Spaces UP/Down
  Default For Y Is 1 and Default For Offset X and Offset Y Are 0
  
  
GetPegQuat(X,[Y],Z,Side)

  This Will Turn The Given Cube Size(X,Y,Z) 
  And Output The Rotation Of A Peg Peg On Side Side
  
  
SIDE TABLE:
  F = Front
  
  B = Back
  
  L = Left
  
  R= Right
  
  T = Top
  

HOW TO USE:
Here Is How To Make A Component Made Using My Tools

The Inital line

  var Test = PrefabBuilder.Custom(() => CBT.createCube(X Size Of Component, [YSize Of Component], Z Size Of Component)
  
  
A Input Peg

  .WithInput(CBT.getPegPos(X Size Of Component, [YSize Of Component], Z Size Of Component, Side Of Peg, [X Offset Of Peg], [Y Offset Of Peg] ),  CBT.getPegQuat(X Size Of Component, [YSize Of Component], Z Size Of Component Side Of Peg),Peg Descripion)

A Output Peg

  .WithOutput(CBT.getPegPos(X Size Of Component, [YSize Of Component], Z Size Of Component, Side Of Peg, [X Offset Of Peg], [Y Offset Of Peg] ),  CBT.getPegQuat(X Size Of Component, [YSize Of Component], Z Size Of Component Side Of Peg),Peg Descripion)
  
  
And Thats It!!
NOTE: Output Pegs Might Look Weird, thats A Problem with PiTUNG, not my tools.

I Will Be Posting A Mod That Uses this Under Ryan-Te/CBT Demo :)

  
