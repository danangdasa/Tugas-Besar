#include <stdio.h>
#include <conio.h>
#include <iostream>
using namespace std;

main(){
    long int No_iden;
    int Jur,Kel,Pen;
    char nama[50];
    float Harga;

    cout<<"\n\t=======================================================\n";
    cout<<"\t      SELAMAT DATANG PEMESANAN TIKET KERETA API        \n";
    cout<<"\t    PEMESANAN KHUSUS PEMBERANGKATAN DARI PURWOKERTO    \n";
    cout<<"\t=======================================================\n\n";

    cout<<"\t Jumlah Penumpang :";
    cin>>Pen;
    cout<<"\n\n";
    cout<<"\t=================\n";
    cout<<"\t     Tujuan   \n";
    cout<<"\t=================";
    cout<<endl;
    cout<<"\t| 1.Cirebon\t|   \n";
    cout<<"\t| 2.Jakarta\t|\n";
    cout<<"\t| 3.Semarang\t|\n";
    cout<<"\t| 4.Surabaya\t|\n";
    cout<<"\t| 5.Yogyakarta\t|\n";
    cout<<"\t=================\n";
    cout<<"\tPilih[1-5]: ";
    cin>>Jur;

    cout<<"\t=================\n";
    cout<<"\t     Kelas       \n";
    cout<<"\t=================";
    cout<<endl;
    cout<<"\t| 1.Bisnis\t|   \n";
    cout<<"\t| 2.Ekonomi\t|\n";
    cout<<"\t| 3.Eksekutif\t|\n";
    cout<<"\t=================\n";
    cout<<"\tPilih[1-3]: ";
    cin>>Kel;

    cout<<"\t=================\n";
    cout<<"\t  Data Penumpang  \n";
    cout<<"\t=================";
    cout<<"\n";
    for(char i=1;i<=Pen;i++){
    cout<<"\tNama Lengkap : ";
    cin>>nama;
    cout<<"\tNo Identintas : ";
    cin>>No_iden;
    }
    {
    cout<<"\n\n";
    cout<<"\t==================================\n";
    cout<<"\t Tiket Kereta Api Yang Anda Pesan  \n";
    cout<<"\t==================================";
    cout<<"\n";
    cout<<"\t Nama  Lengkap     :"<<nama<<"\n";
    cout<<"\t No Identitas      :"<<No_iden<<"\n";

    cout<<"\t Tujuan            :";
    if(Jur==1){
    cout<<"Cirebon\n";
    } else if(Jur==2){
        cout<<"Jakarta\n";
    } else if(Jur==3){
        cout<<"Semarang\n";
    } else if(Jur==4){
        cout<<"Surabya\n";
    } else if(Jur==5){
        cout<<"Yogyakarta\n";
    } else{
        cout<<"Maaf yang anda inputkan salah\n";
    }
    cout<<"\t Kelas Kereta      :";
    if(Kel==1){
    cout<<"Bisnis\n";
    } else if(Kel==2){
        cout<<"Ekonomi\n";
    } else if(Kel==3){
        cout<<"Eksekutif\n";
    }  else{
        cout<<"Maaf yang anda inputkan salah\n";
    }
    cout<<"\t Jumlah Penumpang  :"<<Pen<<"\n";
    cout<<"\t Harga Tiket       :";
    switch(Kel){
    case 1:
        Harga = 250000*Pen ;
        cout<<"Rp "<<Harga ;
    break;
    case 2:
        Harga = 150000*Pen ;
        cout<<"Rp "<<Harga ;
    break;
    case 3:
        Harga = 350000*Pen ;
        cout<<"Rp "<<Harga ;
    break;
    default:
    break;
    }
    }


}
