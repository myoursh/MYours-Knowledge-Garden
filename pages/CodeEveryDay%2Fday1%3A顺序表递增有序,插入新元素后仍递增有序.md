title:: "CodeEveryDay/day1:顺序表递增有序,插入新元素后仍递增有序"

- 问题描述
	- ```c++
	  #include<iostream>
	  using namespace std;
	  #define Maxsize 100
	  typedef struct
	  {
	      int data[Maxsize];
	      int length;
	  }Sqlist;
	  
	  
	  void Insert(Sqlist &L,int x)
	  {
	      int i=0;
	      for(;i<L.length & x>L.data[i];i++)
	      {
	      }
	  /*     for(;i<L.length;++i)
	      {	
	          if(x<L.data[i])
	          {
	              break;
	          }
	      } */
	      for(int j=L.length-1;j>i-1;j--)
	      {
	          L.data[j+1]=L.data[j];
	      }
	      L.data[i]=x;
	      ++(L.length);
	  }
	  
	  int main()
	  {
	    Sqlist L = {{1, 3, 5, 8, 9}, 5};//初始化方式
	    Insert(L, 6);
	    for (int j = 0; j < L.length; ++j)
	      cout << L.data[j] << endl;
	  }
	  ```