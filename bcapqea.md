代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/goozotwil.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gicglbple.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gdzqtrtue.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gmhaxdqbs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/girmzmtqu.sHtML

[R72] 等待端口就绪
来源：http://wap.epnwcf.com/Article/details/gmdhlqmpb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gqmynswvy.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gwjutbryd.sHtML

split -l 1000 big.log part_
来源：http://baike.yfazqb.com/Article/details/gghtnjlvn.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gxpkwwdyi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gmjcuztru.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gblnejdon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gtavrihfp.sHtML

[R76] 使用临时文件
来源：http://m.share.yfazqb.com/Article/details/glrrnqyfp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gwqiqytvo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.vehdjk.com/Article/details/gevtuozla.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/gkrfbnmxj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gjnfsfvdw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gfmhqkhrh.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/gdmnfknyk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fktsv.cn/Article/details/glwyegqgs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.bbcook.cn/Article/details/gfpwtwgym.sHtML

time ./run.sh
来源：http://mobile.tarul.cn/Article/details/gwpvaivos.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gobojtltd.sHtML

S. C / C++ 专题
来源：http://www.blog.fktsv.cn/Article/details/gqkbvukks.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grmmalvdg.sHtML

[S01] C：Hello World
来源：http://read.share.bbcook.cn/Article/details/gkhqeunzp.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gypfwfvvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gizxtrvwy.sHtML

[S02] C：变量与格式化输出
来源：http://wap.yfazqb.com/Article/details/gppvhwbvf.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.tarul.cn/Article/details/gmzannplc.sHtML

[S03] C：读入整数
来源：http://blog.yfazqb.com/Article/details/gkikrumoi.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gwhekbgvw.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gvweiqbxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.bbcook.cn/Article/details/gvivbuzlg.sHtML

[S05] C：字符串长度
来源：http://blog.fktsv.cn/Article/details/glqxdcbdl.sHtML

strlen(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtmfysxil.sHtML

[S06] C：字符串比较
来源：http://baike.fktsv.cn/Article/details/glpuuhqof.sHtML

strcmp(a, b) == 0
来源：http://m.share.fktsv.cn/Article/details/gsggvgiwi.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/goxynixqw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/gpwrkxbyd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/gzeyrzpyo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/grnvnmqca.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gkidtkeoz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.yfazqb.com/Article/details/gvsshpxvc.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/ghxezoiyo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.yfazqb.com/Article/details/gpqxdyavp.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gqapjowdp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gmrktihue.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gnzuyxuft.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gpsyoiqws.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gqoufhaky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/ggucomdkt.sHtML

[S13] C：宏定义
来源：http://baike.bbcook.cn/Article/details/gbeizkvbu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.epnwcf.com/Article/details/gefrmuwjr.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/guhdcdifz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gyeyqqdme.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gjqwxdlrn.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gkriacxvr.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gpbaasmgy.sHtML

x |= (1 << 3);
来源：http://m.share.tarul.cn/Article/details/gdmmadigp.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gyguvuzir.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gajzlbvoy.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gzplbpgnd.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/giqslkhbm.sHtML

[S19] C：快速排序
来源：http://mobile.vehdjk.com/Article/details/glbhzuaox.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gqkagzrsy.sHtML

[S20] C：二分查找
来源：http://wap.epnwcf.com/Article/details/gqiaqfauw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.yfazqb.com/Article/details/gmbbpbgom.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gvgztigfm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.bbcook.cn/Article/details/gatmoklfo.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gjvupylqm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/giepzqxyk.sHtML

[S23] C：随机数
来源：http://blog.epnwcf.com/Article/details/gjunzidkd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gtsfywmja.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gvcghaxyj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/gpanuvjcl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/glbebnbds.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkxakvtu.sHtML

[S26] C：内存清零
来源：http://www.blog.epnwcf.com/Article/details/gwcfsawmj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gqogemhgo.sHtML

[S27] C：定义常量
来源：http://www.m.share.vehdjk.com/Article/details/gfihnxroj.sHtML

const double PI = 3.14159;
来源：http://www.share.fktsv.cn/Article/details/gmjorpzqx.sHtML

[S28] C：静态变量
来源：http://www.share.epnwcf.com/Article/details/grmtiprez.sHtML

static int counter = 0;
来源：http://blog.vehdjk.com/Article/details/gqcofnkvr.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gzjzxwlci.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/giiadylqe.sHtML

[S30] C：头文件保护
来源：http://3g.tarul.cn/Article/details/gulxwzrzw.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gsaijewjq.sHtML

#define X_H
来源：http://www.share.sjlbkw.cn/Article/details/gceosasey.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gwpjljssw.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ggmtktvaq.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gixqhcqfn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.tarul.cn/Article/details/gjdvuqpzh.sHtML

[S32] C++：字符串
来源：http://m.share.tarul.cn/Article/details/guemhornp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.tarul.cn/Article/details/gxxfzitbr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.yfazqb.com/Article/details/gkhqyutqf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.epnwcf.com/Article/details/gfnauwcua.sHtML

[S34] C++：遍历 vector
来源：http://read.share.vehdjk.com/Article/details/gmrcvznzv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.epnwcf.com/Article/details/gptxhpnvc.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/giupgyuyd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gxmxukwdl.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gzhjmjgnw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gqijrwnkp.sHtML

[S37] C++：set
来源：http://wap.epnwcf.com/Article/details/ghkrmffkf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gsrgrrqwh.sHtML

[S38] C++：排序
来源：http://www.m.share.vehdjk.com/Article/details/gtrwiwrla.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gignrcwxn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fktsv.cn/Article/details/grfzluebp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gnigeljjj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gtqsadojn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.tarul.cn/Article/details/gkupirney.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/ghnwfvmcm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gptzklxmz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gawyyxvok.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.vehdjk.com/Article/details/glojwvszu.sHtML

[S43] C++：智能指针
来源：http://blog.epnwcf.com/Article/details/gipcdlive.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gehftvptp.sHtML

[S44] C++：引用传参
来源：http://wap.yfazqb.com/Article/details/gzkduckbr.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkuvsuneu.sHtML

[S45] C++：lambda
来源：http://blog.bbcook.cn/Article/details/gnbjazvra.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gwqodpwcr.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/gfrryxetn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gowasgcad.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gnfvnarue.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gnbsylmen.sHtML

[S48] C++：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/ggzpdmcsh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.epnwcf.com/Article/details/gntpfjsdv.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gtbezvfyk.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gwxbwnccx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.epnwcf.com/Article/details/gmxaejdms.sHtML

[S50] C++：格式化数字
来源：http://mobile.bbcook.cn/Article/details/gbehsdkhh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gwjrmpwqi.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/goybvodjq.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gigjdtgcc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gxuewfygu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.sjlbkw.cn/Article/details/gmjrtkacf.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gtsbqlxhp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.epnwcf.com/Article/details/gsmajyfxo.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/gesuoxent.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.yfazqb.com/Article/details/gzlilksvc.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/gxsiorfvf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/grqwngtqf.sHtML

[S56] C++：optional
来源：http://m.share.tarul.cn/Article/details/goxtslpkx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gsvpdbugn.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gncrcmnar.sHtML

constexpr int N = 10;
来源：http://www.m.share.tarul.cn/Article/details/geziuucqb.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gelflxbex.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.yfazqb.com/Article/details/gmhducxnj.sHtML

[S59] C++：静态断言
来源：http://3g.tarul.cn/Article/details/gfkqegxsg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gyptncpda.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.epnwcf.com/Article/details/ggpzkcaqb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.vehdjk.com/Article/details/gkwobkljy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gsjnyyyhg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gonkuldsy.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghrotcpqp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.yfazqb.com/Article/details/gcymppotg.sHtML

println("Hello")
来源：http://3g.epnwcf.com/Article/details/ginvzmdko.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/gvgoqvgpw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gmotvufqp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/goggpiufk.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gmfxmdoct.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.epnwcf.com/Article/details/gkpgiyggw.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gvqbvzkcl.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fktsv.cn/Article/details/glyagdwfx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gpipnfnrk.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.bbcook.cn/Article/details/gulkeotbo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fktsv.cn/Article/details/gjugcasie.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gxdrbqadl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gkhyjotha.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gxemhvfye.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gsxjmgeef.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gnvoounfo.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.yfazqb.com/Article/details/gqqvdjycy.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fktsv.cn/Article/details/gdnarofos.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gdthqtnku.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/ghxuffboi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/geqfiutbw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.vehdjk.com/Article/details/gwhneogzs.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gzqhtsfqr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/genkjutdq.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/ggzfquovd.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gneizllej.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gtnstjsbk.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.epnwcf.com/Article/details/gjjvzptqh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gxguxpamg.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gwkpwfccb.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gtthyswup.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/ggatveqgf.sHtML

var a = 1;  let b = 2
来源：http://www.blog.yfazqb.com/Article/details/gdfceigfj.sHtML

[T18] Swift：字符串插值
来源：http://3g.yfazqb.com/Article/details/gubnkcelh.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gyvgjlppc.sHtML

[T19] Swift：可选绑定
来源：http://blog.sjlbkw.cn/Article/details/gdsqadyyd.sHtML

if let n = opt { print(n) }
来源：http://www.share.bbcook.cn/Article/details/ggyayxlvb.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/grvxjlyyl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gwhnhzdjc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.vehdjk.com/Article/details/gtyjcxqmo.sHtML

for x in a { print(x) }
来源：http://www.share.fktsv.cn/Article/details/gbakjkhqx.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gzlersape.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gfbkzlwmh.sHtML

[T23] Swift：函数
来源：http://mobile.tarul.cn/Article/details/gfdtzpjtr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.yfazqb.com/Article/details/gikxaqxvi.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gmvxouotp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gmnmysgec.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gidtlfbmy.sHtML

struct P { var x: Int }
来源：http://3g.fktsv.cn/Article/details/gxxszxjet.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/gukqcubdh.sHtML

class A: Base { override func f() {} }
来源：http://blog.fktsv.cn/Article/details/goeoldmjc.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gotklzpbo.sHtML

do { try f() } catch { print(error) }
来源：http://wap.bbcook.cn/Article/details/ghhtwrjhx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/glbjfkdwm.sHtML

enum Color { case red, green }
来源：http://www.share.fktsv.cn/Article/details/gmqqyrtaz.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gdbldsewh.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gpxzhpvby.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gplytkpqy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gawychsol.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gpzzsimqy.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/galoclabx.sHtML

[T32] Lua：局部变量
来源：http://m.share.epnwcf.com/Article/details/gvadejjnm.sHtML

local a = 1
来源：http://www.m.share.vehdjk.com/Article/details/gqdfifcmj.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gjfavrdpu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/ghlwmlhnh.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/ghjcpsfdw.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gcvrxsfuv.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gculctsqs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/gnguyritm.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/gznqftmxo.sHtML

function add(a, b) return a + b end
来源：http://baike.sjlbkw.cn/Article/details/gibgefalh.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gcyumdetv.sHtML

"a" .. "b"
来源：http://baike.yfazqb.com/Article/details/giiuckieq.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gvelrpoak.sHtML

if x > 0 then print("正") end
来源：http://wap.epnwcf.com/Article/details/gbxrjewbb.sHtML

[T39] Lua：模式匹配
来源：http://wap.vehdjk.com/Article/details/gunforvxi.sHtML

string.find(s, "%d+")
来源：http://wap.bbcook.cn/Article/details/gwylwrqju.sHtML

[T40] Lua：元表
来源：http://www.m.share.tarul.cn/Article/details/gfyrfqytv.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqgduagg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gigwfvvee.sHtML

print "Hello\n";
来源：http://read.share.tarul.cn/Article/details/gxvglrxfy.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/glvtzptwd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gjvuxmjgo.sHtML

[T43] Perl：字符串插值
来源：http://m.share.bbcook.cn/Article/details/glgwrpnlz.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gbmtfterl.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gcvvbyakd.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/grqtiharg.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gunhtrvja.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gndudmfzm.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/geneetyzm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpngapbur.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/gkvrnrhun.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.vehdjk.com/Article/details/gewxrgfsp.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gijpjedye.sHtML

$s =~ s/old/new/g;
来源：http://blog.bbcook.cn/Article/details/gtvecmndp.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/guyrdiicy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/ggnzncesv.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gpokcsdlk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.tarul.cn/Article/details/gsenfnaln.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gbibqsqic.sHtML

[T51] Scala：Hello World
来源：http://m.share.vehdjk.com/Article/details/gxbvqsakk.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gjpplalrj.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/gmmnclwuk.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.tarul.cn/Article/details/ggrasafju.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gdfomovpc.sHtML

s"值: $b"
来源：http://baike.vehdjk.com/Article/details/ghwrtursc.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gtvbyavbx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/ggpkddhej.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gzefmcymp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gqtpozurj.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/geyzeflsw.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/gktqevfpq.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gslvwbvmp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gvcladsfw.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gqqxqxkdn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.vehdjk.com/Article/details/gchncfcwd.sHtML

[T59] Scala：循环
来源：http://baike.yfazqb.com/Article/details/gntheqsvb.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gqxmrsrwh.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gzlvwxawu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/ghqtrtcpk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gbpnftsej.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fktsv.cn/Article/details/gskisrkwp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gnlwsuswj.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.yfazqb.com/Article/details/gqpuolaol.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.tarul.cn/Article/details/gpyribudv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gzjlvozrg.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/gerjwlemn.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.tarul.cn/Article/details/gyyomobkg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gwbhyzhlq.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/giprwpzwo.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/gebdyjfbe.sHtML

[U05] Py：列表去重且保序
来源：http://3g.epnwcf.com/Article/details/gnqgdvgcc.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gbnuviwia.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gpbgaftyp.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gngyomrkg.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gygcwhdra.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.tarul.cn/Article/details/gbkmvpjxz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.fktsv.cn/Article/details/ggagdxqdk.sHtML

[y for x in nested for y in x]
来源：http://wap.yfazqb.com/Article/details/gicckgqfa.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.bbcook.cn/Article/details/gaerovrbd.sHtML

max(d, key=d.get)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfltywbmy.sHtML

[U10] Py：按值排序字典
来源：http://3g.bbcook.cn/Article/details/gihmptsjh.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://read.share.epnwcf.com/Article/details/govmjwzgx.sHtML


<!-- 参考信息 -->