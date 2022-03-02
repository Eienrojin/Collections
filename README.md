# Collections
Задание 16
Ввести целочисленный массив, состоящий из 10 элементов. 
Определить сумму и количество элементов, расположенных до первого отрицательного числа.

Листинг
Random random = new();
List<int> myList = new();

int sum = 0;
int count = 0;

for (int i = 0; i < 15; i++)
{
    myList.Add(random.Next(-5, 15));
    Console.WriteLine($"{i + 1}. {myList[i]}");
}

for (int i = 0; i < 10; i++)
{
    if(myList[i] > 0)
    {
        sum += myList[i];
        count++;
    }
    else
    {
        break;
    }
}

Console.WriteLine($"Sum = {sum}" +
                  $"\nCount = {count}");
