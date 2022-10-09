# 8
试题，时间紧，小卷



//打印闰年 1000——2000
int main()
{
	int year = 0;
	int count = 0;
	for (year = 1000; year <= 2000; year++)
	{
		//判断year是否为闰年
		//1、能被4整除并且不能被100整除是闰年
		//2、能被400整除是闰年
		if (year % 4 == 0 && year % 100 != 0)
		{
			printf("%d ", year);
				count ++;
		}
		else if (year % 400 == 0)
		{
			printf("%d ", year);
				count ++;
		}
	}
	printf("\ncount=%d\n", count);
	printf("%d", year);
}
//加入了count可以知道有多少个闰年



打印素数100-200
int main()
{
	int i = 0;
	int count = 0;
	for (i = 100; i <= 200; i++)
	{
		//判读i是否为素数
		//素数判断的规则
		//1.试除法
		//产生2->i-1
		int j = 0;
		for (j = 2; j < i; j++)
		{
			if (i % j == 0)
			{
				break;
			}
		}
		if (j == i)
		{
			count++;
			printf("%d", i);
		}
	}
	printf("\ncount=%d\n", count);
	return 0;
}
