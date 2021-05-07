#include <time.h>
#include<stdio.h>
#pragma warning(disable:4996)
#include <Windows.h> 
#include <conio.h>

void gotoxy(int x, int y)
{
	COORD CursorPosition = { x, y };
	SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE), CursorPosition);
}


int main()
{
	system("mode con: cols=16 lines=16");
	int x = 7, y = 7, a, b,x1=12,y1=12,t;
	char ch;





	while (1)
	{
		if (x==x1&&y==y1)
		{
			break;
		}
		if (7+x1-x>0&&7+x1-x<15&&7+y1-y>0&&7+y1-y<15)
		{
			gotoxy(7 + x1 - x, 7 + y1 - y);
			printf("ㅁ");
		}
		rand(time(0));
		t = rand() % 4;

		if (t == 0 && y1 < 14)
		{
			y1++;
		}
		else if (t == 1 && y1> 1)
		{
			y1--;
		}
		else if (t == 2 && x1 > 1)
		{
			x1--;
		}
		else if (t == 3 && x1 < 14)
		{
			x1++;
		}

		if (x <= 7)
		{
			for (a = 0; a < 16; a++)
			{
				for (b = 0; b < 16; b++)
				{
					if (a == 7 - x && y <= 7 && b >= 7 - y)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (a == 7 - x && y >= 12 && b <= 27 - y)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (a == 7 - x && y > 7 && y < 12)
					{
						gotoxy(a, b);
						printf("0");
					}
				}
			}
		}
		else if (x >= 12)
		{
			for (a = 0; a < 16; a++)
			{
				for (b = 0; b < 16; b++)
				{
					if (a == 27 - x && y <= 7 && b >= 7 - y)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (a == 27 - x && y >= 12 && b <= 27 - y)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (a == 27 - x && y > 7 && y < 12)
					{
						gotoxy(a, b);
						printf("0");
					}
				}
			}
		}
		if (y <= 7)
		{
			for (a = 0; a < 16; a++)
			{
				for (b = 0; b < 16; b++)
				{
					if (b == 7 - y && x <= 7 && a >= 7 - x)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (b == 7 - y && x >= 12 && a <= 27 - x)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (b == 7 - y && x > 7 && x < 12)
					{
						gotoxy(a, b);
						printf("0");
					}
				}
			}
		}
		else if (y >= 12)
		{
			for (a = 0; a < 16; a++)
			{
				for (b = 0; b < 16; b++)
				{
					if (b == 27 - y && x <= 7 && a >= 7 - x)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (b == 27 - y && x >= 12 && a <= 27 - x)
					{
						gotoxy(a, b);
						printf("0");
					}
					else if (b == 27 - y && x > 7 && x < 12)
					{
						gotoxy(a, b);
						printf("0");
					}
				}
			}
		}

		gotoxy(7, 7);
		printf("*");
		ch = getch();
		gotoxy(x, y);
		switch (ch)
		{
		case 'w':if (y > 1) { y--; break; }
		case 's':if (y < 19) { y++; break; }
		case 'a': if (x > 1) { x--; break; }
		case 'd':if (x < 19) { x++; }
		}

		system("cls");

	}
	gotoxy(0, 0);
	printf("GAME OVER");



	return 0;
}
