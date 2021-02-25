using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApp12
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            double x;
            double a;
            x = Convert.ToDouble(textBox1.Text);
            if (x < 0 && x > -5)
                a = Math.Sqrt(Math.Pow(x, 3) + Math.Abs(x));
            else if (x<2 && x>=0)
                a = (5*Math.Pow(x,3))-Math.Cos(x);
            else a = 0;
            label2.Text = Convert.ToString(a);
        }
    }
}
