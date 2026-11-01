代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gqdxxpixc.sHtML

[R66] 定时任务
来源：http://wap.sjlbkw.cn/Article/details/gfzuamtwr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gmtimnbdh.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gggythkmh.sHtML

openssl rand -hex 16
来源：http://www.share.epnwcf.com/Article/details/gmzoxcdzk.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gndjdhkcl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gidgecpna.sHtML

[R69] 生成随机密码
来源：http://mobile.bbcook.cn/Article/details/gqndmyqix.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gsujxkikj.sHtML

[R70] 时间戳与互转
来源：http://www.share.fktsv.cn/Article/details/gftmgatkn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gafzrlwhp.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gbrkvqkqp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gdyvpgset.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gxyrjbgnb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gqszutbot.sHtML

[R73] 分割大日志
来源：http://m.share.sjlbkw.cn/Article/details/gyvupoymc.sHtML

split -l 1000 big.log part_
来源：http://baike.bbcook.cn/Article/details/gcgvawhwk.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gxxroesrx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gnizcpnwb.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/grgdfxalk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gdrlypiwl.sHtML

[R76] 使用临时文件
来源：http://read.share.yfazqb.com/Article/details/gzkdpqmvz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.bbcook.cn/Article/details/gfvekybbh.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/ggtrczzlb.sHtML

read -rp "请输入: " ans
来源：http://read.share.sjlbkw.cn/Article/details/gujaxzvwg.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gpnjecbgo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fktsv.cn/Article/details/gmyhkvnlc.sHtML

[R79] 解析命令行选项
来源：http://wap.yfazqb.com/Article/details/gshquyhzv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.tarul.cn/Article/details/grrrhqxfp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.vehdjk.com/Article/details/gdfzeuakc.sHtML

time ./run.sh
来源：http://read.share.bbcook.cn/Article/details/ggdtkybmr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyxhkqktm.sHtML

S. C / C++ 专题
来源：http://blog.bbcook.cn/Article/details/gojvxkzvk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gsemkcjzp.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gjqwavqln.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gmzaymphm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.bbcook.cn/Article/details/goocxshlb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gaihpkwef.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.tarul.cn/Article/details/gnhnazcnz.sHtML

[S03] C：读入整数
来源：http://3g.fktsv.cn/Article/details/gpthpxpfy.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gwcpyhfsp.sHtML

[S04] C：字符串复制
来源：http://www.m.share.epnwcf.com/Article/details/geghoglih.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fktsv.cn/Article/details/glygdqvwn.sHtML

[S05] C：字符串长度
来源：http://blog.tarul.cn/Article/details/gfdhujoum.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnlvyeixu.sHtML

[S06] C：字符串比较
来源：http://baike.vehdjk.com/Article/details/groflkfof.sHtML

strcmp(a, b) == 0
来源：http://read.share.epnwcf.com/Article/details/gletqiiip.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fktsv.cn/Article/details/gcnahrbor.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gwphbenws.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gktxadccq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/geqsyvhks.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gtmfkawal.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/ggjwjpvbw.sHtML

[S10] C：指针与解引用
来源：http://m.share.yfazqb.com/Article/details/gzjyuzaaq.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/ghsgaaota.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gtfnpdtzb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gwvhdinnk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gtphxfcyy.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gaylvwubj.sHtML

[S12] C：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gxludninu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gltnkvsvy.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/grsfzmzma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gfkdioqpo.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/goghjmzhu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/gmwzfdaqt.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gjkwjfamz.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gbzbnfqge.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gbgpuvbzw.sHtML

x |= (1 << 3);
来源：http://www.share.tarul.cn/Article/details/gwpiibkcd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gifuysetg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fktsv.cn/Article/details/ghotcagep.sHtML

[S18] C：命令行参数
来源：http://3g.epnwcf.com/Article/details/gpmxduuwd.sHtML

int main(int argc, char **argv)
来源：http://wap.tarul.cn/Article/details/gwddhrlri.sHtML

[S19] C：快速排序
来源：http://mobile.bbcook.cn/Article/details/gwqmhfmna.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gqswaiyil.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gyvghrhya.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fktsv.cn/Article/details/gkgamlrxl.sHtML

[S21] C：字符类别判断
来源：http://baike.epnwcf.com/Article/details/gtbtadpsv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.yfazqb.com/Article/details/ghcsaxsbl.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gmbhokdsp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.bbcook.cn/Article/details/gjifeqvod.sHtML

[S23] C：随机数
来源：http://www.share.fktsv.cn/Article/details/garrnyhvd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gpfabrbih.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzroajks.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gwqpautdv.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/gdfisnnwv.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/grkzgelab.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gzqwnjsjd.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gdfyaeuft.sHtML

[S27] C：定义常量
来源：http://baike.sjlbkw.cn/Article/details/gywbyvdnh.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gyzsqdfxh.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxtdihhb.sHtML

static int counter = 0;
来源：http://baike.epnwcf.com/Article/details/gykpyxrjq.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gormvorib.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.sjlbkw.cn/Article/details/gctdlcwgz.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gieyqigao.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/ggayxdvek.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gmpbyhruy.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gxacobozo.sHtML

[S31] C++：Hello World
来源：http://3g.vehdjk.com/Article/details/gmacpccmt.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gxrznjgyf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gvisyipqd.sHtML

[S32] C++：字符串
来源：http://baike.yfazqb.com/Article/details/gdaewrorj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gwouppeyj.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gwkzkejse.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gzxeslivp.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gtfpzxpsh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.epnwcf.com/Article/details/gmmsxgmoh.sHtML

[S35] C++：map
来源：http://www.share.sjlbkw.cn/Article/details/gsjlxflig.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gwxghyviz.sHtML

[S36] C++：unordered_map
来源：http://m.share.sjlbkw.cn/Article/details/ghdfrsnez.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gtwlyunwk.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/goozoktks.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.yfazqb.com/Article/details/gtlztygls.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/gszrsedse.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gbykyrjiz.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.bbcook.cn/Article/details/gbhqlygzy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gdiyafwxy.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gintdvkbv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.vehdjk.com/Article/details/gnbnguxlm.sHtML

[S41] C++：类与构造函数
来源：http://m.share.tarul.cn/Article/details/gtsxefxxz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gfsmhqgyv.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/gborccwlf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gkdkdtdih.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/golarkurt.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.yfazqb.com/Article/details/gxejofltp.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/glzobcofo.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fktsv.cn/Article/details/gbvpuovhn.sHtML

[S45] C++：lambda
来源：http://www.m.share.tarul.cn/Article/details/gzcdlfhpi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.sjlbkw.cn/Article/details/gbegihvve.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gusipkiek.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fktsv.cn/Article/details/gxepvzclj.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gpumlnmzt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gzicsfibf.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gjssakqwq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.tarul.cn/Article/details/gsuqiabus.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/gtkussdpc.sHtML

[S49] C++：写文件
来源：http://wap.bbcook.cn/Article/details/giooidysa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/gaoicikxp.sHtML

[S50] C++：格式化数字
来源：http://read.share.fktsv.cn/Article/details/gjxvpxoyj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/geurrawec.sHtML

[S51] C++：显式类型转换
来源：http://3g.yfazqb.com/Article/details/giaatndvv.sHtML

static_cast<double>(a) / b
来源：http://www.share.sjlbkw.cn/Article/details/gcmqlptet.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.vehdjk.com/Article/details/gmfkgydbc.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/grivzfxlm.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gfjvrispl.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.vehdjk.com/Article/details/gcgejrymc.sHtML

[S54] C++：异常处理
来源：http://www.share.sjlbkw.cn/Article/details/gvffgbcyn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/glumkaelr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.sjlbkw.cn/Article/details/glsgpvifc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gitxmjehb.sHtML

[S56] C++：optional
来源：http://m.share.bbcook.cn/Article/details/gxrgraeiv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.sjlbkw.cn/Article/details/ghwmkrnqe.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gluaadmoi.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/gqxziymyg.sHtML

[S58] C++：命名空间
来源：http://3g.vehdjk.com/Article/details/gjonftcjq.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.bbcook.cn/Article/details/glxuqtzen.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gutzhiatx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/gpxpkgrlq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gbfwazfgx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gkixhcrmk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzjreyitu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.epnwcf.com/Article/details/gmnihebcl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grrzeajfn.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gxcmovdrh.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gcrnnxelt.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gnuedmywj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gaodiniqe.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.yfazqb.com/Article/details/gtqjdvuqe.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gzsosthef.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gfmnpezuh.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gtjtbavwo.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fktsv.cn/Article/details/gljfjdony.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gbxpzbdvj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.epnwcf.com/Article/details/gybqtlkhs.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gkezuoqhy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.tarul.cn/Article/details/gjmwmojrr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gudeuwphq.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/giqeqmooi.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gshgifoup.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/gjwennjxl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gdrmlznwf.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/grzmtrgbk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.tarul.cn/Article/details/gwuksxknz.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gqejqvxjo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/ggstgzpnb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/geitndwch.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fktsv.cn/Article/details/gugnvquwe.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.tarul.cn/Article/details/gyvxggept.sHtML

val m = mapOf("a" to 1)
来源：http://blog.sjlbkw.cn/Article/details/gytatizho.sHtML

[T14] Kotlin：循环
来源：http://www.share.bbcook.cn/Article/details/gojvecyfx.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjtalvhzp.sHtML

[T15] Kotlin：接口
来源：http://wap.fktsv.cn/Article/details/gssbpvyzr.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fktsv.cn/Article/details/gxjnmvzjw.sHtML

[T16] Swift：Hello World
来源：http://m.share.epnwcf.com/Article/details/gtxszynaj.sHtML

print("Hello")
来源：http://blog.bbcook.cn/Article/details/gcxocdvur.sHtML

[T17] Swift：变量与常量
来源：http://3g.bbcook.cn/Article/details/ggezfpxsq.sHtML

var a = 1;  let b = 2
来源：http://m.share.tarul.cn/Article/details/ghrrnzjxn.sHtML

[T18] Swift：字符串插值
来源：http://www.share.bbcook.cn/Article/details/ghnprmvpd.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gdfjcgwxr.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gisqtgwqe.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gfyfoeorl.sHtML

[T20] Swift：数组操作
来源：http://blog.bbcook.cn/Article/details/gpcmhdfka.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.yfazqb.com/Article/details/gkpfreaov.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmynucpyd.sHtML

for x in a { print(x) }
来源：http://3g.sjlbkw.cn/Article/details/gtxlresga.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/giufpkxtf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/goryxajwc.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gdeiznzme.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gxysiqotq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.tarul.cn/Article/details/ghhmvxfvl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gtuekfzmy.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gywtaxggb.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gxjicyviv.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gaaohpwxr.sHtML

class A: Base { override func f() {} }
来源：http://blog.bbcook.cn/Article/details/gbfyipdmj.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/glokhvnmy.sHtML

do { try f() } catch { print(error) }
来源：http://baike.tarul.cn/Article/details/gvrffleqq.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gtqlrfdlk.sHtML

enum Color { case red, green }
来源：http://www.blog.epnwcf.com/Article/details/gibguvjql.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gitkacurs.sHtML

guard let x = opt else { return }
来源：http://3g.sjlbkw.cn/Article/details/gfnzbgxgq.sHtML

[T30] Swift：协议
来源：http://blog.yfazqb.com/Article/details/gvdbeqkvb.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gmueqrhau.sHtML

[T31] Lua：Hello World
来源：http://read.share.tarul.cn/Article/details/gcxswknth.sHtML

print("Hello")
来源：http://wap.yfazqb.com/Article/details/gvcnwbypl.sHtML

[T32] Lua：局部变量
来源：http://mobile.fktsv.cn/Article/details/gbwpwsklg.sHtML

local a = 1
来源：http://baike.sjlbkw.cn/Article/details/gyjcpibsl.sHtML

[T33] Lua：表（数组）
来源：http://blog.tarul.cn/Article/details/gonzxaxbz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gebroiajk.sHtML

[T34] Lua：遍历表
来源：http://baike.tarul.cn/Article/details/gwyrxdizi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.yfazqb.com/Article/details/grmuvrlmo.sHtML

[T35] Lua：字典表
来源：http://wap.fktsv.cn/Article/details/gyxknickr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/giaouvubg.sHtML

[T36] Lua：函数
来源：http://blog.epnwcf.com/Article/details/gdgddcuml.sHtML

function add(a, b) return a + b end
来源：http://baike.yfazqb.com/Article/details/gyfbkjdhw.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gmocuuneu.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gkolxyutj.sHtML

[T38] Lua：条件
来源：http://3g.sjlbkw.cn/Article/details/gbywvvebb.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gpdqesyon.sHtML

[T39] Lua：模式匹配
来源：http://baike.bbcook.cn/Article/details/gyamynvkw.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gojqxoczz.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gkefsyxro.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gezzsazwy.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gvanokkdp.sHtML

print "Hello\n";
来源：http://mobile.epnwcf.com/Article/details/gpddrcspn.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gpzmbjebs.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gevmpyqsz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gattbeutc.sHtML

"值: $a"
来源：http://www.blog.fktsv.cn/Article/details/gikqspxyb.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcqpzjqx.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fktsv.cn/Article/details/gztfweaph.sHtML

[T45] Perl：数组遍历
来源：http://3g.epnwcf.com/Article/details/gekfwuefb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/germbhqrr.sHtML

[T46] Perl：哈希操作
来源：http://www.share.epnwcf.com/Article/details/gkyyjsexa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gaamvkdfm.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.bbcook.cn/Article/details/glbovpsif.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gdadavoyi.sHtML

[T48] Perl：正则替换
来源：http://read.share.fktsv.cn/Article/details/gknkipwqq.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gbxnsqigo.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/glqwlkcmr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.bbcook.cn/Article/details/gafyqptdf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/grxqgieqj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gdiepwtjl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gjylthjtm.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.tarul.cn/Article/details/geqkipnuv.sHtML

println("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/glheimskz.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gdmboibol.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gwkqslbsm.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fktsv.cn/Article/details/ghrbrdxpx.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gjlyrfzbv.sHtML

[T54] Scala：集合映射
来源：http://mobile.vehdjk.com/Article/details/gnylixgkw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/gzmdydhrb.sHtML

[T55] Scala：集合过滤
来源：http://blog.fktsv.cn/Article/details/gtdhdmcfd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gsrccuxjl.sHtML

[T56] Scala：样例类
来源：http://www.share.epnwcf.com/Article/details/gxvhocspf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/gsnmfebjm.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/ghqbecogn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.sjlbkw.cn/Article/details/gnwrgaxpq.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/glxxocdiv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.epnwcf.com/Article/details/gzdejtvej.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/gvkglbsfo.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gytkmdebp.sHtML

[T60] Scala：折叠
来源：http://www.blog.epnwcf.com/Article/details/gegcenhhi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gvncfqatc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gostpmqie.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.yfazqb.com/Article/details/gilzqydwd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxbuzmtgk.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.tarul.cn/Article/details/gibvanymf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.fktsv.cn/Article/details/gdoaisqbn.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.epnwcf.com/Article/details/gxzwppuof.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/geiojxnmf.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.fktsv.cn/Article/details/gqfrafehf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.epnwcf.com/Article/details/gzkprjnzu.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/garbgdcfg.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.fktsv.cn/Article/details/gukmjzrlf.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.fktsv.cn/Article/details/gvaucqhdl.sHtML

list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/gdupntvib.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/ggsxsugrj.sHtML

{**a, **b}
来源：http://baike.vehdjk.com/Article/details/gtmwgawge.sHtML


<!-- 参考信息 -->