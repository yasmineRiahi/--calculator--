# --calculator--


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;

namespace calsulatrice2
{
    /// <summary>
    /// Interaction logic for MainWindow.xaml
    /// </summary>
    public partial class MainWindow : Window
    {
        public MainWindow()
        {
            InitializeComponent();
        }

        private void textBox_TextChanged(object sender, TextChangedEventArgs e)
        {

        }

        private void button_Copy15_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = "0"; 
        }
        double var1 = 0;
        string op = "";
      

        private void button_Copy_Click(object sender, RoutedEventArgs e)
        {
            switch (op)
            {
                case "+":
                    Resultat.Text = (var1 + Double.Parse(Resultat.Text)).ToString() ;
                    break;
                case "-": 
                    Resultat.Text = (var1 - Double.Parse(Resultat.Text)).ToString();
                    break;
               case "/":
                    Resultat.Text = (var1 / Double.Parse(Resultat.Text)).ToString();
                    break;
                case "*":
                    Resultat.Text = (var1 * Double.Parse(Resultat.Text)).ToString();
                    break;
                default:
                    break;
            }  
            var1 = 0; 
        } 

        private void button_Copy12_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "2";
        }

        private void button_Copy9_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "3";
        }

        private void button_Copy14_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "4";
        }

        private void button_Copy11_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "5";
        }

        private void button_Copy8_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "6";
        }

        private void button_Copy16_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "1";
        }

        private void button_Copy17_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "7";
        }

        private void button_Copy10_Click(object sender, RoutedEventArgs e)
        {
           
            Resultat.Text = Resultat.Text + "8";    
        }

        private void button_Copy7_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "9";
        }

        private void button_Copy2_Click(object sender, RoutedEventArgs e)
        {
            Resultat.Text = Resultat.Text + "0";
        }

        private void button_Copy4_Click(object sender, RoutedEventArgs e)
        {
            var1 = var1 + Double.Parse(Resultat.Text);
            Resultat.Text = "0";
            op = "+";
        }

        private void button_Copy5_Click(object sender, RoutedEventArgs e)
        {
            var1 = var1 + Double.Parse(Resultat.Text);
            Resultat.Text = "0";
            op = "*";
        }

        private void button_Copy6_Click(object sender, RoutedEventArgs e)
        {
            var1 = var1 + Double.Parse(Resultat.Text);
            Resultat.Text = "0";
            op = "/";
        }

        private void button_Copy3_Click(object sender, RoutedEventArgs e)
        {
            var1 = var1 + Double.Parse(Resultat.Text);
            Resultat.Text = "0";
            op = "-";
        }
    }
}
