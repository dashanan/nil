# nil
a new program
my program on structures
﻿using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace opsovl
{
    class vect
    {
        int a;
        int b;
        int c;
        public vect()
        { }

        public  vect (int p, int q, int r)
        {
            
           a = p;
            b = q;
            c = r;
        }
        public static bool operator == (vect m,vect n)
        {
            if ((m.a == n.a) && (m.b == n.b) && (m.c == n.c))
            {
                return true;
            }
            else return false;
        }
        public static bool operator !=(vect v1, vect v2)
        {
            return (!(v1 == v2));
        }



    }
            
    
    class Program
    {
        static void Main(string[] args)
        {
            vect a = new vect(1, 2, 3);
            vect b = new vect(4, 5, 6);

            if (a == b)
            {
                Console.WriteLine("equal");
            }
            else Console.WriteLine("not equal");
        }
    }
}
