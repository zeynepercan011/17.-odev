# 17.-odev

/* belli bir a��yla f�rlat�lan bir cismin yere d��me s�resini hesaplayan program� fonskiyon yard�m� ile bulunuz.
toplam s�re= 2*((ilk h�z*sin alfa)/9.80) */

#include<stdio.h>
#include<math.h>

double toplamsure(int gelenHiz, int gelenDerece);

int main(void)
{
	int ilkhiz=0;
	int derece=0;
	
	printf("cismin atildigi ilk hiz: %d \n");
	scanf("%d" , &ilkhiz);
	
	printf("cismin atildigi derece: %d \n");
	scanf("%d" , &derece);
	
	printf("yere ulastigi sure : %lf \n" , toplamsure(ilkhiz,derece));
	
	return 0;
}

double toplamsure(int gelenHiz, int gelenDerece)
{
	double sonuc= 2*((gelenHiz*(gelenDerece*M_PI))/9.80);
	
	return sonuc;
}
