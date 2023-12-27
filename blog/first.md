# Markdown使用教程
## 以下是二级标题使用教程
### 三个就是三级标题
```cpp
#include<bits/stdc++.h>
using namespace std;

int n,m,q,a[1000005];

int find(int x) //二分查找 
{
	int l=1,r=n;
	while (l<r)
	{
		int mid=l+(r-l)/2;
		if (a[mid]>=x) r=mid;
		else l=mid+1;
	}
	
	if (a[l]==x) return l; //找都了就输出他的位置 
	else return -1; // 没找到输出-1 
}

int main()
{
	scanf("%d %d",&n,&m); //读入 
	
	for (int i=1 ; i<=n ; i++)
	    scanf("%d",&a[i]); //还是读入 
	
	for (int i=1 ; i<=m ; i++)
	{
		scanf("%d",&q);
		int ans=find(q); //看看查找的结果 
		printf("%d ",ans); //输出 
	}
	system("pause");
	return 0;
}
``````
有序列表
1. 哈哈哈
2. 有道理
   
无序列表
- 有道理
- 没道理啊
- 我靠markdown牛逼