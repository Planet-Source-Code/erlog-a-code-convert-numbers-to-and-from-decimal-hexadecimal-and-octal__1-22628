<div align="center">

## A\+ code: convert numbers to and from decimal, hexadecimal and octal


</div>

### Description

This code will convert numbers to and from decimal, hexadecimal and octal. It's really useful and simple to follow code - intended for the beginner. If you use it, there's no need to give me credit but lease vote for it, thanks.

-lgr
 
### More Info
 
You need a txtNumber text box for the number display, and then three check boxes (optDecimalButton, optHexButton and optOctalButton). That's it!


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[erLog](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/erlog.md)
**Level**          |Beginner
**User Rating**    |3.7 (33 globes from 9 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0, VB Script
**Category**       |[Math/ Dates](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math-dates__1-37.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/erlog-a-code-convert-numbers-to-and-from-decimal-hexadecimal-and-octal__1-22628/archive/master.zip)





### Source Code

```
'Written by littlegreenrussian
Sub optDecimalButton_click() 'decimal checkbox clicked
	txtNumber.Text = Format(CurrentNum) 'change the format of the txtHumber textbox
End Sub
Sub optHexButton_click() 'hexadecimal checkbox clicked
	txtNumber.Text = Format(CurrentNum) 'change the format of the txtHumber textbox
End Sub
Sub optOctalButton_click() 'octalcheckbox clicked
	txtNumber.Text = Format(CurrentNum) 'change the format of the txtHumber textbox
End Sub
SubtxtNumber_Change()
'Val function - numbers beginning with &O as octal,
'numbers beginning with &H as hexadecimal
If optOctalButton.Value = True Then 'octal button checked
	CurrentNum = Val("&O" & LTrim(txtNumber.Text)& "&") 'change the number to octal
Else if optDecimal.Value = True Then 'decimal checked
	CurrentNum = Val(LTrim(txtNumber.Text)& "&") 'change number to deciaml - note it does NOT require a &D
Else 'otherwise
	CurrentNum = Val("&H" & LTrim(txtNumber.Text)& "&") 'change it to hexadecimal
	End If
End Sub
```

