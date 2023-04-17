# ItogoviProekt-Алгоритм решения:
Делаем перебор значений из исходного массива
Проверяем каждое значение из массива на соответствие условию: длина строки меньше или равна трем
Если строка удовлетворяет условию кладем значение в новый массив
Повторяем пункты 2 и 3 до тех пор пока не достигнем конца исходного массива
Возвращаем новый заполненый массив как результат



Kod: 
string[] array1 = new string[5] {"123", "23", "hello", "world", "res"};
string[] array2 = new string[array1.Length];
int count = 0;
void SecondArrayWithIF(string[] array1, string[] array2)
{
    int count = 0;
    for (int i = 0; i < array1.Length; i++)
    {
    if(array1[i].Length <= 3)
        {
        array2[count] = array1[i];
        count++;
        }
    }
}
void PrintArray(string[] array)
{
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"{array[i]} ");
    }
    Console.WriteLine();
}
SecondArrayWithIF(array1, array2);
PrintArray(array2);


![Блоксхема](https://user-images.githubusercontent.com/131005853/232521260-3c664d27-e56f-4b04-91e3-893f64459b19.png)
