# Tugas-Alpro
2008561106

6.	#include <stdio.h>
#define tglsekarang 16
#define blnsekarang 02
#define thnsekarang 2021

int main(){
	char nama[50],kls[10],almt[100],no[20];
	long nim; 
	int  umur, a, a1, a2, tgl, bln, thn;
    
    printf("Nama 		:");
    scanf("%[^\n]s",&nama);
	printf("NIM  		:");
	scanf("%ld",&nim);
	printf("Kelas		:");
	fflush(stdin);
	scanf("%s",&kls);
	fflush(stdin);
	printf("Alamat		:");
	scanf("%[^\n]s",&almt);
	printf("No HP 		:");
	scanf("%s",&no);
	fflush(stdin);
	printf("Tanggal Lahir (dd-mm-yyyy)	:");
	scanf("%d-%d-%d",&tgl,&bln,&thn); 
	a1 = tgl + ( bln * 31 ) + ( thn * 365 );
	a2 = tglsekarang + ( blnsekarang * 31 ) + ( thnsekarang * 365 );
	a = a2 - a1;
	umur = a / 365;
	printf("********************TERIMAKASIH TELAH MENDAFTAR!********************\n");
	
	printf("\nNama		: %s\n",nama);
	printf("NIM		: %ld\n",nim);
	printf("Kelas		: %s\n",kls);
	printf("Alamat		: %s\n",almt);
	printf("No HP		: %s\n",no);
	printf("Tanggal lahir : %d-%d-%d\n",tgl,bln,thn);
	printf("Umur : %d tahun", umur);
return 0;
}

