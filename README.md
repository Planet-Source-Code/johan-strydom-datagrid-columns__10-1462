<div align="center">

## DataGrid Columns


</div>

### Description

The purpose of the code is to show how to add columns to a VB.NET DataGrid control.
 
### More Info
 
Add a datagrid control to your form. called DataGrid1

Double click on your form and replace the Form1_Load() function with the code...


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Johan Strydom](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/johan-strydom.md)
**Level**          |Beginner
**User Rating**    |4.8 (19 globes from 4 users)
**Compatibility**  |VB\.NET
**Category**       |[Controls/ Forms/ Dialogs/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-dialogs-menus__10-3.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/johan-strydom-datagrid-columns__10-1462/archive/master.zip)





### Source Code

```
'You can't have a data grid column without a DataTable ... I think :)
 Private dbTable As New DataTable("DTBL1")
 Private Sub Form1_Load(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles MyBase.Load
 Dim i = 0
 'Add 4 columns to the table
 For i = 1 To 4
  dbTable.Columns.Add("Col" & i)
 Next
 'Set the datasource to our database table
 DataGrid1.DataSource = dbTable
 End Sub
```

