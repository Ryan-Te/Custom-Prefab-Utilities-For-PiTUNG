# Custom-Builder-Mode-Utilities-For-PiTUNG
Custom Builder Mode Utilities For PiTUNG
This Is A Set Of Functions That Make Using The Custom Builder In PiTUNG Alot Eaiser!
Functions:

NOTE: Things Inside [] Are Optional


createCube(X,[Y]Z)

  This Will Create A Cube Of Size X Y Z, Default For Y is 1
  
  This Function Is A Modified Version Of Falsepatterns Function That Lets You Create Any Sized Cube Instead Of Just 1x1x1 Cubes.
  
  
  
getPegPos(X,[Y],Z,Side,[OffestX],[Offset Y])

  This Will Turn The Given Cube Size(X,Y,Z) 
  And Output The Position Of A Peg On Side Side And Offset The Peg By Offset X TUNG Grid Spaces Left/Right And Offset Y TUNG Grid Spaces UP/Down
  Default For Y Is 1 and Default For Offset X and Offset Y Are 0
  
  
getPegQuat(X,[Y],Z,Side)

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

To Get CBMUFP, Either Download The .cs File Or Check The Source Code

To Use CBMUFP, Put The .cs File Inside Your c# Project And Make sure You Have The UnityEngine As A Refernce!!

NOTE: Output Pegs Might Look Weird, thats A Problem with PiTUNG, not my tools.

I Will Be Posting A Mod That Uses this Under Ryan-Te/CMBUFP Demo :)

https://github.com/Ryan-Te/CBMUFP-Demo

  
