---
layout: post
title: Tugas Tipe Data Turunan (Larik/Array)
comments: true
permalink: tugas-larik-atau-array
---

1. Buatlah program yang menghitung jumlah elemen dalam suatu array (larik) dengan array (larik) 1 dimensi {1,3,5,4,7,2,99,16,45,67,89,45}
2. Buatlah program untuk menampilkan data mahasiswa yang terdiri dari nim dan nama (minimal data adalah 5 data)

## Menghitung Jumlah Elemen Array atau Larik
{% highlight c %}
#include<stdio.h>
int main()
{
	int e,k=0,a[12]={1,3,5,4,7,2,99,16,45,67,89,45};
	for (e=0; e<=11; e++)
	{
		k=k+a[e];
	}
	printf ("Jumlah data = %d\n", k);
	return 0;
}
{% endhighlight %}
{% highlight html %}
[~]-> cd tugas/
[~/tugas]-> ./array1
Jumlah elemen = 383
{% endhighlight %}

## Menampilkan Data Mahasiswa NIM dan Nama
{% highlight c %}
#include<iostream>
#include<string>
#include<iomanip>
using namespace std;
int main()
{
	string nama[5] = {"Eka Putra","Suryana","Dodi Riyanto","Kuswanto","Nunu"};
	int nim[5] = {2014081049, 2014081050, 2014081051, 2014081052, 2014081053};
	cout<<"---------------------------"<<endl;
	cout<<setw(12)<<"Nama"<<"	NIM"<<endl;
	cout<<"---------------------------"<<endl;
		for (int x=0; x<=4; x++)
		{
		cout<<setw(12)<<nama[x]<<"	";
		cout<<nim[x]<<endl;
		}
	cout<<"---------------------------"<<endl;
	return 0;
}
{% endhighlight %}
{% highlight html %}
[~]-> cd tugas/
[~/tugas]-> ./array2
---------------------------
        Nama	NIM
---------------------------
   Eka Putra	2014081049
     Suryana	2014081050
Dodi Riyanto	2014081051
    Kuswanto	2014081052
        Nunu	2014081053
---------------------------
{% endhighlight %}

Happy Programming!
