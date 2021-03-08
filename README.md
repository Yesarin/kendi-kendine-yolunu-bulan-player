#include <stdio.h>
#include<Windows.h>
void ekran(int tablo[11][11])
{
	
	
	for(int i=0;i<11;i++)
	{
	
	for(int j=0;j<11;j++)
	{
	
	
	printf("|%d|",tablo[i][j]);
	}
	printf("\n");
	}
	 printf("\n");
   
}
//xxxxxxxxxxxxxxxxxxxxxxx

 int main()
 {
 
	 
 int tablo[11][11]={};
 int satir=8,sutun=1;
 int i,j;
 int skorx=0;
 int sayacx=0;
 tablo[8][1]=7;
 tablo[1][4]=5;
 tablo[2][7]=5;
 tablo[2][9]=5;
 tablo[3][2]=5;
 tablo[3][4]=5;
 tablo[3][7]=5;
 tablo[3][8]=5;
 tablo[4][5]=5;
 tablo[5][2]=5;
 tablo[5][7]=5;
 tablo[6][3]=5;
 tablo[6][5]=5;
 tablo[6][9]=5;
 tablo[7][1]=5;
 tablo[7][7]=5;
 tablo[7][8]=5;
 tablo[8][2]=5;
 tablo[8][4]=5;
 tablo[8][7]=5;
 tablo[9][4]=5;
 tablo[9][5]=5;
 for(i=0;i<11;i++)
 {
 	for(j=0;j<11;j++)
 	{
 		if(i==0||j==0||j==10||i==10)
 		tablo[i][j]=5;
 	}
 }
 
  
 
 
	
	
	for(i=0;i<11;i++)
	{
	
	for(j=0;j<11;j++)
	{

	printf("|%d|",tablo[i][j]);
	}
	
	printf("\n");
	}
	i=0;
	 printf("\n");
   
   ekran (tablo);

   
   while(skorx<70)
   {
   	if(tablo[satir-1][sutun]==0)
	   { 
   		
   		skorx++;
   		tablo[satir][sutun]=1;
   		tablo[--satir][sutun]=7;          // k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==0)
	  {
	  	
   		skorx++;
   		tablo[satir][sutun]=1;
   		tablo[satir][++sutun]=7;          // d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==0)
	  {
	  	
   		skorx--;
   		tablo[satir][sutun]=1;
   		tablo[satir][--sutun]=7;          // b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==0)
	  {
	  
   		skorx--;
   		tablo[satir][sutun]=1;
   		tablo[++satir][sutun]=7;          //g
	 	ekran(tablo);
	  }
   	
   		else if(tablo[satir-1][sutun]==1)
	   { 
   		
   		skorx++;
   		tablo[satir][sutun]=2;
   		tablo[--satir][sutun]=7;          // k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==1)
	  {
	  	
   		skorx++;
   		tablo[satir][sutun]=2;
   		tablo[satir][++sutun]=7;          // d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==1)
	  {
	  
   		skorx--;
   		tablo[satir][sutun]=2;
   		tablo[satir][--sutun]=7;          // b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==1)
	  {
	  	
   		skorx--;
   		tablo[satir][sutun]=2;
   		tablo[++satir][sutun]=7;          // g
	 	ekran(tablo);
	  }
   	if(satir==5&&sutun==9)
   	{
   		skorx+=100;
   		int a,b; 

    for (a=0;a<5;a++)
    {
    for (b=0;b<a;b++)
    {
        printf("*");
    }
    printf("\n");
    }
    printf("kazandin  %d",skorx);
   		break;
	   }
   	
   	sayacx++;
   }
    printf(" \n  %d hareket yapti",sayacx);
   
   printf(" \n x tablosu bu kadardi ");


printf("\n \n \n");


//yyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy

 
 for(i=1;i<10;i++)
 {
	for(j=1;j<10;j++)     //sıfırlama tabloyu
 	{
	 	tablo[i][j]=0;	
 	}
 }
 
 
satir=1;
sutun=1;
 
 int skory=0;
 int sayacy=0;
 tablo[1][1]=9;
 tablo[1][4]=5;
 tablo[2][7]=5;
 tablo[2][9]=5;
 tablo[3][2]=5;
 tablo[3][4]=5;
 tablo[3][7]=5;
 tablo[3][8]=5;
 tablo[4][5]=5;
 tablo[5][2]=5;
 tablo[5][7]=5;
 tablo[6][3]=5;
 tablo[6][5]=5;
 tablo[6][9]=5;
 tablo[7][1]=5;
 tablo[7][7]=5;
 tablo[7][8]=5;
 tablo[8][2]=5;
 tablo[8][4]=5;
 tablo[8][7]=5;
 tablo[9][4]=5;
 tablo[9][5]=5;
 for(i=0;i<11;i++)
 {
 	for(j=0;j<11;j++)
 	{
 		if(i==0||j==0||j==10||i==10)
 		tablo[i][j]=5;
 	}
 }
 
  
 
 
	
	
	for(i=0;i<11;i++)
	{
	
	for(j=0;j<11;j++)
	{

	printf("|%d|",tablo[i][j]);
	}
	
	printf("\n");
	}
	i=0;
   printf("\n");
   
   ekran (tablo);
  
   
   while(skory<70)
   {
   	if(tablo[satir-1][sutun]==0)
	   { 
   		
   		skory++;
   		tablo[satir][sutun]=1;
   		tablo[--satir][sutun]=9;          //k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==0)
	  {
	  	
   		skory++;
   		tablo[satir][sutun]=1;
   		tablo[satir][++sutun]=9;          //d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==0)
	  {
	  	
   		skory--;
   		tablo[satir][sutun]=1;
   		tablo[satir][--sutun]=9;          //b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==0)
	  {
	  	
   		skory--;
   		tablo[satir][sutun]=1;
   		tablo[++satir][sutun]=9;          //g
	 	ekran(tablo);
	  }
   	
   		else if(tablo[satir-1][sutun]==1)
	   { 
   		
   		skory++;
   		tablo[satir][sutun]=2;
   		tablo[--satir][sutun]=9;          //k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==1)
	  {
	  	
   		skory++;
   		tablo[satir][sutun]=2;
   		tablo[satir][++sutun]=9;          //d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==1)
	  {
	  	
   		skory--;
   		tablo[satir][sutun]=2;
   		tablo[satir][--sutun]=9;          //b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==1)
	  {
	  	
   		skory--;
   		tablo[satir][sutun]=2;
   		tablo[++satir][sutun]=9;          // g
	 	ekran(tablo);
	  }
   	if(satir==5&&sutun==9)
   	{
   		skory+=100;
   		int a,b; 

    for (a=0;a<5;a++)
    {
    for (b=0;b<a;b++)
    {
        printf("*");
    }
    printf("\n");
    }
    printf("kazandin skorun %d ",skory);
   		break;
	   }
   	
   	
   	sayacy++;
   }
   printf(" \n  %d hareket yapti",sayacy);
   
   printf(" \n y tablosu bu kadardi ");

 
printf("\n \n \n");

//zzzzzzzzzzzzzzzzzzzzzzzzzzz
 for(i=1;i<10;i++)
 {
	for(j=1;j<10;j++)     //tabloyu sıfırlama
 	{
	 	tablo[i][j]=0 ;	
 	}
 } 	 
 
 satir=1;
 sutun=9;

 int skorz=0;
 int sayacz=0;
 tablo[1][9]=8;
 tablo[1][4]=5;
 tablo[2][7]=5;
 tablo[2][9]=5;
 tablo[3][2]=5;
 tablo[3][4]=5;
 tablo[3][7]=5;
 tablo[3][8]=5;
 tablo[4][5]=5;
 tablo[5][2]=5;
 tablo[5][7]=5;
 tablo[6][3]=5;
 tablo[6][5]=5;
 tablo[6][9]=5;
 tablo[7][1]=5;
 tablo[7][7]=5;
 tablo[7][8]=5;
 tablo[8][2]=5;
 tablo[8][4]=5;
 tablo[8][7]=5;
 tablo[9][4]=5;
 tablo[9][5]=5;
 for(i=0;i<11;i++)
 {
 	for(j=0;j<11;j++)
 	{
 		if(i==0||j==0||j==10||i==10)
 		tablo[i][j]=5;
 	}
 }
 
  
 
 
	
	
	for(i=0;i<11;i++)
	{
	
	for(j=0;j<11;j++)
	{

	printf("|%d|",tablo[i][j]);
	}
	
	printf("\n");
	}
	i=0;
	 printf("\n");
   
   ekran (tablo);

   
   while(skorz<70)
   {
   	if(tablo[satir-1][sutun]==0)
	   { 
   		
   		skorz++;
   		tablo[satir][sutun]=1;
   		tablo[--satir][sutun]=8;          // k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==0)
	  {
	  	
   		skorz++;
   		tablo[satir][sutun]=1;
   		tablo[satir][++sutun]=8;          //d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==0)
	  {
	  	
   		skorz--;
   		tablo[satir][sutun]=1;
   		tablo[satir][--sutun]=8;          //  b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==0)
	  {
	  
   		skorz--;
   		tablo[satir][sutun]=1;
   		tablo[++satir][sutun]=8;          // g
	 	ekran(tablo);
	  }
   	
   		else if(tablo[satir-1][sutun]==1)
	   { 
   		
   		skorz++;
   		tablo[satir][sutun]=2;
   		tablo[--satir][sutun]=8;          // k
	 	ekran(tablo);
	  }
	  else if(tablo[satir][sutun+1]==1)
	  {
	  	
   		skorz++;
   		tablo[satir][sutun]=2;
   		tablo[satir][++sutun]=8;          //d
	 	ekran(tablo);
	  }
	   else if(tablo[satir][sutun-1]==1)
	  {
	  
   		skorz--;
   		tablo[satir][sutun]=2;
   		tablo[satir][--sutun]=8;          //  b
	 	ekran(tablo);
	  }
	   else if(tablo[satir+1][sutun]==1)
	  {
	  	
   		skorz--;
   		tablo[satir][sutun]=2;
   		tablo[++satir][sutun]=8;          // g
	 	ekran(tablo);
	  }
   	if(satir==5&&sutun==9)
   	{
   		skorz+=100;
   		int a,b; 

    for (a=0;a<5;a++)
    {
    for (b=0;b<a;b++)
    {
        printf("*");
    }
    printf("\n");
    }
    printf("kazandin  %d",skorz);
   		break;
	   }
   	sayacz++;
   	
   }
    printf(" \n z yani 8-->  %d hareket yapti",sayacz);
   
   printf(" \n z tablosu bu kadardi\n \n \n ");

if(skorx>skory&&skorx>skorz)
{
	printf("x oyunu %d puanla birincilikle bitirdi \n",skorx);
	printf("\n");
	if(skory>skorz)
	{
		printf("y oyunu %d puanla ikincilile bitirdi \n",skory);
			printf("\n");
		printf("z oyunu %d puanla ucunculukle bitirip oyunu son kazanan oldu yani kaybetti",skorz);
	printf("\n");

	}
	else if(skorz>skory)
	{
		printf("z oyunu %d puanla ikincilile bitirdi",skorz);
			printf("\n");
		printf("y oyunu % puanla üçüncülükle bitirip oyunu son kazanan oldu yani kaybetti",skory);
	printf("\n");
	}
}
else if(skory>skorz)
{
	printf("y oyunu %d puanla birincilikle bitirdi",skory);
		printf("\n");
	if(skorx>skorz)
	{
		printf("x oyunu %d puanla ikincilile bitirdi",skorx);
			printf("\n");
		printf("z oyunu % puanla üçüncülükle bitirip oyunu son kazanan oldu yani kaybetti",skorz);
	printf("\n");
	}
	else if(skorz>skorx)
	{
		printf("z oyunu %d puanla ikincilile bitirdi",skorz);
			printf("\n");
		printf("x oyunu % puanla üçüncülükle bitirip oyunu son kazanan oldu yani kaybetti",skorx);
	printf("\n");
	}

}
else
{
printf(" z oyunu %d puanla birincilikle bitirdi",skorz);
	printf("\n");
	if(skorx>skory)
	{
		printf("x oyunu %d puanla ikincilile bitirdi",skorx);
			printf("\n");
		printf("y oyunu % puanla üçüncülükle bitirip oyunu son kazanan oldu yani kaybetti",skory);
	printf("\n");
	}
	else if(skory>skorx)
	{
		printf("y oyunu %d puanla ikincilile bitirdi",skory);
		printf("\n");
		printf("x oyunu % puanla üçüncülükle bitirip oyunu son kazanan oldu yani kaybetti",skorx);
	printf("\n");
	}
	
}



}
