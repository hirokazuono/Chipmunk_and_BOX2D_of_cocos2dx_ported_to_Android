Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : Ap = Application.mk , A = Android.mk</b>
&nbsp; , Dir(fld) = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b> topDir of this changing,not abobe helloworldDir.<b>)</b> , <b>t = template(Dir</b> without <b>H</b>)
</pre>
<table><tr>
<td><b>version</b>(right)<br><b>type</b> (below)</td><td>11</td><td>12</td><td>13beta</td></tr>
<tr><td><b>H</b>ofBOX2D<hr>&nbsp; (except <b>H</b>)</td>
<td>Ap&A in <b>j</b>/ A in <b>h</b>(in<b>j)</b>/ A in <b>C</b><br><hr>Ap in <b>t</b>&nbsp;&nbsp;&nbsp;(=5)</td>
<td>Ap&A in <b>j</b>/ A in <b>h</b>(in<b>j)</b>/ A in <b>C</b>(=4)<br><hr></td>
<td>A in <b>j</b>(Ap no modified.No A  in <b>h</b>(in<b>j</b>) & A in <b>C</b>)<br><hr></td></tr>

<tr><td><b>H</b>of chipmunk<hr>(except <b>H</b>)</pre></td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td>
<td><br>&nbsp;</td></tr></table>
  
