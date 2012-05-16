Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : Ap = Application.mk , A = Android.mk</b>
&nbsp; , Dir(fld) = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b> topDir of this changing,not abobe helloworldDir.<b>)</b> , <b>t = template(Dir</b> without <b>H</b>)
</pre>
<table><tr>
<td><b>version</b>(right)</td><td>11</td><td>12</td><td>13beta</td></tr>
<tr><td><b>H</b>ofBOX2D<hr>&nbsp; </td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>A in <b>j</b>(Ap no modified.No A  in <b>h</b>(in<b>j</b>) & A in <b>C</b>)</td></tr>

<tr><td>(except <b>H</b> Dir(fld))</td>
<td>Ap in <b>t</b>&nbsp;&nbsp;&nbsp;(<b>5</b>files change&copy)</td>
<td>&nbsp;&nbsp;&nbsp;(<b>4<・b>files change&copy)</td>
<td>&nbsp;&nbsp;&nbsp;(<b>1</b>files change&copy)</td></tr></table>