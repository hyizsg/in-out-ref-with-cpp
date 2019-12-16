# C++实现参数in、out、ref语义

```
#include <string>
#include <vector>
using namespace std;

#define IN      const&
#define OUT     &
#define REF     &

void test(string IN str, vector<int> REF vec, vector<int> OUT outvec)
{
    // TODO...
}

```


大小写是为了避免跟std内部的定义冲突。

按c++的宏展开，`string IN`其实就是`string const&`，经我在xcode里测试，和`const string&`是一样的，在监视窗口看到的都是`const string&`类型。

如果有兴趣，可以在自己的项目里面试试

欢迎留言交流~


------

# C++ implement in、out、ref

```
#include <string>
#include <vector>
using namespace std;

#define IN      const&
#define OUT     &
#define REF     &

void test(string IN str, vector<int> REF vec, vector<int> OUT outvec)
{
    // TODO...
}

```


The case is to avoid conflicts with definitions inside std.

Expanding according to the C ++ macro, `string IN` is actually `string const &`. After testing in xcode, it is the same as `const string &`. I see all types of `const string &` in the watch window.

If you are interested, you can try it in your own project

