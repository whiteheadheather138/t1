代发 wailian999

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gmegaqovf.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gsdnksdcj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gakdcmggm.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gtypzckal.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gxvgrsaqa.sHtML

[R70] 时间戳与互转
来源：http://3g.tarul.cn/Article/details/gupaseban.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gzkvexose.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gmlswxihc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gqnksxbia.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gbjetgoss.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/geoniktex.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gggaxadaq.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/ghikolxpl.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gelusdpod.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gqbcjhjyr.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gjodkwziw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.tarul.cn/Article/details/gbocybkfy.sHtML

[R76] 使用临时文件
来源：http://www.share.vehdjk.com/Article/details/gftqmmoby.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gfijhnxnj.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gfessuqyw.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.bbcook.cn/Article/details/gryhphxwn.sHtML

[R78] 交互式菜单
来源：http://m.share.sjlbkw.cn/Article/details/ggtgsfxqe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gpuaexwjv.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gyjndxkrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/glpjcidhe.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/gqfkujuyl.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/gjfncpczr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxaoxjoer.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/gosvhcszv.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtgoubayv.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gguylebzm.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/guiakohqm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gwxpfkcqe.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gyjzdeeay.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gqsgbounw.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gsohccnfp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gvydibppb.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gihfkhatc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/grpkrdxvz.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gdeiaxuku.sHtML

strlen(s)
来源：http://m.share.tarul.cn/Article/details/gwveylrcr.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gzanuhnyh.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gpddbhbuu.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/gqwllweut.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.bbcook.cn/Article/details/grvpwvfbb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/ghufvhwrz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gcpbgumnp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gvtpkghoo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.yfazqb.com/Article/details/gkfdzxpqw.sHtML

[S10] C：指针与解引用
来源：http://3g.sjlbkw.cn/Article/details/gawrzlwhy.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gcrygdppf.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gpkwwodqf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.sjlbkw.cn/Article/details/gfrdodmsi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.vehdjk.com/Article/details/gqlkknffv.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gtmvomobi.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gdmgtiice.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gbvibgppc.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/ghbftjhkf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.bbcook.cn/Article/details/gnlukuxln.sHtML

[S14] C：枚举
来源：http://wap.bbcook.cn/Article/details/gloeewwfs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/getvdocps.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/gfrcypibw.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gugrhsoqa.sHtML

[S16] C：位操作置位
来源：http://blog.fktsv.cn/Article/details/grsfqyysk.sHtML

x |= (1 << 3);
来源：http://www.blog.tarul.cn/Article/details/gjudtmeca.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gtzdrgktj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gosjpyick.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gyyfjnazi.sHtML

int main(int argc, char **argv)
来源：http://m.share.sjlbkw.cn/Article/details/gbjaoisie.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gjdplrmhy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.tarul.cn/Article/details/gkpmjxplf.sHtML

[S20] C：二分查找
来源：http://blog.tarul.cn/Article/details/gcucczddo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gwbwlcsxz.sHtML

[S21] C：字符类别判断
来源：http://read.share.bbcook.cn/Article/details/gufbzyggk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/grkkaygoz.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gryadpsph.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gyjmpzboa.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gziqcqtxj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.vehdjk.com/Article/details/grijzjkja.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gzdwigfdb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fktsv.cn/Article/details/gmwtavbfa.sHtML

[S25] C：内存拷贝
来源：http://baike.epnwcf.com/Article/details/gpctihghc.sHtML

memcpy(dst, src, n);
来源：http://mobile.tarul.cn/Article/details/geewdulpv.sHtML

[S26] C：内存清零
来源：http://m.share.tarul.cn/Article/details/gprsuxevl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.yfazqb.com/Article/details/gaklqfqkx.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gzjpvnwhe.sHtML

const double PI = 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/grejgthpl.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/ghotlsymb.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gnkpeqzbj.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/gzmcomafc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.bbcook.cn/Article/details/gwaxfhopa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnjgdplf.sHtML

#ifndef X_H
来源：http://baike.fktsv.cn/Article/details/gbizoqcyw.sHtML

#define X_H
来源：http://www.blog.bbcook.cn/Article/details/gupkoetzc.sHtML

#endif
来源：http://m.share.yfazqb.com/Article/details/gokfihztj.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/ggtmkyfzg.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gwywyarkr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.vehdjk.com/Article/details/grnrelmew.sHtML

[S32] C++：字符串
来源：http://m.share.fktsv.cn/Article/details/gcvwrnobc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.bbcook.cn/Article/details/gswuudoao.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gmozudjeg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.yfazqb.com/Article/details/gdymgboqq.sHtML

[S34] C++：遍历 vector
来源：http://3g.epnwcf.com/Article/details/genmidxne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gtizyvhxw.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/grzitguwm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/grkewontk.sHtML

[S36] C++：unordered_map
来源：http://baike.sjlbkw.cn/Article/details/gipesttzz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gasbfgdws.sHtML

[S37] C++：set
来源：http://m.share.yfazqb.com/Article/details/gcejglial.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gualgqxdz.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gtiurjkaa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.bbcook.cn/Article/details/gapiqzadi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/gurlgwwqo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.vehdjk.com/Article/details/gymjidmae.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gagdfqmyk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/glnvuvqcr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/ghtmzvlik.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gpepkdfun.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gsytchtqm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gvzsxvjte.sHtML

[S43] C++：智能指针
来源：http://wap.vehdjk.com/Article/details/gcttpekkq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gyfcqnvim.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gfplflkrs.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gnbbheinw.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/ghwmtzojl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gfhdhugkf.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gjsiyoenj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/ghakemftr.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.vehdjk.com/Article/details/gaymmyjgs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fktsv.cn/Article/details/gtenvgfmd.sHtML

[S48] C++：逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gjmrfqizv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.vehdjk.com/Article/details/gefhjtqbk.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/guesqgkax.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gcwhvcfeq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gnzfckype.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gldpfsctb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gcvaiebii.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gemhuspkq.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gprrwrzdx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gihmeadmp.sHtML

int size() const noexcept { return n_; }
来源：http://baike.epnwcf.com/Article/details/gdexuclib.sHtML

[S53] C++：移动语义
来源：http://wap.sjlbkw.cn/Article/details/gzpqjailr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/ghhmylzye.sHtML

[S54] C++：异常处理
来源：http://3g.sjlbkw.cn/Article/details/guicjnofn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.sjlbkw.cn/Article/details/gaqixcsxh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.tarul.cn/Article/details/gdspunxav.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/gujzxfwjn.sHtML

[S56] C++：optional
来源：http://read.share.fktsv.cn/Article/details/gcnlbsvpf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fktsv.cn/Article/details/gkblyhdld.sHtML

[S57] C++：编译期常量
来源：http://baike.sjlbkw.cn/Article/details/gsoexmshl.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gnfsikgji.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gtksekwql.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gecidxvrq.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gqdyfyrdx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/gkqzktlsi.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/gyrcxzqop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gesbcyjbx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnwbkslgb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.tarul.cn/Article/details/glcxwktqn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjezhouff.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gylsazqfd.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gcpxinlij.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gqmewyzry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.sjlbkw.cn/Article/details/gdyhftfpy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.yfazqb.com/Article/details/gwfizxnww.sHtML

"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gsbmnzuid.sHtML

[T04] Kotlin：空安全
来源：http://m.share.sjlbkw.cn/Article/details/gcdpclodt.sHtML

val n: String? = null;  n?.length
来源：http://baike.bbcook.cn/Article/details/glseaxozh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gacyyftrw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gtxamumnc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.epnwcf.com/Article/details/gmhpogwxz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gunwxkkpg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.vehdjk.com/Article/details/gyxyaoohr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gnaopyurt.sHtML

[T08] Kotlin：数据类
来源：http://m.share.yfazqb.com/Article/details/gnxonknbr.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.bbcook.cn/Article/details/guvduzvfx.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gzbhktzka.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/ggifmxpyg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/ggneplxet.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gqkpagtxn.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gqzukfjqs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.tarul.cn/Article/details/gkfwapfay.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/ggnxeorbn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gzmppdhcq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.epnwcf.com/Article/details/gotqtxfvg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.epnwcf.com/Article/details/gyptpbtcn.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/glxjwlydz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.vehdjk.com/Article/details/gkwjieylj.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gpcyddoey.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gjwnkyexj.sHtML

[T16] Swift：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gwdeslveu.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gladpolcc.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/grcklsrin.sHtML

var a = 1;  let b = 2
来源：http://3g.sjlbkw.cn/Article/details/gnbmmzioy.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gtzkqcpzw.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gpmfnnyaw.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/gzfkhvpql.sHtML

if let n = opt { print(n) }
来源：http://3g.epnwcf.com/Article/details/gynyqajfg.sHtML

[T20] Swift：数组操作
来源：http://read.share.vehdjk.com/Article/details/geabnhesb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/gjxkdcenn.sHtML

[T21] Swift：遍历
来源：http://baike.yfazqb.com/Article/details/gnwurbxds.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gojveuiij.sHtML

[T22] Swift：字典
来源：http://blog.bbcook.cn/Article/details/gfigalunu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.epnwcf.com/Article/details/gltomully.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/gfbclkiyy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/ghdyexyul.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gexynuard.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.bbcook.cn/Article/details/ghcqowrew.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gkqtgtyvh.sHtML

struct P { var x: Int }
来源：http://www.share.bbcook.cn/Article/details/gxieopbqx.sHtML

[T26] Swift：类与重写
来源：http://read.share.tarul.cn/Article/details/gkcplaxpi.sHtML

class A: Base { override func f() {} }
来源：http://m.share.bbcook.cn/Article/details/gjtdjcmtw.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/grxfgwbcy.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gpmxwiemo.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/gwxswhwku.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gbxekpowy.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fktsv.cn/Article/details/gwioxwevi.sHtML

guard let x = opt else { return }
来源：http://mobile.fktsv.cn/Article/details/gcycxgebi.sHtML

[T30] Swift：协议
来源：http://www.share.vehdjk.com/Article/details/gverwocsz.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.bbcook.cn/Article/details/goagyvyhu.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/goiorkgcj.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gsqahuzaq.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gvqorldcl.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gxhviohtn.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.bbcook.cn/Article/details/gesdfnakn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gbpdfmmcw.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gomzfwvsu.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.epnwcf.com/Article/details/gvvandeud.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gmtaucfje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/ggawhdadq.sHtML

[T36] Lua：函数
来源：http://www.m.share.vehdjk.com/Article/details/gtoeqagho.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gddrxpxeq.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gxwfwqtwd.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gjxkagfog.sHtML

[T38] Lua：条件
来源：http://www.share.fktsv.cn/Article/details/glkhyxgvh.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/gtrbacugv.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gluobsuos.sHtML

string.find(s, "%d+")
来源：http://3g.tarul.cn/Article/details/gtiengfjx.sHtML

[T40] Lua：元表
来源：http://m.share.bbcook.cn/Article/details/ghomeltaq.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.yfazqb.com/Article/details/ghvyrpnsi.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/ghybvekjm.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gnvhybppb.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gjwxiiuxk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gyoflxguy.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/gyamlknin.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gwjtkdzsn.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/gpbzfvixt.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/ghgmttqzl.sHtML

[T45] Perl：数组遍历
来源：http://baike.fktsv.cn/Article/details/gohnghhzx.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gpeimpycf.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gasnifqwx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/guvaynfqf.sHtML

[T47] Perl：正则捕获
来源：http://wap.yfazqb.com/Article/details/gbdcvsnhw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gnqqdyigu.sHtML

[T48] Perl：正则替换
来源：http://baike.sjlbkw.cn/Article/details/gbqzdjzsv.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gewmujytt.sHtML

[T49] Perl：函数
来源：http://www.m.share.vehdjk.com/Article/details/gwqupkyyn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.vehdjk.com/Article/details/gwopgisbz.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gmropkwzp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gyvjqhptq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.tarul.cn/Article/details/ggkopgpru.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjwgiyao.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/gfrkorgym.sHtML

[T52] Scala：变量
来源：http://www.blog.epnwcf.com/Article/details/gpixmrfwv.sHtML

val a = 1;  var b = 2
来源：http://www.share.epnwcf.com/Article/details/geozvmibz.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gndihvcdx.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/gkszuntnh.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/guietcniv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gziloxwdg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gvomgpilu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.tarul.cn/Article/details/gbbctzlch.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gsejckdlb.sHtML

case class User(name: String, age: Int)
来源：http://blog.epnwcf.com/Article/details/gvprpmubo.sHtML

[T57] Scala：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gsiqwzzkd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/gyhzrcmja.sHtML

[T58] Scala：函数定义
来源：http://baike.bbcook.cn/Article/details/gydxowncw.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gvqbbpthm.sHtML

[T59] Scala：循环
来源：http://read.share.fktsv.cn/Article/details/gjxkxjtzh.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gxpbmhfrt.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/gtdrazztu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.tarul.cn/Article/details/gjtmtnpye.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjpsrhwu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/gojgjzurf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtpyebznq.sHtML

[U01] Py：创建虚拟环境
来源：http://m.share.yfazqb.com/Article/details/gvjruhoxw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/ghzojjtiw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/ghbqezqgw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gvynqjrha.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/gbrxppzek.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.tarul.cn/Article/details/gsooasmvx.sHtML

[U04] Py：变量调试打印
来源：http://baike.tarul.cn/Article/details/gjxbcswyq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.bbcook.cn/Article/details/gomvxsbxk.sHtML

[U05] Py：列表去重且保序
来源：http://3g.yfazqb.com/Article/details/gswkaouin.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.sjlbkw.cn/Article/details/gbfydoojn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.tarul.cn/Article/details/gxapqkzat.sHtML

{**a, **b}
来源：http://mobile.vehdjk.com/Article/details/goopgxgoh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.epnwcf.com/Article/details/grijxbqbs.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gujpqekfv.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gjjhziaei.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gigvzehlv.sHtML


<!-- 参考信息 -->