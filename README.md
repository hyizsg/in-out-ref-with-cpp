# C++实现参数in、out、ref语义

```
using namespace std;

#define IN      const&
#define OUT     &
#define REF     &

void test(string IN str, vector<int> REF vec, vector<int> OUT outvec)
{
    // TODO...
}

```
