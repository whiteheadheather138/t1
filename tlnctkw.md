代发 wailian999

df -h;  du -sh *
来源：http://m.share.bbcook.cn/Article/details/gewtzltrs.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/ghzdbbxem.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gfkfhrhuf.sHtML

[R63] 内存与进程
来源：http://www.share.fktsv.cn/Article/details/gmknrnhsq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gdzwluetk.sHtML

[R64] 结束进程
来源：http://read.share.tarul.cn/Article/details/gynuzoaik.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvfvnqqh.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/grrywailw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/gpiwymahv.sHtML

[R66] 定时任务
来源：http://www.share.epnwcf.com/Article/details/gtobbtxpb.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gojtkpwri.sHtML

[R67] 生成随机十六进制串
来源：http://3g.vehdjk.com/Article/details/geuujoqfx.sHtML

openssl rand -hex 16
来源：http://m.share.yfazqb.com/Article/details/gqlulcsqc.sHtML

[R68] 计算文件校验值
来源：http://m.share.bbcook.cn/Article/details/gsfzupaoo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.epnwcf.com/Article/details/gpakupqfs.sHtML

[R69] 生成随机密码
来源：http://m.share.tarul.cn/Article/details/giwozsfnf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gpzspvaip.sHtML

[R70] 时间戳与互转
来源：http://read.share.vehdjk.com/Article/details/guhnqaqyg.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gpjhsbvjq.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gdirlmnvc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.bbcook.cn/Article/details/galqfjthv.sHtML

[R72] 等待端口就绪
来源：http://baike.yfazqb.com/Article/details/gunmgefuy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/glqfnmaxc.sHtML

[R73] 分割大日志
来源：http://m.share.tarul.cn/Article/details/gxcpizipj.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gafolpvyx.sHtML

[R74] 批量重命名
来源：http://read.share.epnwcf.com/Article/details/glbxgqprl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gzuewqpct.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gkoatqvam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.vehdjk.com/Article/details/gouyesomu.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/guarxagyg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gzamxnjih.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gqhwanqis.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/genpimkgj.sHtML

[R78] 交互式菜单
来源：http://baike.fktsv.cn/Article/details/gddphuzue.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gkeviwzth.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gukynktqd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.vehdjk.com/Article/details/gklypnfcx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.tarul.cn/Article/details/gcxwdvxyy.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gvslkbczm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjttdmhwm.sHtML

S. C / C++ 专题
来源：http://wap.fktsv.cn/Article/details/gnsqmfnue.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwujdqauw.sHtML

[S01] C：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gibialkea.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gkkafkchz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.tarul.cn/Article/details/gxvadgjsj.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.yfazqb.com/Article/details/guwmwtugy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.epnwcf.com/Article/details/gvuojddtj.sHtML

[S03] C：读入整数
来源：http://m.share.bbcook.cn/Article/details/gemvobeod.sHtML

int x; scanf("%d", &x);
来源：http://baike.fktsv.cn/Article/details/gxciuffqg.sHtML

[S04] C：字符串复制
来源：http://m.share.bbcook.cn/Article/details/gedymanqv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/gsifbzkls.sHtML

[S05] C：字符串长度
来源：http://m.share.vehdjk.com/Article/details/googqncnt.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/goijbthax.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gipoathtw.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gpoldqndu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gqdcikees.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gdrnoxfqz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.bbcook.cn/Article/details/gkymwklfl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.tarul.cn/Article/details/gutuwlajy.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gzriolmsk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.tarul.cn/Article/details/gqffxwtjl.sHtML

[S10] C：指针与解引用
来源：http://m.share.bbcook.cn/Article/details/gffmqjabj.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gtneihomz.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gnkfzwrwa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.vehdjk.com/Article/details/gksnuuxhd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gismqwoiy.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/ghkyqxuxe.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gwqblurso.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gapvrfksp.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/gfjcyiwst.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fktsv.cn/Article/details/gqdojkyae.sHtML

[S14] C：枚举
来源：http://3g.yfazqb.com/Article/details/gkbgnkiam.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.yfazqb.com/Article/details/gbifnuvfl.sHtML

[S15] C：类型转换
来源：http://wap.bbcook.cn/Article/details/gcytmdphk.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gxzllhjno.sHtML

[S16] C：位操作置位
来源：http://www.share.bbcook.cn/Article/details/gsjbjkval.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gqminwjpt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.vehdjk.com/Article/details/grquwzxlu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gmhhauwhe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gpyphshmj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.vehdjk.com/Article/details/gawgpmjpj.sHtML

[S19] C：快速排序
来源：http://wap.bbcook.cn/Article/details/gbjvznaqn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gjztgwvcz.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gjubqsgmq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.sjlbkw.cn/Article/details/gfrfwxnrx.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gmvbvtmmq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/grmouwzhl.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/glchxdjai.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gnphqclka.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gvbamqdic.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/gdqvlurqo.sHtML

[S24] C：获取本地时间
来源：http://www.blog.bbcook.cn/Article/details/grgwjfdem.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gxwgrovox.sHtML

[S25] C：内存拷贝
来源：http://blog.epnwcf.com/Article/details/gdlgqnbpk.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gsnvbzsgg.sHtML

[S26] C：内存清零
来源：http://read.share.epnwcf.com/Article/details/gormsbxax.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gaohyvhzd.sHtML

[S27] C：定义常量
来源：http://read.share.vehdjk.com/Article/details/gcwofpfss.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gbraknvzi.sHtML

[S28] C：静态变量
来源：http://m.share.fktsv.cn/Article/details/gkwxuhkyd.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gdgfdhytv.sHtML

[S29] C：变参函数
来源：http://blog.bbcook.cn/Article/details/gizwkfxke.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/goolfvshn.sHtML

[S30] C：头文件保护
来源：http://baike.yfazqb.com/Article/details/gyfbxwhyf.sHtML

#ifndef X_H
来源：http://www.blog.epnwcf.com/Article/details/gaawxiogx.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gevwojzvn.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/ggsbairwn.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/guqcpkwek.sHtML

#include <iostream>
来源：http://www.share.epnwcf.com/Article/details/gvzvgpfjt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gprowqevy.sHtML

[S32] C++：字符串
来源：http://mobile.epnwcf.com/Article/details/gzlifsxsn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gmtmcocap.sHtML

[S33] C++：vector 增删
来源：http://3g.vehdjk.com/Article/details/gbszzdrkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.vehdjk.com/Article/details/gmfuudixj.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/ggttpagff.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/glparwiou.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/gmbenehhu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gtxglxrqx.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gyhljgnbb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gzlujxmnz.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gcpktcctx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gdgddxcfm.sHtML

[S38] C++：排序
来源：http://read.share.fktsv.cn/Article/details/gbnxhulde.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/grmyziqxa.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/gpdfxdmpd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.vehdjk.com/Article/details/geoyhydvk.sHtML

[S40] C++：查找元素
来源：http://read.share.fktsv.cn/Article/details/gdvzyttcz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/gaibhiozj.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gswzmaflu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.vehdjk.com/Article/details/gokawhouj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.bbcook.cn/Article/details/gyvtgvtyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.epnwcf.com/Article/details/gxjnqigfw.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gcihgcrhw.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gpvglrsbw.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gfnirzpdv.sHtML

void inc(int &x) { ++x; }
来源：http://3g.sjlbkw.cn/Article/details/gyxgyussq.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gmksqcbik.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gqqkwrukh.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gmqziqeiz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gktwiloic.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.sjlbkw.cn/Article/details/glumdqprf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.epnwcf.com/Article/details/geebehhrx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gjkevprnh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/grnfdjyyd.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.sjlbkw.cn/Article/details/ggsvccjws.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gelkgmiov.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.vehdjk.com/Article/details/guljawwdp.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/glwhgvgwa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gtpajgmdg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/ganjttaxm.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gvzvpnzld.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gdhbsskog.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/ghxsfxcvr.sHtML

[S53] C++：移动语义
来源：http://mobile.vehdjk.com/Article/details/gwzqcjaeh.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gbqcohnrr.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gxuzvsfqy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gffbjiiao.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwarteiw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gywzoqnrt.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gynqkslyd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.vehdjk.com/Article/details/gckuikcmm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvqjqewf.sHtML

constexpr int N = 10;
来源：http://baike.tarul.cn/Article/details/gjmajggck.sHtML

[S58] C++：命名空间
来源：http://www.blog.epnwcf.com/Article/details/gnrpjnlcs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gzsugrrdd.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gmeesvtpx.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fktsv.cn/Article/details/guwrcymzu.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gfnzscbyu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gyidxdwnk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/giwzudakr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.bbcook.cn/Article/details/gqxbocypc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvzpgdsim.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gzohsendy.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gszbvvghe.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/gxdmomgqn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gnwyhrcrl.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gbrgpazmy.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gtesedxcc.sHtML

[T04] Kotlin：空安全
来源：http://www.share.sjlbkw.cn/Article/details/gaeydtnre.sHtML

val n: String? = null;  n?.length
来源：http://www.share.yfazqb.com/Article/details/gzkecliyh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gwwwgxqvp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.vehdjk.com/Article/details/gubcveobh.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.tarul.cn/Article/details/gvujheqfx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.epnwcf.com/Article/details/ggjfectpy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/givhrwxju.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gnvwntpcu.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gzvpddylp.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gmutomgwm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.epnwcf.com/Article/details/gyzfkyako.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gndaampgj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gphnydfnt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gmhebmjhz.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/ghifieyff.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.yfazqb.com/Article/details/gsnroohpy.sHtML

[T12] Kotlin：解构声明
来源：http://3g.epnwcf.com/Article/details/gkhgekved.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.bbcook.cn/Article/details/gxmmgiboc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gczpsbdcg.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/godzixvtl.sHtML

[T14] Kotlin：循环
来源：http://blog.vehdjk.com/Article/details/gnyergdio.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/gcoxdrpzs.sHtML

[T15] Kotlin：接口
来源：http://3g.tarul.cn/Article/details/gkctszcen.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gwgltnqjs.sHtML

[T16] Swift：Hello World
来源：http://www.share.tarul.cn/Article/details/goeketupt.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gbtiznewy.sHtML

[T17] Swift：变量与常量
来源：http://www.share.bbcook.cn/Article/details/gktgfitgk.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fktsv.cn/Article/details/gguydcmey.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gctuqevmx.sHtML

"值: \(b)"
来源：http://www.blog.sjlbkw.cn/Article/details/gtakprmvx.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/gqgnhyufx.sHtML

if let n = opt { print(n) }
来源：http://blog.fktsv.cn/Article/details/gasikecdj.sHtML

[T20] Swift：数组操作
来源：http://3g.fktsv.cn/Article/details/gzixgymgp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gptdqvggr.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gvogxnezv.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gopcrthcu.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gmscjljlf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.tarul.cn/Article/details/gkhkszoav.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gaeizwbcx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.sjlbkw.cn/Article/details/gwpvedyze.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gkrjoncih.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gdvooobrm.sHtML

[T25] Swift：结构体
来源：http://blog.vehdjk.com/Article/details/gofoyvvqt.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gzxssmwxf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.epnwcf.com/Article/details/gytqwfepx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fktsv.cn/Article/details/ggidvzion.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.epnwcf.com/Article/details/gspwmnfpo.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.tarul.cn/Article/details/gahvctyiq.sHtML

[T28] Swift：枚举
来源：http://www.share.yfazqb.com/Article/details/genjykbcd.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/gzuckonig.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.epnwcf.com/Article/details/gdijhelmb.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/gipjomwdp.sHtML

[T30] Swift：协议
来源：http://wap.tarul.cn/Article/details/gfkwgxdme.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/gntnjndzw.sHtML

[T31] Lua：Hello World
来源：http://wap.tarul.cn/Article/details/gmoikzhtb.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/glemomioa.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gackmjiha.sHtML

local a = 1
来源：http://www.m.share.bbcook.cn/Article/details/gxtodwpvi.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/ggjlsotqd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/glkpwxzdh.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/gzydysdek.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.tarul.cn/Article/details/gbrawnzmx.sHtML

[T35] Lua：字典表
来源：http://read.share.fktsv.cn/Article/details/gjxpdoypv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gfcjsqlij.sHtML

[T36] Lua：函数
来源：http://m.share.yfazqb.com/Article/details/gresppqlw.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gohzxlmpn.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/gfnhveslt.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gpucobdwo.sHtML

[T38] Lua：条件
来源：http://mobile.bbcook.cn/Article/details/gfyamwpea.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gcoisplnl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gcpvkvtpd.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gvkqstphy.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/gzwccmlbc.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.tarul.cn/Article/details/gsnvygcll.sHtML

[T41] Perl：Hello World
来源：http://read.share.yfazqb.com/Article/details/gnnxzrndp.sHtML

print "Hello\n";
来源：http://www.share.vehdjk.com/Article/details/gthlvxnkx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gjdowkrej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gwdvxwgfa.sHtML

[T43] Perl：字符串插值
来源：http://mobile.bbcook.cn/Article/details/glqclzofa.sHtML

"值: $a"
来源：http://m.share.fktsv.cn/Article/details/gxvteypir.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gykujexvc.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.sjlbkw.cn/Article/details/gctivifwj.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.vehdjk.com/Article/details/guarskvkt.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gzjuefhvy.sHtML

[T46] Perl：哈希操作
来源：http://wap.vehdjk.com/Article/details/gjqrwbmqi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gjtdqmtkl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gclumskph.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/gaqhkjxca.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfbpfeqm.sHtML

$s =~ s/old/new/g;
来源：http://blog.yfazqb.com/Article/details/goitavdct.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gdzactbga.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.sjlbkw.cn/Article/details/giwuyeuya.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gcesoalcn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/ghsvcfsip.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gmulxwzxo.sHtML

[T51] Scala：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/guqwrojuu.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gbspqobuw.sHtML

[T52] Scala：变量
来源：http://www.share.tarul.cn/Article/details/gwucnesix.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gofpioffs.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gsutgdlhn.sHtML

s"值: $b"
来源：http://www.blog.vehdjk.com/Article/details/gsbhugqcu.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gldobkrir.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.tarul.cn/Article/details/gltxcqvav.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gojmmsjcr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gnvjxgoat.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gdnqcqlum.sHtML

case class User(name: String, age: Int)
来源：http://www.share.bbcook.cn/Article/details/gmfsokssq.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gtscgomvh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/glpyhwxvb.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/goqwwuyri.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.fktsv.cn/Article/details/getnwelqe.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/gxbhdesew.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gjlpbuger.sHtML

[T60] Scala：折叠
来源：http://baike.yfazqb.com/Article/details/gjulllnhz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/ghhqchewc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gavwhoqlf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/glzzsolip.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdobojdfh.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/goufpgjrj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gwekxolnv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.sjlbkw.cn/Article/details/gnjitezgq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gkxvkutqv.sHtML


<!-- 参考信息 -->