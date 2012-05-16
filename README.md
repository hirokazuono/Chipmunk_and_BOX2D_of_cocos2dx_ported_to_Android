Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
  
<pre><table><tr><tr><td align=center colspan=4><pre>
<b><pre>NOTE : Ap = Application.mk , A = Android.mk , j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, t = template(Dir) , HW = HelloWorld(Dir.topDir of this changing,not abobe helloworldDir.)</b>
, Dir(fld) = Directory(or Folder)</pre></td></tr>

<td>type( right )<br>ver( below )</td><td>11</td><td>12</td><td>13beta</td></tr>
<tr><td>BOX2D in<b>H</b><br>&nbsp; ( without <b>H</b> )</td>
<td>Ap & A in<b>j</b> , A in <b>j</b> in <b>h</b> , A in <b>C</b> (4)<br></td>
<td>Ap & A in<b>j</b> , A in <b>j</b> in <b>h</b> , A in <b>C</b> (4)<br></td>
<td>A in<b>j</b>(Ap no modified.No A in <b>j</b> in <b>h</b> & A in <b>C</b>)<br></td></tr>

<tr><td>chipmunk in<b>H</b><br>&nbsp; ( without <b>H</b> )</pre></td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td></tr></table>

</pre>

  
