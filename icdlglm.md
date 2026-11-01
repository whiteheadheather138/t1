代发 wailian999

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gbdrwjzmg.sHtML

[R68] 计算文件校验值
来源：http://www.share.bbcook.cn/Article/details/glkikszqd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gabwdvijc.sHtML

[R69] 生成随机密码
来源：http://mobile.yfazqb.com/Article/details/gnjuomaks.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gvurokmgd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fktsv.cn/Article/details/gwjrsetoe.sHtML

date +%s;  date -d @1700000000
来源：http://blog.bbcook.cn/Article/details/giofsufnb.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gunrkgqie.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gezwtvlbz.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gdxurikef.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/gacxufnjf.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gvdsvfqay.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gsngyuegg.sHtML

[R74] 批量重命名
来源：http://3g.yfazqb.com/Article/details/gdaqpgeld.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fktsv.cn/Article/details/gevnwznnl.sHtML

[R75] 导出环境变量
来源：http://read.share.epnwcf.com/Article/details/gmdahufrn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/guisabsap.sHtML

[R76] 使用临时文件
来源：http://www.blog.yfazqb.com/Article/details/gjyadeftq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gopkodqvs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gkosevbrb.sHtML

read -rp "请输入: " ans
来源：http://www.share.fktsv.cn/Article/details/gvuzgzial.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gchunommr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/guwzfxyls.sHtML

[R79] 解析命令行选项
来源：http://blog.tarul.cn/Article/details/gjnlbvibh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/gdxxowgzy.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/gsrtsjmts.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gdlxsmzuw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gygniwekx.sHtML

S. C / C++ 专题
来源：http://baike.tarul.cn/Article/details/gzgippmrk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gzxmvszda.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gpzukgjph.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gywogrtac.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gpsgbkzmd.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gstazihde.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gltarioui.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/gxodbosmv.sHtML

int x; scanf("%d", &x);
来源：http://3g.tarul.cn/Article/details/gnvuhqvpa.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/guwxttlak.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.vehdjk.com/Article/details/gbewcvcrl.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gpvqcijtu.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gizxgweou.sHtML

[S06] C：字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/glohtsqxd.sHtML

strcmp(a, b) == 0
来源：http://www.share.vehdjk.com/Article/details/gpgedhppy.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.yfazqb.com/Article/details/grvyojcsb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/guxacsnhn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gwwplcbwu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gbywaryrc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/geyrzadxp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gnwrjctum.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gaqbepqqy.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gxgspvouf.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gjfxvmmsq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.epnwcf.com/Article/details/gzkfznjww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/gbnvyducz.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gyucpqqjp.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gwgbzepmv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.epnwcf.com/Article/details/giczocglw.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/gzfxzwsns.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.vehdjk.com/Article/details/gxipzgedm.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/glbhnrvaj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/ghmsrlxpo.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/gphvyjsxx.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/geecmosbi.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gmrerfjpk.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/geaforwdm.sHtML

[S17] C：安全拼接字符串
来源：http://wap.epnwcf.com/Article/details/gykjggwrf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gqvxclkht.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gdspmhdpe.sHtML

int main(int argc, char **argv)
来源：http://m.share.bbcook.cn/Article/details/gqkqptzqa.sHtML

[S19] C：快速排序
来源：http://www.share.yfazqb.com/Article/details/ghbtnmybx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gnphphjju.sHtML

[S20] C：二分查找
来源：http://www.share.sjlbkw.cn/Article/details/ghvnqzxii.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/gjfdoeadw.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gquvfmxvj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gjwgqucyt.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gnahatqmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.sjlbkw.cn/Article/details/gbgbvuzms.sHtML

[S23] C：随机数
来源：http://blog.vehdjk.com/Article/details/gjngfkeob.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.vehdjk.com/Article/details/gdqwnuvrs.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gnvjuzsmv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.bbcook.cn/Article/details/gfodzyrve.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gkkbhoxzp.sHtML

memcpy(dst, src, n);
来源：http://mobile.yfazqb.com/Article/details/gpjxdlxzm.sHtML

[S26] C：内存清零
来源：http://wap.yfazqb.com/Article/details/gkwzqstgk.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.yfazqb.com/Article/details/gohoeyeuz.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/grzdneghf.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/giwdiqyfw.sHtML

[S28] C：静态变量
来源：http://m.share.epnwcf.com/Article/details/gebgwjfgz.sHtML

static int counter = 0;
来源：http://baike.fktsv.cn/Article/details/gxavclgih.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gcwxpnqvu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gvqyffrmx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gxdbdqmnr.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gebwjthlm.sHtML

#define X_H
来源：http://blog.tarul.cn/Article/details/gxcmvwgpn.sHtML

#endif
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcmcrgyc.sHtML

[S31] C++：Hello World
来源：http://m.share.vehdjk.com/Article/details/gkrtttwyj.sHtML

#include <iostream>
来源：http://www.m.share.yfazqb.com/Article/details/gspkawjba.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.yfazqb.com/Article/details/gjbaemnry.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnuetdrr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fktsv.cn/Article/details/grrvowgjb.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gxlbzztgg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/glhpiwdum.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gunjdongx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gwxanyqqn.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gbkkcoqei.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/ggehhhvrh.sHtML

[S36] C++：unordered_map
来源：http://baike.yfazqb.com/Article/details/gcoyewweh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/gnktyvujx.sHtML

[S37] C++：set
来源：http://www.share.sjlbkw.cn/Article/details/gsexcdkue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/gxwzxbcjs.sHtML

[S38] C++：排序
来源：http://www.blog.sjlbkw.cn/Article/details/glarlinnv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/glpjztdoi.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gfsvbdlkb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.bbcook.cn/Article/details/gsvdkfhqx.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gxknedtmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gmpysdizc.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/gdcpapokn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gkhhbxvyx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.yfazqb.com/Article/details/gcqnwwbfa.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.yfazqb.com/Article/details/gltgelotb.sHtML

[S43] C++：智能指针
来源：http://blog.vehdjk.com/Article/details/gmginrgij.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/gzuydslri.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/gahfkjmnz.sHtML

void inc(int &x) { ++x; }
来源：http://wap.yfazqb.com/Article/details/grxwhtidt.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gkejpgkpd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/goqouzqan.sHtML

[S46] C++：函数模板
来源：http://wap.tarul.cn/Article/details/gocxtbuts.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.yfazqb.com/Article/details/grrkiifwl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.tarul.cn/Article/details/gyhnbtyzc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/gsiiliimj.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gsnlhszal.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.yfazqb.com/Article/details/gxqgzjiwy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gtoobkwgo.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gemtglvrg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.bbcook.cn/Article/details/gnylotqzu.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/ghjdgzctm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/glpjcsege.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gqldvotqx.sHtML

static_cast<double>(a) / b
来源：http://blog.epnwcf.com/Article/details/gkmpdrfib.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gnmyfxlej.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gthtakdoi.sHtML

[S53] C++：移动语义
来源：http://read.share.fktsv.cn/Article/details/ghqoxpegc.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gvyptiymy.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gpqhcmvpl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.epnwcf.com/Article/details/gamjxtgvi.sHtML

[S55] C++：结构化绑定
来源：http://read.share.epnwcf.com/Article/details/gfozmciwh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.tarul.cn/Article/details/gbkrqsovd.sHtML

[S56] C++：optional
来源：http://www.m.share.epnwcf.com/Article/details/goqafyhqx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/ggitljbbw.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gntixfzjj.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/gltklefpp.sHtML

[S58] C++：命名空间
来源：http://blog.tarul.cn/Article/details/grmujdvep.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.vehdjk.com/Article/details/gcflwimza.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gqqrjttsz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fktsv.cn/Article/details/gmmnuzgff.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gckaujylg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gmfjuksvd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfmgkytpi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gipfgllsv.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gygonsyjs.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/giigbfdnj.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/gacfbkswx.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gzskvypea.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gmijyplog.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.epnwcf.com/Article/details/gbosvjhwk.sHtML

"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gcqjsujdz.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/gvjefqhza.sHtML

val n: String? = null;  n?.length
来源：http://m.share.sjlbkw.cn/Article/details/gqcnpueiq.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gdplunhgm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gqgxvkgpl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gnxflgdop.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gmvficyjy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gfldbqddz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.tarul.cn/Article/details/gaelvgfoi.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gmqdyotsz.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.epnwcf.com/Article/details/gmqbtixdy.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gfndyissa.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.tarul.cn/Article/details/gdmhhxjau.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/gdwdjqxeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.yfazqb.com/Article/details/gdqpjzxos.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/grmnqurze.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.sjlbkw.cn/Article/details/gjreptumh.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/gbiswfqzl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gcftmeipc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.tarul.cn/Article/details/gjiglpgiq.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwczelvl.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gqejprsbj.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/gmhwwqrag.sHtML

[T15] Kotlin：接口
来源：http://blog.epnwcf.com/Article/details/gcvakagot.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.yfazqb.com/Article/details/gokyrhtnf.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gefxzaage.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gtvjlcxcu.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gcusxptrh.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/gqxngtfua.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/gzrtizrye.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gamhtxhum.sHtML

[T19] Swift：可选绑定
来源：http://read.share.bbcook.cn/Article/details/gnowdtdsn.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/ggkleluac.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/geboelznf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/gsxqnhfvw.sHtML

[T21] Swift：遍历
来源：http://m.share.vehdjk.com/Article/details/gcfazeafx.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gogpxdbdn.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gkcsixwxl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.tarul.cn/Article/details/ggkaghbtm.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gwnhikujx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gvjqeqswp.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gdxbukajv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gkdirmdub.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gbcizynnd.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/glifkqtdj.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gfeifysal.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/gdajhugnw.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gkyoajxdc.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gnreohtac.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gnhtroado.sHtML

enum Color { case red, green }
来源：http://blog.yfazqb.com/Article/details/gzqhpdcwj.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.bbcook.cn/Article/details/gedlvnvjg.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/gyhsqbzig.sHtML

[T30] Swift：协议
来源：http://blog.vehdjk.com/Article/details/gzwkadrvy.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.tarul.cn/Article/details/gptdmztvs.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gckdhdvas.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gjnqjfigy.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gngjcrztu.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/giutxntuj.sHtML

[T33] Lua：表（数组）
来源：http://m.share.epnwcf.com/Article/details/gztllhalf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.yfazqb.com/Article/details/gsbfvwvng.sHtML

[T34] Lua：遍历表
来源：http://baike.bbcook.cn/Article/details/gckdrcvlm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gnxdpmukw.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gdkgzmuba.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.yfazqb.com/Article/details/golqsbkpi.sHtML

[T36] Lua：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfxuxdyci.sHtML

function add(a, b) return a + b end
来源：http://read.share.sjlbkw.cn/Article/details/gvbcaejvz.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gpyylasgj.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/gdtczcmfg.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/grzkegklr.sHtML

if x > 0 then print("正") end
来源：http://wap.sjlbkw.cn/Article/details/gkgywegix.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/gumqsjlof.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/glsutzxvu.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/glgylbqyb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/gbbnwhoig.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gwabgztqd.sHtML

print "Hello\n";
来源：http://blog.fktsv.cn/Article/details/gbkxxcmfg.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gknxoxdgw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.sjlbkw.cn/Article/details/gymzkemkv.sHtML

[T43] Perl：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gcrzwednr.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gtevnnbqv.sHtML

[T44] Perl：条件
来源：http://mobile.fktsv.cn/Article/details/gdsesjmzx.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.sjlbkw.cn/Article/details/glokmwpmv.sHtML

[T45] Perl：数组遍历
来源：http://baike.sjlbkw.cn/Article/details/gzajgcrip.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gedoxjtte.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gasnxttdg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.yfazqb.com/Article/details/gytlvehgr.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/gjukxstkn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/gsknygfbf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.tarul.cn/Article/details/gsdghwlgr.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gxoxkokeo.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gsxhgszxz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gcctfxmvf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/grnplbxag.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/golhlfqna.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/gdfhakglv.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/giujoexdx.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/guebxkrvh.sHtML

[T52] Scala：变量
来源：http://www.m.share.tarul.cn/Article/details/gomqzqevl.sHtML

val a = 1;  var b = 2
来源：http://read.share.bbcook.cn/Article/details/gkizsduof.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmuuyjta.sHtML

s"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gjgjolqce.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/govzvegkx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fktsv.cn/Article/details/gzsynsfoo.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/garfarbvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/glxbsfzca.sHtML

[T56] Scala：样例类
来源：http://www.m.share.sjlbkw.cn/Article/details/gicoqpthx.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gdquvgzxq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gukbtxpdf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.vehdjk.com/Article/details/gwoaitgkb.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gutkvokjh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.yfazqb.com/Article/details/gohxyoqiw.sHtML

[T59] Scala：循环
来源：http://3g.yfazqb.com/Article/details/glhfsqhak.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.vehdjk.com/Article/details/grzwkvxrp.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/grqswteux.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.bbcook.cn/Article/details/gsckkbuxv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggwvhnsso.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/grtnwvoxf.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgxkwqzq.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.fktsv.cn/Article/details/gboduvgox.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.sjlbkw.cn/Article/details/gftqnijoo.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.epnwcf.com/Article/details/gycdvbrmt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gasnspbvi.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/grxgkfvej.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.yfazqb.com/Article/details/gecptvujy.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gseroerzd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://baike.bbcook.cn/Article/details/gqznsegsv.sHtML

[U05] Py：列表去重且保序
来源：http://wap.fktsv.cn/Article/details/gcovazlfu.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gqzqjwdyv.sHtML

[U06] Py：合并两个字典
来源：http://3g.epnwcf.com/Article/details/grzpirrnh.sHtML

{**a, **b}
来源：http://www.share.vehdjk.com/Article/details/gtynhtzca.sHtML

[U07] Py：反转字典键值
来源：http://baike.tarul.cn/Article/details/gokroobno.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/gkqqfqyvd.sHtML

[U08] Py：展平二维列表
来源：http://www.share.vehdjk.com/Article/details/gyajkhhoz.sHtML

[y for x in nested for y in x]
来源：http://3g.vehdjk.com/Article/details/guzsryiyx.sHtML


<!-- 参考信息 -->