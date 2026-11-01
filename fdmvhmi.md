代发 wailian999

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gisyiavie.sHtML

[R68] 计算文件校验值
来源：http://www.blog.tarul.cn/Article/details/gsewqoghm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/gebjpehpn.sHtML

[R69] 生成随机密码
来源：http://baike.fktsv.cn/Article/details/gsrwgyfml.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.sjlbkw.cn/Article/details/gbtqwmqew.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gyhoytezb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gickylymc.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gqatbadtz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.yfazqb.com/Article/details/gwcmkqtra.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gfsqyerma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gdiiqpijq.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gocxpinof.sHtML

split -l 1000 big.log part_
来源：http://www.share.vehdjk.com/Article/details/gkxeqfpzz.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gygvbpvfr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fktsv.cn/Article/details/gsidwjirm.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gjsbjalbb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gyxhwnbvr.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/glnkrzrdw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.bbcook.cn/Article/details/gsznpydgo.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/ghukrrayf.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gtxrozwpg.sHtML

[R78] 交互式菜单
来源：http://blog.epnwcf.com/Article/details/gyuzbnpjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/grmxvvpgm.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gylldhzhw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gnkzxlttx.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.tarul.cn/Article/details/gpwsvsxww.sHtML

time ./run.sh
来源：http://www.blog.yfazqb.com/Article/details/gcbwcvfyg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gymtgpjat.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gcdimjpku.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpzhblfyj.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/grynzuozx.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gpzhadslu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.vehdjk.com/Article/details/gldmzrryc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.sjlbkw.cn/Article/details/gdbrudveo.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/ghxcaxtpj.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gtfhvprzp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.yfazqb.com/Article/details/gndwahfkk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gxerfjaue.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/gzfiskkep.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gpiirjinp.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gcgglavlh.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gtpunxiyu.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/glbjarkvo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gfeorkkjn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.sjlbkw.cn/Article/details/grajwlrhh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/goaxyebwc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fktsv.cn/Article/details/gmsiaoqnm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.epnwcf.com/Article/details/gnwgdrzcz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/gorblfimz.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/ghtdkxchh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.sjlbkw.cn/Article/details/gzelinhsu.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gowkjkyyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.bbcook.cn/Article/details/ghhjugzwx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gscqrtgaa.sHtML

fclose(f);
来源：http://blog.yfazqb.com/Article/details/geckbzmjn.sHtML

[S12] C：写文件
来源：http://wap.yfazqb.com/Article/details/guqqlgrxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gqmbvloon.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/grfisacsc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/guaqaykev.sHtML

[S14] C：枚举
来源：http://blog.fktsv.cn/Article/details/gitcojyha.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fktsv.cn/Article/details/gnidstquy.sHtML

[S15] C：类型转换
来源：http://m.share.fktsv.cn/Article/details/gutdwubvu.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/gwglfrsxc.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/gxqkpfefi.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/giwtdlexp.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gkbmwtjea.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gsqopclly.sHtML

[S18] C：命令行参数
来源：http://m.share.tarul.cn/Article/details/ggxhhffam.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gqczpizrr.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gvrnsbioc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gwhilmplc.sHtML

[S20] C：二分查找
来源：http://baike.sjlbkw.cn/Article/details/gmyoacjrm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gbuugbipi.sHtML

[S21] C：字符类别判断
来源：http://blog.tarul.cn/Article/details/ggfvynzha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.vehdjk.com/Article/details/gyvxcajyy.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/getgxwrcx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/gpklgiyvu.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/ghqqsqwfv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/ghfmemmsd.sHtML

[S24] C：获取本地时间
来源：http://blog.tarul.cn/Article/details/gigdierwk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.yfazqb.com/Article/details/gxwlwhydy.sHtML

[S25] C：内存拷贝
来源：http://read.share.fktsv.cn/Article/details/gtjlwgdgl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/givvqutll.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gyhzopskg.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/ghpuszubc.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/gosatshge.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/giwnyuixi.sHtML

[S28] C：静态变量
来源：http://wap.yfazqb.com/Article/details/gmlxlucuo.sHtML

static int counter = 0;
来源：http://www.m.share.yfazqb.com/Article/details/gxpnaybpg.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gdnpwyqgj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/ghmfbslkb.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gxqliihpa.sHtML

#ifndef X_H
来源：http://www.m.share.yfazqb.com/Article/details/gwbkahtlb.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gnyxetseu.sHtML

#endif
来源：http://read.share.fktsv.cn/Article/details/gmevotwdg.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gimgvtnvx.sHtML

#include <iostream>
来源：http://read.share.sjlbkw.cn/Article/details/ghhfoqjrr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.tarul.cn/Article/details/guvgbgjcu.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gpogpykoc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.bbcook.cn/Article/details/gsctbvfxm.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gitshqqzn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.tarul.cn/Article/details/gljqrdasc.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/goulhtrks.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.yfazqb.com/Article/details/gletwkzyg.sHtML

[S35] C++：map
来源：http://baike.fktsv.cn/Article/details/gdzdcncll.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/ghauhudqc.sHtML

[S36] C++：unordered_map
来源：http://www.blog.yfazqb.com/Article/details/gpvirhxnp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gdlspvrne.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gcyncuvup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/gscpvvbso.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gsxdgobph.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gbpohekwq.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gcwwcmyfw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.epnwcf.com/Article/details/gokqzalfu.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/giihsodgp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/gyzpellwl.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gnlkqrdeq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gkupapbzb.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gnqdydkgw.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.bbcook.cn/Article/details/gzaipeoan.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gldjjkrzg.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gvcopkylw.sHtML

[S44] C++：引用传参
来源：http://blog.yfazqb.com/Article/details/gdmqfbnsj.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gupzbmsze.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/gjidgwhzn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.bbcook.cn/Article/details/grjuslict.sHtML

[S46] C++：函数模板
来源：http://baike.epnwcf.com/Article/details/gotfvhpdd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gzekxfbrn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.vehdjk.com/Article/details/grlpiyipd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gtnnahskn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gzfdthaad.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.vehdjk.com/Article/details/gdswogdkt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/ggtzhvzpw.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gaqsqynob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gbcaixevn.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gmzgdnixv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gljfaaxwt.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/gaahgqqik.sHtML

static_cast<double>(a) / b
来源：http://www.blog.yfazqb.com/Article/details/gwznkvrtg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/glvvfhyym.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gaoenspcv.sHtML

[S53] C++：移动语义
来源：http://www.share.tarul.cn/Article/details/gwumpqjfi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/gvtlzwdut.sHtML

[S54] C++：异常处理
来源：http://m.share.fktsv.cn/Article/details/galrjmdja.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gsfuxpowq.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gvmspesmz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gdmuubdou.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gzwgguwhl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.tarul.cn/Article/details/goharbpcv.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gvgmdjhbt.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/gaybjnrwr.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gibmtvupw.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gizfnauwr.sHtML

[S59] C++：静态断言
来源：http://read.share.vehdjk.com/Article/details/gtbawarkw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gbjqcokrx.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gfcdspkfu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gogdoarjd.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gufawybdr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/gutgyyrpb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvfzuzqjj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fktsv.cn/Article/details/gzxnwgjtp.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gjripxvwz.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/gpgqwcbte.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.bbcook.cn/Article/details/gztfvwdao.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.yfazqb.com/Article/details/gfqjufthd.sHtML

"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/gxmreadip.sHtML

[T04] Kotlin：空安全
来源：http://blog.vehdjk.com/Article/details/ghheqxrfv.sHtML

val n: String? = null;  n?.length
来源：http://wap.sjlbkw.cn/Article/details/grwcrqaag.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gzdwslxnu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gnvnpvzuk.sHtML

[T06] Kotlin：集合映射
来源：http://baike.yfazqb.com/Article/details/gwcrdztok.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.epnwcf.com/Article/details/gimpkrvzl.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.epnwcf.com/Article/details/ggyudouoy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/gquxawlsy.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fktsv.cn/Article/details/gtwnymvjp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gmemqgmyx.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fktsv.cn/Article/details/gdqoetovn.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.yfazqb.com/Article/details/gohyxpmky.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.epnwcf.com/Article/details/gxbmdmseb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gzdfmnfva.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/grveqwvze.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gnlpysdff.sHtML

[T12] Kotlin：解构声明
来源：http://baike.epnwcf.com/Article/details/geaeaacfb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gxxquuhmv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gidryhdim.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gukwasixa.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/grkjnsnzn.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/ghdmpqary.sHtML

[T15] Kotlin：接口
来源：http://blog.yfazqb.com/Article/details/giuounvte.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkccnbyor.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gozplzptw.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/gqvbanbss.sHtML

[T17] Swift：变量与常量
来源：http://baike.fktsv.cn/Article/details/geysqssou.sHtML

var a = 1;  let b = 2
来源：http://mobile.fktsv.cn/Article/details/gizdbzaxz.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gfsnrwxim.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gknpemvxy.sHtML

[T19] Swift：可选绑定
来源：http://3g.yfazqb.com/Article/details/guyxeksva.sHtML

if let n = opt { print(n) }
来源：http://mobile.epnwcf.com/Article/details/grwbmgpun.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/gflxxqzta.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/givhuvkpg.sHtML

[T21] Swift：遍历
来源：http://www.blog.sjlbkw.cn/Article/details/grtpxkbap.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/gmhemceof.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/ggcslsmwe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.yfazqb.com/Article/details/guiqufama.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gpppigfmh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/grhgykzri.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gilottbcl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/grcemrlqr.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/gerxmowzu.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/ghnohqbhf.sHtML

[T26] Swift：类与重写
来源：http://m.share.epnwcf.com/Article/details/gddsfbwlk.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gcrooalje.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/ggsocdbxd.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gegsvjnuo.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gcsnkfqqi.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gplwlgobr.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fktsv.cn/Article/details/gfebmllkk.sHtML

guard let x = opt else { return }
来源：http://www.m.share.tarul.cn/Article/details/gisvsnucw.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gcrayabdn.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.sjlbkw.cn/Article/details/gkqzlbqpj.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gndekbdsz.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gtfdzwztm.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gcliymxab.sHtML

local a = 1
来源：http://read.share.bbcook.cn/Article/details/gvlrkyfmu.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/grvetodmg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gobjhrfch.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gplibyvyk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gthnzrgjo.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/gbltltteg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gafgsbxzq.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/gmiitruhm.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/gzmpiwdhe.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gfjlhljmo.sHtML

"a" .. "b"
来源：http://m.share.sjlbkw.cn/Article/details/ghwsjifmp.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gkpzkmhef.sHtML

if x > 0 then print("正") end
来源：http://m.share.sjlbkw.cn/Article/details/ghicvxbrq.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gmanotcbc.sHtML

string.find(s, "%d+")
来源：http://www.blog.fktsv.cn/Article/details/gknkfrrgs.sHtML

[T40] Lua：元表
来源：http://www.share.sjlbkw.cn/Article/details/gsoafbusa.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gwvdyfbkm.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gvitjfpvn.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gjbjrjhjb.sHtML

[T42] Perl：变量类型
来源：http://blog.bbcook.cn/Article/details/grgdeobjy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.bbcook.cn/Article/details/gsefdtaae.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gjskinzgf.sHtML

"值: $a"
来源：http://www.m.share.yfazqb.com/Article/details/gaywntlrh.sHtML

[T44] Perl：条件
来源：http://baike.fktsv.cn/Article/details/glcixzwed.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gozepvxsj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.sjlbkw.cn/Article/details/gxwytlbds.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.epnwcf.com/Article/details/gzypbndek.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.epnwcf.com/Article/details/gafkudlux.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/ggzlyftkn.sHtML

[T47] Perl：正则捕获
来源：http://baike.sjlbkw.cn/Article/details/gaxiuuksl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.sjlbkw.cn/Article/details/ghsgtkega.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gilvlgprh.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gmzjyhgny.sHtML

[T49] Perl：函数
来源：http://read.share.fktsv.cn/Article/details/gamijwwxv.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/gjriupzim.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gnhfolyxo.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gczsfhyzj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.sjlbkw.cn/Article/details/gxmxfwhll.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ggegtkfob.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gycwezdsn.sHtML

[T52] Scala：变量
来源：http://wap.sjlbkw.cn/Article/details/gtzvhypwy.sHtML

val a = 1;  var b = 2
来源：http://www.share.tarul.cn/Article/details/goqfarwvs.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gradqqmdv.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gucxqwdzw.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gsmqzubnt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gwalfdvli.sHtML

[T55] Scala：集合过滤
来源：http://m.share.epnwcf.com/Article/details/gjsuocedc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.bbcook.cn/Article/details/gnthmkwks.sHtML

[T56] Scala：样例类
来源：http://blog.bbcook.cn/Article/details/gwnilzurd.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/gcphunztt.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gutpvsxsx.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.epnwcf.com/Article/details/gztyoolew.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/gokexozjm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/gbglpdtxw.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gpiprpxec.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gmosqqdrz.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/ghqhzgdli.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gjvshyumq.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gomszlxsb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.tarul.cn/Article/details/gjnbyavzc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdrrnibfp.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.sjlbkw.cn/Article/details/gmvhwnmth.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.epnwcf.com/Article/details/gstdmmrqk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.fktsv.cn/Article/details/gunvrdeow.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gtgssgnmg.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gycdamovx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.epnwcf.com/Article/details/gxqsijqmn.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gqtexnjov.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.yfazqb.com/Article/details/giiefnfpi.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.bbcook.cn/Article/details/gpsfdxrgi.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/gwoefpwqn.sHtML

[U06] Py：合并两个字典
来源：http://mobile.epnwcf.com/Article/details/ggvpsshse.sHtML

{**a, **b}
来源：http://mobile.yfazqb.com/Article/details/ggxatxiqo.sHtML

[U07] Py：反转字典键值
来源：http://3g.epnwcf.com/Article/details/giyrffert.sHtML

{v: k for k, v in d.items()}
来源：http://3g.sjlbkw.cn/Article/details/gthzkcmgn.sHtML

[U08] Py：展平二维列表
来源：http://wap.epnwcf.com/Article/details/gwcfobvmm.sHtML

[y for x in nested for y in x]
来源：http://m.share.tarul.cn/Article/details/gfeqbduuq.sHtML


<!-- 参考信息 -->