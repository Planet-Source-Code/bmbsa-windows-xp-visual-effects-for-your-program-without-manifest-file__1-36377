<div align="center">

## Windows XP visual effects for  your program without manifest file


</div>

### Description

This article tells you how to get the Windows XP visual themes into your program without having the manifest file.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[bmbsa](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/bmbsa.md)
**Level**          |Advanced
**User Rating**    |4.7 (61 globes from 13 users)
**Compatibility**  |VB 6\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__1-1.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/bmbsa-windows-xp-visual-effects-for-your-program-without-manifest-file__1-36377/archive/master.zip)





### Source Code

```
<p><b>Step1:</b> download 'Resource Hacker' v3.4.0 from
<a href="http://delphi.icm.edu.pl/ftp/tools/ResHack.zip">here</a>, if you have
it then skip this step and go to <b>step2</b></p>
<p><b>Step2: </b>add the following code to your program before converting to
.exe file:</p>
<table border="1" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="100%" id="AutoNumber1">
 <tr>
 <td width="100%"><font face="Courier New" size="2">Private Declare Function
 <font color="#000080">InitCommonControls</font> Lib "comctl32.dll" () As
 Long<br>
 <br>
 Private Sub Form_Initialize()<br>
 <font color="#000080">InitCommonControls</font><br>
 End Sub</font></td>
 </tr>
</table>
<p dir="ltr"><b>Step3: </b>Open the notepad and copy the following code into it
and save it as a .txt file.</p>
<table border="1" cellspacing="0" style="border-collapse: collapse" bordercolor="#111111" width="100%" id="AutoNumber2">
 <tr>
 <td width="100%"><font face="Courier New" size="2"><?xml version="1.0"
 encoding="UTF-8" standalone="yes"?><br>
 <assembly xmlns="urn:schemas-microsoft-com:asm.v1" manifestVersion="1.0"><br>
 <assemblyIdentity<br>
 name="yourAppName"<br>
 processorArchitecture="x86"<br>
 version="4.34.0.0"<br>
 type="win32"/><br>
 <description>Your Program Name</description><br>
 <dependency><br>
 <dependentAssembly><br>
 <assemblyIdentity<br>
 type="win32"<br>
 name="Microsoft.Windows.Common-Controls"<br>
 version="6.0.0.0"<br>
 processorArchitecture="x86"<br>
 publicKeyToken="6595b64144ccf1df"<br>
 language="*"<br>
 /><br>
 </dependentAssembly><br>
 </dependency><br>
 </assembly></font></td>
 </tr>
</table>
<p><b>Step4: </b>open your .exe file with resource hacker by clicking open in
the file menu. (or open your resuorce file .res if you don't want to edit your program each time you rebuild the project)</p>
<p><img border="0" src="http://mycode.jeeran.com/images/res1.jpg"></p>
<p dir="ltr"><b>Step5:</b> Click on '<b>Add a new Resource...</b>' from the '<b>Action</b>'
menu</p>
<p dir="ltr">
<img border="0" src="http://mycode.jeeran.com/images/res2.jpg" width="682" height="368"></p>
<p dir="ltr"> </p>
<p dir="ltr"><b>Step6:</b> the following dialog will show up</p>
<p dir="ltr">
<img border="0" src="http://mycode.jeeran.com/images/res3.jpg" width="273" height="350"></p>
<p dir="ltr">Click on the button called '<b>open file with new resource...</b>'
and choose the .txt file you saved in <b>Step3</b></p>
<p dir="ltr"><b>Step7:</b> In the <u>Resource Type:</u> type <b>24</b>, In the
<u>Resource Name</u> type: <b>1 </b>and In the <u>Resource Language</u> type: <b>
1033. </b>and then click on '<b>Add Resource</b>'</p>
<p dir="ltr">
<img border="0" src="http://mycode.jeeran.com/images/res4.jpg" width="273" height="350"></p>
<p dir="ltr"> </p>
<p dir="ltr"><b>Step8:</b> Save the changes by clicking on '<b>Save</b>' from
the '<b>File</b>' menu. Finally, Terminate the Resource Hacker.</p>
<p dir="ltr">
<img border="0" src="http://mycode.jeeran.com/images/res5.jpg" width="682" height="368"></p>
<p dir="ltr">Done!</p>
<p dir="ltr">open your .exe file and notice the cool interface :)</p>
```

