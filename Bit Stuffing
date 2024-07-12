#include <stdio.h>
#include <conio.h>
#include <string.h>

void main()
{
int x[50], y[50], n; int i, j, k, count = 1;
printf("Enter bit string size:");
scanf("%d", &n);
printf("Enter the bits string 0 and 1:");
for (i = 0; i < n; i++)
{
scanf("%d", &x[i]);
}

i = 0;
j = 0;

while (i < n)
{
if (x[i] == 1)
{
y[j] = x[i];
for (k = i + 1; x[k] == 1 && k < n && count < 5; k++)
{
j++;
y[j] = x[k]; count++;

if (count == 5)
{
j++; y[j] = 0;
}
i = k;
}
}
else
{
y[j] = x[i];
}
i++;
j++;
}
printf("RESULT OF THE BIT STUFFING:");
for (i = 0; i < j; i++)
{
printf("%d", y[i]);
}
getch();
}
