Chipmunk-of-cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : Ap = Application.mk , A = Android.mk</b>
&nbsp; , Dir(fld) = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b>(fld). TopDir of this changing , not "helloworld(Dir)" abobe. <b>)</b>
&nbsp; , <b>t = template(Dir</b>(fld). Other than(<b>Out of</b>) <b>H</b>elloWorld Dir(fld). <b>)</b>
</pre>
<table><tr>
<td><b>version</b>(right)</td>
<td>11</td><td>12</td>
<td>13beta</td></tr>
<tr>
<td rowspan=2>in <b>H</b>Dir(fld)
<br>in <b>t</b>Dir(fld)</td>

<td rowspan=2>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b>
<br>Ap in <b>t</b> =<b>5</b>(files chge&copy)</td>

<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b> =<b>4</b></td>
<td>A in <b>j</b>(Ap no modified.No A in <b>h</b>(in<b>j</b>) & in <b>C</b>)</b> =<b>1</b></td></tr>

<tr>
<td></td>
<td></td></tr></table>