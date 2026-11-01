代发 wailian999

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gteyjchvh.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gkxwzhesk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gudezstsd.sHtML

[R79] 解析命令行选项
来源：http://blog.yfazqb.com/Article/details/gjmbkpflz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/ggubgjojo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/grtyhffvy.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gmbhvnxks.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gkxypiqjd.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/gzezeylzd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnatytffr.sHtML

[S01] C：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/grqvtchki.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gcalauwyz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/ggdedynxc.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gursfwnjo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gbnneoncx.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gdbuvogff.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.yfazqb.com/Article/details/gzdczwgwd.sHtML

[S04] C：字符串复制
来源：http://www.m.share.tarul.cn/Article/details/gnabcmkti.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gigsjtwys.sHtML

[S05] C：字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoqeiqyx.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gkqswfvme.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gkuoimnic.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gotgujkuc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gkgscwmop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/glwwiyedc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.yfazqb.com/Article/details/gsxrzalqu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.epnwcf.com/Article/details/gaxcscibr.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gvevbsrer.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.yfazqb.com/Article/details/ghncqgcgy.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/glmjbyasg.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/gbdzymbda.sHtML

[S11] C：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/ggfosqydj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.bbcook.cn/Article/details/gbxqyqxcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gzoeohwmq.sHtML

fclose(f);
来源：http://read.share.fktsv.cn/Article/details/gevyazuzz.sHtML

[S12] C：写文件
来源：http://www.blog.tarul.cn/Article/details/gcmqqmtvj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/glgrjoorh.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/gbfjgluon.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/goimdpxzk.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/ggfyyhpne.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gmdrkxgif.sHtML

[S15] C：类型转换
来源：http://baike.vehdjk.com/Article/details/glmvwmovn.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/grrstrvuc.sHtML

[S16] C：位操作置位
来源：http://wap.yfazqb.com/Article/details/gcmgheiix.sHtML

x |= (1 << 3);
来源：http://www.blog.fktsv.cn/Article/details/gabvcirxc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwjoaegvb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gchszgqev.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gsxsoauks.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gtdzvzifx.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gigrdkpac.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gikvxmxco.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gckgzjlws.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/grgugroza.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gkyklhdts.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.vehdjk.com/Article/details/gsbeksiha.sHtML

[S22] C：字符串转数字
来源：http://blog.yfazqb.com/Article/details/guzojbzqx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/ghyjxhqfa.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/ggctazqdy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gpaffybkn.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gdfrxpxnc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gieuhhzvh.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gdjfugapl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gaqvwurzq.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/guifllpjs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gsrvbcmzm.sHtML

[S27] C：定义常量
来源：http://3g.epnwcf.com/Article/details/gujeyotav.sHtML

const double PI = 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gerswpzte.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/ghprvucxs.sHtML

static int counter = 0;
来源：http://m.share.sjlbkw.cn/Article/details/ggwfropbe.sHtML

[S29] C：变参函数
来源：http://blog.tarul.cn/Article/details/gfgivjhzw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gcfmvrzqv.sHtML

[S30] C：头文件保护
来源：http://wap.bbcook.cn/Article/details/gdyiandgh.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gnsnyomnj.sHtML

#define X_H
来源：http://baike.bbcook.cn/Article/details/ggvybiwka.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gwmfeyoqu.sHtML

[S31] C++：Hello World
来源：http://m.share.yfazqb.com/Article/details/gjostldwy.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/gdwuwvngw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.epnwcf.com/Article/details/gmapcmlpr.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gcalbkitx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gxnlluwlr.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gvkskabyz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gbxoybrie.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gbcrpvlrl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.epnwcf.com/Article/details/gzmlicuhh.sHtML

[S35] C++：map
来源：http://baike.vehdjk.com/Article/details/gwbxhclhi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/goqnuzetn.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gyfevgmxq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gwstpsehp.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gjkbolgxv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gsmwncqua.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gignfjemt.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.vehdjk.com/Article/details/gnuxbsluj.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/gawgpgvcw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fktsv.cn/Article/details/gdsfqjapv.sHtML

[S40] C++：查找元素
来源：http://read.share.epnwcf.com/Article/details/gphjmsnyh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.epnwcf.com/Article/details/gobpvucpm.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gvviatlbx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/ghkmlxzne.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gqivlkhst.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/ghaiixhhp.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/gedpeqpol.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.yfazqb.com/Article/details/gcafntowr.sHtML

[S44] C++：引用传参
来源：http://www.blog.tarul.cn/Article/details/gkdvgfiiy.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.sjlbkw.cn/Article/details/gbkhwudmh.sHtML

[S45] C++：lambda
来源：http://www.m.share.bbcook.cn/Article/details/gnqosowas.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fktsv.cn/Article/details/gfcyjpvhr.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gucsgnuzf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.bbcook.cn/Article/details/gcnhzdbrq.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gyebzevqq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoxievqv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.tarul.cn/Article/details/gapgbeyni.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.epnwcf.com/Article/details/guvajefmb.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/goeaujdzt.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gemmaxzip.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/gdkefdncb.sHtML

[S50] C++：格式化数字
来源：http://mobile.yfazqb.com/Article/details/gwonmatse.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.epnwcf.com/Article/details/grxqjzhgs.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.sjlbkw.cn/Article/details/gnspwnjuj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.yfazqb.com/Article/details/gwlythuir.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/geoqnzdfn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gaazvhzcr.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/grtjyumvm.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.yfazqb.com/Article/details/gnlcadnhr.sHtML

[S54] C++：异常处理
来源：http://baike.bbcook.cn/Article/details/gjayoyktj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fktsv.cn/Article/details/gzqvlaeso.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fktsv.cn/Article/details/grapexrhl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gialiizar.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gtjxnyajo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.epnwcf.com/Article/details/gktzhljnz.sHtML

[S57] C++：编译期常量
来源：http://baike.vehdjk.com/Article/details/gnpoyqhgc.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gvpaphwtc.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gbckipreb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gdwdjfjte.sHtML

[S59] C++：静态断言
来源：http://read.share.yfazqb.com/Article/details/gynocvkkr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/gjsagkvvy.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.sjlbkw.cn/Article/details/geeohnsgq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gkimbtsex.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grbqkbwfl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gdpadqwzn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gagzhfrod.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gueoijedr.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gedvdybud.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gyyrpvhfd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gjdcdklbs.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gutlcwxbs.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gvhnzcpwh.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/gryoetyed.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gmjavhyfv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gnslltspr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gtyletgsp.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gbwuvwfwj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fktsv.cn/Article/details/gtuewssxi.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gixwbetdb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gmzqymggk.sHtML

[T08] Kotlin：数据类
来源：http://www.share.sjlbkw.cn/Article/details/gusszmofv.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gfksytfzn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gsozaegpu.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.tarul.cn/Article/details/grcahxuoe.sHtML

[T10] Kotlin：默认参数
来源：http://blog.sjlbkw.cn/Article/details/gjtzirusr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/gqedumqfe.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gwrwjvhaw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gzipjijqo.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gyzcbteds.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gzoqjuqhg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/gbiyzauhi.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gvfcredyu.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gyakgmdue.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gjzcpngpf.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/gaxrocsur.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gidwcblif.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gvrnweldw.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gconngvin.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/ghipfboba.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/gkeklagwt.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gopvsyfjh.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gzztcrron.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/guzjjsgtz.sHtML

if let n = opt { print(n) }
来源：http://m.share.fktsv.cn/Article/details/ghyexyzvi.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.bbcook.cn/Article/details/ghfqrygzs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gfiaxagfh.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/gexwbsekl.sHtML

for x in a { print(x) }
来源：http://mobile.fktsv.cn/Article/details/gubagcpfu.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/giteekyxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gpsckwjuv.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gpoqauasp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.bbcook.cn/Article/details/gnoispori.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gaekwtoob.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gghzrghqg.sHtML

[T25] Swift：结构体
来源：http://www.blog.bbcook.cn/Article/details/gcstmxabo.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/gfzpqtbmx.sHtML

[T26] Swift：类与重写
来源：http://mobile.vehdjk.com/Article/details/glhkzjbpq.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/gwkidbyax.sHtML

[T27] Swift：错误处理
来源：http://www.share.sjlbkw.cn/Article/details/glzbjtrzd.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gtxtrihda.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gfdqzsveq.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/guxajjrpb.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fktsv.cn/Article/details/gngoclqex.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gubqkkank.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gkaksxmfd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.epnwcf.com/Article/details/gvxqprmwu.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gngglpcez.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/glybjwwjk.sHtML

[T32] Lua：局部变量
来源：http://blog.fktsv.cn/Article/details/gtthtvfkf.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gddnyzpfk.sHtML

[T33] Lua：表（数组）
来源：http://blog.fktsv.cn/Article/details/gulkfmapm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.yfazqb.com/Article/details/gpebwgqwv.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/glcinrriw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.sjlbkw.cn/Article/details/gfybhpcqn.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gofwdqslv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gcqieslbo.sHtML

[T36] Lua：函数
来源：http://baike.fktsv.cn/Article/details/gzkuymkzp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.bbcook.cn/Article/details/gipstjuty.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gracuoyqh.sHtML

"a" .. "b"
来源：http://3g.sjlbkw.cn/Article/details/gwppzwdwi.sHtML

[T38] Lua：条件
来源：http://mobile.yfazqb.com/Article/details/gwidfikaz.sHtML

if x > 0 then print("正") end
来源：http://read.share.bbcook.cn/Article/details/gstmwxlig.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/gtqwpbjmb.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gkbodpeap.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gygorjslg.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.vehdjk.com/Article/details/goriesxbt.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gbpectger.sHtML

print "Hello\n";
来源：http://www.m.share.vehdjk.com/Article/details/gzozspwta.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/grvtkiofn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/grjeoelad.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gmigxnytm.sHtML

"值: $a"
来源：http://blog.epnwcf.com/Article/details/groeznyzg.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/gvcnmejhr.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.sjlbkw.cn/Article/details/gxepomlfx.sHtML

[T45] Perl：数组遍历
来源：http://blog.epnwcf.com/Article/details/gqrdayiiz.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/guvmbqrji.sHtML

[T46] Perl：哈希操作
来源：http://www.share.sjlbkw.cn/Article/details/gyapjxfqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.vehdjk.com/Article/details/grxkwtfzj.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gwpolforv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.sjlbkw.cn/Article/details/gvnuzsqmn.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gjuzkkccf.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gejitfhzm.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gfwafvefr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.tarul.cn/Article/details/gmwsqxzgu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gzhxkbptv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.sjlbkw.cn/Article/details/ghfiiptlc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/godohmeja.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gimxhfzxu.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gjlhdcyth.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/ghuqecdvr.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gsfolkxzr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gqqedrhyo.sHtML

s"值: $b"
来源：http://mobile.tarul.cn/Article/details/gszhfqjah.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gcqbrewmg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.yfazqb.com/Article/details/gukdtogij.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/guahafnyg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/gwrybfbos.sHtML

[T56] Scala：样例类
来源：http://www.blog.sjlbkw.cn/Article/details/glkznroyt.sHtML

case class User(name: String, age: Int)
来源：http://blog.yfazqb.com/Article/details/ggztqzono.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gxjhkrold.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.yfazqb.com/Article/details/goxnqgdkv.sHtML

[T58] Scala：函数定义
来源：http://wap.yfazqb.com/Article/details/ghkrzrjrv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gcijkdfsi.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gwggnjazk.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gfmncileu.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/gwolucqdz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gjwzvcntb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gkphcmtfp.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gdhlazaci.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxemhikdf.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gtykoslfp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.tarul.cn/Article/details/ghtgsdxdt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/ggmuhstgy.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gaqltzcld.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.bbcook.cn/Article/details/glkmvnbwd.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.sjlbkw.cn/Article/details/gjcyfnbqx.sHtML

[U04] Py：变量调试打印
来源：http://wap.yfazqb.com/Article/details/gbrpucozy.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/grtblicsv.sHtML

[U05] Py：列表去重且保序
来源：http://blog.tarul.cn/Article/details/gsjyqocce.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.vehdjk.com/Article/details/gvpghaavl.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/gjqcdcooc.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/glwumvotw.sHtML

[U07] Py：反转字典键值
来源：http://read.share.bbcook.cn/Article/details/gkyitgctp.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.yfazqb.com/Article/details/gchgbssvp.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gayvaasdz.sHtML

[y for x in nested for y in x]
来源：http://m.share.sjlbkw.cn/Article/details/goztfawaq.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.bbcook.cn/Article/details/gcvyeasxa.sHtML

max(d, key=d.get)
来源：http://www.share.epnwcf.com/Article/details/gjrsrgcjq.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gkkxbxgss.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.tarul.cn/Article/details/gelzdeqhb.sHtML

[U11] Py：生成器表达式
来源：http://3g.tarul.cn/Article/details/gssrsotap.sHtML

(x * 2 for x in arr)
来源：http://3g.yfazqb.com/Article/details/gyiqzuqzf.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gfltlalru.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gzcasugte.sHtML

[U13] Py：固定长度队列
来源：http://wap.fktsv.cn/Article/details/grjkoufms.sHtML

deque(maxlen=10)
来源：http://wap.epnwcf.com/Article/details/gvjmnnedr.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.fktsv.cn/Article/details/gmbounurn.sHtML

defaultdict(list)
来源：http://mobile.sjlbkw.cn/Article/details/gjbsuvfqe.sHtML

[U15] Py：高精度计时
来源：http://read.share.fktsv.cn/Article/details/gadxvcdcp.sHtML

t = time.perf_counter()
来源：http://www.share.vehdjk.com/Article/details/gbftcehbc.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.bbcook.cn/Article/details/gvyrmyjqn.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.epnwcf.com/Article/details/gamrwnguq.sHtML

[U17] Py：初始化日志
来源：http://blog.tarul.cn/Article/details/gltgzolfy.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhmscdbv.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gtqfjbuva.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.yfazqb.com/Article/details/gfddlymmq.sHtML


<!-- 参考信息 -->