# Flag-Viewer
C#/Windows Form (Visual Studio) Flag viewer code

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace WindowsFormsApplication1
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void Form1_Load(object sender, EventArgs e)
        {

        }

        private void checkBox2_CheckedChanged(object sender, EventArgs e)
        {
            if (CountryNameCheckBox.Checked == true)
            {
                CountryNameLabel.Visible = true;
            }
            else
                CountryNameLabel.Visible = false;
        }


        private void checkBox1_CheckedChanged(object sender, EventArgs e)
        {
            if (TitleCheckBox.Checked == true)
            {
                FlagViewer.Visible = true;
            }
            else
                FlagViewer.Visible = false;
        }

        private void NorwayPicture_Click(object sender, EventArgs e)
        {
            JapanPicture.Visible = true;
            SouthKoreaPicture.Visible = false;
            NorwayPicture.Visible = false;
            NewZealandPicture.Visible = false;
        }

        private void JapanRadioButton_CheckedChanged(object sender, EventArgs e)
        {
            JapanPicture.Visible = true;
            CountryNameLabel.Text = "Japan";
            SouthKoreaPicture.Visible = false;
            NorwayPicture.Visible = false;
            NewZealandPicture.Visible = false;
        }

        private void SouthKoreaRadioButton_CheckedChanged(object sender, EventArgs e)
        {
            JapanPicture.Visible = false;
            SouthKoreaPicture.Visible = true;
            CountryNameLabel.Text = "South Korea";
            NorwayPicture.Visible = false;
            NewZealandPicture.Visible = false;
        }

        private void NorwayRadioButton_CheckedChanged(object sender, EventArgs e)
        {
            JapanPicture.Visible = false;
            SouthKoreaPicture.Visible = false;
            NorwayPicture.Visible = true;
            CountryNameLabel.Text = "Norway";
            NewZealandPicture.Visible = false;
        }

        private void NewZealandRadioButton_CheckedChanged(object sender, EventArgs e)
        {
            JapanPicture.Visible = false;
            SouthKoreaPicture.Visible = false;
            NorwayPicture.Visible = false;
            NewZealandPicture.Visible = true;
            CountryNameLabel.Text = "New Zealand";

        }

        
        private void ProgrammerCheckBox_CheckedChanged(object sender, EventArgs e)
        {
            if (ProgrammerCheckBox.Checked == true)
            {
                MyName.Visible = true;
            }
            else
                MyName.Visible = false;
        }

        private void MyName_Click(object sender, EventArgs e)
        {

        }

        private void FlagViewer_Click(object sender, EventArgs e)
        {

        }
    }
}
