代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/ggptmkcbb.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gjbgkvhnz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gpsucykkz.sHtML

[R71] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gzrccuqer.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gxdgnshyi.sHtML

[R72] 等待端口就绪
来源：http://3g.sjlbkw.cn/Article/details/gbcfxjopa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gftwlfqbb.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gerslpuyb.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gywfunzuo.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gegvpixiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.yfazqb.com/Article/details/ggheezjkp.sHtML

[R75] 导出环境变量
来源：http://wap.fktsv.cn/Article/details/gihpzmxlm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gkglbxskv.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gnmcauyft.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gnskmjwlg.sHtML

[R77] 读取用户输入
来源：http://read.share.epnwcf.com/Article/details/gukxhnpyw.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gsebdgkqt.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/gpexsemnf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gpddnpglb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/gqjuazczr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.vehdjk.com/Article/details/geurvzflm.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gqctqkijz.sHtML

time ./run.sh
来源：http://read.share.yfazqb.com/Article/details/gyeneioek.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gejjckssb.sHtML

S. C / C++ 专题
来源：http://wap.bbcook.cn/Article/details/gvpovsrxv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkwzvevds.sHtML

[S01] C：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gdifvrmbg.sHtML

#include <stdio.h>
来源：http://blog.sjlbkw.cn/Article/details/gwcafcoeu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.yfazqb.com/Article/details/gfqllcfka.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gxwcxwbli.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.epnwcf.com/Article/details/gshzmgbch.sHtML

[S03] C：读入整数
来源：http://baike.fktsv.cn/Article/details/gwvvmwtll.sHtML

int x; scanf("%d", &x);
来源：http://m.share.sjlbkw.cn/Article/details/gankobrfq.sHtML

[S04] C：字符串复制
来源：http://mobile.vehdjk.com/Article/details/gkykvtwly.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/grblupavi.sHtML

[S05] C：字符串长度
来源：http://wap.sjlbkw.cn/Article/details/ggdlhtdec.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gbtrhvmdl.sHtML

[S06] C：字符串比较
来源：http://wap.tarul.cn/Article/details/glfuanjdp.sHtML

strcmp(a, b) == 0
来源：http://blog.bbcook.cn/Article/details/gkvmfwhyv.sHtML

[S07] C：数组遍历求和
来源：http://blog.yfazqb.com/Article/details/glauzoakh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gzmovvgvx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gygceikoi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gevlchyhn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gopinnfwl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/ghsiyzsyp.sHtML

[S10] C：指针与解引用
来源：http://blog.fktsv.cn/Article/details/gyjyffcjb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.epnwcf.com/Article/details/gehbvboyh.sHtML

[S11] C：逐行读文件
来源：http://wap.tarul.cn/Article/details/gaumrqcfe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fktsv.cn/Article/details/ghqdzaxbx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gqfjkspju.sHtML

fclose(f);
来源：http://wap.vehdjk.com/Article/details/gknvfgrxw.sHtML

[S12] C：写文件
来源：http://read.share.bbcook.cn/Article/details/gvrsnobdz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/gbcuiovaq.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gdcjjuwnu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gvpvbfibw.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gkricdssb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/glyljbvaw.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gwanqbuld.sHtML

(double) a / b
来源：http://www.m.share.tarul.cn/Article/details/gbzmbbhat.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gutkvrkiq.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gtrgfkamk.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gusbaikja.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/grohwylec.sHtML

[S18] C：命令行参数
来源：http://www.share.bbcook.cn/Article/details/ghwyusdtv.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/gpkmnwqag.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/gxvtctler.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gagctzkpc.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gkhyivdty.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gtmfzltes.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gpmgbvrxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/grxnvucrc.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gyhfpakem.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gpgpuigsa.sHtML

[S23] C：随机数
来源：http://3g.bbcook.cn/Article/details/gqwqgvnzq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.epnwcf.com/Article/details/gkdlcnjeb.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gljpsfxio.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdslansn.sHtML

[S25] C：内存拷贝
来源：http://mobile.yfazqb.com/Article/details/glqmpqfem.sHtML

memcpy(dst, src, n);
来源：http://3g.tarul.cn/Article/details/gxgiapxrc.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gtrrhxbkm.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/glgsjymkv.sHtML

[S27] C：定义常量
来源：http://www.m.share.tarul.cn/Article/details/gazjnufpg.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gmzparxpo.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gbdsgbsms.sHtML

static int counter = 0;
来源：http://wap.bbcook.cn/Article/details/gpqqywucs.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gkfjxywal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gsqnocniz.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/ghmildhwj.sHtML

#ifndef X_H
来源：http://mobile.sjlbkw.cn/Article/details/gambwhjnn.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/gemsygbnk.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/geztpycgj.sHtML

[S31] C++：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gnlzjruzi.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/gutgtbpug.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/grhdcqwwi.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gjqmijaia.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gvuuubgkw.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/gfhpwsxjf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.vehdjk.com/Article/details/gxaihscsm.sHtML

[S34] C++：遍历 vector
来源：http://baike.tarul.cn/Article/details/gtmveegmy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gzofcigqj.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/ggsdbuqkm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gvxtdbyhs.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gglnjfahc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gipyykdoa.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gnijuncrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gvamhduza.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gyqjhicpc.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/gubotisww.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gbpodwzuc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gnnyamhth.sHtML

[S40] C++：查找元素
来源：http://wap.tarul.cn/Article/details/gzzbgygqy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.yfazqb.com/Article/details/gbcxzkmgd.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/grswpuciz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gbabcecqo.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrefubs.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gchyyucxw.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gqikifljr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gqenbboly.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/gxwxnplpm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gtirrhbgx.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gzofnmzfq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.vehdjk.com/Article/details/gqydnujsr.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/gkegngqyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.yfazqb.com/Article/details/gzoiwmyhx.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gvfephnxr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.vehdjk.com/Article/details/gbntgxqnm.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gaaszwtth.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gvdhnwzyy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.tarul.cn/Article/details/gdylpcoja.sHtML

[S49] C++：写文件
来源：http://blog.tarul.cn/Article/details/gjbpdqmuq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.vehdjk.com/Article/details/gstetxbuf.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fktsv.cn/Article/details/gcixocdij.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fktsv.cn/Article/details/gdvmarppb.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gabiedlyq.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/gpeemttro.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/ggswzcyvh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gkwlvoxcu.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gvasvncpl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/guxcwypah.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gqoqxmvqx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fktsv.cn/Article/details/gprfvcdws.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gzzfqenpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.tarul.cn/Article/details/gaoymlacq.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gxmwqmrqy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.tarul.cn/Article/details/gqzrchxcb.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gmlkweeua.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gdcjzqimu.sHtML

[S58] C++：命名空间
来源：http://www.blog.bbcook.cn/Article/details/ggchqxyqz.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/gmdngteau.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gmxcnbsik.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gyrpsjxxz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.vehdjk.com/Article/details/gaagquhkl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/giutcynhq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gabdllnrm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/grzovzxor.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaaflspnk.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gmtucadqu.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/ghoyddovf.sHtML

[T02] Kotlin：变量
来源：http://blog.bbcook.cn/Article/details/gzyubhyty.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gsnzhplke.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gsnqwoegw.sHtML

"值: $b"
来源：http://mobile.tarul.cn/Article/details/gqqbxwjgv.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gmwwsrznh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gjbanwvez.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.vehdjk.com/Article/details/gxquymsad.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gcnofkkah.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.tarul.cn/Article/details/gzqycngxj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gwsnyanws.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/grbdfpzma.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gabxmxytq.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gegsomxmh.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gjeetfrkb.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gvzsgbzqs.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gsjhnwgjt.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gwrrlqjiq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fktsv.cn/Article/details/gcdltsfbd.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gsnwqtqtj.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gpffqqpex.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/gwwpwisxm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gpunejrxf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.epnwcf.com/Article/details/giqamzwvk.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.vehdjk.com/Article/details/gxzqmytly.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.tarul.cn/Article/details/gqacjetif.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gzxkmbckc.sHtML

[T15] Kotlin：接口
来源：http://wap.epnwcf.com/Article/details/gseijyakc.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fktsv.cn/Article/details/grqyctweq.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gsylzmfgk.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gzgrkjnpb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/grolydmmb.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gtgvnpxjt.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gqcgbkiyp.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gaubcydlj.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gjbigvsbb.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/gnjgsfukt.sHtML

[T20] Swift：数组操作
来源：http://3g.tarul.cn/Article/details/gycvqqmpi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.bbcook.cn/Article/details/gwhaxfywl.sHtML

[T21] Swift：遍历
来源：http://read.share.fktsv.cn/Article/details/gfmbkzotz.sHtML

for x in a { print(x) }
来源：http://www.share.sjlbkw.cn/Article/details/gynwewnpj.sHtML

[T22] Swift：字典
来源：http://3g.bbcook.cn/Article/details/gwljlcsxo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fktsv.cn/Article/details/gusztlazh.sHtML

[T23] Swift：函数
来源：http://read.share.bbcook.cn/Article/details/gmrbdqplk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gfgypnrgq.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gmjigesne.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gbtzwtavc.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/gvitmjjaf.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gpevqohwm.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gnjojqfsz.sHtML

class A: Base { override func f() {} }
来源：http://3g.sjlbkw.cn/Article/details/gfxxsvtwp.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gpdjhcamz.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.bbcook.cn/Article/details/grlunrmgx.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gzoyjcdwj.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gztciatmt.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/gukwhoqdx.sHtML

guard let x = opt else { return }
来源：http://blog.fktsv.cn/Article/details/gxfkynjta.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gqykvnywe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gmnmrtnxn.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gjriqsbtg.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/guoabujnl.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gjwvgglmy.sHtML

local a = 1
来源：http://3g.vehdjk.com/Article/details/gyojwxogl.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gapcdxopr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fktsv.cn/Article/details/gaxyjngna.sHtML

[T34] Lua：遍历表
来源：http://m.share.tarul.cn/Article/details/giffxtlly.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gnvoufemh.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/girnuqofu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/gemmohhvo.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/guowfpotp.sHtML

function add(a, b) return a + b end
来源：http://www.share.vehdjk.com/Article/details/gzbwhugdy.sHtML

[T37] Lua：字符串拼接
来源：http://3g.vehdjk.com/Article/details/giupezmep.sHtML

"a" .. "b"
来源：http://www.share.bbcook.cn/Article/details/gfneufmkh.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/grevwloiu.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gmiombzjx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gmutxapjs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfnsqica.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gjttzewsb.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gefdnugrj.sHtML

[T41] Perl：Hello World
来源：http://www.share.tarul.cn/Article/details/gxzdneihs.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gnbgubtfj.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/gqzuvcywo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/gbhdxljdp.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gittbjzao.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gdtgvhizx.sHtML

[T44] Perl：条件
来源：http://m.share.yfazqb.com/Article/details/gqzvpdevi.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.fktsv.cn/Article/details/grjvqebov.sHtML

[T45] Perl：数组遍历
来源：http://blog.yfazqb.com/Article/details/ggtdruzif.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gdwbdyuak.sHtML

[T46] Perl：哈希操作
来源：http://www.share.tarul.cn/Article/details/gfipaqwrk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.bbcook.cn/Article/details/gpycybcxy.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gcfqnnrzc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gslxwtrcg.sHtML

[T48] Perl：正则替换
来源：http://blog.epnwcf.com/Article/details/gyveujocg.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gpsvmxyfx.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gfnosndrn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/gsdagouxa.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gcoyfbbax.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.tarul.cn/Article/details/glhkgnqkw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.epnwcf.com/Article/details/gqtmwwzpn.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/gksscvzik.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gqgndoqdt.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gpbxrodon.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/gosbkareg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gufgbwsxd.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gxubbqrso.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gwubmhrod.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/givgtijmc.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gfwpkchwb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gactjzcwi.sHtML

[T56] Scala：样例类
来源：http://www.m.share.epnwcf.com/Article/details/gfbxqjlys.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gzfrspxfb.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gavayqcny.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.yfazqb.com/Article/details/giylrlvoj.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/ghbgmdsfb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gnpkimvce.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/ggtxzvhbs.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.vehdjk.com/Article/details/grkaezfrc.sHtML

[T60] Scala：折叠
来源：http://www.m.share.fktsv.cn/Article/details/gkusyppyq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gvtfexxyu.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcuhlamgo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gzuxugusf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gcbrotjoi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.yfazqb.com/Article/details/gdudjxuru.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gryesvfwl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.fktsv.cn/Article/details/gcsyltfgd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gvxfgywks.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fktsv.cn/Article/details/gpxajssnq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gppvnyrlh.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gkgtubemj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.sjlbkw.cn/Article/details/grqctnhup.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gruefxfty.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gubjqtlce.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gadyhatli.sHtML

{**a, **b}
来源：http://baike.sjlbkw.cn/Article/details/geiipbfux.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gchwfuchl.sHtML

{v: k for k, v in d.items()}
来源：http://blog.tarul.cn/Article/details/gfjdmdieg.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gabhdjhad.sHtML

[y for x in nested for y in x]
来源：http://blog.vehdjk.com/Article/details/ggyrmzzhm.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.epnwcf.com/Article/details/gasqpajyq.sHtML

max(d, key=d.get)
来源：http://www.m.share.bbcook.cn/Article/details/gsgebtxyu.sHtML

[U10] Py：按值排序字典
来源：http://3g.sjlbkw.cn/Article/details/grpwcfmra.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gthfjiqaw.sHtML


<!-- 参考信息 -->