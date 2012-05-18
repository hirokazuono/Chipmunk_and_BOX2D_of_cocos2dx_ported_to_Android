Chipmunk_and_Box2D_of_cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : Ap = Application.mk , A = Android.mk</b>
&nbsp; , Dir(fld) = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b>(fld). TopDir of this changing , not "helloworld(Dir)" above. <b>)</b>
&nbsp; , <b>t = template(Dir</b>(fld). Other than(<b>Out of</b>) <b>H</b>elloWorld Dir(fld). <b>)</b>
</pre>
<table><tr>
<td><b>version</b> →</td>
<td>11</td><td>12</td>
<td>13beta</td></tr>
<tr>
<td>into<b>H</b> Dir</td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b> =<b>4</b></td>
<td>A in <b>j</b>(Ap no modified.No A in <b>h</b>(in<b>j</b>) & in <b>C</b>)</b> =<b>1</b></td></tr>

<tr>
<td></td>
<td colspan=3>(& <b>"Only 11</b>(except 12or13b) Box2D's <b>Box2D" Dir</b>(above(<b>outside of</b>) <b>H</b>Dir)ectry are copied into <b>C</b>(in <b>H</b>)<b>Dir</b>ectry. )</td>
</tr>

<tr>
<td>into<b>&nbsp;t</b> Dir</td>
<td>Ap in <b>t</b> =<b>5(</b>&11B2D's <b>1dir)</b></td>
<td></td>
<td></td>
</tr></table>
***
1. At the 1st,Create **xCode's cocos2d-x files** by **install-templates-xcode.sh** in a dir(fld) of 11 or 12 or 13beta's files  
that are downloads from cocos2d-x.org(&zip extracting).  
( Each xCode's cocos2d-x files(of 11,12,&13beta) create by **"./install-templates-xcode.sh -uf "**  
&nbsp;&nbsp;&nbsp;within each downloaded dir(fld,of 11,12,&13beta from cocos2d-x.org). &nbsp;&nbsp; In addition , not only these files  
&nbsp;&nbsp;that are created, **xCode's working also will change** to behavior of the each version of the files created. However,  
&nbsp;&nbsp;&nbsp;their **xCode types**(files&working) **can be changed to other xCode files** by **"-uf"**( above) , any time soon & freely. )  
And also you should create each files of chipmunk or Box2D that you want to create,  
but only enough to use the files "2." as follows downloaded in "this page".  
(**This reason of enough is explained by 3 below ,** as e.g. **difference of each cocos2d-x files**. )
2. Change & copy some of **"1.**&nbsp;(above. &nbsp; =(equal) the **chg**(change)**&copy list** at the beginning**)" .** It should be noted that  
**these "chg&copy list files** (of the changed files from the original files(exceptB2Ddir))**" download in "this page"**.  
If you use them , **apps can be created soon and quickly**. &nbsp;&nbsp;Moreover , **the changes are minimum changes  
as can (** and many changes of the fileshave been **added annotation**(e.g."# ~ 1205xx xx:xx chg ~ ). **) .** &nbsp; Because  
I believe very safe that "anyone **can be easy to understand the changes** , not only can create apps soon & quickly ".  
(For this reason,**Box2D**Dir(B2Ddir)**doesn't  download in "this page". save xCode's files of 1.**above **&copy** into position.)  
3. **The way of these porting and Description of**  
**the minimum changes(& difference of each cocos2d-x files** of versions and types(chipmunk&B2D and android&xCode)**)**  
as follows. &nbsp;&nbsp; &nbsp; ( **the way are bold.** &nbsp;&nbsp; &nbsp; / &nbsp; &nbsp;&nbsp; description of difference aren't not bold. )
<pre>
<b>After "1." of the above(i.e.after creating xCode's files of versions & types that you want to create),
please also create android's cocos2d-x files of versions and types that you want to create
by create-android-project.sh.
and copy 
</b>

</pre>