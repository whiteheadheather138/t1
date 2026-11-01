代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/gkbifkyvf.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gihvxrrxz.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/ggvgqbbkf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.epnwcf.com/Article/details/gfohrhrzu.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gboefmjmu.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gwztpxhnm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.bbcook.cn/Article/details/gzvomemvg.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/ggofufnpz.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fktsv.cn/Article/details/gcygbbnke.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gfxubztlr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpqyqwtj.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gmcjkmpcm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gfhdlwtly.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gyejmnyof.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/ggdekdxhh.sHtML

[R73] 分割大日志
来源：http://wap.epnwcf.com/Article/details/gfhqtyvpv.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gfgpzwnkg.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/ghndedmof.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/ghoooclsp.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/geopwgwyw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/ghwnlpxer.sHtML

[R76] 使用临时文件
来源：http://3g.bbcook.cn/Article/details/gmxhnlewz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.bbcook.cn/Article/details/gmgorbnbo.sHtML

[R77] 读取用户输入
来源：http://m.share.fktsv.cn/Article/details/gxpsmtmnm.sHtML

read -rp "请输入: " ans
来源：http://mobile.vehdjk.com/Article/details/gfjhmatco.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gnzehprcy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.yfazqb.com/Article/details/gkeicxzmt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gzxsxywhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.bbcook.cn/Article/details/gkivikcau.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.bbcook.cn/Article/details/goyeymmfo.sHtML

time ./run.sh
来源：http://wap.fktsv.cn/Article/details/gbmtgyoud.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvgjwtbop.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gyazghkim.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjlgjtczq.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/goqcepklv.sHtML

#include <stdio.h>
来源：http://3g.vehdjk.com/Article/details/gvaabcioq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.yfazqb.com/Article/details/gwofcqkjg.sHtML

[S02] C：变量与格式化输出
来源：http://3g.tarul.cn/Article/details/gmwgloerh.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gptsjjfvk.sHtML

[S03] C：读入整数
来源：http://3g.epnwcf.com/Article/details/gdzjvabhn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.sjlbkw.cn/Article/details/grfiphnpk.sHtML

[S04] C：字符串复制
来源：http://mobile.fktsv.cn/Article/details/gvsklxctg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/ggygywcay.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gctsidrgd.sHtML

strlen(s)
来源：http://3g.fktsv.cn/Article/details/gbqlncvku.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gltumhefr.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/gsygmqmgo.sHtML

[S07] C：数组遍历求和
来源：http://wap.sjlbkw.cn/Article/details/gryxgflvi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.vehdjk.com/Article/details/gvtqyuyva.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.tarul.cn/Article/details/gjtgmabbv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.vehdjk.com/Article/details/gkrjwjylm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/guipxmhat.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/ggxnlachk.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gwoypbybd.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.yfazqb.com/Article/details/gssdvbfbp.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gxdnwjxet.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gbusxohfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gunxtudik.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/ghyltdeut.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gezwuijml.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fktsv.cn/Article/details/gulerbpkw.sHtML

[S13] C：宏定义
来源：http://www.blog.vehdjk.com/Article/details/glqrjndml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/glmmrrbul.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gmygiocgc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/giqkphcog.sHtML

[S15] C：类型转换
来源：http://baike.bbcook.cn/Article/details/gloetvpmj.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/grvdruxnt.sHtML

[S16] C：位操作置位
来源：http://baike.yfazqb.com/Article/details/guetyjswu.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/ghgxgbtfs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gapmosnob.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gcchlpswt.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gbtuvgkfg.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gjsmuynuv.sHtML

[S19] C：快速排序
来源：http://www.blog.fktsv.cn/Article/details/gaqkmaarv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/gxzvfyvvn.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gghugdzny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gehlhujrk.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gmnhxrsac.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.yfazqb.com/Article/details/gryldnfya.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gsvnzojhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.tarul.cn/Article/details/gjnzjkmtt.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/glnnivndi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyerpqxr.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/ggspyjtmx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gaslrzoaq.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/gekmirtpc.sHtML

memcpy(dst, src, n);
来源：http://read.share.fktsv.cn/Article/details/gmdcylads.sHtML

[S26] C：内存清零
来源：http://3g.sjlbkw.cn/Article/details/gqttxdqyv.sHtML

memset(a, 0, sizeof a);
来源：http://baike.tarul.cn/Article/details/glohdodzk.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/golkllfsa.sHtML

const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gibminsgi.sHtML

[S28] C：静态变量
来源：http://read.share.vehdjk.com/Article/details/guxjibuvi.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gjrowiure.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gwnfhzoyu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gxyajvrow.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gorgrcsie.sHtML

#ifndef X_H
来源：http://wap.fktsv.cn/Article/details/gxgdwaphs.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gybywypmp.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/glwhjsjtq.sHtML

[S31] C++：Hello World
来源：http://wap.sjlbkw.cn/Article/details/grahylcis.sHtML

#include <iostream>
来源：http://blog.bbcook.cn/Article/details/gmngewlmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/ghblbazgs.sHtML

[S32] C++：字符串
来源：http://3g.yfazqb.com/Article/details/gpdbmhpic.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.bbcook.cn/Article/details/gwndfshvp.sHtML

[S33] C++：vector 增删
来源：http://wap.epnwcf.com/Article/details/gqnxrlfkz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gylroeirk.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.epnwcf.com/Article/details/gdflvtfnt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gptvglnwt.sHtML

[S35] C++：map
来源：http://3g.yfazqb.com/Article/details/guhydxskm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gqvgkjoda.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gnvwqfggp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.epnwcf.com/Article/details/gpvrhdrwy.sHtML

[S37] C++：set
来源：http://baike.epnwcf.com/Article/details/gxosqlwnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fktsv.cn/Article/details/gyomylvdo.sHtML

[S38] C++：排序
来源：http://wap.epnwcf.com/Article/details/gpapabxvv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrgzcsez.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fktsv.cn/Article/details/gfgdfffxf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gxnbyhrxi.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gqhvoiamb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gkjwfyadu.sHtML

[S41] C++：类与构造函数
来源：http://wap.yfazqb.com/Article/details/gsrvwohxn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.tarul.cn/Article/details/ggzjmeeqw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gfzxupbge.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gzzrvuxyc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.yfazqb.com/Article/details/gewhnzgli.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gcthfcmvr.sHtML

[S44] C++：引用传参
来源：http://www.blog.bbcook.cn/Article/details/gtpufbrtt.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fktsv.cn/Article/details/gqafbqmme.sHtML

[S45] C++：lambda
来源：http://baike.fktsv.cn/Article/details/gvfrdiula.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.tarul.cn/Article/details/gpvemcqay.sHtML

[S46] C++：函数模板
来源：http://www.share.yfazqb.com/Article/details/girvrvesy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.epnwcf.com/Article/details/gjgfsaehi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.bbcook.cn/Article/details/gybqegutb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/glujicyrc.sHtML

[S48] C++：逐行读文件
来源：http://baike.bbcook.cn/Article/details/gsvnkdbah.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gstduywgc.sHtML

while (std::getline(in, line)) { }
来源：http://blog.vehdjk.com/Article/details/gekdcmbdm.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gkzfhtzjd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fktsv.cn/Article/details/gwhgvnjin.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.epnwcf.com/Article/details/gllcqhtpe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gutrhazjg.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gytdzfvrq.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gkqrqfpdl.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gwjdavleo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.vehdjk.com/Article/details/gmjhgxlqd.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gtaaviqlh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/gfbwftlbi.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fktsv.cn/Article/details/gvongitxs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gdkveucwb.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/gqqelykht.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.vehdjk.com/Article/details/gmbotajrv.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gxcnljoys.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.vehdjk.com/Article/details/gywiibvas.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/ghnigolmy.sHtML

constexpr int N = 10;
来源：http://blog.bbcook.cn/Article/details/gbnbpzsol.sHtML

[S58] C++：命名空间
来源：http://mobile.tarul.cn/Article/details/gfuknunyq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.yfazqb.com/Article/details/gundakjsc.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gmxaqewrp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gfnjjupmb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gxilhpust.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gxagugdmj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmvijlydx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gvbrqkmdi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gdizqiwlx.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.tarul.cn/Article/details/geprmtnzu.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/giuwkinii.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/ghxndmypm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gzoaatfhr.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gpsewbsku.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/gtspgybns.sHtML

[T04] Kotlin：空安全
来源：http://blog.fktsv.cn/Article/details/gusvngknp.sHtML

val n: String? = null;  n?.length
来源：http://baike.tarul.cn/Article/details/gmuznijqs.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gjdjeakda.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.vehdjk.com/Article/details/gjmvjeszk.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/guzpseznx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gebicsure.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gqchvhzhv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gxopedesj.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/ggtvwonwp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gsiltjywp.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.bbcook.cn/Article/details/gfikcyaoo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhdlydih.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.vehdjk.com/Article/details/gnyusyceb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/gejjmndsg.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gyzqszibg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gtrxogdon.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gggxzxiru.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/guectqfmv.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/ggbsuzaoa.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gajjmtjnv.sHtML

[T14] Kotlin：循环
来源：http://read.share.bbcook.cn/Article/details/gbuwkoupk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gbxpqrgqn.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/gcfnkhifg.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/geqtzzovp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gtqbvnyjt.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gvlmstyan.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gzvuvhpef.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gnpuuslqc.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gkktemwpr.sHtML

"值: \(b)"
来源：http://3g.bbcook.cn/Article/details/gpcavflmf.sHtML

[T19] Swift：可选绑定
来源：http://wap.yfazqb.com/Article/details/gvdbvazor.sHtML

if let n = opt { print(n) }
来源：http://m.share.yfazqb.com/Article/details/gdybckoub.sHtML

[T20] Swift：数组操作
来源：http://mobile.vehdjk.com/Article/details/ggrmisgni.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/gwpwdlcvb.sHtML

[T21] Swift：遍历
来源：http://3g.vehdjk.com/Article/details/gyqoctbub.sHtML

for x in a { print(x) }
来源：http://wap.fktsv.cn/Article/details/gtfxicxyw.sHtML

[T22] Swift：字典
来源：http://www.blog.yfazqb.com/Article/details/gpuziglnx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.yfazqb.com/Article/details/gnqrarfzh.sHtML

[T23] Swift：函数
来源：http://blog.sjlbkw.cn/Article/details/gtyfkgzbj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.epnwcf.com/Article/details/gnvixnitr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.yfazqb.com/Article/details/glizyhsgb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gxuvjqhls.sHtML

[T25] Swift：结构体
来源：http://3g.bbcook.cn/Article/details/geoiwlmho.sHtML

struct P { var x: Int }
来源：http://www.m.share.bbcook.cn/Article/details/gxdmeygdf.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gioafuqlw.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gjghuuvvb.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvzusbiz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gslpdzssr.sHtML

[T28] Swift：枚举
来源：http://www.m.share.vehdjk.com/Article/details/gykqctpqo.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gqhgxhivq.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gzvrljdyn.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gsilsdity.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gvtudsehj.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gnsitlpnq.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gjxdrxbcv.sHtML

print("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gkfvshdkq.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gxgldvdtz.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gegkvsyqt.sHtML

[T33] Lua：表（数组）
来源：http://www.share.yfazqb.com/Article/details/gpmwsrihu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.tarul.cn/Article/details/gxzmsyyne.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gmbnmicri.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gplqfesut.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/ghsaxfawa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.vehdjk.com/Article/details/gueqyxvyq.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gffmcfjcj.sHtML

function add(a, b) return a + b end
来源：http://blog.tarul.cn/Article/details/ggkgcfmkw.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gejixaaki.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/givcxctpb.sHtML

[T38] Lua：条件
来源：http://3g.epnwcf.com/Article/details/gzyzrnhfh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.tarul.cn/Article/details/gfscvqodo.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gjtdliwum.sHtML

string.find(s, "%d+")
来源：http://3g.sjlbkw.cn/Article/details/gbqlkcplh.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gmnbjqhkm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gbhglkgiz.sHtML

[T41] Perl：Hello World
来源：http://baike.tarul.cn/Article/details/gkmbbqkis.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/grsohbbte.sHtML

[T42] Perl：变量类型
来源：http://baike.bbcook.cn/Article/details/guziavugj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/gtfxnhtso.sHtML

[T43] Perl：字符串插值
来源：http://baike.tarul.cn/Article/details/gllzzscpw.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gjblyxdqr.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/givvsdmrg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fktsv.cn/Article/details/gjybojpvs.sHtML

[T45] Perl：数组遍历
来源：http://wap.epnwcf.com/Article/details/gnxjybsvt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/geogjbcik.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/guektzoqa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/gdjnfvndf.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gswrhunqa.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gdlhpymfm.sHtML

[T48] Perl：正则替换
来源：http://mobile.bbcook.cn/Article/details/gdxoowenj.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/ggwcfwipu.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gdybumyuy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.fktsv.cn/Article/details/gzbraisyc.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gplcohroh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/gvrcclxzx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gfhymekga.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/griraefvl.sHtML

println("Hello")
来源：http://read.share.vehdjk.com/Article/details/gstuxntin.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/ghudcuswu.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gqrplkode.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gldzaruao.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gximisdcm.sHtML

[T54] Scala：集合映射
来源：http://mobile.sjlbkw.cn/Article/details/gmfaqmnyj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.vehdjk.com/Article/details/gwzwktbvn.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/gkdlqlopu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.vehdjk.com/Article/details/gtstcqfkp.sHtML

[T56] Scala：样例类
来源：http://mobile.fktsv.cn/Article/details/ghtohlyuh.sHtML

case class User(name: String, age: Int)
来源：http://mobile.tarul.cn/Article/details/gxdalcuen.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/gphblevtc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.sjlbkw.cn/Article/details/gxvjudogq.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/gxcenducc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.vehdjk.com/Article/details/gugojmqmy.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gjybxamhd.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/glvldtraj.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/geghgiqxg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gzffdfttd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gzhgnfoje.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.epnwcf.com/Article/details/gvnvsobuz.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/grhmckyai.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.sjlbkw.cn/Article/details/gqzwzzqhf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.bbcook.cn/Article/details/gigdcifjl.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/ganflprzw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.tarul.cn/Article/details/gdrntatnt.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/ghojkckyn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.epnwcf.com/Article/details/grcxurwwx.sHtML

[U04] Py：变量调试打印
来源：http://blog.tarul.cn/Article/details/gkvfwnwoz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.fktsv.cn/Article/details/gmagvvlok.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/ghdohtxuk.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gpqieawgw.sHtML

[U06] Py：合并两个字典
来源：http://www.blog.vehdjk.com/Article/details/gsldbxbrl.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/guvigexgj.sHtML


<!-- 参考信息 -->