#include <bits/stdc++.h>
#include<string>
#define sz(v)   ((int)(v).size())
#define  eps      0.0000000001
#define  all(v)    ((v).begin()),((v).end())
#define  allr(v)    ((v).rbegin()),((v).rend())
#define   pb         push_back
#define   mp         make_pair
#define   inf        0x7fffffff
#define    PI        3.1415926536
#define    clr(v,d)      memset( v, d ,sizeof(v))
#define    vi       vector<int>
#define    vd       vector<double>
#define    vvi      vector< vector<int> >
#define    vvpi     vector< vector< pair<int,int> > >
#define    vvpll     vector< vector< pair<long long,long long> > >
#define    vvd      vector< vector<double> >
#define    vs       vector<string>
#define    vvs      vector< vector<string> >
#define     vc        vector<char>
#define     vpi        vector< pair<int ,int> >
#define      pi        pair<int ,int>
#define      pll       pair<long long ,long long>
#define     vpd        vector< pair<double ,double> >
#define     vpll        vector< pair<long long ,long long> >
#define    vll       vector<long long>
#define    dqi        deque< int >
#define     si         set<int>
#define     spi        set< pair<int ,int > >
#define     row          vector< ll >
#define     matrix            vector< row >
#define    lp(i,n)    for(i=0;i<n;i++)
#define     si         set<int>
#define    oo         100000000000
#define   MOD         1000000007
#define    X            real
#define    Y            imag
#define   angle(n)      atan2((n.imag()),(n.real()))
#define   vec(a,b)       ((b)-(a))
#define   length(a)      hypot( (a.imag()),(a.real()) )
#define   normalize(a)      (a)/(length(a))
#define    dp(a,b)          (((conj(a))*(b)).real())
#define    cp(a,b)          (((conj(a))*(b)).imag())
#define    lengthsqrt(a)       dp(a,a)
#define    rotate0( a,ang)    ((a)*exp( point(0,ang) ))
#define    rotateA(about,p,ang)   (rotate0(vec(about,p),ang)+about)
#define    lcm(a,b)                ((a*b)/(__gcd(a,b)))
#define    reflection0(m,v)         (conj((v)/(m))*(m))
#define     reflectionA(m,v,p0)     (conj( (vec(p0,v))/(vec(p0,m)) ) * (vec(p0,m)) ) + p0
#define     same(p1,p2)               ( dp(  vec(p1,p2),vec(p1,p2)) < eps )
#define     point                    complex<double>
#define    scani(n)                  scanf("%d",&n)
#define    scanll(n)                  scanf("%I64d",&n)
#define    printi(n)                 printf("%d",n)
#define    printll(n)                 printf("%I64d",n)
#define    scand(n)                  scanf("%lf",&n)
#define    printd(n)                 printf("%lf",n)
#define    scans(n)                  scanf("%s",&n)
#define    prints(n)                 printf("%s",n)
typedef  long long     ll ;
typedef  unsigned long long ull;
using namespace std;
int dcmp(double a,double b){   return fabs(a-b)<=eps ? 0: (a>b)? 1:-1 ;}
 
vpi v1;
 
int main()
{
    int t;
 
  cin>>t;
 
  while(t--)
  {
 
      v1.clear();
 
      int no,m,n,i,s=0,v=1,h=1,val,d;
 
      cin>>m>>n;
 
 
 
 
 
 
 
      for(i=0;i<m-1;i++)
      {
          cin>>no;
          v1.pb(mp(no,1));
 
 
 
      }
      for(i=0;i<n-1;i++)
      {
          cin>>no;
          v1.pb(mp(no,0));
      }
 
 
      sort(allr(v1));
 
 
      for(i=0;i<sz(v1);i++)
      {
        val=v1[i].first;
        d=  v1[i].second ;
 
 
 
 
 
          if(d==0)
           {
              s+=(val*v);
              h++;
           }
          else if(d==1)
          {
            s+=(val*h);
            v++;
          }
 
 
 
 
 
 
 
      }
 
 
 
 
      cout<<s<<endl;
  }
 
}
 
