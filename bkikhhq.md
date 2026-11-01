代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gyckpysii.sHtML

[R66] 定时任务
来源：http://www.m.share.fktsv.cn/Article/details/gdadyrzft.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gpzmdcvtw.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fktsv.cn/Article/details/guqdhoamv.sHtML

openssl rand -hex 16
来源：http://www.blog.vehdjk.com/Article/details/gobiblohy.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gtvhrltyo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.sjlbkw.cn/Article/details/grqdvhcfl.sHtML

[R69] 生成随机密码
来源：http://www.share.yfazqb.com/Article/details/gltyqdtxu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gtwsuhvyb.sHtML

[R70] 时间戳与互转
来源：http://mobile.tarul.cn/Article/details/gqjtnquot.sHtML

date +%s;  date -d @1700000000
来源：http://wap.epnwcf.com/Article/details/grsrnnjxw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gsadkilzh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.vehdjk.com/Article/details/gxpnagzik.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/gydebngwi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvqgqaiea.sHtML

[R73] 分割大日志
来源：http://read.share.epnwcf.com/Article/details/gbhppusyb.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gvhqnwhbk.sHtML

[R74] 批量重命名
来源：http://blog.yfazqb.com/Article/details/gommeawpm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fktsv.cn/Article/details/gbnltsxfl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gykbgminl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/gsyfhnobs.sHtML

[R76] 使用临时文件
来源：http://mobile.sjlbkw.cn/Article/details/givuzlnjh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gdwatvhmy.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gvrwhddgk.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gjtyexeiq.sHtML

[R78] 交互式菜单
来源：http://read.share.sjlbkw.cn/Article/details/gwgysjsyi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gyqpnflhp.sHtML

[R79] 解析命令行选项
来源：http://m.share.yfazqb.com/Article/details/guwntvfun.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gzexwjbvr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gjtejmxrx.sHtML

time ./run.sh
来源：http://3g.bbcook.cn/Article/details/giknclmal.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdoqfmrzo.sHtML

S. C / C++ 专题
来源：http://www.blog.tarul.cn/Article/details/gjfribezb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gedhjhnch.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gsztkujuk.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gqdgrurna.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gmmpnyvrz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gegmgpibs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.vehdjk.com/Article/details/gdberbvja.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/guyfyffuc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fktsv.cn/Article/details/gvwmyjcev.sHtML

[S04] C：字符串复制
来源：http://3g.yfazqb.com/Article/details/gjdxgxpvn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gzgntqsvx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gvahgfadm.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gxouhedfk.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gebcvutcw.sHtML

strcmp(a, b) == 0
来源：http://baike.yfazqb.com/Article/details/gibmzdbvn.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/grcbysvlb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gumegwdth.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.tarul.cn/Article/details/gkytxwwli.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fktsv.cn/Article/details/glewjuatp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fktsv.cn/Article/details/gnsxadpir.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gilmyghhc.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gvgblorhx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyjusofj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsewaxim.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gkozsvkze.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/grkdvfnqa.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/glpliulsb.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/glxktldus.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.epnwcf.com/Article/details/gtomvnzvn.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/ggawfgetm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/gvwlwzlef.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gfcbazzww.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fktsv.cn/Article/details/gtnmnbjjb.sHtML

[S15] C：类型转换
来源：http://mobile.tarul.cn/Article/details/gvpctmezy.sHtML

(double) a / b
来源：http://wap.sjlbkw.cn/Article/details/gytvqrwqo.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/grorkvirx.sHtML

x |= (1 << 3);
来源：http://www.m.share.yfazqb.com/Article/details/gsbkdlxkf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/grkuruwio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/galybldyb.sHtML

[S18] C：命令行参数
来源：http://blog.tarul.cn/Article/details/gjveqcwfy.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gvvwavjpt.sHtML

[S19] C：快速排序
来源：http://baike.fktsv.cn/Article/details/gpxjpdsls.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/getkhyaae.sHtML

[S20] C：二分查找
来源：http://wap.tarul.cn/Article/details/guzdwwwek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/gqgkiahaf.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gxlfmrdnn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gvdviblwo.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/ghxizfmxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fktsv.cn/Article/details/gmyufekae.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gxvheuyfo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.sjlbkw.cn/Article/details/gaydefdwe.sHtML

[S24] C：获取本地时间
来源：http://read.share.bbcook.cn/Article/details/gjmaqvtvo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gfffhfyow.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/ggsriuuxt.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gkhpxbrup.sHtML

[S26] C：内存清零
来源：http://www.m.share.yfazqb.com/Article/details/gsjbemsou.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gzogewkpe.sHtML

[S27] C：定义常量
来源：http://www.m.share.fktsv.cn/Article/details/guwbaxgox.sHtML

const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gnwpcphtx.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/guhlxhsff.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gwovmwqfk.sHtML

[S29] C：变参函数
来源：http://baike.bbcook.cn/Article/details/gauekkrxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fktsv.cn/Article/details/gvkjxtekd.sHtML

[S30] C：头文件保护
来源：http://wap.epnwcf.com/Article/details/gfijhivjl.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gpkjtcgcr.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gyfabboqy.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gbgfuraly.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/glnkwbmmd.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/gfvagjurs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.vehdjk.com/Article/details/gllkanwyn.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gxnrmzbhb.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.epnwcf.com/Article/details/gtswnvdrx.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/geekdbgge.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.yfazqb.com/Article/details/ggicgracj.sHtML

[S34] C++：遍历 vector
来源：http://baike.vehdjk.com/Article/details/gafcfyfqs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/gpcwjsnhu.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gabekoroo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gzjrfmdwp.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/glenusrjz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gxxterwqu.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gwabfykdc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gzbypucuy.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/ghqfduiat.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gfmavttjh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.bbcook.cn/Article/details/goezabdnq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.bbcook.cn/Article/details/glllirxdr.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gapcjbhvt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gcmbgahcx.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fktsv.cn/Article/details/gbmyxtjsr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/gvebpttxe.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.yfazqb.com/Article/details/gmibalfqt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/ghykutmrn.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gzwleyexy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.epnwcf.com/Article/details/gouienbie.sHtML

[S44] C++：引用传参
来源：http://wap.sjlbkw.cn/Article/details/gomsivrfi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggltubsmo.sHtML

[S45] C++：lambda
来源：http://3g.yfazqb.com/Article/details/glltyyinh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/gjyaiqncv.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gniakfutp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.sjlbkw.cn/Article/details/gmbluxvon.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/gkbuupjcn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/gunfgedwx.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/grxxrrrda.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gzcuquruq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/geevwgzpl.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/guwtlpsic.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/ghagjnkqb.sHtML

[S50] C++：格式化数字
来源：http://www.blog.vehdjk.com/Article/details/gtskgqbhn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/gflryjevs.sHtML

[S51] C++：显式类型转换
来源：http://wap.epnwcf.com/Article/details/ggaejmlwn.sHtML

static_cast<double>(a) / b
来源：http://m.share.tarul.cn/Article/details/gsdtaktlp.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gtrbmxzys.sHtML

int size() const noexcept { return n_; }
来源：http://3g.bbcook.cn/Article/details/glqwsuzvp.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/givtdlicf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/grrpkomki.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gzmvegshs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gvbqqndzo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/gthptijep.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gdzssmvvl.sHtML

[S56] C++：optional
来源：http://baike.yfazqb.com/Article/details/gvfqiqqlk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.yfazqb.com/Article/details/gjquviomu.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/gprryekzi.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gfwsuxrwy.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gfvxvrnao.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.yfazqb.com/Article/details/gfiviroqs.sHtML

[S59] C++：静态断言
来源：http://www.m.share.epnwcf.com/Article/details/gsgrtqeyw.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/guqdlavor.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fktsv.cn/Article/details/gvffnvvrm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gqrzhzqbs.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzxvbedwl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gpdbmyjps.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gruwhoidx.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gdjbzunhl.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gltzpplrh.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gkdoteoea.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.tarul.cn/Article/details/ghaxzkuoh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gexinmgxl.sHtML

"值: $b"
来源：http://baike.tarul.cn/Article/details/gumyibakp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gpuztxyvy.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gmzpzxnhe.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gatbvaerl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gjhgurwfk.sHtML

[T06] Kotlin：集合映射
来源：http://wap.bbcook.cn/Article/details/gptesaltb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.epnwcf.com/Article/details/gyshdvfvf.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gchdsnjuf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/geixoytfh.sHtML

[T08] Kotlin：数据类
来源：http://baike.vehdjk.com/Article/details/gtxckigqi.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fktsv.cn/Article/details/gfiqzatyf.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.vehdjk.com/Article/details/gbwtbckwo.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gvlpvdbna.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/gcczmhnnj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fktsv.cn/Article/details/gawuzqebt.sHtML

[T11] Kotlin：协程
来源：http://www.share.fktsv.cn/Article/details/ggpvcxdte.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gwidmrefj.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.bbcook.cn/Article/details/gqqcbxjzx.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gibyenhst.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gqnuckhmd.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gvgtjuvbt.sHtML

[T14] Kotlin：循环
来源：http://wap.bbcook.cn/Article/details/guefkubgp.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gylnvlkfh.sHtML

[T15] Kotlin：接口
来源：http://wap.bbcook.cn/Article/details/grvlzheox.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gezjepfyb.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gqgjfwzge.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/giseqkmdl.sHtML

[T17] Swift：变量与常量
来源：http://read.share.epnwcf.com/Article/details/gfbeuldkx.sHtML

var a = 1;  let b = 2
来源：http://baike.sjlbkw.cn/Article/details/gwnlasrhw.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/ghhzfrjcr.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/gvaqsepvg.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/gqayriuel.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/greexcgqy.sHtML

[T20] Swift：数组操作
来源：http://www.share.sjlbkw.cn/Article/details/gllqhxrxm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.vehdjk.com/Article/details/gehxkngks.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gpkkwhmcp.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gzvantzsz.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/glivbocap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.tarul.cn/Article/details/guguiydbi.sHtML

[T23] Swift：函数
来源：http://www.share.vehdjk.com/Article/details/gqjhnacwg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/guzkwjyuj.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gvnipuwku.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gzrcgqvli.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gvdcmfvlh.sHtML

struct P { var x: Int }
来源：http://baike.sjlbkw.cn/Article/details/gfzjrkvay.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gxtquelht.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.tarul.cn/Article/details/gkdakhjti.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gyagrezhn.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.yfazqb.com/Article/details/gvbvuevbt.sHtML

[T28] Swift：枚举
来源：http://baike.vehdjk.com/Article/details/gfhdqrpop.sHtML

enum Color { case red, green }
来源：http://m.share.sjlbkw.cn/Article/details/gyuqnhjjl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gfxithgoh.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gcdncpriq.sHtML

[T30] Swift：协议
来源：http://www.share.tarul.cn/Article/details/gdzxgynoh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.vehdjk.com/Article/details/gicffyfmb.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gtxfradov.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/gdethmrgb.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/giqobbbgf.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gdslgolgk.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gyzicepzg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gapqvnyob.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gcyhlhlmd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.epnwcf.com/Article/details/gqjfchkgb.sHtML

[T35] Lua：字典表
来源：http://www.share.epnwcf.com/Article/details/gagftopri.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.epnwcf.com/Article/details/ghoorgyxn.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gytsugczy.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gvgnqbsws.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/glptrtugx.sHtML

"a" .. "b"
来源：http://read.share.yfazqb.com/Article/details/gphafesni.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gzugobywn.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gjhqczxsv.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gilpkhdln.sHtML

string.find(s, "%d+")
来源：http://www.blog.bbcook.cn/Article/details/ggssqgzvk.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gptmaetur.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fktsv.cn/Article/details/gtvxktvkd.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/glkzannmb.sHtML

print "Hello\n";
来源：http://read.share.bbcook.cn/Article/details/gahliengx.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/ggxpczjhm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gpjwvafzc.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gzidubpnb.sHtML

"值: $a"
来源：http://www.share.yfazqb.com/Article/details/giexrxbhb.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gmsgwcgsj.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fktsv.cn/Article/details/gbdhxfkac.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/gftfaewap.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gsjxkwcya.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gupmqslja.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.epnwcf.com/Article/details/gvqotqjcg.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/griprhkdw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fktsv.cn/Article/details/ghlzetkbv.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/gycwwsozg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gfhfyvlvp.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gmgkbdiub.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gslqtsmsr.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fktsv.cn/Article/details/gtfifupaa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.bbcook.cn/Article/details/gdstwxktn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gnoqamrrk.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/gagyvflcm.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gqyelfwua.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/ghlklaqqg.sHtML

val a = 1;  var b = 2
来源：http://baike.vehdjk.com/Article/details/gngtnwfoc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gwerrgbuw.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gqgniosuu.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/grsszuatl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/geudriclu.sHtML

[T55] Scala：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/goufvdzpp.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.vehdjk.com/Article/details/gxdmofebu.sHtML

[T56] Scala：样例类
来源：http://baike.tarul.cn/Article/details/gahhnkrhx.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gzbgwhfyy.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/grpcjbkmc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.yfazqb.com/Article/details/gjevtgagd.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/gbbcbudes.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gimqwniiy.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/glwyaynqa.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.yfazqb.com/Article/details/gacvdvlaj.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gtnqscaic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.epnwcf.com/Article/details/gcxqlznze.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyeibwmrm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.yfazqb.com/Article/details/gqbygdyvw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gzpginytl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.yfazqb.com/Article/details/godraxolb.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.tarul.cn/Article/details/gufogxevb.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.bbcook.cn/Article/details/gkeumxrrz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.yfazqb.com/Article/details/gpojjaxsv.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.sjlbkw.cn/Article/details/gthiysekk.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.fktsv.cn/Article/details/gualbgcax.sHtML

[U04] Py：变量调试打印
来源：http://read.share.tarul.cn/Article/details/gwwrwmmgp.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gsjpyosga.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/glffimnsl.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gxnnkfgdn.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gwgvhblxs.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gmskvucrk.sHtML


<!-- 参考信息 -->