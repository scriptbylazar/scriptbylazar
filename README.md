int[] Tomb = { 22, 5, 4, 2 };
int n = Tomb.Length;
int asd;
for (int k = 0; k < n; k++)
{
    Console.Write($"{a[k]}, ");
}
    for (int i = n - 1; i > 0; i--) //for (int i=0;i<n-1;i++)
    {
        for (int j = 0; j < i; j++) //for (int j=i+1;j<n;j++)
        {
            if (a[j] > a[j + 1]) // if(a[i] > a[j])
        {
                asd = a[j];
                a[j] = a[j + 1]; //a[j] = a[i];
                a[j + 1] = asd; //a[i] = asd;
        }
    }
}
for (int k = 0; k < n; k++)
{
    Console.Write(a[k] + ", ");
