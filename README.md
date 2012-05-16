Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.
 
**NOTE : Ap = Application.mk , A = Android.mk , j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir) , t = template(Dir)
  HW = HelloWorld(Dir.topDir of this changing,not abobe helloworldDir.)** Dir(fld) = Directory(or Folder)
  
<table><tr><td>type( right )<br>ver( below )</td><td>11</td><td>12</td><td>13beta</td></tr>
<tr><td>BOX2Din **H**<br>&nbsp; witwout **H**</td>
<td>Ap&A in **j** / A in **j** in **h** / A in **C**(4)<br></td>
<td>Ap&A in **j** / A in **j** in **h** / A in **C**(4)<br></td>
<td>A in **j** (Ap no modified. No A in **j** in **h** &A in **C** )<br></td></tr>

<tr><td>chipmunk(in **H**)<br>&nbsp;( witwout **H**)</td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td></tr></table>

</pre>

  
