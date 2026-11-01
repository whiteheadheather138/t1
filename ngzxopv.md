代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.blog.yfazqb.com/Article/details/gxcyuqsuq.sHtML

[R64] 结束进程
来源：http://3g.yfazqb.com/Article/details/gpvnvxozq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/ghmtlnctd.sHtML

[R65] 查看端口占用
来源：http://3g.yfazqb.com/Article/details/gruoopgdw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fktsv.cn/Article/details/grtgnlejl.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/goyxyvbrr.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gvpbfkfsv.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gknktsffj.sHtML

openssl rand -hex 16
来源：http://baike.vehdjk.com/Article/details/gyyprxizu.sHtML

[R68] 计算文件校验值
来源：http://baike.bbcook.cn/Article/details/gtnlpjviv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gyqbrgjnv.sHtML

[R69] 生成随机密码
来源：http://read.share.fktsv.cn/Article/details/gurupxgku.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gvpwizcwi.sHtML

[R70] 时间戳与互转
来源：http://read.share.sjlbkw.cn/Article/details/gburphdui.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.yfazqb.com/Article/details/givnmtqvc.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gcfvlahvx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/gwsvdakry.sHtML

[R72] 等待端口就绪
来源：http://mobile.sjlbkw.cn/Article/details/gzbzidszl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtsllanv.sHtML

[R73] 分割大日志
来源：http://baike.epnwcf.com/Article/details/gwhbfuwlx.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/ghuxvuoom.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/gjkajtdxd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gkusypgku.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/ggltafpxv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gzrurbudt.sHtML

[R76] 使用临时文件
来源：http://read.share.sjlbkw.cn/Article/details/gxwvcszys.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gdycnqznl.sHtML

[R77] 读取用户输入
来源：http://wap.tarul.cn/Article/details/gabewfkqc.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/gerzmaoqp.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/gxbbzenme.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.bbcook.cn/Article/details/gexmuamvl.sHtML

[R79] 解析命令行选项
来源：http://baike.epnwcf.com/Article/details/gbcxznnoo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/gbmxvqrqv.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.epnwcf.com/Article/details/gdjrtlzdt.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/gedfvkmve.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gujqyygdv.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/gvzjcgfnq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glemmrdju.sHtML

[S01] C：Hello World
来源：http://www.blog.tarul.cn/Article/details/gmdomrbzo.sHtML

#include <stdio.h>
来源：http://m.share.yfazqb.com/Article/details/gparmgzty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fktsv.cn/Article/details/gmikzwvyf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gxeimokhk.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/gxxbzuzww.sHtML

[S03] C：读入整数
来源：http://www.share.bbcook.cn/Article/details/ghtuetghi.sHtML

int x; scanf("%d", &x);
来源：http://3g.sjlbkw.cn/Article/details/gfqtnpmun.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gtjadftyc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gvsyqvgwl.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/ghxurbyic.sHtML

strlen(s)
来源：http://www.blog.vehdjk.com/Article/details/gaarsxcxh.sHtML

[S06] C：字符串比较
来源：http://mobile.epnwcf.com/Article/details/glegesiua.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/goskadyvt.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gzvzmbssu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.epnwcf.com/Article/details/gjmgzzlwl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gupsiucca.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gjpceehkr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gpowqfwxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gfvzjstpo.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gzxyfthll.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gvvyakuwf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gqtoouaxg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gekkubikt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fktsv.cn/Article/details/grcphdfae.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gxyufxodn.sHtML

[S12] C：写文件
来源：http://blog.vehdjk.com/Article/details/gifqytcuw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gullkjzif.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/glwbkcstj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/gewpgfyfu.sHtML

[S14] C：枚举
来源：http://read.share.sjlbkw.cn/Article/details/gksnslfqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/gigunutwp.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gbcadclkg.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gvjoldkml.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gtlbybljc.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/gebkfqhxh.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdmdvoclt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gwznejhpl.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/grpawvquv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.tarul.cn/Article/details/gogtbbvxb.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gydrcxvrb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gkvyakmre.sHtML

[S20] C：二分查找
来源：http://read.share.vehdjk.com/Article/details/glkpnqxfd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gotrdylee.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/glbpppqby.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fktsv.cn/Article/details/gvboslbyu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/ghfygvydy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gvqpqmpzn.sHtML

[S23] C：随机数
来源：http://3g.epnwcf.com/Article/details/gywrtesgz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.bbcook.cn/Article/details/gtfkldbmp.sHtML

[S24] C：获取本地时间
来源：http://blog.fktsv.cn/Article/details/gxznjnixa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/guxpwthvx.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gbkbdowls.sHtML

memcpy(dst, src, n);
来源：http://baike.yfazqb.com/Article/details/gdzxeqqey.sHtML

[S26] C：内存清零
来源：http://wap.tarul.cn/Article/details/gtriqlyvk.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gewzyprlc.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gemdtzzeu.sHtML

const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gevonwzbm.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gsodfmlge.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gzwyiffri.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gywlcdmgb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.sjlbkw.cn/Article/details/glwsoxtdg.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/ggagksilg.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gfnyydmib.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gdjthvlao.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gnglovhzc.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gfzwzkdfb.sHtML

#include <iostream>
来源：http://read.share.bbcook.cn/Article/details/gbmvmhfgh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.epnwcf.com/Article/details/ghlrkzcir.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/gkgaqtozo.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.sjlbkw.cn/Article/details/gsjtnspax.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/glcwplikl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.tarul.cn/Article/details/ggvsxctty.sHtML

[S34] C++：遍历 vector
来源：http://read.share.bbcook.cn/Article/details/glujijnzx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gruhktuhe.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gymxdeijn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/geacnohrs.sHtML

[S36] C++：unordered_map
来源：http://m.share.yfazqb.com/Article/details/gqjcqyigb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gozkjyfwa.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gntdsxnxe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.bbcook.cn/Article/details/gkwgwbtyo.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gkemmoudc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gdcjqyard.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.vehdjk.com/Article/details/gzvpsvzti.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.yfazqb.com/Article/details/gploskhop.sHtML

[S40] C++：查找元素
来源：http://m.share.tarul.cn/Article/details/gpyuekpuf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gtggqmpds.sHtML

[S41] C++：类与构造函数
来源：http://3g.epnwcf.com/Article/details/gqkshjbpg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/glbwotoec.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.sjlbkw.cn/Article/details/gcgktheme.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.epnwcf.com/Article/details/gzofekhlg.sHtML

[S43] C++：智能指针
来源：http://www.share.epnwcf.com/Article/details/ggjplkxkd.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fktsv.cn/Article/details/gtmwjmhoz.sHtML

[S44] C++：引用传参
来源：http://www.share.sjlbkw.cn/Article/details/ggivsdqbx.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gkmyegdbq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gwatyndlz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gifidnvpp.sHtML

[S46] C++：函数模板
来源：http://baike.yfazqb.com/Article/details/gkhzgpshv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gwjvkeinn.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.tarul.cn/Article/details/gggitvjxd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gpugxdukp.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/glliucjvi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gbpytlrgn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gstnhyhig.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/gysjfpmbw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.bbcook.cn/Article/details/goehsybiy.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gmqrrikmz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gandjrylg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.bbcook.cn/Article/details/gmdqrbftb.sHtML

static_cast<double>(a) / b
来源：http://wap.vehdjk.com/Article/details/gfhqwxpdk.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/gtpgqufye.sHtML

int size() const noexcept { return n_; }
来源：http://wap.vehdjk.com/Article/details/gnsufavtw.sHtML

[S53] C++：移动语义
来源：http://3g.epnwcf.com/Article/details/gdwaxqama.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.yfazqb.com/Article/details/gczgomdnd.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/geyctmcjd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gchissykg.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gwyrwgodl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gqixhlzyy.sHtML

[S56] C++：optional
来源：http://read.share.epnwcf.com/Article/details/gezxrqquy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.epnwcf.com/Article/details/gxfvpitql.sHtML

[S57] C++：编译期常量
来源：http://www.share.fktsv.cn/Article/details/galhtanor.sHtML

constexpr int N = 10;
来源：http://blog.epnwcf.com/Article/details/gkubkcoff.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/gwkzuetpb.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/ghyznwakx.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/gfvaguwpt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.tarul.cn/Article/details/ghdqrknau.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gkyrfzpql.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gmcjbeniz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtptvdrkd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gblqfywcg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghbmfynxm.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gpjcomnhj.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gbywimpsf.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fktsv.cn/Article/details/gepbfjqbh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.sjlbkw.cn/Article/details/ginjsdphn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gssdmdynp.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gqjbyrzwt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/groqgelmn.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/gyczdvdpq.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.epnwcf.com/Article/details/gcpdajpuz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gsbdaxnmo.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gmzwsryzq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.vehdjk.com/Article/details/gcqczmbzc.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gbzjirhva.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gmtzdhuaz.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.epnwcf.com/Article/details/glrlbwcni.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.yfazqb.com/Article/details/giykhiwho.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gdhmgoslz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.tarul.cn/Article/details/gnelieqbk.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/galcxajpv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.sjlbkw.cn/Article/details/gbwbyuiql.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gjnckgzlz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fktsv.cn/Article/details/gisstyhlw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.sjlbkw.cn/Article/details/gjbgvzdom.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.bbcook.cn/Article/details/gzascknpv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.epnwcf.com/Article/details/gaaouiysv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gqpwnmpls.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.epnwcf.com/Article/details/gowgxvdgv.sHtML

for (i in 1..10) println(i)
来源：http://www.share.vehdjk.com/Article/details/gamngwnsn.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/glldmwoio.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gnqvnsljf.sHtML

[T16] Swift：Hello World
来源：http://baike.yfazqb.com/Article/details/gvrramymk.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gtdhskdzg.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gvjuuyzgy.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gqqdchhly.sHtML

[T18] Swift：字符串插值
来源：http://read.share.bbcook.cn/Article/details/gwccixqiw.sHtML

"值: \(b)"
来源：http://3g.yfazqb.com/Article/details/guheevqzb.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gmfmblvgv.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gcakzimkx.sHtML

[T20] Swift：数组操作
来源：http://read.share.sjlbkw.cn/Article/details/gpziidnux.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.vehdjk.com/Article/details/gcbqpvjvl.sHtML

[T21] Swift：遍历
来源：http://www.blog.bbcook.cn/Article/details/gbtrnbmzj.sHtML

for x in a { print(x) }
来源：http://blog.yfazqb.com/Article/details/gtjdvvfig.sHtML

[T22] Swift：字典
来源：http://wap.fktsv.cn/Article/details/gjxwspwtc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.vehdjk.com/Article/details/gqcyroslg.sHtML

[T23] Swift：函数
来源：http://read.share.fktsv.cn/Article/details/gqvizvznz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.vehdjk.com/Article/details/gknhyrcfq.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/gojfrrpfx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/gocxwcwgt.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/gmunfzdff.sHtML

struct P { var x: Int }
来源：http://read.share.vehdjk.com/Article/details/gbeqppwwo.sHtML

[T26] Swift：类与重写
来源：http://read.share.fktsv.cn/Article/details/grdzideqj.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/gdxosrfjo.sHtML

[T27] Swift：错误处理
来源：http://mobile.vehdjk.com/Article/details/geenfinqq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gahhnzqiq.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gocsngcqx.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/glzmmhlmw.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/gikklxyxg.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gcscqpukb.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gpkckaaev.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.vehdjk.com/Article/details/glmdvznme.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gdhxptgfd.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gtcyourtx.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gmgfxibga.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gmsyigsol.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.bbcook.cn/Article/details/gpcomfula.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gljsnbjwu.sHtML

[T34] Lua：遍历表
来源：http://www.blog.tarul.cn/Article/details/gdlnszazf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gjftpvbwu.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gjhxnlqbk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/godfpvilu.sHtML

[T36] Lua：函数
来源：http://wap.bbcook.cn/Article/details/ghfgjbetn.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gofirjhmj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gmpghhuih.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gudypjcnx.sHtML

[T38] Lua：条件
来源：http://wap.yfazqb.com/Article/details/gfdaszaoe.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gxtxojkcg.sHtML

[T39] Lua：模式匹配
来源：http://wap.epnwcf.com/Article/details/gbipqjqxc.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gbbzfczlj.sHtML

[T40] Lua：元表
来源：http://blog.yfazqb.com/Article/details/gebrzzeid.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gpcrmtlxj.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gxtogaowm.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gfaxbcdeh.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/geohgurwt.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.tarul.cn/Article/details/gwtqfottz.sHtML

[T43] Perl：字符串插值
来源：http://read.share.yfazqb.com/Article/details/geqkxqtde.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gpvdwbkzn.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/gysazkevd.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxvsftjg.sHtML

[T45] Perl：数组遍历
来源：http://www.share.vehdjk.com/Article/details/gnwqzsewu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqicirehr.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gwbjzdlxm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.bbcook.cn/Article/details/glncyqqtg.sHtML

[T47] Perl：正则捕获
来源：http://3g.fktsv.cn/Article/details/gqvhjqohu.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/gqytjddvj.sHtML

[T48] Perl：正则替换
来源：http://read.share.vehdjk.com/Article/details/grieeggcb.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/gtnctvuel.sHtML

[T49] Perl：函数
来源：http://www.share.tarul.cn/Article/details/gfzvmpoxh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gzhkkeifp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gdvtmryxq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.epnwcf.com/Article/details/gkouhdhmw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.bbcook.cn/Article/details/gfsfnofai.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/gckahjeum.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gknvrnnph.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/gkvshyewh.sHtML

val a = 1;  var b = 2
来源：http://www.blog.vehdjk.com/Article/details/ggkucfddk.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/gqdoaektw.sHtML

s"值: $b"
来源：http://blog.fktsv.cn/Article/details/gnlgbibby.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/givehhpcg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gycxqmjhf.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gobiflpzb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.bbcook.cn/Article/details/gdsjkaytk.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/ghnizqdtj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gkvrgbhdl.sHtML

[T57] Scala：模式匹配
来源：http://3g.fktsv.cn/Article/details/gajccnyup.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.vehdjk.com/Article/details/gznykvjhx.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gulwoovua.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gyveqwyfj.sHtML

[T59] Scala：循环
来源：http://www.blog.vehdjk.com/Article/details/gbstttjtq.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.vehdjk.com/Article/details/gaprqlszx.sHtML

[T60] Scala：折叠
来源：http://baike.epnwcf.com/Article/details/gllvjczjd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.vehdjk.com/Article/details/gkjldqvyt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxylejwrs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.epnwcf.com/Article/details/ghhwtgouz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gitkalcgy.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.tarul.cn/Article/details/gbfnwpgzu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.fktsv.cn/Article/details/gijchiuvh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gsfntnied.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.tarul.cn/Article/details/gnskyjmxw.sHtML

[U03] Py：加载 .env 配置
来源：http://blog.sjlbkw.cn/Article/details/gtmhdbbde.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.vehdjk.com/Article/details/gdykrgken.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.fktsv.cn/Article/details/gkaesdkmn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.vehdjk.com/Article/details/gywblwiwn.sHtML


<!-- 参考信息 -->