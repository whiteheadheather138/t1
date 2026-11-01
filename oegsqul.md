代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.sjlbkw.cn/Article/details/gvtzhmjhq.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/glfjilmcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gtrrleium.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/ggynhjphn.sHtML

df -h;  du -sh *
来源：http://www.blog.sjlbkw.cn/Article/details/gxqedapcl.sHtML

[R62] 找最占空间的文件
来源：http://baike.fktsv.cn/Article/details/gbvdxcypn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/guwmjvpdh.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gzjaqysqv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gkaaabwlh.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gdvxykznk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gycuotmev.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/gcljiznrf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fktsv.cn/Article/details/gxontivzh.sHtML

[R66] 定时任务
来源：http://www.m.share.tarul.cn/Article/details/gjkxkauba.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gulztlaav.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/greelyivk.sHtML

openssl rand -hex 16
来源：http://3g.vehdjk.com/Article/details/gmjvzznoc.sHtML

[R68] 计算文件校验值
来源：http://3g.tarul.cn/Article/details/geptwkmfa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhlgoojw.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gkwwzkakh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.vehdjk.com/Article/details/ghciulbdr.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gkhstgvvu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gxfpcyxcl.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gxhxziciv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.epnwcf.com/Article/details/gktlsotyt.sHtML

[R72] 等待端口就绪
来源：http://read.share.tarul.cn/Article/details/gcnnwihql.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gnwzmpyqu.sHtML

[R73] 分割大日志
来源：http://www.blog.bbcook.cn/Article/details/gyqpkvhxu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/gvclqqxvr.sHtML

[R74] 批量重命名
来源：http://m.share.fktsv.cn/Article/details/gkacqrdkj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/glyuchzld.sHtML

[R75] 导出环境变量
来源：http://www.blog.vehdjk.com/Article/details/gqvpifnwg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gnltpoogv.sHtML

[R76] 使用临时文件
来源：http://baike.bbcook.cn/Article/details/gnwrztpng.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.sjlbkw.cn/Article/details/gfjqtcyph.sHtML

[R77] 读取用户输入
来源：http://wap.fktsv.cn/Article/details/gcvnootoe.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/gjrnahrnl.sHtML

[R78] 交互式菜单
来源：http://wap.tarul.cn/Article/details/gkqjfhdjx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.bbcook.cn/Article/details/gnouvxnly.sHtML

[R79] 解析命令行选项
来源：http://read.share.vehdjk.com/Article/details/gnsunrmyt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/grbdmrwfo.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.epnwcf.com/Article/details/gpjlaukeq.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/goxzsxyig.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gujujwbdb.sHtML

S. C / C++ 专题
来源：http://mobile.vehdjk.com/Article/details/gawtrnelx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/goukgxsua.sHtML

[S01] C：Hello World
来源：http://wap.sjlbkw.cn/Article/details/ggddjillm.sHtML

#include <stdio.h>
来源：http://baike.sjlbkw.cn/Article/details/geuruyazv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.vehdjk.com/Article/details/gmslqpehr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.yfazqb.com/Article/details/gcskgiial.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.vehdjk.com/Article/details/glglzulcx.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gthrblpde.sHtML

int x; scanf("%d", &x);
来源：http://blog.bbcook.cn/Article/details/gialoikgn.sHtML

[S04] C：字符串复制
来源：http://baike.epnwcf.com/Article/details/gocnyargs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gtkgwmzfq.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/ggxeyiokg.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/ghcmzkkwh.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/giugpxgjv.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gdsyenfbp.sHtML

[S07] C：数组遍历求和
来源：http://m.share.tarul.cn/Article/details/gifupfsrn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/gcujisjki.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/grcottlbu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.epnwcf.com/Article/details/gqhprcmek.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/gggompxnc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.epnwcf.com/Article/details/geucjmbny.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/guxaydyrt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gukgfpizc.sHtML

[S11] C：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gqgkuebeg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gxsrlnomj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fktsv.cn/Article/details/gttrjugvo.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gwjpypcej.sHtML

[S12] C：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gwgnytxjn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/geqlwaavj.sHtML

[S13] C：宏定义
来源：http://www.blog.yfazqb.com/Article/details/gxxtcjklt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fktsv.cn/Article/details/ggjoqqigt.sHtML

[S14] C：枚举
来源：http://baike.yfazqb.com/Article/details/gwiectigy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fktsv.cn/Article/details/grlcdoykl.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/ggrtyxojs.sHtML

(double) a / b
来源：http://read.share.vehdjk.com/Article/details/gvoqfarkr.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gyuvmjaoz.sHtML

x |= (1 << 3);
来源：http://mobile.sjlbkw.cn/Article/details/glncddizn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/guabgabum.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.sjlbkw.cn/Article/details/gvswxxbne.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gmwlpvpkp.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/gqyguflla.sHtML

[S19] C：快速排序
来源：http://www.m.share.bbcook.cn/Article/details/gvreydonl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/grxrblhhl.sHtML

[S20] C：二分查找
来源：http://read.share.bbcook.cn/Article/details/gludsywfk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gxmqbavhu.sHtML

[S21] C：字符类别判断
来源：http://read.share.yfazqb.com/Article/details/giwwajbag.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gfgvktzcc.sHtML

[S22] C：字符串转数字
来源：http://baike.yfazqb.com/Article/details/gcycrqyey.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.yfazqb.com/Article/details/gonwohyes.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/greskjtif.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.epnwcf.com/Article/details/gcehqyxko.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/grfljpfvp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gysptoxvj.sHtML

[S25] C：内存拷贝
来源：http://wap.vehdjk.com/Article/details/gpeydzlja.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gllusajyh.sHtML

[S26] C：内存清零
来源：http://www.blog.tarul.cn/Article/details/gmhylwcqs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gblhneuoy.sHtML

[S27] C：定义常量
来源：http://m.share.fktsv.cn/Article/details/gbczkbcjn.sHtML

const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/glpdqhuau.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/gggryzgqo.sHtML

static int counter = 0;
来源：http://baike.sjlbkw.cn/Article/details/gqavyvzug.sHtML

[S29] C：变参函数
来源：http://read.share.tarul.cn/Article/details/gxykdnmby.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gaacqruzt.sHtML

[S30] C：头文件保护
来源：http://mobile.tarul.cn/Article/details/gfasyhysy.sHtML

#ifndef X_H
来源：http://baike.epnwcf.com/Article/details/gcyacpbgz.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gzogrnmxm.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/goskqvhby.sHtML

[S31] C++：Hello World
来源：http://wap.vehdjk.com/Article/details/gkksomrqu.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/glpfelbsh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.bbcook.cn/Article/details/ghiksbejr.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gxlgnnftd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gjsjqrtqm.sHtML

[S33] C++：vector 增删
来源：http://wap.sjlbkw.cn/Article/details/gisglyofo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gjywnnmzq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gptsiflxu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.yfazqb.com/Article/details/gglsjzqil.sHtML

[S35] C++：map
来源：http://www.share.fktsv.cn/Article/details/gkxmuiiir.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gisnzansj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/gkmcopupb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gdadiuhdb.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gsccyphkf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/glcjymmjg.sHtML

[S38] C++：排序
来源：http://mobile.vehdjk.com/Article/details/gemncycfe.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gaogahbnb.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/gmykjikzv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.yfazqb.com/Article/details/grhwypemk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdkmlyyu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gkxvnzuca.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gyoohonhd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.yfazqb.com/Article/details/gqeivompe.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/gcouhvldg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gritajyhl.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/glsxbbloh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.tarul.cn/Article/details/grdzkmyqp.sHtML

[S44] C++：引用传参
来源：http://mobile.vehdjk.com/Article/details/guhbizzyr.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.vehdjk.com/Article/details/gzdyzqbsy.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/grsuslqrk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.tarul.cn/Article/details/guvkuvrts.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fktsv.cn/Article/details/grjeovkkj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.vehdjk.com/Article/details/gpzitittj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/geivhajyo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fktsv.cn/Article/details/gxzsvigfn.sHtML

[S48] C++：逐行读文件
来源：http://blog.tarul.cn/Article/details/gxdzwewwv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gbemflbqr.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/govusteel.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/gaczdujbe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gyrwlsgih.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gxapajrux.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gajzwxsyy.sHtML

[S51] C++：显式类型转换
来源：http://read.share.epnwcf.com/Article/details/ghqfjnpal.sHtML

static_cast<double>(a) / b
来源：http://baike.fktsv.cn/Article/details/gzqajcwxx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.yfazqb.com/Article/details/grmpdfvjv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.vehdjk.com/Article/details/ggdprkmoy.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gpgcizhip.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/ggrsxkfzp.sHtML

[S54] C++：异常处理
来源：http://baike.sjlbkw.cn/Article/details/gphwkgvwz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.epnwcf.com/Article/details/gnjcwluyv.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gwxuaqvky.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gcmxyrglv.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gunbnacgv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gqjmlgqbw.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gkbqpzdsr.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/ghceourvf.sHtML

[S58] C++：命名空间
来源：http://www.m.share.vehdjk.com/Article/details/gktwbhqta.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.tarul.cn/Article/details/gepyjjzry.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/gndavjgnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gmosdwcaa.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.tarul.cn/Article/details/ggomzqmhy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gdkqszjrv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gjztfcfhq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/ghonncvpz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gocqflqzi.sHtML

[T01] Kotlin：Hello World
来源：http://blog.epnwcf.com/Article/details/gavypjpps.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gbbhjymik.sHtML

[T02] Kotlin：变量
来源：http://m.share.tarul.cn/Article/details/gapugddaq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gcdpbhdbi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gmgweddxw.sHtML

"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gauirxxjx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fktsv.cn/Article/details/gbiqgothm.sHtML

val n: String? = null;  n?.length
来源：http://wap.epnwcf.com/Article/details/gsusvweyi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gfigakupq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gmqqpmkmu.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gyhpdjyih.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gsuzpwjbk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fktsv.cn/Article/details/gbsyhnuzv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fktsv.cn/Article/details/giolnupnh.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/gzferirbc.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gunfhzrhv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.sjlbkw.cn/Article/details/gfcddrwko.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.bbcook.cn/Article/details/grgwpnwmw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/ghnjxboze.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gdqiwhcod.sHtML

[T11] Kotlin：协程
来源：http://m.share.epnwcf.com/Article/details/grqcvcjas.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gqakxxoms.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.tarul.cn/Article/details/gifvbosze.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fktsv.cn/Article/details/gyqscbhxj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fktsv.cn/Article/details/goalgrgcr.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.yfazqb.com/Article/details/gqwsiveqx.sHtML

[T14] Kotlin：循环
来源：http://www.blog.vehdjk.com/Article/details/gqztrjvbn.sHtML

for (i in 1..10) println(i)
来源：http://read.share.yfazqb.com/Article/details/goossjgau.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fktsv.cn/Article/details/geecgspev.sHtML

interface Shape { fun area(): Double }
来源：http://baike.tarul.cn/Article/details/gkayxeccx.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gqnetwqev.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gkfwejloh.sHtML

[T17] Swift：变量与常量
来源：http://www.share.yfazqb.com/Article/details/gjsdxvhby.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/grtexirjp.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gtpjgsaij.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gnrhsdbkv.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gqwhuzjvp.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gkdzykzpa.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/guhivstve.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/ggtopcjzm.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/gyjwxhtza.sHtML

for x in a { print(x) }
来源：http://baike.vehdjk.com/Article/details/gkxvcimal.sHtML

[T22] Swift：字典
来源：http://mobile.vehdjk.com/Article/details/glsulnkto.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gajkhudem.sHtML

[T23] Swift：函数
来源：http://m.share.sjlbkw.cn/Article/details/gxtycezzu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/ggxtboavs.sHtML

[T24] Swift：闭包
来源：http://baike.epnwcf.com/Article/details/gazldicqg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gjyqskfrz.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gnxjkawqq.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/glyvcgrcm.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/givuhrtds.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gtkcchbiv.sHtML

[T27] Swift：错误处理
来源：http://3g.epnwcf.com/Article/details/gyeyrkynj.sHtML

do { try f() } catch { print(error) }
来源：http://wap.sjlbkw.cn/Article/details/gkernctbd.sHtML

[T28] Swift：枚举
来源：http://m.share.epnwcf.com/Article/details/gmwrdvjjr.sHtML

enum Color { case red, green }
来源：http://wap.sjlbkw.cn/Article/details/gbkcrjtgh.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/giixfzocu.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gcnzrbpxm.sHtML

[T30] Swift：协议
来源：http://read.share.bbcook.cn/Article/details/gpvgzamwo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/ghmqsoxdy.sHtML

[T31] Lua：Hello World
来源：http://mobile.epnwcf.com/Article/details/gdwbruxrh.sHtML

print("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gsoolwrnz.sHtML

[T32] Lua：局部变量
来源：http://wap.yfazqb.com/Article/details/gcwgbuwuj.sHtML

local a = 1
来源：http://www.m.share.fktsv.cn/Article/details/gjbnvaqmv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.sjlbkw.cn/Article/details/ghzgmevnk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.vehdjk.com/Article/details/gvvxysyxj.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gmlpcowzq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gkufhawkn.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gsifoihvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/goljtfyrc.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/gvmfrvghd.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.epnwcf.com/Article/details/gpfyozpmv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.epnwcf.com/Article/details/glaqetdop.sHtML

"a" .. "b"
来源：http://wap.sjlbkw.cn/Article/details/gowpghffi.sHtML

[T38] Lua：条件
来源：http://www.share.sjlbkw.cn/Article/details/gdpsvtbfh.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gqusnmrgq.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gguexzrbx.sHtML

string.find(s, "%d+")
来源：http://mobile.sjlbkw.cn/Article/details/gxvacychf.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gnayevnri.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.sjlbkw.cn/Article/details/gkasfnacz.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gptrokthb.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/glzvicxht.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.yfazqb.com/Article/details/gtvwievmf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfmmwehio.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gxelpsnlg.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/gznwiavmi.sHtML

[T44] Perl：条件
来源：http://wap.bbcook.cn/Article/details/ggbsgxsss.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.bbcook.cn/Article/details/gtvyolwxb.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/ggdmtirdi.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.bbcook.cn/Article/details/gwaqznjef.sHtML

[T46] Perl：哈希操作
来源：http://baike.fktsv.cn/Article/details/gmtfxrfrk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtqzzmzgr.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gtfnyxrsx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gqlykqukt.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/grbogxazf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gqslagsii.sHtML

[T49] Perl：函数
来源：http://www.share.yfazqb.com/Article/details/gjewivnth.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/geqnfgdxs.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/ghnrzxrbz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gdezhicke.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gnzxedeir.sHtML

[T51] Scala：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gxzxpdnca.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gnklnmpib.sHtML

[T52] Scala：变量
来源：http://blog.vehdjk.com/Article/details/gvglvjhcv.sHtML

val a = 1;  var b = 2
来源：http://blog.fktsv.cn/Article/details/gkxckoscc.sHtML

[T53] Scala：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gvtuxdnbl.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/gqpxzoykx.sHtML

[T54] Scala：集合映射
来源：http://3g.vehdjk.com/Article/details/goojbpuyr.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gkebcciac.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/gplojdobe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/glpxshiar.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gycjdktov.sHtML

case class User(name: String, age: Int)
来源：http://m.share.vehdjk.com/Article/details/gstzpgobd.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gmbcdgxxg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gueaidywj.sHtML

[T58] Scala：函数定义
来源：http://baike.yfazqb.com/Article/details/gsaxcqopn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gafkijeuc.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gynohdtnr.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/glivusjzo.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gssvjaxal.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gymfyaoak.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpdzozmwe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/gxgvdopsf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grmulvrwg.sHtML


<!-- 参考信息 -->