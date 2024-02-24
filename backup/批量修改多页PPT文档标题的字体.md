修改下面的微软雅黑为你想要修改的字体（三个都修改）即可，然后运行宏：

Sub modify_Title()
'修改PPT标题
Dim i, j, ib, jb, num As Integer
On Error Resume Next
For i = 1 To ActivePresentation.Slides.Count '判断修改的页数
ActiveWindow.View.GotoSlide Index:=i
num = ActiveWindow.Selection.SlideRange.Shapes.Count '计算该幻灯片上的元素个数
For j = 1 To num
With ActiveWindow.Selection.SlideRange.Shapes.Title.TextFrame.TextRange.Font '对该幻灯片的标题文字格式进行修改
.NameAscii = "微软雅黑"  '你可换成自己想要的字体
.NameOther = "微软雅黑 "
.NameFarEast = "微软雅黑"
End With
Next j
Next i
End Sub