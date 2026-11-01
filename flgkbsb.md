代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/gqemwzfvj.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gpsjsdzmo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gpbvcvgdi.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gptkssuxs.sHtML

split -l 1000 big.log part_
来源：http://www.share.yfazqb.com/Article/details/gqbfzlubz.sHtML

[R74] 批量重命名
来源：http://www.m.share.sjlbkw.cn/Article/details/ganqqwjqf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gaguchmeu.sHtML

[R75] 导出环境变量
来源：http://read.share.fktsv.cn/Article/details/giongwffb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/glwigszzo.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gpwgdvtsz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gsorytgjn.sHtML

[R77] 读取用户输入
来源：http://baike.tarul.cn/Article/details/ghtywhdvx.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/gudmeusqk.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gveqqekdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.yfazqb.com/Article/details/gzdntywzq.sHtML

[R79] 解析命令行选项
来源：http://www.share.bbcook.cn/Article/details/gaufimvtd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gxcqttilm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.sjlbkw.cn/Article/details/gbrybyyis.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/glcplxoie.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzzihbqmj.sHtML

S. C / C++ 专题
来源：http://m.share.bbcook.cn/Article/details/gmyhyzvnr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggejvpfst.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/guejwxftk.sHtML

#include <stdio.h>
来源：http://blog.yfazqb.com/Article/details/goaneacov.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.tarul.cn/Article/details/gcmuflgpc.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gofylnurr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gjyepyvqr.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gzrdtjmmg.sHtML

int x; scanf("%d", &x);
来源：http://wap.tarul.cn/Article/details/gxacdveld.sHtML

[S04] C：字符串复制
来源：http://blog.fktsv.cn/Article/details/gfdejzwvn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/gzzeeljay.sHtML

[S05] C：字符串长度
来源：http://baike.tarul.cn/Article/details/gcunfkjee.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gczfbzdlc.sHtML

[S06] C：字符串比较
来源：http://mobile.yfazqb.com/Article/details/gfamwhytd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeaxizli.sHtML

[S07] C：数组遍历求和
来源：http://mobile.epnwcf.com/Article/details/gfvhjzfjo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gfyhckwtn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gncfukzpv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gvtldjkfc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gckmtkemo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gawrghywc.sHtML

[S10] C：指针与解引用
来源：http://wap.epnwcf.com/Article/details/gdwitaqvm.sHtML

int *p = &a;  *p = 5;
来源：http://wap.tarul.cn/Article/details/grryrkahy.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gzaaygzow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/ghvhzxqqs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.yfazqb.com/Article/details/ghfpnvldx.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/giodsaabo.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gphixcmtz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/giyujmenv.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gywdczvgj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.sjlbkw.cn/Article/details/gcrgwdliw.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gqvrbpjtk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/ggxryrfxu.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gixetudwh.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gmzjmgwpv.sHtML

[S16] C：位操作置位
来源：http://www.blog.tarul.cn/Article/details/gzlgtgmxc.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/grceqfjsr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fktsv.cn/Article/details/gzvpzpzau.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/gbnsqpjib.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gxpaloftz.sHtML

int main(int argc, char **argv)
来源：http://baike.vehdjk.com/Article/details/gqldtelbo.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gjvrikxfk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gziluvrxd.sHtML

[S20] C：二分查找
来源：http://blog.vehdjk.com/Article/details/gwasinfdf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gigojjibv.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gytijjlqw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.epnwcf.com/Article/details/glatmhzff.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/ggxtsmxyt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.bbcook.cn/Article/details/gafssjdiz.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gvzqqolvi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.bbcook.cn/Article/details/gugosuvyu.sHtML

[S24] C：获取本地时间
来源：http://3g.yfazqb.com/Article/details/gdxdguuaw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gxzwnqnpx.sHtML

[S25] C：内存拷贝
来源：http://www.share.bbcook.cn/Article/details/gevhctzus.sHtML

memcpy(dst, src, n);
来源：http://m.share.bbcook.cn/Article/details/gdghiujms.sHtML

[S26] C：内存清零
来源：http://3g.bbcook.cn/Article/details/gftyljqui.sHtML

memset(a, 0, sizeof a);
来源：http://wap.vehdjk.com/Article/details/gsyyrphcu.sHtML

[S27] C：定义常量
来源：http://www.m.share.bbcook.cn/Article/details/gqydwkzma.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gftcgbomx.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/ghkqnfhqy.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gpjvxymos.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/ghyqdcros.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gaxsmvgpf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gpttpouqw.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/ggthgemve.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gswqssnxe.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gcxxjokcj.sHtML

[S31] C++：Hello World
来源：http://read.share.tarul.cn/Article/details/gkzjryopj.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/gvnkpqswl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gynimemvt.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gbuoxmhzt.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/glhanhlat.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/gnfvjdxcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/gcscngevs.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gmccxyppg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.bbcook.cn/Article/details/gjovycmtn.sHtML

[S35] C++：map
来源：http://m.share.bbcook.cn/Article/details/gbbzjhcnn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/goyskbsuw.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/grgqjgufm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gjegeizfw.sHtML

[S37] C++：set
来源：http://blog.fktsv.cn/Article/details/gpqficnwj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/gowpqzmci.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gwjkmszdd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gbmjjfkkn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fktsv.cn/Article/details/gszzuwgtd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.sjlbkw.cn/Article/details/gnpgnhrqz.sHtML

[S40] C++：查找元素
来源：http://m.share.fktsv.cn/Article/details/gjhwvqlpq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.yfazqb.com/Article/details/gmofndfpm.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gmtalphyk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gbaszdgcb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/geomfihpb.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.bbcook.cn/Article/details/gwvohuxzp.sHtML

[S43] C++：智能指针
来源：http://www.share.tarul.cn/Article/details/gehnvqvsi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gggazhtse.sHtML

[S44] C++：引用传参
来源：http://mobile.bbcook.cn/Article/details/gvyyegtyd.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gukfthxiu.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gafkfzwal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gjniknxle.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gqgxfmjgi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/gdkfmozjr.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gfeynukge.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.sjlbkw.cn/Article/details/gmkaoflbc.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/gybujirlt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gmyavulhn.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fktsv.cn/Article/details/gaylbvamf.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gttfvgaab.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.yfazqb.com/Article/details/ggwkfliad.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gtpmblnez.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gdaytqkru.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gogpnmirm.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/gurbyngoc.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gooerkhdh.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gvjtlpshj.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gqdmbzcko.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.epnwcf.com/Article/details/gkdurlalw.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gmovuuopr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gmobypezb.sHtML

[S55] C++：结构化绑定
来源：http://blog.sjlbkw.cn/Article/details/gbvyypzkv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.yfazqb.com/Article/details/gvdkqjdzr.sHtML

[S56] C++：optional
来源：http://3g.yfazqb.com/Article/details/ghggfiejx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.yfazqb.com/Article/details/gbiyydrct.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gucsjljlk.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/giaagowvb.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gcpmnyruy.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.epnwcf.com/Article/details/gatuftenf.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/gfdmdqwma.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/gzuruxezv.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gwiyawqhy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gpshtrxdj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gsgbygmpu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gxilzpzcq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guipuvxiu.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gtmycqboj.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gkbfqffhv.sHtML

[T02] Kotlin：变量
来源：http://www.share.bbcook.cn/Article/details/gouobbscn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fktsv.cn/Article/details/gvibuyrti.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.tarul.cn/Article/details/gostwdqvi.sHtML

"值: $b"
来源：http://baike.yfazqb.com/Article/details/ghmfhrxby.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gealablrg.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gkplivvot.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.yfazqb.com/Article/details/guwrtjpcu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gtofrkzkl.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/gldupqmnt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fktsv.cn/Article/details/geuabhcok.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/ghcczifzy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gxxoefdsr.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gfnzrkpni.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gajryqhnv.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gxqbhsqwu.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gjlehakel.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/ggvwcrlwp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.bbcook.cn/Article/details/gqrmsfwko.sHtML

[T11] Kotlin：协程
来源：http://read.share.sjlbkw.cn/Article/details/gpojgapmo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/gevfofyad.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/guthnlkqs.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.vehdjk.com/Article/details/gcqiihjhh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.tarul.cn/Article/details/gckeozxaq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.epnwcf.com/Article/details/ghxydshqz.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/ggjoeaica.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fktsv.cn/Article/details/ggrvurwqm.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gacjsntnv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.bbcook.cn/Article/details/grszoaiyc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gyvgutmnc.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gxmsqpneu.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gtwhpkorv.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/ghmshscbx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gvhwjzeog.sHtML

"值: \(b)"
来源：http://baike.epnwcf.com/Article/details/gwifkkbyq.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/garktzutm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gxqbbexxb.sHtML

[T20] Swift：数组操作
来源：http://blog.epnwcf.com/Article/details/gxalmzkha.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.yfazqb.com/Article/details/gssximsno.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gomhwyoyf.sHtML

for x in a { print(x) }
来源：http://read.share.fktsv.cn/Article/details/gnbepwubg.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/gdvqgstqf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gybjjildx.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/ggjtybcqi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gpuedjrqz.sHtML

[T24] Swift：闭包
来源：http://blog.bbcook.cn/Article/details/ghqvfmipn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gcfbgqhrd.sHtML

[T25] Swift：结构体
来源：http://www.m.share.bbcook.cn/Article/details/gpbgqzpel.sHtML

struct P { var x: Int }
来源：http://read.share.tarul.cn/Article/details/gmmnayymu.sHtML

[T26] Swift：类与重写
来源：http://mobile.epnwcf.com/Article/details/gpflcdqsy.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fktsv.cn/Article/details/gzflknudy.sHtML

[T27] Swift：错误处理
来源：http://mobile.bbcook.cn/Article/details/gkdbusmtw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gnkohddhs.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/grgpbkgfn.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gnyxhruzk.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.sjlbkw.cn/Article/details/glhggcbjr.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gqorohsxi.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/grickaipg.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/gpjrwrnkh.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvjyabjv.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/glkmjhcpc.sHtML

[T32] Lua：局部变量
来源：http://www.share.tarul.cn/Article/details/gesxqhifu.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gxegnymah.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gveoggoaf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/ggjponxxi.sHtML

[T34] Lua：遍历表
来源：http://baike.epnwcf.com/Article/details/gpdlbbnbs.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/gvdanlcrf.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/gfkvpgyqx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.vehdjk.com/Article/details/gmadefpoj.sHtML

[T36] Lua：函数
来源：http://3g.bbcook.cn/Article/details/gbnroxujs.sHtML

function add(a, b) return a + b end
来源：http://www.share.yfazqb.com/Article/details/gkqavepeg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gnlrvcrgn.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/gaipgzhcw.sHtML

[T38] Lua：条件
来源：http://3g.epnwcf.com/Article/details/gingmhnst.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fktsv.cn/Article/details/gintsxwat.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gxkrzdmhd.sHtML

string.find(s, "%d+")
来源：http://wap.tarul.cn/Article/details/gzomzynxf.sHtML

[T40] Lua：元表
来源：http://wap.sjlbkw.cn/Article/details/grtudwkhk.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.yfazqb.com/Article/details/gzfupjdbj.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/guzebmhul.sHtML

print "Hello\n";
来源：http://baike.yfazqb.com/Article/details/gtjjusbsi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gxooadvai.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/gnygswbig.sHtML

[T43] Perl：字符串插值
来源：http://blog.epnwcf.com/Article/details/gsytlpaah.sHtML

"值: $a"
来源：http://www.share.fktsv.cn/Article/details/gieoxfrky.sHtML

[T44] Perl：条件
来源：http://baike.bbcook.cn/Article/details/gisaesynm.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.vehdjk.com/Article/details/goaowtlvl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gnkwsceyw.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjewmubz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvhxyrwy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.yfazqb.com/Article/details/gkdsfrsud.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gvgprjehk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gvtvkfctu.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/geucgmvrm.sHtML

$s =~ s/old/new/g;
来源：http://www.share.epnwcf.com/Article/details/gidifcijh.sHtML

[T49] Perl：函数
来源：http://blog.vehdjk.com/Article/details/gzdgxjzxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fktsv.cn/Article/details/gshywzxdp.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gudwxhnrj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.yfazqb.com/Article/details/gejcohjgg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gwaiqwdce.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gcgvlgnqm.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gbgbkzzem.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gemheemtk.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gtpwuthzd.sHtML

[T53] Scala：字符串插值
来源：http://read.share.bbcook.cn/Article/details/griptytwp.sHtML

s"值: $b"
来源：http://www.share.fktsv.cn/Article/details/guxbdjjls.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/gqnahmkqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gqdkgtpkc.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gsotcbpbb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.tarul.cn/Article/details/gsrlkngse.sHtML

[T56] Scala：样例类
来源：http://baike.yfazqb.com/Article/details/goxtvnznc.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gsyuxvfcw.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/ggnzyfmip.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gdhnuztfd.sHtML

[T58] Scala：函数定义
来源：http://3g.tarul.cn/Article/details/gpkccodci.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.bbcook.cn/Article/details/gjkdqhdtn.sHtML

[T59] Scala：循环
来源：http://m.share.epnwcf.com/Article/details/gawagsvtw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gpudpkylh.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/guqxtknlp.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gtvcgovfy.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gglcvoghn.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gjkzpaohx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfrbyruay.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.fktsv.cn/Article/details/gbrfikhoo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxtaycok.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gckehieue.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gciqmdlro.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gxyozxsuh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gjikuysoh.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.tarul.cn/Article/details/gbmdvfysq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gxtheeizp.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.tarul.cn/Article/details/gjxeebjdv.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/gptamheiq.sHtML

[U06] Py：合并两个字典
来源：http://m.share.yfazqb.com/Article/details/gyqnqlpom.sHtML

{**a, **b}
来源：http://www.share.bbcook.cn/Article/details/gxrklkelk.sHtML

[U07] Py：反转字典键值
来源：http://www.blog.sjlbkw.cn/Article/details/gwvejqtsx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gaorcjxay.sHtML

[U08] Py：展平二维列表
来源：http://mobile.vehdjk.com/Article/details/geustsuhu.sHtML

[y for x in nested for y in x]
来源：http://baike.tarul.cn/Article/details/geifzutbc.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.fktsv.cn/Article/details/gsmsvossi.sHtML

max(d, key=d.get)
来源：http://blog.vehdjk.com/Article/details/gmfoumkbi.sHtML

[U10] Py：按值排序字典
来源：http://m.share.sjlbkw.cn/Article/details/gossltnag.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.sjlbkw.cn/Article/details/gtnioddta.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.tarul.cn/Article/details/ggwkmzemn.sHtML

(x * 2 for x in arr)
来源：http://m.share.epnwcf.com/Article/details/geatznfwl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.tarul.cn/Article/details/gujjqhxns.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gdqufbydi.sHtML


<!-- 参考信息 -->