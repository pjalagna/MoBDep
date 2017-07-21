# MoBDep
Model Based Deployment
html?
<table> <!-- history -->
<tr> <td> Name </td> <td> Date </td> <td> reason </td> </tr> 
<tr> <td> Paul </td> <td> 7/21/2017 </td> <td> original </td> </tr> 
</table>
<table> <!-- overview -->
<tr> <td> Overview </td> <td> . </td> </tr> 
<tr> <td> . </td> 
<td> Model Based deployment is a set of languages and processes that are used during JAD sessions 
(therefore understood by humans) and that can be directly compiled into a completed system
</td> </tr> 
</table>
<table> <!-- screen language -->
<tr> <td> Screen Language </td> <td> . </td> </tr> 
<tr> <td> . </td> 
<td> 
def screen :=</br>
[1] ="screen" <name> =":=" ="(" // screenStuff =")" =name ="screen" =";" . </br>
[2] "badly formed screen statement" error . </br>
; </br>

def screenStuff :- </br>
[1] <x1> </br>
[2] ?x1="Line" // linestuff tail. </br>
[3] ?x1="object" // objectStuff tail.</br>
[4] ?x1="hidden" // hiddenStuff tail.</br>
[4.5] ?x1="css" // cssStuff tail. </br>
[5] ?x1=")" .</br>
[6] "badly formed screen (internal) statement" error .</br>
;</br>

</td> 
</tr> 
<tr> <td> example </td> <td> . </td> </tr> 
<tr> <td> . </td> 
<td> 
screen logon ( </br>
CSS : ( BLogon.color = RED ) ; </br>
Line 1 : "   " , "User Name" , txt-user ; object user ( l1.min=6 , l1.max=10 ) ;</br>
Line 2 : "   " , "Password"  , pwd-pcode ; object pcode ( l1.min = 1 ) ;</br>
Line 3 : ; </br>
Line 4 : "   " , "Role" , list-Role ; object Role ( load=SQL2() l1.min=1 ) ;</br>
Line 5 : button-BLogon("Process") ; object Logon ( onClick=encode1() , to=LogonProc.php );</br>
hidden : date ; object date ( load=dateload() ) ;</br>
) logon screen ;</br>
</td> 
</tr> 
</table>

template is a 2x2 or 3x3
<table> <!-- 2x2 -->
<tr> <td> . </td> <td> . </td> </tr> 
<tr> <td> . </td> <td> . </td> </tr> 
</table>
<table> <!-- 3x3 -->
<tr> <td> . </td> <td> . </td> <td> . </td> </tr> 
<tr> <td> . </td> <td> . </td> <td> . </td> </tr> 
</table>
