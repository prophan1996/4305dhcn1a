# 4305dhcn1a
Phát triển phần mềm mã nguồn mở
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace congtrunhanchia
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

        private void button1_Click(object sender, EventArgs e)
        {
            int soThuNhat = Convert.ToInt32(txta.Text);
            int soThuHai = Convert.ToInt32(txtb.Text);
            int Kq = soThuNhat + soThuHai;
            txtkq.Text = Kq.ToString();
        }

        private void button2_Click(object sender, EventArgs e)
        {
            int soThuNhat = Convert.ToInt32(txta.Text);
            int soThuHai = Convert.ToInt32(txtb.Text);
            int Kq = soThuNhat - soThuHai;
            txtkq.Text = Kq.ToString();
        }

        private void button3_Click(object sender, EventArgs e)
        {
            int soThuNhat = Convert.ToInt32(txta.Text);
            int soThuHai = Convert.ToInt32(txtb.Text);
            int Kq = soThuNhat * soThuHai;
            txtkq.Text = Kq.ToString();
        }

        private void button4_Click(object sender, EventArgs e)
        {
            float soThuNhat = float.Parse(txta.Text);
            float soThuHai = float.Parse(txtb.Text);
            if (soThuHai == 0)
            {
                MessageBox.Show("nhap so b khac 0");
            }
            else
            {
                float chia = soThuNhat / soThuHai;
                txtkq.Text = chia.ToString();
            }
        }
    }
}
