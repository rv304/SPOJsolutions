[Problem Statement][1]


`

## C code

    #include<stdio.h>
    #include<math.h>
    int main()
    {
    int a[12],i,b,c,count;
    for(i=0;i<12;i++)
    a[i]=pow(5,i+1);
    scanf("%d",&b);
    while(b)
    {count=0;
    scanf("%d",&c);
    count=c/5;
    for(i=1;i<12;i++)
    count+=c/a[i];
    printf("%d\n",count);
    b--;
    }
    return 0;
    }
## C++ code ##

    #include<iostream>
    #include<math.h>
    using namespace std;
    
    int main()
    {
    int a[12],i,b,c,count;
    for(i=0;i<12;i++)
    a[i]=pow(5,i+1);
    cin>>b;
    while(b)
    {count=0;
    cin>>c;
    count=c/5;
    for(i=1;i<12;i++)
    count+=c/a[i];
    cout<<count<<endl;
    b--;
    }
    return 0;
    }
    
> Written with [StackEdit](https://stackedit.io/).


  [1]: http://www.spoj.com/problems/FCTRL/