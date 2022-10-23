-using System;

using System.Collections.Generic;

using System.ComponentModel;

using System.Data;

using System.Drawing;

using System.Linq;

using System.Text;


using System.Threading.Tasks;

using System.Windows.Forms;

namespace WindowsFormsApp1

{

    public partial class Form1 : Form
    
    {
    
        char _islem;
        
        bool _ekrantemizle;
        
        int _ilksayi;
        


        public Form1()
        {
            InitializeComponent();
        }

        private void sayı1button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
            label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
            label1.Text = "";
            label1.Text += "1";
        }

        private void sayı2button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
            label1.Text = "";
            label1.Text += "2";
        }

        private void sayı3buuton_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
            label1.Text = "";
            label1.Text += "3";
        }

        private void sayı4button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
            label1.Text = "";
            label1.Text += "4";
        }

        private void sayı5button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "5";
        }

        private void sayı6button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "6";
        }

        private void sayı7button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "7";
        }

        private void sayı8button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "8";
        }

        private void sayı9button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "9";
        }

        private void sayı0button_Click(object sender, EventArgs e)
        {
            if (_ekrantemizle == true)
            {
                label1.Text = "";
                _ekrantemizle = false;
            }
            if (label1.Text == "0")
                label1.Text = "";
            label1.Text += "0";
        }

        private void toplabutton_Click(object sender, EventArgs e)
        {
            _islem = '+';
            _ekrantemizle = true;
            _ilksayi = Convert.ToInt32(label1.Text);
        }

        private void esittirbutton_Click(object sender, EventArgs e)
        {
            int ikinisayi = Convert.ToInt32(label1.Text);
            int sonuç;



            switch(_islem)
            {
                case '+':
                    sonuç = _ilksayi + ikinisayi;
                    break;
                case '-':
                    sonuç = _ilksayi - ikinisayi;
                    break;
                case '*':
                    sonuç = _ilksayi * ikinisayi;
                    break;
                case '/':
                    sonuç = _ilksayi / ikinisayi;
                    break;
                default:
                    sonuç = 0;
                    break;
            }

            label1.Text = Convert.ToString(sonuç);

        }

        private void cıkarbuttn_Click(object sender, EventArgs e)
        {
            _islem = '-';
            _ekrantemizle = true;
            _ilksayi = Convert.ToInt32(label1.Text);
        }

        private void carpbutton_Click(object sender, EventArgs e)
        {
            _islem = '*';
            _ekrantemizle = true;
            _ilksayi = Convert.ToInt32(label1.Text);
        }

        private void bolbutton_Click(object sender, EventArgs e)
        {
            _islem = '/';
            _ekrantemizle = true;
            _ilksayi = Convert.ToInt32(label1.Text);
        }

        private void CsilButton_Click(object sender, EventArgs e)
        {
            label1.Text = "0";
        }
    }
}
