# linked-list

//sap_xep_tang_dan

# include <iostream>
using namespace std;
int main()
{
    int n;
    cin >> n ;
    int f[n];
    for (int i=0; i<=n-1;i++)
    {
        cin >> f[i];
    }
    int T;
    for (int j=n-1;j>=1;j--)
    {
    for (int i=0; i<=j;i++)
        {
           if (f[i]>f[i+1]) 
              {
                 T=f[i+1];
                 f[i+1]=f[i];
                 f[i]=T;
             }
        }
    }
    for (int i=0;i<=n-1;i++)
    {
        cout << f[i] << ' ' ;
    }
    return 0;
}

//doi_cho_2_phan_tu_x_va_y

# include <iostream>
using namespace std;
int main(){
    int n;
    cin >> n;
    int f[n];
    for (int i=0;i<=n-1;i++){
        cin >> f[i];
    }
    int x,y;
    cin >> x >> y;
    int T=0;
    T=f[x-1];
    f[x-1]=f[y-1];
    f[y-1]=T;
    for (int i=0;i<=n-1;i++){
        cout <<f[i] << ' ';
    }
    return 0;
}

//
