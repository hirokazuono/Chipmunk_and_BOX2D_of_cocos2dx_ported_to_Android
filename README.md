Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : Ap = Application.mk , A = Android.mk</b>
&nbsp; , Dir(fld) = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b> topDir of this changing,not "helloworldDir" abobe.<b>)</b>
&nbsp; , <b>t = template(Dir</b> other than(<b>out of</b>) <b>H</b>)
</pre>
<table><tr>
<td><b>version</b>(right)</td><td>11</td><td>12</td><td>13beta</td></tr>
<tr><td>in <b>H</b>Dir(fld)</td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b> =<b>4</b></td>
<td>A in <b>j</b>(Ap no modified.No A in <b>h</b>(in<b>j</b>) &A in <b>C</b>)</b> =<b>1</b></td></tr>

<tr><td>in <b>t</b>Dir(fld)</td>
<td>Ap in <b>t</b> =<b>5</b>files change&copy</td>
<td>(<b>4</b>files change&copy)</td>
<td>(<b>1</b>files change&copy)</td></tr></table>