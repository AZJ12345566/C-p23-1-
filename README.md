# C-p23-1-
C 语言学习笔记 p23 作业详解(1)
#include<stdio.h>
void Init(int arr[],int sz)
{
  int i=0;
  for(i=0;i<sz;i++)
  {
    arr[i]=0;
  }
}
void Print(int arr[],int sz)
{
  int i=0;
  for(i=0;i<sz;i++)
  {
      printf("%d",arr[i]);
  }
  printf("/n");
}
void Reverse(left<right)
{
    int left=0;
    int right=sz-1;
    while()
    {
      int tmp=arr[left];
      arr[left]=arr[right];
      arr[right]=tmp;
      left++;
      right--;
    }
}
int main()
{
    int arr[10]={1,2,3,4,5,6,7,8,9,10};
    int sz=sizeof(arr)/sizeof(arr[0]);
    Init(arr,sz);//把数组初始化为0
    Print(arr,sz);
    Reverse(arr,sz);
    Print(arr,sz);
    return 0;
}

int mian()
{
    int arr1[]={1.3.5.7.9};
    int arr2[]={2,4,6,8,0};
    int tmp=0;
    int i=0;
    int sz=sizeof(arr)/sizeof(arr[0]);
    for(i=0;i<sz;i++)
    {
      tmp=arr1[i];
      arr1[i]=arr2[i];
      arr2[i]=tmp;
    }
}

int i;//全局变量不初始化-默认为0
int main()
{
    i--;
    if(i>sizeof(i))//sizeof()-计算变量/类型所占内存的大小 >=0 返回无符号数，所以这里为-1
    {
        printf(">\n");
    }
    else
    {
        printf("<\n");
    }
}

int main()
{
    int a,b,c;
    a=5;
    c=++a;
    b=++c,c++,++a,a++;
    b+=a++ + c;
    printf("a=%d b=%d c=%d\n",a,b,c);
    return 0;
}//输出为9，23，8
