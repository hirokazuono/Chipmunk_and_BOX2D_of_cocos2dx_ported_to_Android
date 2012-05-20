Chipmunk_and_Box2D_of_cocos2dx_ported_to_Android-Apps_as_to_work.
=============================
I ported **cocos2d-x**( or cocos2dx? that is one of the famous game libraries)**'s "chipmunk" & "BOX2D"**  
to the Android Apps(applications) as  to work.  
<pre><b>NOTE : HWc&h = HelloWorldScene.cpp and HelloWorldScene.h</b> ( are "C++(cpp & h) files". )
<b>, Ap = Application.mk , A = Android.mk</b>  ( are "mk files". )
<b>Dir(fld)</b> = Directory(or Folder) , <b>j = jni(Dir) , h =  helloworld(Dir) , C = Classes(Dir)
, H = HelloWorld(Dir</b>(fld). TopDir of this changing&creating , not "helloworld(Dir)" above. <b>)</b>
, <b>t = template(Dir</b>(fld). Other than(<b>Out of</b>) <b>H</b>elloWorld Dir(fld). <b>)</b> &nbsp;&nbsp; &nbsp; <b>/ &nbsp;&nbsp; B2D = Box2D</b>(Dirs or files)
</pre>
<table><tr>
<td>version→</td>
<td>11</td><td>12</td>
<td>13beta</td></tr>
<tr>
<td rowspan=3>into<b>H</b> Dir</td>
<td>HWc&h in <b>C</b>(in <b>H</b>)<b>Dir</b>(=2)</td>
<td>HWc&h in <b>C</b>(in <b>H</b>)<b>Dir</b>(=2)</td>
<td>HWc&h in <b>C</b>(in <b>H</b>)<b>Dir</b>(=2/<b>All are the same.</b>)</td></tr>

<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b></td>
<td>Ap&A in <b>j</b> / A in <b>h</b>(in<b>j)</b> / A in <b>C</b> =<b>6</b></td>
<td>A in <b>j</b>(Ap no modified.No A in <b>h</b>(in<b>j</b>) & in <b>C</b>) =<b>3</b></td></tr>

<tr>
<td colspan=3>( & <b>"Only 11</b>(except 12or13b)Box2D's <b>Box2D" Dir</b>(<b>on the outside of HDir</b>)ectry are copied into <b>C</b>(in <b>H</b>)<b>Dir</b>ectry. )</td>
</tr>

<tr>
<td>into<b>&nbsp;t</b> Dir</td>
<td>Ap in <b>t</b> =<b>7(&1 Dir</b> of v11 B2D<b>)</b></td>
<td></td>
<td></td>
</tr></table>
***
1. At the 1st,Create **xCode's cocos2d-x files** by **install-templates-xcode.sh** in a Dir(fld) of 11 or 12 or 13beta  
that is one of Dirs(flds) maked by **" the downloaded from cocos2d-x.org and extracted zip file(s) "** .  
**(** Each xCode's cocos2d-x files(of 11,12,&13beta) create by **"./install-templates-xcode.sh -uf "**  
&nbsp;&nbsp;&nbsp;within each Dir(fld,of 11,12,&13beta from cocos2d-x.org) as above. &nbsp;&nbsp; In addition , not only these files  
&nbsp;&nbsp;that are created, **xCode's working also will change** to behavior of the each version of the files created. However,  
&nbsp;&nbsp;&nbsp;their **xCode types**(files&working) **can be changed to other xCode files** by **"-uf**( above)**"**, **any time quickly & freely. )**  
And also you may have to use each files of chipmunk or Box2D  
that you want to create, but only enough to use the files "2." as follows downloaded in "this page".  
**( This reason of enough is** also mentioned in next **2.** as follows:i.e. " **B2D** files of no change **aren't be downloaded** ". **)**
2. Change & copy some of **"1.**&nbsp;(above. &nbsp; =(equal) the **chg**(change)**&copy list** at the beginning**)" .** It should be noted that  
**these "chg&copy list files** (of the changed files from the original files**(except B2D** files)**)" are downloaded in "this page"**.  
If you use them , **apps can be created soon and quickly**. &nbsp;&nbsp;Moreover , **the changes are minimum changes  
as can (** and many changes of the files have been **added annotation**(e.g."# ~ 1205110818 chg ~ ). **) .** &nbsp; Because  
I believe very safe that "anyone **can be easy to understand the changes** , not only can create apps soon & quickly ".  
( So **B2D** files of no change **aren't be downloaded in "this page". save xCode's files of 1.** above **&copy** into position. )  
3. **The way of these porting and Description of**  
**the minimum changes(& difference of each cocos2d-x files** of versions and types(chipmunk&B2D and android&xCode) **)**  
as follows. &nbsp;&nbsp; &nbsp; ( &nbsp; **the way of these porting are bold.** &nbsp;&nbsp; &nbsp; / &nbsp; &nbsp;&nbsp; description of difference aren't not bold. &nbsp; )
<pre>
<b>(A</b>(=1.)<b>) After "1."</b>as above
<b>(i.e. after creating xCode's files of versions and types that you want to create),
please also create android's cocos2d-x files of versions and types that you want to create
by create-android-project.sh.</b> Incidentally, I think no need particularly for descriptions
about <b>modifing "NDK_ROOT_LOCAL" and "ANDROID_SDK_ROOT_LOCAL"</b> at the beginning of
this "create-android-project.sh" because many descriptions already exist in various other places.
Such as <b>NDK_ROOT_LOCAL="/home/laschweinski/android/android-ndk-r5"( → "/xxx/android-ndk-r(6,7etc)")
ANDROID_SDK_ROOT_LOCAL="/home/xxxxx/android/android-sdk-linux_86"( → "/Applications/android-sdk")
and "the created files of the name that you want to create are used (C) below.</b>
<hr>
<b>(B</b>(=2.)<b>) Please copy the files that are on the "chg&copy list" as of the list.</b>
By the way, In All versions(as 11,12,and 13beta) which are created by "create-android.sh",
11 includes a "Resourace" directory but it's "(ending in s and) Resources" in 12 and 13b.
(As a result, "A in <b>C</b>"<b>( =</b> Android.mk in <b>C(</b>(lasses in H(lloWorld))<b>Dir</b>(ectry)<b>)</b> <b>)</b> of 11
&nbsp; are only differd , among the "mk.files". )
However, the contents in each Directories also are almost the same
&nbsp;except that " 12 and 13 don't exist the icon.png but exist the font Dir,
&nbsp; &nbsp; on the contrary, only 11 don't exists the font Dir but exist icon.png ".
That's why all you need to do is <b>copy the contents in the "Resource(s)" Dir</b>(ectry)
&nbsp;<b>to the "Resource(s)" Dir</b>(ectry) <b>in C(</b>(lasses in H(lloWorld))<b>Dir</b>(ectry)<b>)</b> that you want create.
( As an aside,&nbsp; Not only the files described in the above list,
&nbsp; &nbsp; you can be downloaded <b>"several types of image files (for B2D)"</b> in this page.
&nbsp; These <b>can be chenged as you modify HelloWorldScene.h(</b>of <b>HWc&h</b> files<b>) any time quickly & freely.</b> )
<b>And only if you want to use B2D,</b>
each person please <b>save xCode's files</b> of 1. above <b>and copy into position</b> such as sorry in repeating<b>.</b>
( Besides, also as an aside,
&nbsp; &nbsp; HelloWorldScene.cpp( among the HWc&h( = HelloWorldScene.cpp and HelloWorldScene.h) )
&nbsp; are used in each cocos2d-x files of versions and types( = chipmunk & B2D and android & xCode ).
&nbsp; &nbsp; All of them already have been fixed for all type and version. but HelloWorldScene.cpp
&nbsp; for each types( = chipmunk or B2D ) are not changed at all and used in exactly the same content
&nbsp; &nbsp; except that 11 and 12 are "CCPoint point = touch->locationInView(touch->view());"
&nbsp; but only newest 13beta is without "touch->view()" as "CCPoint point = touch->locationInView();".
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; http://omaena.com/diff_cocos2dxVer11-13b.txt&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; )
<hr>
<b>(C) After (A) and (B) , 
prease move to the inside of "android Dir" in "a Dir of the name that you want to create</b><b>"
in "android's cocos2d-x Dir</b>( that you want to create)<b>" and compile using "./build_native.sh".
I think you create the completed App as above.</b>
<hr>
<b>(C'</b>(C2)<b>) If your created App remains named "Hello World",
You need to move to the inside of "android Dir" in "H</b>(HelloWorld)<b>Dir" </b>such as <b>(C)</b> above
<b>and modify "NDK_ROOT_LOCAL" and "COCOS2DX_ROOT_LOCAL"
at the beginning of "build_native.sh" in this "android Dir".
such as NDK_ROOT_LOCAL=/cygdrive/d/programe/android/ndk/android-ndk-r6b( → /xxx/android-ndk-r(6,7etc))
COCOS2DX_ROOT_LOCAL="/home/xxxxx/android/android-sdk-linux_86"( → (the pass of android's cocos2d-x) &nbsp;)
and compile using this build_native.sh as "./build_native.sh"</b>(such as <b>(C)</b> above)<b>.
or </b>
( Although I am sorry a little that I don't check and try still firmly in fact, )
Using "perl -i -p -e 's/HelloWorld/the_name_that_you_want_to_create/g' `find . -type f`"
in H(HelloWorld)Dir and renaming "HelloWorld" to the name that you want to create
is also may be possible. <b>Maybe You're easier the way as above, 
but not creating e.g."proguard.cfg"</b> as perhaps not compiling the "apk" file <b>.
( If you only changed the name of App that you want to create,
&nbsp; &nbsp; The easiest and most effortless way, might be "only the modifying of string.xml ". )</b>
</pre>