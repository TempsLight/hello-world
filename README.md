#include <iostream>

using namespace std;

int main()
{



    start:
    system("cls");
    cout << endl;
    char anes, anes1;
    string name= "", add="", con="", cont="", name1="";
    cout << "                   Electric Billing System           "<<endl<<endl;
    cout << "                   Electric Consumer Type            "<<endl;
    cout << "-----------------------------------------------------" <<endl<<endl;
    cout << " Press Enter to start"<<endl<<endl;
    getline (cin,name);
    cout << " Name: ";
    getline (cin,name);
    cout << " Address: ";
    getline (cin,add);
    cout << " Consumer Number: ";
    getline (cin,con);
    cout << "-----------------------------------------------------" <<endl<<endl;

    cout << ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>" <<endl<<endl;
    cout << " [R] Residential   [C] Commericial   [I] Industrial  " <<endl<<endl;
    cout << "                   [Q] Exit Program                  " <<endl<<endl;
    cout << "Select Consumer: ";
    cin >> anes, anes1;
    cout <<endl<<endl<< ">>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>" <<endl;
    cout << endl;


    //Residential Condition
    if (anes=='R' || anes=='r')
    {
        cout << "Residential Consumer"<<endl<<endl;

        double prv, prs, cns;
        cout<<"Enter Present: ";
        cin >> prs;
        cout<<"Enter Previous: ";
        cin >> prv;

        cns = prs - prv;

        if (cns >= 300)//rate15.25
        {
            double resi1 = 15.25;
            double rtcost;

            rtcost= resi1*cns;
            cout<<"Total Consumption: "<<cns<<endl;
            cout<<"Rate: "<<resi1<<endl;
            cout<<"rtcost: "<<rtcost<<endl;
            if (rtcost >=1000 )
            {
                double rac = 200;
                double rtax;
                rtax = 0.05*rtcost;
                int tp;

                tp = rtax + rtcost + rac;
                cout<<"Total Price: "<<tp<<endl;
            }
            else if (rtcost >= 500 && rtcost <1000)
            {
                double rac1;
                    double rtax1;
                    double rtp1;

                    rac1 = 100;
                    rtax1 = 0.03 * rtcost;
                    rtp1 = rtax1 + rtcost + rac1;
                    cout<<"Total Price: "<<rtp1<<endl;
            }
            else
            {
                double rac2;
                   double rtax2;
                   double rtp2;

                rac2 = 0;
                rtax2 = 0;
                rtp2 = rtax2 + rtcost + rac2;
                cout<<"Total Price: "<<rtp2<<endl;
            }

        }
        else if (cns >= 200 && cns <=300)
        {
        double resi2 = 14.50;
        double rtcos1;

        rtcos1 = resi2 * cns;
        cout<<"Total Consumption: "<<cns<<endl;
        cout<<"Rate: "<<resi2<<endl;
        cout<<"tcost: "<<rtcos1<<endl<<endl;
        if (rtcos1 >=1000 )
        {
            double rac3 = 200;
            double rtax3;
            double tp3;
            rtax3 = 0.05 * rtcos1 ;
            tp3 = rtax3 + rtcos1 + rac3;
            cout<<"Total Price: "<<tp3<<endl<<endl;
        }
        else if(rtcos1 >= 500 && rtcos1 <1000)
        {
            double rac4;
            double rtax4;
            double rtp4;

            rac4 = 100;
            rtax4 = 0.03 * rtcos1;
            rtp4 = rtax4 + rtcos1 + rac4;
            cout<<"Total Price: "<<rtp4<<endl<<endl;
        }
        else
        {
            double rac5;
                 double rtax5;
                 double rtp5;

                 rac5 = 0;
                 rtax5 = 0;
                 rtp5 = rtax5 + rtcos1 + rac5;
                 cout<<"Total Price: "<<rtp5<<endl<<endl;
        }

        }
        else
        {
            double resi3 = 13.75;
       double rtcost2;

       rtcost2 = resi3 * cns;
       cout<<"Total Consumption: "<<cns<<endl;
       cout<<"Rate: "<<resi3<<endl;
       cout<<"tcost: "<<rtcost2<<endl;
        if (rtcost2 >=1000 )
        {
            double rac6 = 200;
               double rtax6;
               double rtp6;

               rtax6 = 0.05 * rtcost2 ;
               rtp6 = rtax6 + rtcost2 + rac6;
               cout<<"Total Price: "<<rtp6<<endl<<endl;
        }
        else if(rtcost2 >= 500 && rtcost2 <1000)
        {
            double rac7;
                double rtax7;
                double rtp7;

                rac7 = 100;
                rtax7 = 0.03 * rtcost2;
                rtp7 = rtax7 + rtcost2 + rac7;
                cout<<"Total Price: "<<rtp7<<endl<<endl;
        }
        else
        {
            double rac8;
                double rtax8;
                double tp8;

                rac8 = 0;
                rtax8 = 0;
                tp8 = rtax8 + rtcost2 + rac8;
                cout<<"Total Price: "<<tp8<<endl<<endl;
        }
      }
      cout << "Residential Type of Billing"<<endl<<endl;
    }
    //Commercial
    if (anes=='C' || anes=='c')
    {
        double prs1;
    double prv1;
    double cns1;

    cout<<"Enter Present: ";
    cin>>prs1;
    cout<<"Enter Previous: ";
    cin>>prv1;

    cns1 = prs1 - prv1;

    if (cns1 >= 300)//rate15.25
    {
       double crate1 = 15.25;
       double ctcost1;



       cout<<"Total Consumption: "<<cns1<<endl;
       cout<<"Rate: "<<crate1<<endl;
                    ctcost1 = crate1 * cns1;
                    if (ctcost1 >=1000 )
                {
                    double cac1 = 200;
                    double ctax1;
                    int ctp1;

                    ctax1 = 0.07 * ctcost1 ;
                    ctp1 = ctax1 + ctcost1 + cac1;
                    cout<<"Total Price: "<<ctp1<<endl;
                }
                    else if (ctcost1 >=500 && ctcost1 <1000)
                {
                     double cac2;
                    double ctax2;
                    int ctp2;

                    cac2 = 100;
                    ctax2 = 0.05 * ctcost1;
                    ctp2 = ctax2 + ctcost1 + cac2;
                    cout<<"Total Price: "<<ctp2<<endl;
                }
                    else
                {
                   double cac3=100;
                   double ctax3;
                   int ctp3;

                ctax3 = 0.02 * ctcost1;
                ctp3 = ctax3 + ctcost1 + cac3;
                cout<<"Total Price: "<<ctp3<<endl;
                }


    }

        else if (cns1 >= 200 && cns1 <=300)
    {
       double crate2 = 17.80;
       double ctcost2;

       ctcost2 = crate2 * cns1;
       cout<<"Total Consumption: "<<cns1<<endl;
       cout<<"Rate: "<<crate2<<endl;
       ctcost2 = crate2 * cns1;
                if (ctcost2 >=1000 )
                {
                double cac4 = 200;
                double ctax4;
                int ctp4;

                ctax4 = 0.07 * ctcost2 ;
                ctp4 = ctax4 + ctcost2 + cac4;
                cout<<"Total Price: "<<ctp4<<endl;

                }
                 else if(ctcost2 >= 500 && ctcost2 <1000)
                {
                 double cac5;
                 double ctax5;
                 int ctp5;

                 cac5 = 100;
                 ctax5 = 0.05 * ctcost2;
                 ctp5 = ctax5 + ctcost2 + cac5;
                 cout<<"Total Price: "<<ctp5<<endl;

                }
                 else
                {
                 double cac6;
                 double ctax6;
                 int ctp6;

                 cac6 = 100;
                 ctax6 = 0.02 * ctcost2;
                 ctp6 = ctax6 + ctcost2 + cac6;
                 cout<<"Total Price: "<<ctp6<<endl;


                }

    }
    else
    {
       double crate3 = 16.85;
       double ctcost3;

       ctcost3 = crate3 * cns1;
       cout<<"Total Consumption: "<<cns1<<endl;
       cout<<"Rate: "<<crate3<<endl;
       ctcost3 = crate3 * cns1;
                    if (ctcost3 >=1000 )
             {
               double cac7 = 200;
               double ctax7;
               int ctp7;

               ctax7 = 0.07 * ctcost3 ;
               ctp7 = ctax7 + ctcost3 + cac7;
               cout<<"Total Price: "<<ctp7<<endl;

            }
            else if(ctcost3 >= 500 && ctcost3 <1000)
            {
                double cac8;
                double ctax8;
                int ctp8;

                cac8 = 100;
                ctax8 = 0.05 * ctcost3;
                ctp8 = ctax8 + ctcost3 + cac8;
                cout<<"Total Price: "<<ctp8<<endl;

            }
            else
            {
                double cac9;
                double ctax9;
                int ctp10;

                cac9 = 100;
                ctax9 = 0.02*ctcost3;
                ctp10 = ctax9 + ctcost3 + cac9;
                cout<<"Total Price: "<<ctp10<<endl;


            }

    }


cout<<"Billing : Commercial "<<endl<<endl;
    }
    //Industrial
    if (anes=='I' || anes=='i')
    {
        double prs2;
    double prv2;
    double cns2;

    cout<<"Enter Present: ";
    cin>>prs2;
    cout<<"Enter Previous: ";
    cin>>prv2;

    cns2 = prs2 - prv2;

    if (cns2 >= 300)//rate15.25
    {
       double irate = 21.25;
       double itcost;



       cout<<"Total Consumption: "<<cns2<<endl;
       cout<<"Rate: "<<irate<<endl;
                    itcost = irate * cns2;
                    if (itcost >=1000 )
                {
                    double iac = 500;
                    double itax;
                    int itp;

                    itax = 0.07 * itcost ;
                    itp = itax + itcost + iac;
                    cout<<"Total Price: "<<itp<<endl;
                }
                    else if (itcost >=500 && itcost <1000)
                {
                     double iac1;
                    double itax1;
                    int itp1;

                    iac1 = 300;
                    itax1 = 0.05 * itcost;
                    itp1 = itax1 + itcost + iac1;
                    cout<<"Total Price: "<<itp1<<endl;
                }
                    else
                {
                   double iac2=200;
                   double itax2;
                   int itp2;

                itax2 = 0.02 * itcost;
                itp2 = itax2 + itcost + iac2;
                cout<<"Total Price: "<<itp2<<endl;
                }


    }

        else if (cns2 >= 200 && cns2 <=300)
    {
       double irate1 = 22.45;
       double itcost1;

       itcost1 = irate1 * cns2;
       cout<<"Total Consumption: "<<cns2<<endl;
       cout<<"Rate: "<<irate1<<endl;
       itcost1 = irate1 * cns2;
                if (itcost1 >=1000 )
                {
                double iac3 = 500;
                double itax3;
                int itp3;

                itax3 = 0.07 * itcost1 ;
                itp3 = itax3 + itcost1 + iac3;
                cout<<"Total Price: "<<itp3<<endl;

                }
                 else if(itcost1 >= 500 && itcost1 <1000)
                {
                 double iac4;
                 double itax4;
                 int itp4;

                 iac4 = 300;
                 itax4 = 0.05 * itcost1;
                 itp4 = itax4 + itcost1 + iac4;
                 cout<<"Total Price: "<<itp4<<endl;

                }
                 else
                {
                 double iac5;
                 double itax5;
                 int itp5;

                 iac5 = 200;
                 itax5 = 0.02 * itcost1;
                 itp5 = itax5 + itcost1 + iac5;
                 cout<<"Total Price: "<<itp5<<endl;


                }

    }
    else
    {
       double irate2 = 23.65;
       double itcost2;

       itcost2 = irate2 * cns2;
       cout<<"Total Consumption: "<<cns2<<endl;
       cout<<"Rate: "<<irate2<<endl;
       itcost2 = irate2 * cns2;
                    if (itcost2 >=1000 )
             {
               double iac6 = 500;
               double itax6;
               int itp6;

               itax6 = 0.07 * itcost2 ;
               itp6 = itax6 + itcost2 + iac6;
               cout<<"Total Price: "<<itp6<<endl;

            }
            else if(itcost2 >= 500 && itcost2 <1000)
            {
                double iac7;
                double itax7;
                int itp7;

                iac7 = 300;
                itax7 = 0.05 * itcost2;
                itp7 = itax7 + itcost2 + iac7;
                cout<<"Total Price: "<<itp7<<endl;

            }
            else
            {
                double iac8;
                double itax8;
                int itp8;

                iac8 = 200;
                itax8 = 0.02*itcost2;
                itp8 = itax8 + itcost2 + iac8;
                cout<<"Total Price: "<<itp8<<endl;


            }
         cout<<"Billing : Industrial "<<endl<<endl;
    }


    }

    {
        tanong:
        //system("cls");
        cout <<  "Thank you and have a nice day!"<< endl<<endl;
        cout << "   Do you want to continue [N/Y]? ";
        cin >> anes1;

         if (anes1=='Y' || anes1=='y')
        {
            goto start;
        }
        else if (anes1=='N' || anes1=='n')
        {
            goto pagwakas;
        }
        else if (anes1=='Q' || anes1=='q')
        {
            goto tanong;
        }
        else
        {
            goto pagwakas;
        }

    }


        pagwakas:
        system("cls");
        cout << endl<< "Thank you and have a nice day!"<< endl<<endl;
        cout << endl<< "Programmer: Mark Angelo De Guzman" << endl<<endl;

    return 0;
}
