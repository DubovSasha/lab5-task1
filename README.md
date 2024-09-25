# lab6-task1
#include <locale.h>
#include <stdio.h>

int main()
{
	setlocale(LC_ALL, "RUS");
	int yeas, res1, res2 ;
	puts("Введите какой сейчяас год");
	scanf("%d", &yeas);
	res1  = yeas % 4;
	res2  = yeas % 100;
	if (((res1 == 0) && (res2 != 0)) || ((yeas % 400) == 0))
	{
		printf ("Год %d - высикосный", yeas);
	}
	else printf ("Год %d - не высикосный", yeas);
