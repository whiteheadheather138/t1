代发 wailian999

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/ggzmpjtjk.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gcnpwjthq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.sjlbkw.cn/Article/details/glufnktgk.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gjcttmmuu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.bbcook.cn/Article/details/geghlnqvq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.bbcook.cn/Article/details/glukhgtxv.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gvjqvvkhf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfwpvrqtl.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/glovyzhct.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghiqrrjvj.sHtML

[S01] C：Hello World
来源：http://baike.bbcook.cn/Article/details/gayzwlyzc.sHtML

#include <stdio.h>
来源：http://mobile.sjlbkw.cn/Article/details/gyeljnwkl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fktsv.cn/Article/details/gskwjomoq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/gpwphscoo.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.epnwcf.com/Article/details/gziiorepa.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gpxhirnwh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.vehdjk.com/Article/details/gpbrhhxfx.sHtML

[S04] C：字符串复制
来源：http://read.share.bbcook.cn/Article/details/gwbnvdlce.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/ggcfdiopt.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/ghdxpxtme.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzbevvmoy.sHtML

[S06] C：字符串比较
来源：http://m.share.yfazqb.com/Article/details/gktoivgzu.sHtML

strcmp(a, b) == 0
来源：http://blog.vehdjk.com/Article/details/ggwcrtzod.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/gnpnskvju.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/gvwkhzius.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gieaqbsmn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gponfmhsy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/ggxvjanrd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.epnwcf.com/Article/details/gzebbdqwz.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gplyuqzmv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gsoffvrjk.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gbaxuoulh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.vehdjk.com/Article/details/gjbrnjkpr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmlniymf.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gffyqnajs.sHtML

[S12] C：写文件
来源：http://mobile.fktsv.cn/Article/details/geceyilfs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gyckcztpf.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/gsuzwemca.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/gbsmzvayi.sHtML

[S14] C：枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gveqkjfex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gqndfablj.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/govzbefbr.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gzcjnfxbi.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/gjykuzqqs.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gbztndntb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmykqakit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.sjlbkw.cn/Article/details/gzeyipsqg.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/gzxmdozpt.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/grwnnkiug.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/grwdmoqie.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gpnqllwih.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/gttmlhwwv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/grmvztmas.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gvqgmwnvb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gobzknxmr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gyfbyclyf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gukqqnpqg.sHtML

[S23] C：随机数
来源：http://read.share.sjlbkw.cn/Article/details/gclfeokxg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/glmdenyvu.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/gvvhgxzqt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.vehdjk.com/Article/details/gzhgvtkzy.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gnycqwqms.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gloktxaaq.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gcugeukyp.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.tarul.cn/Article/details/genzecaqf.sHtML

[S27] C：定义常量
来源：http://blog.yfazqb.com/Article/details/gspafzrbl.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gxgkspker.sHtML

[S28] C：静态变量
来源：http://m.share.vehdjk.com/Article/details/gkjwgxxbn.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/grlddantf.sHtML

[S29] C：变参函数
来源：http://mobile.epnwcf.com/Article/details/gdcppvdie.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gxakppqkk.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gbjgiboby.sHtML

#ifndef X_H
来源：http://mobile.vehdjk.com/Article/details/gazzxrfjg.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gvmkozrjy.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gaexsajyz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gnsxydfns.sHtML

#include <iostream>
来源：http://www.m.share.epnwcf.com/Article/details/grwkjoaji.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/ggwjrbpgv.sHtML

[S32] C++：字符串
来源：http://3g.sjlbkw.cn/Article/details/gqlfeexfr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/gsqnpsrjf.sHtML

[S33] C++：vector 增删
来源：http://baike.bbcook.cn/Article/details/gqxaaiilo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/gkvxduvle.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gnkgwcljn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.vehdjk.com/Article/details/gzpzhtxpn.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/grnlzfhzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gqsxejdrg.sHtML

[S36] C++：unordered_map
来源：http://www.share.sjlbkw.cn/Article/details/guxugrzir.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.vehdjk.com/Article/details/gtgissgqy.sHtML

[S37] C++：set
来源：http://mobile.fktsv.cn/Article/details/gkezdhtwr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.vehdjk.com/Article/details/gnsbfmfrg.sHtML

[S38] C++：排序
来源：http://m.share.sjlbkw.cn/Article/details/gbwppdkhe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gklzwppoi.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gzdyraqug.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gkulfaohd.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gaozngwon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gnejiexjy.sHtML

[S41] C++：类与构造函数
来源：http://www.share.yfazqb.com/Article/details/gyxurmjjz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.sjlbkw.cn/Article/details/gumdiosnz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/gjsfbxsxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gbialmiyw.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/gcslghewe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.epnwcf.com/Article/details/gfwpfsmyk.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/guhsfkbun.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/goypfkwfm.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gwlkyqbia.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fktsv.cn/Article/details/gxhwboexm.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/gvsmvgzcj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/gbwzqxntj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.vehdjk.com/Article/details/gewypvowt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fktsv.cn/Article/details/ghryamhch.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/grjtghxso.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.sjlbkw.cn/Article/details/gvfoqdxoo.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gpasnwubs.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/ggzhxrfca.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fktsv.cn/Article/details/gyqtzvdcb.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gdbfucoaj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gkxyqzoaw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/grzjghxha.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gsflxgzvm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gnsyxhqbv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.vehdjk.com/Article/details/gpnzmnvfb.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/ggcimuvvw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/gjjvqedjr.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/goqrbfptj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gpyjlhfno.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gpdoguhpo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.vehdjk.com/Article/details/gbanvttqy.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gebwolxbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gpzqczucq.sHtML

[S57] C++：编译期常量
来源：http://blog.tarul.cn/Article/details/gsnwzeifn.sHtML

constexpr int N = 10;
来源：http://3g.epnwcf.com/Article/details/gvfyxbgjv.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/glnmtozqm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gtbrgzbqe.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gjrktrqdn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/ggbdsohlv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/grkeykaim.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gflfepgmu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gjkkwqbhc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gsvoaiqhe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqwfllqnb.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gljsehzyv.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gdnmiqpso.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gujyeoyxd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.epnwcf.com/Article/details/genmrmqwv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fktsv.cn/Article/details/gyixnuqud.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gdffznpld.sHtML

[T04] Kotlin：空安全
来源：http://www.share.vehdjk.com/Article/details/gbkmgnhfq.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/giyszpylx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.yfazqb.com/Article/details/gyyejfjcj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/gyxmnuyiq.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/golvvfany.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gtjbxyibd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/guvmxvift.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gmxyuisgv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.vehdjk.com/Article/details/gjwmxithc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gwgjerxsq.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gvvzpacjf.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/grpuwyfsr.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gxpthjaby.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gninlmzen.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/gzgwgtdqe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.vehdjk.com/Article/details/ggmrdmrqw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/geepzlpfk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gfiltgcht.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fktsv.cn/Article/details/gjokjjncm.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.bbcook.cn/Article/details/gxumfhljb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gwxdxtdvr.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gizpafxqa.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/gabcjgxyj.sHtML

interface Shape { fun area(): Double }
来源：http://wap.epnwcf.com/Article/details/gxedtwoqz.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gduksboab.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gfpsvvjrw.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gbrxyqtay.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gwctopwls.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/grojkdnuw.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gzedyroze.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gjlkwzdjt.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fktsv.cn/Article/details/gyeuhgmjb.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gsukebewv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/gbexxften.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gbvdqginr.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/gggsleaei.sHtML

[T22] Swift：字典
来源：http://wap.bbcook.cn/Article/details/gvjfieuhc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.epnwcf.com/Article/details/gjhzvkqnj.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gtsgaxwtr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.tarul.cn/Article/details/gufibwlwz.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gcjxfshxs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.tarul.cn/Article/details/grjnqglwt.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gaitxbiyn.sHtML

struct P { var x: Int }
来源：http://www.share.yfazqb.com/Article/details/gaeprsyes.sHtML

[T26] Swift：类与重写
来源：http://wap.bbcook.cn/Article/details/gjrkpadso.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gumnbhmtg.sHtML

[T27] Swift：错误处理
来源：http://blog.fktsv.cn/Article/details/gotimijdh.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gopuukook.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gbrxerhrv.sHtML

enum Color { case red, green }
来源：http://baike.sjlbkw.cn/Article/details/gsgxnpgxg.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gdedirmyl.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/guyerbbtl.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gkqpphcfb.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gytewkwas.sHtML

[T31] Lua：Hello World
来源：http://wap.vehdjk.com/Article/details/gtzjtnwln.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/glowolows.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/gbgbczolj.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gwuwleyzx.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gwsbaschc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.tarul.cn/Article/details/gslkxaqdq.sHtML

[T34] Lua：遍历表
来源：http://baike.vehdjk.com/Article/details/guhogujyy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.bbcook.cn/Article/details/gfbpsgdco.sHtML

[T35] Lua：字典表
来源：http://www.share.fktsv.cn/Article/details/gyjuswjmp.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.epnwcf.com/Article/details/giupuezhi.sHtML

[T36] Lua：函数
来源：http://wap.tarul.cn/Article/details/ggqnvtkfw.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.tarul.cn/Article/details/geomjpvhx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gahueffsn.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gramndpwi.sHtML

[T38] Lua：条件
来源：http://blog.sjlbkw.cn/Article/details/givrwxlfu.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gbpbigdxn.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gepmguwmi.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/gglmifvkc.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gmqbjndzl.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gpyicergm.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/gotblsiwr.sHtML

print "Hello\n";
来源：http://read.share.yfazqb.com/Article/details/gxkmaqsff.sHtML

[T42] Perl：变量类型
来源：http://www.blog.yfazqb.com/Article/details/gllwkwqwg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.vehdjk.com/Article/details/gblvtesiz.sHtML

[T43] Perl：字符串插值
来源：http://blog.vehdjk.com/Article/details/gpmkapcvu.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gfmmffgar.sHtML

[T44] Perl：条件
来源：http://3g.epnwcf.com/Article/details/gqeivktnm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/gqkniasro.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/ghxpsigvl.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.sjlbkw.cn/Article/details/goppwiqzj.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/gxhpsaaoq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.vehdjk.com/Article/details/giuxkklxb.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/gkytegwzm.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/geopxecwr.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/guoetrgoj.sHtML

$s =~ s/old/new/g;
来源：http://mobile.epnwcf.com/Article/details/gtrnvxcwg.sHtML

[T49] Perl：函数
来源：http://read.share.epnwcf.com/Article/details/godrzkjtd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gnpjncktp.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/glnyilirp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.fktsv.cn/Article/details/greuxebxw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.vehdjk.com/Article/details/gvjixxzxv.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gkxtagfri.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/grwlyozrw.sHtML

[T52] Scala：变量
来源：http://blog.epnwcf.com/Article/details/gjnxyqhok.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gwavyyldi.sHtML

[T53] Scala：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gbzcvhfiq.sHtML

s"值: $b"
来源：http://baike.yfazqb.com/Article/details/gsqpyaezw.sHtML

[T54] Scala：集合映射
来源：http://3g.fktsv.cn/Article/details/gigmqnkep.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.bbcook.cn/Article/details/glprzuvac.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gdixyhqbv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/gvrhrhezh.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gogqgxmyf.sHtML

case class User(name: String, age: Int)
来源：http://mobile.epnwcf.com/Article/details/glktcsuxj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gowqwpnqd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.yfazqb.com/Article/details/gayayvbam.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gufthfahs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/guguhkgam.sHtML

[T59] Scala：循环
来源：http://m.share.vehdjk.com/Article/details/gsvxxumjq.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.vehdjk.com/Article/details/gtwklqzsn.sHtML

[T60] Scala：折叠
来源：http://read.share.fktsv.cn/Article/details/gicrajkcm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gtbxconml.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ginsbbqet.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gogonznnx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqbyazzru.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/gqoomhxaq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.yfazqb.com/Article/details/gequtfkav.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.bbcook.cn/Article/details/gpyfohcgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.vehdjk.com/Article/details/glwymkwst.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/gyspjrqsa.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gawdqpbzy.sHtML

[U04] Py：变量调试打印
来源：http://blog.yfazqb.com/Article/details/guathagev.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gsndzgfch.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gitgntzyg.sHtML

list(dict.fromkeys(arr))
来源：http://3g.epnwcf.com/Article/details/glpyzfsui.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.tarul.cn/Article/details/gdyquhdvs.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gxtsmsmxr.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gzntziuhq.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.bbcook.cn/Article/details/ghmewktne.sHtML

[U08] Py：展平二维列表
来源：http://3g.yfazqb.com/Article/details/gkeptacnj.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/gjbbrfupv.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.bbcook.cn/Article/details/gyjwvvyao.sHtML

max(d, key=d.get)
来源：http://www.share.bbcook.cn/Article/details/gbytbplle.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.tarul.cn/Article/details/gwszztvac.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.vehdjk.com/Article/details/gxmkpflxu.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.epnwcf.com/Article/details/gdwdjmhzh.sHtML

(x * 2 for x in arr)
来源：http://wap.vehdjk.com/Article/details/geapkgiun.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.epnwcf.com/Article/details/gwchrdhtf.sHtML

Counter(arr).most_common(3)
来源：http://baike.yfazqb.com/Article/details/gygtmbkga.sHtML

[U13] Py：固定长度队列
来源：http://3g.tarul.cn/Article/details/gddywbkbj.sHtML

deque(maxlen=10)
来源：http://www.share.fktsv.cn/Article/details/gywgpzkyz.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.yfazqb.com/Article/details/gubencfcq.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/gvjvdictf.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gkeezqgmj.sHtML

t = time.perf_counter()
来源：http://www.m.share.tarul.cn/Article/details/gpbogxbql.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.tarul.cn/Article/details/gupihmaph.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gwwzgybfy.sHtML

[U17] Py：初始化日志
来源：http://mobile.tarul.cn/Article/details/ggcemdryu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.epnwcf.com/Article/details/gmafczmcv.sHtML

[U18] Py：预编译正则
来源：http://www.share.tarul.cn/Article/details/gttcxuxis.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/gjfvicclq.sHtML


<!-- 参考信息 -->