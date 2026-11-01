代发 wailian999

openssl rand -hex 16
来源：http://baike.tarul.cn/Article/details/gclfsazkp.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/gazbqrbyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gmwcheiej.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gnawptxzl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.bbcook.cn/Article/details/gdqvwwclg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/gqqpjcndg.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/gtrixzhnc.sHtML

[R71] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gabigtmqq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.sjlbkw.cn/Article/details/gujlcdhsa.sHtML

[R72] 等待端口就绪
来源：http://www.share.fktsv.cn/Article/details/gzusqfwey.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gxdfafizu.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gmazswxbw.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.bbcook.cn/Article/details/gypvkibnk.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/ggigxgscv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gcpncudlv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gfzhmzwyr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.vehdjk.com/Article/details/gkqfskbat.sHtML

[R76] 使用临时文件
来源：http://baike.vehdjk.com/Article/details/gjprwvjve.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gpomtvszq.sHtML

[R77] 读取用户输入
来源：http://baike.fktsv.cn/Article/details/gmpwagklf.sHtML

read -rp "请输入: " ans
来源：http://3g.epnwcf.com/Article/details/gbafwzuqm.sHtML

[R78] 交互式菜单
来源：http://blog.vehdjk.com/Article/details/ghwtxpxqy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.bbcook.cn/Article/details/gpwwqzssx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gdobbkxnw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.sjlbkw.cn/Article/details/gjusedhxr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.epnwcf.com/Article/details/gvrnozfmn.sHtML

time ./run.sh
来源：http://blog.epnwcf.com/Article/details/gyqoajlql.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gflegpwlt.sHtML

S. C / C++ 专题
来源：http://3g.epnwcf.com/Article/details/gbhjohqbd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxecyxyqo.sHtML

[S01] C：Hello World
来源：http://mobile.yfazqb.com/Article/details/gcowuilbb.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gokkumiev.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gbahpijll.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fktsv.cn/Article/details/gimkkeyub.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.yfazqb.com/Article/details/gzjbvsnab.sHtML

[S03] C：读入整数
来源：http://www.blog.sjlbkw.cn/Article/details/guvhcwyts.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gkhkffthe.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/ghjvievtf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.vehdjk.com/Article/details/gqsvqygob.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/ggnqeoxbq.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/gpudemlix.sHtML

[S06] C：字符串比较
来源：http://blog.fktsv.cn/Article/details/gizkmuxfb.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/ghiuprtwv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fktsv.cn/Article/details/gicvwndku.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxypgcud.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.sjlbkw.cn/Article/details/gritbjqjm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.yfazqb.com/Article/details/gjfeqhwqj.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.sjlbkw.cn/Article/details/grwaojxhl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.bbcook.cn/Article/details/gpshdyijc.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/gcclezftf.sHtML

int *p = &a;  *p = 5;
来源：http://3g.epnwcf.com/Article/details/gxikxshfg.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gleoavtsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gyuusrnuj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gsquwmajf.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gvyaucrpj.sHtML

[S12] C：写文件
来源：http://www.blog.yfazqb.com/Article/details/gizgjfyvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/glpbyvdsz.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gilsptlzg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/gsmshdqay.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gcsjhfnvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/ghbxzpolc.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/gfwwhsrzq.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gibqeberi.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/gzbfcltce.sHtML

x |= (1 << 3);
来源：http://blog.bbcook.cn/Article/details/gnqpulgkt.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/gblxnboap.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/gdxvwdnkb.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gangadmlt.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gsuwiqlwe.sHtML

[S19] C：快速排序
来源：http://wap.yfazqb.com/Article/details/gvediihfb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gmplfaezq.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/ghikdofwd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gblwzgpdy.sHtML

[S21] C：字符类别判断
来源：http://baike.yfazqb.com/Article/details/gesmznanw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gznhpgqzy.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/gmvzhuugo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/ghjzknjcn.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/gsmyvxsbt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gfdmhlmur.sHtML

[S24] C：获取本地时间
来源：http://3g.bbcook.cn/Article/details/gdtiidwzh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.vehdjk.com/Article/details/gptgutsjn.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gwmchmrmh.sHtML

memcpy(dst, src, n);
来源：http://blog.fktsv.cn/Article/details/giffcxtux.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gklrcdoyk.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.epnwcf.com/Article/details/gsylfzrnd.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gerlskznx.sHtML

const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gpviivmar.sHtML

[S28] C：静态变量
来源：http://blog.fktsv.cn/Article/details/gfnqsgwlt.sHtML

static int counter = 0;
来源：http://3g.sjlbkw.cn/Article/details/gtgxigutp.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/gczzvslxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gkcaskkwi.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gqucozxiq.sHtML

#ifndef X_H
来源：http://wap.sjlbkw.cn/Article/details/gypsuhaaq.sHtML

#define X_H
来源：http://read.share.tarul.cn/Article/details/gspxtgamc.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gcjjouaco.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gjmruawlm.sHtML

#include <iostream>
来源：http://baike.vehdjk.com/Article/details/gekmycgmc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.bbcook.cn/Article/details/ggxcfwrga.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/ghcgszgvr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.vehdjk.com/Article/details/gosctexsy.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gqgcraozi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/gyweddgiu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.tarul.cn/Article/details/gxftczhvs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gymrytaya.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/guzecvhrp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gaopsyokc.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gguicsjcn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gsjnxwqax.sHtML

[S37] C++：set
来源：http://baike.sjlbkw.cn/Article/details/gkocpcdly.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gulzvhipb.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/giqmoplwx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gpxaxsoec.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.yfazqb.com/Article/details/gxmjkhkhm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/gbbtxxqkm.sHtML

[S40] C++：查找元素
来源：http://read.share.tarul.cn/Article/details/gnxphduxp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gfowcuehz.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/ghhwrzfvf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.tarul.cn/Article/details/gqdhvlrbd.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fktsv.cn/Article/details/gwzzmqssw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gtkpcyoum.sHtML

[S43] C++：智能指针
来源：http://www.m.share.tarul.cn/Article/details/gtnspwaro.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.sjlbkw.cn/Article/details/gbvceiwrs.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gktnjhlgy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gejosxwbr.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gfdogowhe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gqwfylhft.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gstjmwwwx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gcjqvnkan.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gvvrgkljg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.tarul.cn/Article/details/ghqhddnxz.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gjtrrinxo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.yfazqb.com/Article/details/ggnpoiupn.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.bbcook.cn/Article/details/gkfdiduvx.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gfrvnwwbt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gyiiegwcv.sHtML

[S50] C++：格式化数字
来源：http://wap.epnwcf.com/Article/details/gqhwzbrfq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gkjhdpecm.sHtML

[S51] C++：显式类型转换
来源：http://baike.fktsv.cn/Article/details/gwibfsteg.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gondlwieq.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.epnwcf.com/Article/details/ggsdbmatv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fktsv.cn/Article/details/gkxbwkjsl.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gzabqkxuw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/giulseebq.sHtML

[S54] C++：异常处理
来源：http://blog.vehdjk.com/Article/details/gncsyndrt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fktsv.cn/Article/details/gobzhmszo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.bbcook.cn/Article/details/grttdrrjq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/guxiekbwh.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gpacbzxtp.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/gwmgzbxdi.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/grnfhgcua.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/ggalquytd.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gdxrkdirn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gahcrkvrm.sHtML

[S59] C++：静态断言
来源：http://mobile.epnwcf.com/Article/details/gkvniqfvj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/galpsuvwi.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gsqeibcaq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gptqagxts.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvkqpkhqe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gixfeqjhg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grkjurakm.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fktsv.cn/Article/details/gvddauznr.sHtML

println("Hello")
来源：http://www.share.yfazqb.com/Article/details/ghsbwbzop.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gpusgplug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.bbcook.cn/Article/details/gsmletfgp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gnbvbgltt.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/gifupwhpi.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gllrwvggy.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gthymzgjs.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.vehdjk.com/Article/details/glqzleaml.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fktsv.cn/Article/details/gaidxlgmz.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/gkieinwkb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/glgeuwtzb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gvfmnklxr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gfoaaxdfk.sHtML

[T08] Kotlin：数据类
来源：http://m.share.epnwcf.com/Article/details/grgmhzjzf.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.yfazqb.com/Article/details/ghzbqqrum.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.tarul.cn/Article/details/ggkpanrbf.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gyljnoewy.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gndefwrnn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/gpxnsdzyn.sHtML

[T11] Kotlin：协程
来源：http://3g.tarul.cn/Article/details/grzwqvjcc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gwdutwrct.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/gvmbtaguh.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.vehdjk.com/Article/details/gabxwfrjm.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gqfkhrnrp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gabkvnird.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gjltwqvsb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gadahuwqt.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gsxsszeuk.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.yfazqb.com/Article/details/gxurcqgws.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gyagamfck.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/guodtoxxh.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gfscvssng.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/ghcdjkcea.sHtML

[T18] Swift：字符串插值
来源：http://wap.yfazqb.com/Article/details/gvcypfqsa.sHtML

"值: \(b)"
来源：http://baike.bbcook.cn/Article/details/gvivtxuux.sHtML

[T19] Swift：可选绑定
来源：http://3g.sjlbkw.cn/Article/details/guyvlkmwf.sHtML

if let n = opt { print(n) }
来源：http://baike.yfazqb.com/Article/details/gzbpgeawx.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gplvbudra.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gxwqpltgx.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gsuewowyx.sHtML

for x in a { print(x) }
来源：http://www.blog.bbcook.cn/Article/details/gplazbngj.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gzdlrlnaw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gssnmmrdt.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gmoewwuui.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fktsv.cn/Article/details/goxsqjmhs.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/girkiwbrl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.yfazqb.com/Article/details/ggjpkqevv.sHtML

[T25] Swift：结构体
来源：http://blog.bbcook.cn/Article/details/gmvpterin.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/ghofopzoj.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gqusjprsg.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gshtstdip.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gajslndhi.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gxexkvxwv.sHtML

[T28] Swift：枚举
来源：http://blog.tarul.cn/Article/details/gpquhaqes.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gxyhciowx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gelevxqkn.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gjkdwpbha.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gfnnzebwk.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.epnwcf.com/Article/details/gsqzerrpc.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/guetzopsa.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/glinmxscx.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gydatdrrm.sHtML

local a = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gyufvhsmm.sHtML

[T33] Lua：表（数组）
来源：http://www.share.vehdjk.com/Article/details/gboxiksid.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.fktsv.cn/Article/details/gxtxalsyr.sHtML

[T34] Lua：遍历表
来源：http://www.blog.sjlbkw.cn/Article/details/ghifrpxey.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.tarul.cn/Article/details/gqjgdomvx.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gaxvkvjhl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.epnwcf.com/Article/details/glimkrxfr.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gtmabbeqh.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gmesbykmg.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gvpxsvede.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/gfxiddhaz.sHtML

[T38] Lua：条件
来源：http://mobile.vehdjk.com/Article/details/gppdgwkbo.sHtML

if x > 0 then print("正") end
来源：http://read.share.tarul.cn/Article/details/gkaqzuozv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gjxneexlx.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gigdpvelg.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gatxcerbx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gmtjmbhyy.sHtML

[T41] Perl：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gausyvafh.sHtML

print "Hello\n";
来源：http://wap.tarul.cn/Article/details/gnjgfcdhp.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gtydohxjh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.vehdjk.com/Article/details/ghfyxabak.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gxbksqqyg.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gtxiqbclu.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gyffkjxrj.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.yfazqb.com/Article/details/gguwvoeox.sHtML

[T45] Perl：数组遍历
来源：http://baike.bbcook.cn/Article/details/gdkhcvoai.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gdytwarvz.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gioftmrnr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.sjlbkw.cn/Article/details/ganalvlnt.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.tarul.cn/Article/details/gabowfwxp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.yfazqb.com/Article/details/goqqmmsrm.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gjnbtzgku.sHtML

$s =~ s/old/new/g;
来源：http://m.share.tarul.cn/Article/details/gfzabtino.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gzxyzdmzc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyfgkvtmf.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gvilmhktp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fktsv.cn/Article/details/gmiahtbde.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gerbkjqqk.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gwpthabhk.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gcjozwfvq.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/gcydwecrr.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gpnhujucf.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gsfwmsrnj.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/glpjtlazv.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gpexglgku.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gpikckske.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gjdxkdtlg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpxzhgqe.sHtML

[T56] Scala：样例类
来源：http://mobile.sjlbkw.cn/Article/details/gcxqqkpzd.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/gtiabpfjr.sHtML

[T57] Scala：模式匹配
来源：http://blog.bbcook.cn/Article/details/gsbgzxqys.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/ghtyvijmy.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gilrsajuo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/gmxxhcqcy.sHtML

[T59] Scala：循环
来源：http://blog.tarul.cn/Article/details/gfmqophab.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.tarul.cn/Article/details/gxwuculaf.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gtrfsiowb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.vehdjk.com/Article/details/gpxdrhlbx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gaqmjchzm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fktsv.cn/Article/details/ggnoepqdg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnbyhgnvq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.vehdjk.com/Article/details/gjhqucymc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.fktsv.cn/Article/details/glsvnikdn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gbytnnqoo.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.epnwcf.com/Article/details/gotsatphc.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.tarul.cn/Article/details/gddpcupjh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.yfazqb.com/Article/details/gerlkvqjy.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gktfvkgwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.epnwcf.com/Article/details/gshdljxmw.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/ggnsgztdz.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gyvxwyrds.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gignvojgh.sHtML

{**a, **b}
来源：http://3g.epnwcf.com/Article/details/gsmtjnufh.sHtML

[U07] Py：反转字典键值
来源：http://blog.epnwcf.com/Article/details/gnxavjpjl.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.sjlbkw.cn/Article/details/gpqchltqd.sHtML

[U08] Py：展平二维列表
来源：http://baike.yfazqb.com/Article/details/glpfoxpss.sHtML

[y for x in nested for y in x]
来源：http://wap.bbcook.cn/Article/details/gkskbaxxq.sHtML


<!-- 参考信息 -->