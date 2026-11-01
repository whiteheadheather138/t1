代发 wailian999

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gyvapvagq.sHtML

[R62] 找最占空间的文件
来源：http://blog.bbcook.cn/Article/details/goruxrcmh.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/ggkenbxxk.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/ggfinpteg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/gkqbiwfvm.sHtML

[R64] 结束进程
来源：http://www.blog.fktsv.cn/Article/details/gtrxdtsin.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/ggveclvzy.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gtpqthurm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.bbcook.cn/Article/details/gchluafkb.sHtML

[R66] 定时任务
来源：http://blog.tarul.cn/Article/details/gviyzmfwf.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/gbppbvhrx.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gliklfzwg.sHtML

openssl rand -hex 16
来源：http://read.share.epnwcf.com/Article/details/gvdgglrcg.sHtML

[R68] 计算文件校验值
来源：http://wap.tarul.cn/Article/details/gnommbfhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gumpxapoc.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gsvtrjoid.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gjlpyytub.sHtML

[R70] 时间戳与互转
来源：http://www.share.sjlbkw.cn/Article/details/ghprmntdh.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.bbcook.cn/Article/details/gerboedvk.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/geumoqheo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gawezddap.sHtML

[R72] 等待端口就绪
来源：http://wap.tarul.cn/Article/details/gqvejxgnm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/grfoaxqwo.sHtML

[R73] 分割大日志
来源：http://www.share.fktsv.cn/Article/details/gaguycncx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.sjlbkw.cn/Article/details/gwvtzkeyi.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gttuofmet.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsbhrxof.sHtML

[R75] 导出环境变量
来源：http://mobile.epnwcf.com/Article/details/gulgwvoat.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.yfazqb.com/Article/details/ggwnudnsq.sHtML

[R76] 使用临时文件
来源：http://mobile.epnwcf.com/Article/details/gzkrnqlcc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gpiqgkhsm.sHtML

[R77] 读取用户输入
来源：http://wap.bbcook.cn/Article/details/gcqoouhsq.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gaboqpmno.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gzjtbdmjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.yfazqb.com/Article/details/gigxqyfvp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/gbcffgnru.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gwotvhxmf.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gwiqeapnn.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gzmafhjfe.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/geteicmeb.sHtML

S. C / C++ 专题
来源：http://m.share.yfazqb.com/Article/details/glrzctwkd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gffbqexvw.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/guptrtmuy.sHtML

#include <stdio.h>
来源：http://baike.fktsv.cn/Article/details/gepfvqmpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gjhnaydir.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gyqaaztef.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/goobtrazw.sHtML

[S03] C：读入整数
来源：http://read.share.yfazqb.com/Article/details/giiiozcvn.sHtML

int x; scanf("%d", &x);
来源：http://mobile.tarul.cn/Article/details/gvdvfjhoz.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/godaghelk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.bbcook.cn/Article/details/gbrwbhldn.sHtML

[S05] C：字符串长度
来源：http://baike.vehdjk.com/Article/details/gqtfdistx.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/guyuxfkio.sHtML

[S06] C：字符串比较
来源：http://mobile.vehdjk.com/Article/details/gfpcmfxxu.sHtML

strcmp(a, b) == 0
来源：http://3g.sjlbkw.cn/Article/details/gawnhfreg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.yfazqb.com/Article/details/gzwfkbple.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gkpwjltnk.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gwchmwjpp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.sjlbkw.cn/Article/details/gtxjxylkt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/gcmjivmkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gydqbhbhb.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gxqwdbuud.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gmnyopdmd.sHtML

[S11] C：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gttwwvkcf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gdcozhuuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.tarul.cn/Article/details/gfnwdpuxi.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/gklrqynvf.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/gyyxvxmeh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.yfazqb.com/Article/details/gahwyhoje.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/ghgrkkmlq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gnzcsyqws.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gdgkztnfz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gqimhqdny.sHtML

[S15] C：类型转换
来源：http://m.share.epnwcf.com/Article/details/giwmfzjws.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/goqlvjmph.sHtML

[S16] C：位操作置位
来源：http://wap.fktsv.cn/Article/details/giyjdfaxg.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gqfutvsyl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/ggrvtqqwc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.epnwcf.com/Article/details/gkxvijbst.sHtML

[S18] C：命令行参数
来源：http://www.blog.tarul.cn/Article/details/gpdzkgcsa.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gzbkafyqc.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/ggujffegc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gpmsrqnej.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gfxjhmvzg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/glaffyurj.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/glqwjdwlc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.vehdjk.com/Article/details/gtydizqaz.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/grmwadnwm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gddvrxqvs.sHtML

[S23] C：随机数
来源：http://wap.epnwcf.com/Article/details/gjmbafzrz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/ghswnindz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fktsv.cn/Article/details/goopuvyau.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gonieyxig.sHtML

[S25] C：内存拷贝
来源：http://baike.vehdjk.com/Article/details/gletpkerk.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/ggxgmxmvy.sHtML

[S26] C：内存清零
来源：http://read.share.tarul.cn/Article/details/grjnpqpqx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.sjlbkw.cn/Article/details/gxxcffkfv.sHtML

[S27] C：定义常量
来源：http://3g.fktsv.cn/Article/details/gqmaqzans.sHtML

const double PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gbosvrfee.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gftuneqrw.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/garjymmvg.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gbcpaovqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.tarul.cn/Article/details/gglrriobx.sHtML

[S30] C：头文件保护
来源：http://www.blog.vehdjk.com/Article/details/gabofblhd.sHtML

#ifndef X_H
来源：http://3g.vehdjk.com/Article/details/gaasckywe.sHtML

#define X_H
来源：http://www.share.yfazqb.com/Article/details/ggknqooan.sHtML

#endif
来源：http://m.share.tarul.cn/Article/details/gvzodalsh.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/gjssprtsa.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gboscrpgy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gaasbksni.sHtML

[S32] C++：字符串
来源：http://www.m.share.vehdjk.com/Article/details/gbntjpven.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.bbcook.cn/Article/details/gxicqqjhg.sHtML

[S33] C++：vector 增删
来源：http://m.share.epnwcf.com/Article/details/gudsskcrt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.epnwcf.com/Article/details/gyxpryicl.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.yfazqb.com/Article/details/gcbltcxss.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gfdizuaqd.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gzefnebbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gsmzpzavs.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gxkglpjpu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gkwwwtihd.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gwialyxmb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.tarul.cn/Article/details/gccqnluky.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gmccktrxb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.epnwcf.com/Article/details/gbgbwobqx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.tarul.cn/Article/details/giisayvqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuiswpoi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.bbcook.cn/Article/details/gqqscthfc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gnofkhuxf.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gkryvatpn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.bbcook.cn/Article/details/ggtyzaywu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.yfazqb.com/Article/details/geoonnfyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.tarul.cn/Article/details/gvnqljahr.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/ghqjnyehy.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.tarul.cn/Article/details/gvubjbhzn.sHtML

[S44] C++：引用传参
来源：http://mobile.yfazqb.com/Article/details/gdtjqowrm.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.yfazqb.com/Article/details/glbkexhuh.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gjnpqudcn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gqlscezsv.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gtxftlgpk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gqhyzquwp.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/ghmsixors.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.vehdjk.com/Article/details/gjiotnkjs.sHtML

[S48] C++：逐行读文件
来源：http://3g.yfazqb.com/Article/details/gmjkdphme.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gpgkiinna.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gzmmojdii.sHtML

[S49] C++：写文件
来源：http://mobile.yfazqb.com/Article/details/gqasoyqgb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.epnwcf.com/Article/details/grzsansto.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gxjnkzaaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fktsv.cn/Article/details/gvdbnhwuc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.bbcook.cn/Article/details/gbrgnajxx.sHtML

static_cast<double>(a) / b
来源：http://baike.yfazqb.com/Article/details/gzabdjvsz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/glakaqnqw.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gdboihjqt.sHtML

[S53] C++：移动语义
来源：http://wap.fktsv.cn/Article/details/gnncitlsi.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gjzzpyfvw.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/gexlzpsib.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.epnwcf.com/Article/details/gpxtthddm.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/giykcqxmj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/gbiyyvmcw.sHtML

[S56] C++：optional
来源：http://www.share.epnwcf.com/Article/details/gfyhnavrz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/glqyqhloy.sHtML

[S57] C++：编译期常量
来源：http://m.share.tarul.cn/Article/details/gslayqhjf.sHtML

constexpr int N = 10;
来源：http://mobile.fktsv.cn/Article/details/guweuwpjn.sHtML

[S58] C++：命名空间
来源：http://3g.sjlbkw.cn/Article/details/guivqunci.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/ghgbeekie.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gjmagetll.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gqgclxnoy.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gvobdzbqp.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.vehdjk.com/Article/details/givnjnvfk.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmnvrtsqx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.epnwcf.com/Article/details/grbfuftkq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxvohvvlu.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gqiukqhkj.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/ggkejzfud.sHtML

[T02] Kotlin：变量
来源：http://mobile.yfazqb.com/Article/details/guitwmgdr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/gnufijbkz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.bbcook.cn/Article/details/goyqgbriv.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/gjgbkqovz.sHtML

[T04] Kotlin：空安全
来源：http://mobile.epnwcf.com/Article/details/gxiczyheu.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gvahnsemo.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/ggcshkvdn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.epnwcf.com/Article/details/gfofmpjxj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gkhxokevk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gqftzaylg.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.yfazqb.com/Article/details/gwecdgmub.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gbnfqoray.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gilvpoink.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.bbcook.cn/Article/details/gyepkvefl.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gbonhxibj.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gjcayqnrk.sHtML

[T10] Kotlin：默认参数
来源：http://3g.tarul.cn/Article/details/gxrfiwvca.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/giubmpqcw.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gmnxdxuqw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gtwmetxpx.sHtML

[T12] Kotlin：解构声明
来源：http://baike.tarul.cn/Article/details/ghxidqhse.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/glnuqgmmv.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.vehdjk.com/Article/details/ggdwebegc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.vehdjk.com/Article/details/gneinehxx.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gientsbbm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gsjmyammf.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/gtwgokdhw.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.yfazqb.com/Article/details/guirfjdyp.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/goxjfukci.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/goyokrumq.sHtML

[T17] Swift：变量与常量
来源：http://m.share.bbcook.cn/Article/details/ghwzajexn.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gdhnjimdv.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/grrtathoh.sHtML

"值: \(b)"
来源：http://www.share.sjlbkw.cn/Article/details/gnzgbrsoo.sHtML

[T19] Swift：可选绑定
来源：http://m.share.bbcook.cn/Article/details/gobnbbbzf.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.yfazqb.com/Article/details/gdytmxxzr.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/godyuftdt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.yfazqb.com/Article/details/gbejpgkfh.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gpdivyfvh.sHtML

for x in a { print(x) }
来源：http://www.blog.vehdjk.com/Article/details/gmijwmndp.sHtML

[T22] Swift：字典
来源：http://mobile.fktsv.cn/Article/details/gfceahtsj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.epnwcf.com/Article/details/goyinhtfv.sHtML

[T23] Swift：函数
来源：http://baike.tarul.cn/Article/details/gvxpuyjsl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.yfazqb.com/Article/details/ggfqjpekq.sHtML

[T24] Swift：闭包
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgeodxat.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gelfiwcig.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gohaoszay.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gmbprfjdt.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gfcechuyr.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gxdvtsxky.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/ggxpafdps.sHtML

do { try f() } catch { print(error) }
来源：http://blog.yfazqb.com/Article/details/geyszgrjz.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gstwmvfcs.sHtML

enum Color { case red, green }
来源：http://mobile.vehdjk.com/Article/details/guebqpsij.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.sjlbkw.cn/Article/details/gyfkpstuu.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gcmctgdre.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gikmypzmr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fktsv.cn/Article/details/gmrwgsbxl.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gevzcewpq.sHtML

print("Hello")
来源：http://baike.epnwcf.com/Article/details/glufavwev.sHtML

[T32] Lua：局部变量
来源：http://wap.fktsv.cn/Article/details/gxhwlamnp.sHtML

local a = 1
来源：http://read.share.vehdjk.com/Article/details/gtqaccafq.sHtML

[T33] Lua：表（数组）
来源：http://baike.tarul.cn/Article/details/gmrlxjcky.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gekjyqwaz.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/gdpqimkhk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gcxztdcem.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gdvhnsgix.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/grbzwormn.sHtML

[T36] Lua：函数
来源：http://read.share.sjlbkw.cn/Article/details/gssmhschy.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/glbdontud.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gcamekkjr.sHtML

"a" .. "b"
来源：http://www.blog.bbcook.cn/Article/details/gwvrihglc.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gzeoghqhv.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gfmcqtuud.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gbghtqriu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gscqzvtty.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/gumihledp.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gmjnmmfyy.sHtML

[T41] Perl：Hello World
来源：http://wap.vehdjk.com/Article/details/gqmggvavv.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gxdxryffn.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gowltccve.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.epnwcf.com/Article/details/geamnpzha.sHtML

[T43] Perl：字符串插值
来源：http://m.share.fktsv.cn/Article/details/gvjapnnnf.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gvhmfapsc.sHtML

[T44] Perl：条件
来源：http://baike.sjlbkw.cn/Article/details/grnwrdtzs.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.bbcook.cn/Article/details/gffwswcaj.sHtML

[T45] Perl：数组遍历
来源：http://mobile.tarul.cn/Article/details/gjacwncwi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.bbcook.cn/Article/details/gsbaifzgg.sHtML

[T46] Perl：哈希操作
来源：http://3g.sjlbkw.cn/Article/details/gqkqpkdas.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.tarul.cn/Article/details/gxzutvvxv.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.epnwcf.com/Article/details/gngnnwaxh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.yfazqb.com/Article/details/gqyqamxof.sHtML

[T48] Perl：正则替换
来源：http://wap.vehdjk.com/Article/details/gtvmkajxc.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fktsv.cn/Article/details/gsbuqwuew.sHtML

[T49] Perl：函数
来源：http://read.share.tarul.cn/Article/details/goyjcrynb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnwxcbsy.sHtML

[T50] Perl：逐行读文件
来源：http://blog.yfazqb.com/Article/details/gfjhbegfm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.epnwcf.com/Article/details/gfbqdxbul.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gkmlgtued.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/giebqgqcn.sHtML

println("Hello")
来源：http://www.blog.epnwcf.com/Article/details/ggsqnjoal.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/gzbxrzsas.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gqnnfpnot.sHtML

[T53] Scala：字符串插值
来源：http://blog.fktsv.cn/Article/details/gytkxelkf.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gxtzjlzpl.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gtravvadt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.vehdjk.com/Article/details/ggnpalumb.sHtML

[T55] Scala：集合过滤
来源：http://baike.epnwcf.com/Article/details/gypmhwghf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gllcylcus.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gqrelgsis.sHtML

case class User(name: String, age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gekgprtdh.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gedemenqs.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gmtkejvgz.sHtML

[T58] Scala：函数定义
来源：http://baike.sjlbkw.cn/Article/details/gmsdthpos.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gvsspghcx.sHtML

[T59] Scala：循环
来源：http://m.share.epnwcf.com/Article/details/glebvxigc.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.sjlbkw.cn/Article/details/gzzksrbje.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gmmaqsyjm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.sjlbkw.cn/Article/details/gnuoqxrle.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbnjgflil.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fktsv.cn/Article/details/gibvaqgfr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkkxsnvnn.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gvcgdaylp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gijfaaumv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/groleicgu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.bbcook.cn/Article/details/ggdcxxemc.sHtML


<!-- 参考信息 -->