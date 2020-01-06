#if !defined _CRT_SECURE_NO_WARNINGS
	#define _CRT_SECURE_NO_WARNINGS
#endif
#include <stdio.h>
#include <stdlib.h>

int linearSearch(int* a, int key, int imin, int imax)
{
	for (int i = imin; i <= imax; i++)
	{
		if (a[i] == key)
			return i;

	}
	
	return -1;

}



int main()
{

	int* arr = NULL;
	int num, key, loc;

	printf("How many numbers: ");
	scanf("%d", &num);

	arr = (int*)malloc(6 * sizeof(int));
	printf("Enter the numbers: ");
	for (int k = 1; k <= num; k++)        // hier wordt de arr array gevuld met integers
	{
		scanf("%d", &arr[k]);
	}

	printf("Enter a search key: ");
	scanf("%d", &key);
	
	loc = linearSearch(arr, key, 1, num);

	if (loc == -1)
	{
		printf("Key not found.\n");
	}
	else 
	{
		printf("Key found at position: %d\n", loc);
	}

	free(arr);
	arr = NULL;
	printf("Check if array: %d, and mem location %p have been succesfully freed.", arr, arr);
	return 0;
}
