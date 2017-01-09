using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace kolo3
{
    class Skladnik : IComparable<MainWindow>
    {
        private string nazwaSkladnika;
        private double cenaSkladnika;
        
        public Skladnik(string nazwaSkladnika, double cenaSkladnika)
    {
        this.nazwaSkladnika = nazwaSkladnika;
        this.cenaSkladnika = cenaSkladnika;
    }



        public double GetCena()
        {
            return cenaSkladnika;
        }




        public int CompareTo(Skladnik other)
        {
            if (this.nazwaSkladnika == other.nazwaSkladnika)
            {
                return other.nazwaSkladnika.CompareTo(this.nazwaSkladnika);
            }
            return other.nazwaSkladnika.CompareTo(this.nazwaSkladnika);
        }








    }
}
