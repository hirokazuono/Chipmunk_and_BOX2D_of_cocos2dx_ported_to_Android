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
<td><b>version</b>( → )</td>
<td>11</td><td>12</td>
<td>13beta</td></tr>
<tr>
<td>in <b>H</b> Dir(fld)</td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b> =<b>4</b></td>
<td>A in <b>j</b>(Ap no modified.No A in <b>h</b>(in<b>j</b>) & in <b>C</b>)</b> =<b>1</b></td></tr>
<tr>
<td>in <b>&nbsp;t</b> Dir(fld)</td>
<td>Ap in <b>t</b> , =<b>5</b>(files chge&copy.)</td>
<td></td>
<td></td>
</tr></table>
***
1. At the 1st,Create **xCode's cocos2d-x files** by **install-templates-xcode.sh** in a dir(fld) of 11 or 12 or 13beta's files  
that are downloads from cocos2d-x.org(&zip extracting).  
( Each xCode's cocos2d-x files(of 11,12,&13beta) create by **"./install-templates-xcode.sh -uf "**  
&nbsp;&nbsp;&nbsp; within each downloaded dir(fld,of 11,12,&13beta from cocos2d-x.org). In addition , not only these files  
&nbsp;&nbsp;that are created, **xCode's working also will change** to behavior of the each version of the files created.  
&nbsp;&nbsp; &nbsp; However, their **xCode types**(files&working) **can be changed to other xCode files** by **"-uf"**( above),  any time soon & freely. )
  
2. Some files of **1**(abobe ,equal the files of the **chg&copy files list** of 1st) **change(=chg) & copy**(as same as that **chg&copy list** ).
  
The **C**lasses dir(fld) in **BOX2D** is copied 