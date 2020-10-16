PROGRAM FOR SHOWIGN THE IMPLEMENTATION OF ARMSTRONG NO.
Public Class Form1
Private Sub Button1_Click(sender As Object, e As EventArgs) Handles Button1.Click
 		       Dim num As Integer = 0
        		Dim rmd As Integer = 0
        		Dim sum As Integer = 0
        		Dim orginal As Integer
        		Dim tempNum As Integer
        		Dim count As Integer = 0
        		num = TextBox1.Text
        		orginal = num
        		tempNum = num
        		While tempNum <> 0
            		count = count + 1
            		tempNum = Math.Floor(tempNum / 10)
        		End While
        		While num > 0
            		rmd = Math.Floor(num Mod 10)
            		num = Math.Floor(num / 10)
            		sum = sum + Math.Pow(rmd, count)
        		End While
        		If sum = orginal Then
            		MessageBox.Show(“Armstrong”)
        		Else
            		MessageBox.Show(“Not Armstrong”)
        		End If
    			End Sub
End Class
