# Toggle Full Screen

**Main Class**

```cs
using System.Windows.Forms;

namespace Devloli.Modules
{
    internal class ToggleFullScreen
    {
        public static void GoFullscreen(bool fullscreen)
        {
            if (fullscreen)
            {
                Form form = new Form();
                form.FormBorderStyle = FormBorderStyle.None;
                form.WindowState = FormWindowState.Maximized;
                form.Show();
                form.Focus();
                form.BringToFront();
                form.TopMost = true;
                form.Focus();
            }
            else
            {
                Form form = new Form();
                form.FormBorderStyle = FormBorderStyle.Sizable;
                form.WindowState = FormWindowState.Normal;
                form.Show();
                form.Focus();
                form.BringToFront();
                form.TopMost = true;
                form.Focus();
            }
        }
    }
}
 
```
