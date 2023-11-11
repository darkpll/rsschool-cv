# MYCV 
## About me
> **Hello I'm Ramazan Salahov. I'm a student and I love programming.**
## Contact
> - My email: **style_gg@vk.com**
> - My spotify: **style_gg**
## My goals
> Learn to program in React, TypeScript and C#. I want to start speaking English better.
## My skills
> - HTML
> - CSS
> - Figma
> - TailwindCSS
> - Basic C#
> - Basic JS
> - PHP
> - Basic Python
> - PostgreSQL
## Code Examples
```
using System;

namespace WorkWithArrays
{
    class Program
    {

        static void Resize(ref int[] arr, int count)
        {
            arr = new int[count];
        }

        static void Insert(ref int[] arr, int value, int index)
        {
            int[] newArray = new int[arr.Length + 1];
            newArray[index] = value;


            for (int i = 0; i < index; i++)
                newArray[i] = arr[i];
            for (int i = index; i < arr.Length; i++)
                newArray[i + 1] = arr[i];

            arr = newArray;
        }

        static void AddFirst(ref int[] arr, int value)
        {
            Insert(ref arr, value, 0);
        }

        static void AddLast(ref int[] arr, int value)
        {
            Insert(ref arr, value, arr.Length);
        }

        static void RemoveAt(ref int[] arr, int value, int index)
        {
            int[] newArray = new int[arr.Length - 1];

            for (int i = 0; i < index; i++)
                newArray[i] = arr[i];
            for (int i = index + 1; i < arr.Length; i++)
                newArray[i - 1] = arr[i];

            arr = newArray;
        }

        static void DeleteFirst(ref int[] arr, int value)
        {
            RemoveAt(ref arr, value, 0);
        }

        static void DeleteLast(ref int[] arr, int value)
        {
            RemoveAt(ref arr, value, arr.Length - 1);
        }

        static void Main(string[] args)
        {
            int[] myArray = { 10, 3, 6, 8, 1 };

            AddFirst(ref myArray, -28);
            AddLast(ref myArray, -3);
        }
    }
}
```

