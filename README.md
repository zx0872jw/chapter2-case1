# chapter3-case1
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace GreenvilleRevenueGUI
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            int ThisYear;
            int LastYear;
            int ThisYear_Rev;
            ThisYear = Convert.ToInt32(this_year.Text);
            LastYear = Convert.ToInt32(last_year.Text);
            ThisYear_Rev = ThisYear * 25;
            this_label.Text = "This years contestants total: " + ThisYear;
            last_label.Text = "Last years contestants total: " + LastYear;
            rev_label.Text = "This years revenue is $" + ThisYear_Rev;
            if (ThisYear > LastYear)
            {
                contest_label.Text = "There is more contestants this year than last year.";
            }
            else
            {
                contest_label.Text = "There were more contestants last year than this year.";
            }
        }
    }
}

