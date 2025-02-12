# programing_study

```c
//등비수열 n 번 째 수 구하기
#include <stdio.h>

int func(int a, int r, int n){
    long long int cnt=1;
    for(int i=0;i<n-1;i++){
        cnt*=r;
    }
    return a*cnt;
}
int main()
{
    int a,r,n;
    scanf("%d %d %d",&a,&r,&n);
    printf("%d",func(a,r,n));
    return 0;
}
```

```c
// 수열에서 a*m+d n 번 반복하기
#include <stdio.h>

int func(int a, int m, int d, int n){
    long long int cnt=1;
    for(int i=0;i<n-1;i++){
        cnt*=m;
        cnt+=d;
    }
    return a*cnt;
}
int main()
{
    int a,m,d,n;
    scanf("%d %d %d %d",&a,&m,&d,&n);
    printf("%d",func(a,m,d,n));
    return 0;
}
```
