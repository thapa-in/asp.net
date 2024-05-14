```
public int GRP_ID = 0;

private void LastSelectedRow()
{
    try
    {
        int indx = 0;
        if (GRP_ID != 0)
        {
            foreach (DataGridViewRow row in dgvEvents.Rows)
            {
                if (row.Cells[1].Value != null)
                {
                    if (row.Cells["Group_ID"].Value.ToString() == GRP_ID.ToString())
                    {
                        defaultSelectedRow = indx;
                        dgvEvents.CurrentCell = dgvEvents.Rows[defaultSelectedRow].Cells[0];
                        break;
                    }
                    indx++;
                }
            }
        }
        else
        {
            dgvEvents.Rows[defaultSelectedRow].Selected = true;
        }
    }
    catch (Exception ex)
    {
        ErrorrInStatus(ex.Message.ToString());
    }
}
```
