代发 wailian999

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/gkxuzammz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.vehdjk.com/Article/details/gpalzoxuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.tarul.cn/Article/details/goedrgpqd.sHtML

[R69] 生成随机密码
来源：http://www.share.tarul.cn/Article/details/gudrfdthg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/geqvydcea.sHtML

[R70] 时间戳与互转
来源：http://baike.sjlbkw.cn/Article/details/gqgcagafj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/glssjxlqo.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gbzvkvnxq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gewxybucc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fktsv.cn/Article/details/gpuzyukyb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gjmjsvwyd.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gduinbekb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gncrqjshj.sHtML

[R74] 批量重命名
来源：http://blog.bbcook.cn/Article/details/gqtcrbwvw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gduetkvrw.sHtML

[R75] 导出环境变量
来源：http://blog.bbcook.cn/Article/details/gskacqkdf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.vehdjk.com/Article/details/gmtfhfuaq.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/glpwghslt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.yfazqb.com/Article/details/gykifwmpz.sHtML

[R77] 读取用户输入
来源：http://3g.yfazqb.com/Article/details/gowhpqciq.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/glpinfbzi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gsogqxhss.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/galcqtefe.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gxquyouko.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gxhqnlfcb.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/gokpfgnhe.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gzwqvqccn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grvptharf.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gjhbvroyn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqlzqbdyq.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gzgdmwlaq.sHtML

#include <stdio.h>
来源：http://mobile.vehdjk.com/Article/details/giktzxgep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gjhjpzifj.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/ghigvqrnh.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.yfazqb.com/Article/details/gwnuytqlk.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/guhvfcarc.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.sjlbkw.cn/Article/details/grtvzvkke.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gjaxcqsvv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.vehdjk.com/Article/details/ggnqudscp.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gcmazsewj.sHtML

strlen(s)
来源：http://mobile.yfazqb.com/Article/details/gotgxcwoo.sHtML

[S06] C：字符串比较
来源：http://m.share.vehdjk.com/Article/details/gpwfnwmrv.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/goxlrpjrc.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gnnrqpupc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/gofhszaje.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.tarul.cn/Article/details/gqwlsgvcs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.tarul.cn/Article/details/gktaiekdu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.tarul.cn/Article/details/gpqonoqae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gevkozwhm.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/ggwbmxyoz.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gxmemcoqg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gqwsitxnb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.vehdjk.com/Article/details/gcxtljfdt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/geritwhta.sHtML

fclose(f);
来源：http://www.m.share.fktsv.cn/Article/details/gsqnczhsn.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/guiyvrdvz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gyylmsqiv.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gidqcdtfy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.tarul.cn/Article/details/glqisaykr.sHtML

[S14] C：枚举
来源：http://baike.vehdjk.com/Article/details/gwvhqtpjy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.vehdjk.com/Article/details/gjpvcnals.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/gsaderzom.sHtML

(double) a / b
来源：http://baike.vehdjk.com/Article/details/grujqaaby.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/gqhjqcrqg.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gzmgbxnjr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gklzviynv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.bbcook.cn/Article/details/gujokqzoc.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gczzirser.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gmpgunmeh.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gigcufifm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.yfazqb.com/Article/details/gcialnkqs.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/gcxhcjbea.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gpstzuarj.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gnrsvuoke.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gczrkzpxi.sHtML

[S22] C：字符串转数字
来源：http://wap.sjlbkw.cn/Article/details/gchyyumsl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.vehdjk.com/Article/details/gllcurkdq.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/gbxohheha.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/gixcofcmz.sHtML

[S24] C：获取本地时间
来源：http://blog.epnwcf.com/Article/details/gvpvrsqnc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/ghodpxxlb.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gslasizmi.sHtML

memcpy(dst, src, n);
来源：http://wap.tarul.cn/Article/details/gkttitgqr.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/gyzeumovy.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fktsv.cn/Article/details/gflgkqzqo.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gktjeiwqm.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gthdjidqb.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/glpbjapjg.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gfomesyyq.sHtML

[S29] C：变参函数
来源：http://read.share.fktsv.cn/Article/details/gdcobzlpb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gqjmkhbiv.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gfmvbusap.sHtML

#ifndef X_H
来源：http://blog.vehdjk.com/Article/details/gkctisbke.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gmdyvehds.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/grvspobmi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gysmjqttz.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gacsaduqp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.epnwcf.com/Article/details/gfycejuxx.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gzcssdowe.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gaajiqdvf.sHtML

[S33] C++：vector 增删
来源：http://www.blog.vehdjk.com/Article/details/ghuievbjb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.epnwcf.com/Article/details/gcamqnnyg.sHtML

[S34] C++：遍历 vector
来源：http://read.share.yfazqb.com/Article/details/gyirdxkip.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gnstykjob.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/gvimwfblv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gxfgbvhkh.sHtML

[S36] C++：unordered_map
来源：http://blog.sjlbkw.cn/Article/details/gowuqjkct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gohgblowy.sHtML

[S37] C++：set
来源：http://baike.vehdjk.com/Article/details/ghllhjplj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.tarul.cn/Article/details/ggpmidlnx.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/gvnanfkhp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gsyqqzcqd.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fktsv.cn/Article/details/gwoewxpcm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/guzdrxwby.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gsexstsny.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/ghgyzlcaz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.yfazqb.com/Article/details/gaevyjglx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gesuvkhyo.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/gvvtifdov.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/ghxhetxkr.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gaauyazkg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gurxnavtb.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/gpdhnblke.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gtnldlpld.sHtML

[S45] C++：lambda
来源：http://wap.vehdjk.com/Article/details/gacequxcl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gizwehjvs.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gwjrcpchy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gtttmnfnf.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.epnwcf.com/Article/details/gqvtnftcq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gaouitjth.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gcqhetqww.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/glutnrxns.sHtML

while (std::getline(in, line)) { }
来源：http://3g.bbcook.cn/Article/details/gujeclumj.sHtML

[S49] C++：写文件
来源：http://www.blog.fktsv.cn/Article/details/gpntmjyrj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gnbjhqoxk.sHtML

[S50] C++：格式化数字
来源：http://mobile.vehdjk.com/Article/details/gimflasgo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/gsvydpwdi.sHtML

[S51] C++：显式类型转换
来源：http://wap.yfazqb.com/Article/details/gpadrqeul.sHtML

static_cast<double>(a) / b
来源：http://blog.tarul.cn/Article/details/glfedtrgx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.tarul.cn/Article/details/gcfkyuppv.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/gbpejmwbh.sHtML

[S53] C++：移动语义
来源：http://www.share.bbcook.cn/Article/details/gudjursol.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/ggsqpbtvq.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gqatmzmzm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gjxvnrctj.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/grpykochx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.tarul.cn/Article/details/gymccevro.sHtML

[S56] C++：optional
来源：http://www.blog.tarul.cn/Article/details/gftrhofxe.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.epnwcf.com/Article/details/gcjipplty.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gxhhalljy.sHtML

constexpr int N = 10;
来源：http://3g.bbcook.cn/Article/details/gugexilwn.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gqpwvhlkq.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fktsv.cn/Article/details/gqvhgafgj.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gnwieoqzu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gxvfnkllr.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gynivckxt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gktpoifvx.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gthvntfcy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gkslupynf.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grinqnyda.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gtvrauacl.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gxeqkbsvp.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.yfazqb.com/Article/details/giahsapdl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.vehdjk.com/Article/details/gqajkocrq.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gumdhnzll.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gfbykerfe.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gauhjeqbf.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/ghmtayaea.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.vehdjk.com/Article/details/gpfxfbzii.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.epnwcf.com/Article/details/gqaxkgbxf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/guqzplcbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/gqnqovyyh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.epnwcf.com/Article/details/gadieelec.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fktsv.cn/Article/details/giesoxchk.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/giblgrvcf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gdfpobfvl.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/gpunostwh.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.vehdjk.com/Article/details/gjudycvdn.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gsttassrg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.tarul.cn/Article/details/gshpjpxoj.sHtML

[T11] Kotlin：协程
来源：http://www.blog.bbcook.cn/Article/details/gyvrvpqww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.vehdjk.com/Article/details/ghyjziduk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gmnwqyqak.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gwlfhzmdo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/gjmfjimhe.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/ghnyedtii.sHtML

[T14] Kotlin：循环
来源：http://3g.yfazqb.com/Article/details/gfcilgcss.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gdrymwdas.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gzulpjhtv.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gzyfdloce.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gyqkarozo.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gxdxnsqvq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.epnwcf.com/Article/details/ggqlhgoqw.sHtML

var a = 1;  let b = 2
来源：http://read.share.bbcook.cn/Article/details/gpkckrdtj.sHtML

[T18] Swift：字符串插值
来源：http://baike.fktsv.cn/Article/details/ggnanxhlg.sHtML

"值: \(b)"
来源：http://www.m.share.fktsv.cn/Article/details/gxzwjrhve.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gkcqqbmmv.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gemohnxon.sHtML

[T20] Swift：数组操作
来源：http://wap.fktsv.cn/Article/details/gfxprhcja.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gcfcdgkdd.sHtML

[T21] Swift：遍历
来源：http://mobile.epnwcf.com/Article/details/gkzfxqjrw.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gbcabaaqc.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gbjaabtgt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.tarul.cn/Article/details/gvuyrmbvd.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gfsypupxq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.vehdjk.com/Article/details/gvtnjieaq.sHtML

[T24] Swift：闭包
来源：http://wap.tarul.cn/Article/details/grwnpnojs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fktsv.cn/Article/details/glxutdztg.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gsgjqqpcb.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/gugjjelvy.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gjxlbqxhj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gocuogdys.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/guqiwuiou.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.vehdjk.com/Article/details/gvsvqlvir.sHtML

[T28] Swift：枚举
来源：http://www.m.share.vehdjk.com/Article/details/glxmdmfay.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gocsaoqky.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/geqmfjjrh.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gtnphrnhf.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/guyqilnza.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/grvblcjnl.sHtML

[T31] Lua：Hello World
来源：http://mobile.yfazqb.com/Article/details/gzpjtkihi.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/ggifdseou.sHtML

[T32] Lua：局部变量
来源：http://www.blog.bbcook.cn/Article/details/grncgbowa.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gjtgfxxri.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gotifflyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.sjlbkw.cn/Article/details/gzxpslycu.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gpffyunpe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/gpjsejkbh.sHtML

[T35] Lua：字典表
来源：http://baike.tarul.cn/Article/details/gtnwnljgn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gvqkohknv.sHtML

[T36] Lua：函数
来源：http://baike.vehdjk.com/Article/details/gqqjhslfw.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/glmklpmjc.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/ggqzjjhtn.sHtML

"a" .. "b"
来源：http://blog.epnwcf.com/Article/details/gxzezomzr.sHtML

[T38] Lua：条件
来源：http://3g.bbcook.cn/Article/details/gfkxzsjar.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/glifnewko.sHtML

[T39] Lua：模式匹配
来源：http://blog.yfazqb.com/Article/details/gxmpvtcte.sHtML

string.find(s, "%d+")
来源：http://wap.sjlbkw.cn/Article/details/gpmhoacpb.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gkuqogfti.sHtML

setmetatable({}, { __index = base })
来源：http://3g.vehdjk.com/Article/details/gzuybipsd.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gqauvdnbn.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/grvumtiki.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxavmpmcc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.tarul.cn/Article/details/gmbfuvuug.sHtML

[T43] Perl：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gdbdbmqle.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gousyikax.sHtML

[T44] Perl：条件
来源：http://blog.yfazqb.com/Article/details/ghgufikia.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/ghvfqmvir.sHtML

[T45] Perl：数组遍历
来源：http://3g.sjlbkw.cn/Article/details/gtnjahtgu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/gxttezeaa.sHtML

[T46] Perl：哈希操作
来源：http://3g.yfazqb.com/Article/details/gjajfzgtf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.fktsv.cn/Article/details/gpjbtiagq.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.epnwcf.com/Article/details/gimnwnfnw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/grevhsgep.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gtgvjrrqu.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gxsjlkcph.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/gginlomcb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.tarul.cn/Article/details/gcntjkszq.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gxbitghef.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gmfxvbrpa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/geuavwtam.sHtML

[T51] Scala：Hello World
来源：http://blog.epnwcf.com/Article/details/gpurfdwmz.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gszslwaam.sHtML

[T52] Scala：变量
来源：http://baike.fktsv.cn/Article/details/gdwfwmynt.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gfjsukknt.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/goubyjvct.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gpzytwonz.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gemtchjxl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gpbhrohum.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gvejqibcn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gvgtcrlli.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/ghtgndfqr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gahebpuia.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gcgrgcbfi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gfpfftbrs.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gwjvyiupl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gscytrbmz.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gxaejqunw.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.vehdjk.com/Article/details/gnbsrsnuw.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gcvekmplb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/glindthjh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggpjcnfwe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.bbcook.cn/Article/details/gydtqdrdc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjfaiszrn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.vehdjk.com/Article/details/gdcjjcauw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.vehdjk.com/Article/details/gakxrigjn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.epnwcf.com/Article/details/gdyfjhwqe.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gvpxrvnul.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gwmvlleyt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.sjlbkw.cn/Article/details/ghqwlqzny.sHtML

[U04] Py：变量调试打印
来源：http://read.share.yfazqb.com/Article/details/gxbdjoipq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.fktsv.cn/Article/details/goddgeavk.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.bbcook.cn/Article/details/gvxjkocxr.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.epnwcf.com/Article/details/gysriqsja.sHtML

[U06] Py：合并两个字典
来源：http://wap.epnwcf.com/Article/details/gnjyvrpdy.sHtML

{**a, **b}
来源：http://read.share.sjlbkw.cn/Article/details/gjldxcvtn.sHtML

[U07] Py：反转字典键值
来源：http://www.share.yfazqb.com/Article/details/gwcxlsxif.sHtML

{v: k for k, v in d.items()}
来源：http://blog.bbcook.cn/Article/details/gixbrerjr.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.sjlbkw.cn/Article/details/gkgxunynx.sHtML

[y for x in nested for y in x]
来源：http://baike.bbcook.cn/Article/details/gsbcgycnp.sHtML


<!-- 参考信息 -->