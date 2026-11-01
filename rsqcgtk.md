代发 wailian999

openssl rand -hex 16
来源：http://m.share.vehdjk.com/Article/details/gytmahbri.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/gxywjmtig.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gcfsnyoco.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gcpxblswa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gfzqhjskr.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gkyysowyq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fktsv.cn/Article/details/gohjidknt.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gebhwehbf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/grjdwnrgj.sHtML

[R72] 等待端口就绪
来源：http://blog.vehdjk.com/Article/details/glwdldxes.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gffbbeidb.sHtML

[R73] 分割大日志
来源：http://blog.fktsv.cn/Article/details/gaxpcgbeg.sHtML

split -l 1000 big.log part_
来源：http://wap.epnwcf.com/Article/details/grlsqtqwe.sHtML

[R74] 批量重命名
来源：http://www.share.vehdjk.com/Article/details/gnqjzwlfi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.bbcook.cn/Article/details/gdtcfmqhk.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gmuvjoxac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.sjlbkw.cn/Article/details/gegggaczw.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gcwpjcajm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gjrbluwsq.sHtML

[R77] 读取用户输入
来源：http://www.share.fktsv.cn/Article/details/gvyrdyzbw.sHtML

read -rp "请输入: " ans
来源：http://www.share.epnwcf.com/Article/details/ggyodnkad.sHtML

[R78] 交互式菜单
来源：http://blog.sjlbkw.cn/Article/details/guteezjvj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/ghgzukoaw.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/ghajfktih.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/gcaqfzijn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.yfazqb.com/Article/details/gngmwnsdk.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gomiahrjh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvjyxauts.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gctjekzxw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goiebltee.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gtfitxnrb.sHtML

#include <stdio.h>
来源：http://www.share.epnwcf.com/Article/details/gccnvnruv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/ggtegyyks.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gstswixpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.vehdjk.com/Article/details/gdzlwmvhw.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gipuzvemv.sHtML

int x; scanf("%d", &x);
来源：http://3g.yfazqb.com/Article/details/gloubdfsv.sHtML

[S04] C：字符串复制
来源：http://www.share.tarul.cn/Article/details/gaulqfxmd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gycqrxdpb.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gikmjuhsf.sHtML

strlen(s)
来源：http://www.share.fktsv.cn/Article/details/ggcfkjpqa.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gfykcysck.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gczrbaogg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.tarul.cn/Article/details/gawiaxjlg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gmjoamfmi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.vehdjk.com/Article/details/goiakldul.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gmwnbfmtl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.epnwcf.com/Article/details/gmqellfcc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gjueobhjj.sHtML

[S10] C：指针与解引用
来源：http://wap.vehdjk.com/Article/details/gjcvowzpz.sHtML

int *p = &a;  *p = 5;
来源：http://wap.yfazqb.com/Article/details/gcitnyvzs.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gnjkntnbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gffkiztmu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.vehdjk.com/Article/details/gzoyyflnk.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gistoepzr.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gctpzramy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.epnwcf.com/Article/details/gdutrzjqi.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gctvesoxs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/ggkgvivhx.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gerlhsnmb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.sjlbkw.cn/Article/details/gloslilbx.sHtML

[S15] C：类型转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gbimwyldk.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gvzycnymc.sHtML

[S16] C：位操作置位
来源：http://www.blog.vehdjk.com/Article/details/gypzgitmj.sHtML

x |= (1 << 3);
来源：http://www.blog.yfazqb.com/Article/details/ggdhxolox.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/glfnnrqbo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.bbcook.cn/Article/details/gxeoutpnc.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gamowrbxy.sHtML

int main(int argc, char **argv)
来源：http://mobile.yfazqb.com/Article/details/guzgknlkz.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/gvkpoijpo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.epnwcf.com/Article/details/gxhiokrki.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/ghzfpxyrj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/gboecsjjd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.vehdjk.com/Article/details/gfkaoowlq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.epnwcf.com/Article/details/gpfixbhbi.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/geenhqtdn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.bbcook.cn/Article/details/gbokhyojl.sHtML

[S23] C：随机数
来源：http://www.blog.sjlbkw.cn/Article/details/gehhpwyyz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gpuheswtq.sHtML

[S24] C：获取本地时间
来源：http://wap.epnwcf.com/Article/details/gnffmqrcw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.epnwcf.com/Article/details/govblzrap.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gpzeywzjl.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gtvrfxvft.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gymbsbfwz.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/gkcefvqlv.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gmqcjucqi.sHtML

const double PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/glghfvovh.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gvjkazchd.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/guoanymdq.sHtML

[S29] C：变参函数
来源：http://blog.yfazqb.com/Article/details/gxmuwudhq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gnufbifbs.sHtML

[S30] C：头文件保护
来源：http://m.share.yfazqb.com/Article/details/gkjhiuoed.sHtML

#ifndef X_H
来源：http://www.m.share.fktsv.cn/Article/details/gkzfewarw.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gcgfsrqjr.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gxnkalkec.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/geozdlwhc.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpckjgyp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/glvhyjjde.sHtML

[S32] C++：字符串
来源：http://www.blog.tarul.cn/Article/details/gipyjxhuk.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.bbcook.cn/Article/details/gnbcthqsy.sHtML

[S33] C++：vector 增删
来源：http://blog.vehdjk.com/Article/details/gpibeyraf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gzamvhydl.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gvluogbdv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.yfazqb.com/Article/details/ggzrsmazv.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gpfaqvmwz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gtczottnc.sHtML

[S36] C++：unordered_map
来源：http://3g.tarul.cn/Article/details/gbqfxcjpy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gepclpjto.sHtML

[S37] C++：set
来源：http://m.share.bbcook.cn/Article/details/gecneqnec.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gwzhkasga.sHtML

[S38] C++：排序
来源：http://read.share.vehdjk.com/Article/details/gfdarcsqj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gdlpdnyre.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gojqdtssv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.sjlbkw.cn/Article/details/gjxzuxyxj.sHtML

[S40] C++：查找元素
来源：http://3g.sjlbkw.cn/Article/details/gsqpwczgw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gxfrlagok.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gmjtojbua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/glfdbaqmv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gvvxhfzfv.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gtgjzqpan.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gsdvliirc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.sjlbkw.cn/Article/details/gbddfgtbu.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/ghlbstlsx.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbfdtlsrk.sHtML

[S45] C++：lambda
来源：http://read.share.yfazqb.com/Article/details/goqdntmat.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gwvabrsll.sHtML

[S46] C++：函数模板
来源：http://wap.epnwcf.com/Article/details/gomttwsqi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggcyfsoxv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gkommuwpb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gidudscdt.sHtML

[S48] C++：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gochxummb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.yfazqb.com/Article/details/gjibwghyl.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.yfazqb.com/Article/details/gmurtwgaj.sHtML

[S49] C++：写文件
来源：http://3g.yfazqb.com/Article/details/gfwvvplix.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.yfazqb.com/Article/details/gkeykjdal.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/ghlvdzqdj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gjwlaytwc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.bbcook.cn/Article/details/gqtaxtxqp.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gmsxsuqar.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gyzcxtchp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fktsv.cn/Article/details/ggwgufwxb.sHtML

[S53] C++：移动语义
来源：http://wap.vehdjk.com/Article/details/gkevewthy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gxeetpcgk.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gknmxxiom.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.sjlbkw.cn/Article/details/gwotjzpbf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.tarul.cn/Article/details/gwbtqfttt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gxesordhk.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gzcypzoff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/guugxukye.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/gdzispsey.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gbpurasme.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gpivigpgs.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/gnmfvxcyv.sHtML

[S59] C++：静态断言
来源：http://wap.fktsv.cn/Article/details/grawnmcqg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.epnwcf.com/Article/details/gsssamgxi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.sjlbkw.cn/Article/details/gxyzivbji.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/galttdklc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggxvqblad.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/ghocwpodp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gntimvvpo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gzpzfvnsv.sHtML

println("Hello")
来源：http://m.share.bbcook.cn/Article/details/ghtvuzmwl.sHtML

[T02] Kotlin：变量
来源：http://3g.yfazqb.com/Article/details/gyvgfyaya.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.tarul.cn/Article/details/ghijlqwuo.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.bbcook.cn/Article/details/ghgbvjoxr.sHtML

"值: $b"
来源：http://www.m.share.fktsv.cn/Article/details/gpuwnqubt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.tarul.cn/Article/details/gbbfsjwqc.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.vehdjk.com/Article/details/gccbmvniq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gudhvadbf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fktsv.cn/Article/details/gtavaahle.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gtgfhqmyi.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.vehdjk.com/Article/details/gfithanso.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/ghrcyplhk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.yfazqb.com/Article/details/gvvvwxtxn.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gmjomnwgo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gxnqixsdg.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gsdyvrgyn.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/garyaummh.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gzxagozes.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fktsv.cn/Article/details/gnnzokxfd.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/grovespmf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.epnwcf.com/Article/details/galeztiwh.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.bbcook.cn/Article/details/goxgxlgpt.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fktsv.cn/Article/details/gaxxcpxnq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fktsv.cn/Article/details/glujeiiup.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gmxxrpwoa.sHtML

[T14] Kotlin：循环
来源：http://3g.bbcook.cn/Article/details/gcdlsckmt.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gdkdndtlf.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gqsmsgbxb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/glzaqmovt.sHtML

[T16] Swift：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/goigbedsf.sHtML

print("Hello")
来源：http://wap.fktsv.cn/Article/details/gmwbuxhum.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gmztbdmin.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/glqniswta.sHtML

[T18] Swift：字符串插值
来源：http://baike.bbcook.cn/Article/details/gcprzscqe.sHtML

"值: \(b)"
来源：http://baike.tarul.cn/Article/details/gdidqlydm.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gqsnyvkdm.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/grqtchooq.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gtkalquqw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gkfolbeiy.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gtxmqknms.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/gupmlysmj.sHtML

[T22] Swift：字典
来源：http://3g.vehdjk.com/Article/details/guhomrklt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.vehdjk.com/Article/details/gsnyqhurp.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/ghjwkugqe.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gwqubsgjn.sHtML

[T24] Swift：闭包
来源：http://baike.bbcook.cn/Article/details/garmkvwon.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gbcphsffu.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/gntqskfyz.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gmxoazjhh.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gwfqxhozt.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gtqzlhmwd.sHtML

[T27] Swift：错误处理
来源：http://blog.sjlbkw.cn/Article/details/gklsshaln.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fktsv.cn/Article/details/goubgpwgl.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gcqhythbk.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/ghpfpnkmj.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gjovklqya.sHtML

guard let x = opt else { return }
来源：http://www.share.bbcook.cn/Article/details/gjacbmtti.sHtML

[T30] Swift：协议
来源：http://m.share.fktsv.cn/Article/details/gotopauur.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.epnwcf.com/Article/details/gigwiuwzw.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/glporjznb.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gqbdddjen.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/gjdwqdxtr.sHtML

local a = 1
来源：http://www.share.bbcook.cn/Article/details/gjneyotgx.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/gupkutpvl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.yfazqb.com/Article/details/gntosqrnc.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gtssljabt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fktsv.cn/Article/details/gndvvfjdv.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gpvzgfnfj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gajfhttsz.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gzydzseje.sHtML

function add(a, b) return a + b end
来源：http://mobile.sjlbkw.cn/Article/details/gmazijtds.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gejgnekcn.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gbokjdfmq.sHtML

[T38] Lua：条件
来源：http://wap.sjlbkw.cn/Article/details/gapsxnfxd.sHtML

if x > 0 then print("正") end
来源：http://www.blog.vehdjk.com/Article/details/gpgjnrrqa.sHtML

[T39] Lua：模式匹配
来源：http://baike.yfazqb.com/Article/details/gljtceffr.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gijpoamdg.sHtML

[T40] Lua：元表
来源：http://m.share.epnwcf.com/Article/details/gexbpphqz.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gmotbmjpl.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gtxopouty.sHtML

print "Hello\n";
来源：http://mobile.sjlbkw.cn/Article/details/grjzfykbc.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gldigesir.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gewjmsmsf.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/goyvwhejn.sHtML

"值: $a"
来源：http://www.share.sjlbkw.cn/Article/details/gbvagdidm.sHtML

[T44] Perl：条件
来源：http://www.m.share.tarul.cn/Article/details/grruqbzsu.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gavuhkmld.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gbxxqitau.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gczmhznea.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gwrcfnqkg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gotzjaqxt.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.vehdjk.com/Article/details/gizishpag.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.vehdjk.com/Article/details/gxswvpoii.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gmwzmofzy.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/glskhrtjp.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gaykgmnkx.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fktsv.cn/Article/details/gsfzrwwcs.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gymshkogy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gjwdipxgf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gnpzblkpi.sHtML

[T51] Scala：Hello World
来源：http://www.share.epnwcf.com/Article/details/gwlturqcn.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gmxtzjdad.sHtML

[T52] Scala：变量
来源：http://www.blog.bbcook.cn/Article/details/gbnorkeuv.sHtML

val a = 1;  var b = 2
来源：http://m.share.bbcook.cn/Article/details/gcvlmihto.sHtML

[T53] Scala：字符串插值
来源：http://blog.yfazqb.com/Article/details/gzmyzxlir.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gnpogvymd.sHtML

[T54] Scala：集合映射
来源：http://wap.bbcook.cn/Article/details/ghnjvrjyf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.yfazqb.com/Article/details/gzxbixcry.sHtML

[T55] Scala：集合过滤
来源：http://www.share.tarul.cn/Article/details/grxjbbnbk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gcyfrprgc.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gxykyswfo.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gwwlzffra.sHtML

[T57] Scala：模式匹配
来源：http://read.share.tarul.cn/Article/details/gtplocpwv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gslmsekbf.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gzsqfesfg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fktsv.cn/Article/details/giqkgivrv.sHtML

[T59] Scala：循环
来源：http://mobile.sjlbkw.cn/Article/details/gbxhtibvt.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gjeedmrrs.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gjqzreeyf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdrihqkg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gwasbikwo.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gvimuiksu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gffoxnpuf.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.bbcook.cn/Article/details/gcserumze.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.fktsv.cn/Article/details/gazigzwrt.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gkujquapj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.epnwcf.com/Article/details/gfpeoygqn.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/gjxyhwjjw.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnrxrwyk.sHtML

[U04] Py：变量调试打印
来源：http://m.share.epnwcf.com/Article/details/gpnsyqldq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.epnwcf.com/Article/details/gnfcdtutw.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/gntcqfrkm.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/ghlfasvky.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gkpcrslqj.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gcqqiakqi.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/gifygvsah.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.sjlbkw.cn/Article/details/gvtasowhv.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gwxwxungs.sHtML

[y for x in nested for y in x]
来源：http://m.share.vehdjk.com/Article/details/grqhbuhoa.sHtML


<!-- 参考信息 -->