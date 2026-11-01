代发 wailian999

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/geocjzhxl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.yfazqb.com/Article/details/gmyxmhdgf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gbemhwrgg.sHtML

[R63] 内存与进程
来源：http://read.share.tarul.cn/Article/details/gowgwchfs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.bbcook.cn/Article/details/guzvremyd.sHtML

[R64] 结束进程
来源：http://baike.epnwcf.com/Article/details/gssronvwo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gceztifya.sHtML

[R65] 查看端口占用
来源：http://mobile.epnwcf.com/Article/details/gxtxkdfqs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/gypzhvvrp.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gwjomggts.sHtML

crontab -e;  crontab -l
来源：http://blog.epnwcf.com/Article/details/gmaqpamlm.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/godmoqpae.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gjicztulm.sHtML

[R68] 计算文件校验值
来源：http://wap.sjlbkw.cn/Article/details/guafiysfx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/geeganelc.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gpbvxoauk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gyfuprtxf.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gonjyoucb.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gvkztigdk.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/geiaexlam.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.sjlbkw.cn/Article/details/gcfvtsyte.sHtML

[R72] 等待端口就绪
来源：http://www.blog.tarul.cn/Article/details/glcsyozko.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gaxgdwtgn.sHtML

[R73] 分割大日志
来源：http://3g.vehdjk.com/Article/details/givesgkyo.sHtML

split -l 1000 big.log part_
来源：http://read.share.yfazqb.com/Article/details/gpdhaxvsr.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/gzraeywvi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/grnuxpxbk.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/geixnljrv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.epnwcf.com/Article/details/gjusxinxn.sHtML

[R76] 使用临时文件
来源：http://www.share.sjlbkw.cn/Article/details/gcgufguvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/goeoqbcjx.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gmilutgri.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gozeegyik.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gmvriwbix.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.vehdjk.com/Article/details/guznptmyn.sHtML

[R79] 解析命令行选项
来源：http://3g.bbcook.cn/Article/details/gkcfvnfic.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gjnomemin.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.sjlbkw.cn/Article/details/gjfqatqlg.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/grdgsmurw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gaewhkqna.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gemklpapn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gomllfsqj.sHtML

[S01] C：Hello World
来源：http://blog.vehdjk.com/Article/details/gginymaos.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gxnckdjky.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gsxucljnu.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/garecvcuc.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/gceesugvo.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gqabqtoyf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.yfazqb.com/Article/details/gjebqnyqe.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/grsjinaad.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/gflxgwqsx.sHtML

[S05] C：字符串长度
来源：http://wap.vehdjk.com/Article/details/gbupkwlsu.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/ghdujkwue.sHtML

[S06] C：字符串比较
来源：http://wap.fktsv.cn/Article/details/gqvuabxul.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gaabuetnj.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.vehdjk.com/Article/details/gtulwqqvg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fktsv.cn/Article/details/gnmrekcfn.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeurhvso.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/grincreng.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gqxunvgwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/gujoncsji.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/guczyjneo.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/gbusesnsa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gppzttukh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gfjbqedpy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.vehdjk.com/Article/details/gutxvgsdy.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/guuwyefiq.sHtML

[S12] C：写文件
来源：http://wap.bbcook.cn/Article/details/gxjbuzjww.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/glqoqslkb.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/ggffnobdw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gbgvvlsjg.sHtML

[S14] C：枚举
来源：http://m.share.sjlbkw.cn/Article/details/gxslszlmx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/gygfjxywp.sHtML

[S15] C：类型转换
来源：http://wap.vehdjk.com/Article/details/gdabvxnoj.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gjlnxpsyf.sHtML

[S16] C：位操作置位
来源：http://baike.vehdjk.com/Article/details/gefmmcgmj.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gloxjlzau.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gagxuomja.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.yfazqb.com/Article/details/gfaktfmzj.sHtML

[S18] C：命令行参数
来源：http://www.share.yfazqb.com/Article/details/gaifvmxaa.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/gzhjzihkx.sHtML

[S19] C：快速排序
来源：http://m.share.bbcook.cn/Article/details/gnjuyiadq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gvniirdhb.sHtML

[S20] C：二分查找
来源：http://www.share.tarul.cn/Article/details/gkgdtmkxp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/gfgcgzytk.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gkrkrkquy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fktsv.cn/Article/details/gdxqnpvil.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gcqqpavuc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gptwzxnrp.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gpgqnuusk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.yfazqb.com/Article/details/gzdvunrrx.sHtML

[S24] C：获取本地时间
来源：http://3g.sjlbkw.cn/Article/details/gkmoucvrh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.tarul.cn/Article/details/gbklardbp.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gsgehwujn.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gsrneycok.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gvjtiuieg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.yfazqb.com/Article/details/ggflomqnb.sHtML

[S27] C：定义常量
来源：http://read.share.yfazqb.com/Article/details/gfkbuujyu.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gkupbylep.sHtML

[S28] C：静态变量
来源：http://3g.tarul.cn/Article/details/gcdekqznb.sHtML

static int counter = 0;
来源：http://mobile.yfazqb.com/Article/details/gcoctlacy.sHtML

[S29] C：变参函数
来源：http://wap.bbcook.cn/Article/details/giigeqijg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/ghnhvpled.sHtML

[S30] C：头文件保护
来源：http://read.share.sjlbkw.cn/Article/details/guzkipngw.sHtML

#ifndef X_H
来源：http://3g.epnwcf.com/Article/details/germtuhzi.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gvimggbrp.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/godptkpai.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/ghwuqpnds.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gdlrxylej.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/gvlnucbje.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gujnmpbwm.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.tarul.cn/Article/details/gmgjsomwv.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/grpbpipeq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gvtlweyaq.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/ghmqjtvpo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gmmxvyrta.sHtML

[S35] C++：map
来源：http://mobile.sjlbkw.cn/Article/details/gpflsjwif.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gekjfnsok.sHtML

[S36] C++：unordered_map
来源：http://m.share.epnwcf.com/Article/details/gbfurjglx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/gnoubhnga.sHtML

[S37] C++：set
来源：http://read.share.epnwcf.com/Article/details/gucpcrlal.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/godpofemt.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gyivqfpwc.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.sjlbkw.cn/Article/details/gaycyghvz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.vehdjk.com/Article/details/gzswqlccm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/gegbfwjlx.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/geyvbvncc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gkbzhtlja.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gvxsnbzpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fktsv.cn/Article/details/gkacowzwl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.sjlbkw.cn/Article/details/grycypilu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.epnwcf.com/Article/details/ghpbodbxa.sHtML

[S43] C++：智能指针
来源：http://blog.sjlbkw.cn/Article/details/gvwvscagi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/ghuxwdjgz.sHtML

[S44] C++：引用传参
来源：http://3g.bbcook.cn/Article/details/gwhfnbagr.sHtML

void inc(int &x) { ++x; }
来源：http://blog.yfazqb.com/Article/details/gxndxeceg.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmvmsqyk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gzjjeupxo.sHtML

[S46] C++：函数模板
来源：http://read.share.tarul.cn/Article/details/gimgbiofr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gobggmskt.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.yfazqb.com/Article/details/gosghlbvp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fktsv.cn/Article/details/gxrygtpdc.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gryojfaov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/ggckpdubg.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.yfazqb.com/Article/details/gqdjwtvfm.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gteijqxee.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.sjlbkw.cn/Article/details/gsmjdeook.sHtML

[S50] C++：格式化数字
来源：http://m.share.vehdjk.com/Article/details/gmgmhhqas.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/ghchvwozu.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/gftmuhlez.sHtML

static_cast<double>(a) / b
来源：http://read.share.tarul.cn/Article/details/glfbsmhyq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.tarul.cn/Article/details/gpovxepyo.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gimadpimb.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gebqiwqwk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gloxmdhbe.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/giglmbfam.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.vehdjk.com/Article/details/gjmaaxogd.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fktsv.cn/Article/details/gorklrjna.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gxhivtvtv.sHtML

[S56] C++：optional
来源：http://wap.bbcook.cn/Article/details/gupnsludh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/ghjidvafq.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gidtgwkfw.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gqraninsf.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/grzdnoeae.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.vehdjk.com/Article/details/gariqopkj.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/giknhaxlm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gneoorbai.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/guudjevye.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gpacojdxn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvimxjwtw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.vehdjk.com/Article/details/gcvnmbkqd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gohlibilk.sHtML

[T01] Kotlin：Hello World
来源：http://baike.yfazqb.com/Article/details/gaapceawg.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gvsaunyso.sHtML

[T02] Kotlin：变量
来源：http://3g.epnwcf.com/Article/details/gzkgbpuve.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gkdzkzppz.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gifcrjtpq.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/goljfsrzm.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gguiynemi.sHtML

val n: String? = null;  n?.length
来源：http://wap.bbcook.cn/Article/details/gakusozft.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.vehdjk.com/Article/details/glxtankjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gtnzgthzc.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gdprlzajg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/gfcjucgqt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gtrvjgiwd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gjrdjrlaa.sHtML

[T08] Kotlin：数据类
来源：http://read.share.sjlbkw.cn/Article/details/goqruavdp.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.vehdjk.com/Article/details/guforqmva.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gafrndbsa.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.vehdjk.com/Article/details/gnpujbrxa.sHtML

[T10] Kotlin：默认参数
来源：http://baike.yfazqb.com/Article/details/gdbbapdrc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gcbwafbgi.sHtML

[T11] Kotlin：协程
来源：http://m.share.vehdjk.com/Article/details/grfpyczxl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/grvaaulyv.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/grfyduyzw.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/gvptafuoj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.vehdjk.com/Article/details/gknlhqrut.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/grngujoil.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/grteqmsyj.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gotilcgpy.sHtML

[T15] Kotlin：接口
来源：http://baike.vehdjk.com/Article/details/gpmukcvcm.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.tarul.cn/Article/details/girrxdoeb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gtfinmefe.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gaimgwdoy.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.yfazqb.com/Article/details/gbylnehcz.sHtML

var a = 1;  let b = 2
来源：http://baike.yfazqb.com/Article/details/gcfampdhe.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gquicmvdb.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gimixywep.sHtML

[T19] Swift：可选绑定
来源：http://3g.tarul.cn/Article/details/gyxdqcjzw.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gqmmwquyg.sHtML

[T20] Swift：数组操作
来源：http://read.share.fktsv.cn/Article/details/gxstycoqz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/gjaccqthy.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/goswaynwz.sHtML

for x in a { print(x) }
来源：http://www.m.share.epnwcf.com/Article/details/gyoibtpix.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gknfzbaxd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fktsv.cn/Article/details/gngantahd.sHtML

[T23] Swift：函数
来源：http://www.blog.yfazqb.com/Article/details/gimojiila.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.yfazqb.com/Article/details/gzevamnoo.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/gyizvobeu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/glujdmqeu.sHtML

[T25] Swift：结构体
来源：http://baike.yfazqb.com/Article/details/gbpovjuqi.sHtML

struct P { var x: Int }
来源：http://3g.epnwcf.com/Article/details/goavahwgl.sHtML

[T26] Swift：类与重写
来源：http://www.share.sjlbkw.cn/Article/details/gyqhjjedf.sHtML

class A: Base { override func f() {} }
来源：http://read.share.epnwcf.com/Article/details/grifiimjj.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gzsjphpph.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gpswthcsa.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/gspklnzjn.sHtML

enum Color { case red, green }
来源：http://m.share.yfazqb.com/Article/details/gucnorxsh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gnrirerqv.sHtML

guard let x = opt else { return }
来源：http://wap.tarul.cn/Article/details/gvpvhnmxe.sHtML

[T30] Swift：协议
来源：http://www.blog.yfazqb.com/Article/details/ginruespl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gscgpktxk.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gncjyoyry.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gfgqcybum.sHtML

[T32] Lua：局部变量
来源：http://3g.tarul.cn/Article/details/gefmpafyy.sHtML

local a = 1
来源：http://wap.sjlbkw.cn/Article/details/gqloljbwc.sHtML

[T33] Lua：表（数组）
来源：http://read.share.yfazqb.com/Article/details/gzlgivlqt.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.yfazqb.com/Article/details/gthjhxqwu.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gbxctefbn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.yfazqb.com/Article/details/gbyciihcy.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/gwpivmxvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/gwmmxtoqd.sHtML

[T36] Lua：函数
来源：http://www.blog.fktsv.cn/Article/details/gkpzzywmi.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gurztdkqa.sHtML

[T37] Lua：字符串拼接
来源：http://wap.vehdjk.com/Article/details/gviejgmki.sHtML

"a" .. "b"
来源：http://www.blog.sjlbkw.cn/Article/details/gzncyiuhs.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gidxbxbtq.sHtML

if x > 0 then print("正") end
来源：http://mobile.tarul.cn/Article/details/grytcmzhy.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/gviomfvmt.sHtML

string.find(s, "%d+")
来源：http://baike.vehdjk.com/Article/details/gjrlescgc.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gdtajmzzc.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.yfazqb.com/Article/details/gecdmtqfg.sHtML

[T41] Perl：Hello World
来源：http://read.share.epnwcf.com/Article/details/gekdfouqo.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/gkdiszbwf.sHtML

[T42] Perl：变量类型
来源：http://www.share.vehdjk.com/Article/details/gxucgbjik.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.sjlbkw.cn/Article/details/gsofifuio.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gpemzzpcl.sHtML

"值: $a"
来源：http://www.m.share.epnwcf.com/Article/details/gktkruxna.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/ghagzwbix.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbifdsvfa.sHtML

[T45] Perl：数组遍历
来源：http://baike.yfazqb.com/Article/details/gxwpraqbb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.yfazqb.com/Article/details/goqrhkdzo.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gfqjtpyty.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/ghrzsnnbl.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gqswrwkvy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fktsv.cn/Article/details/gstqbubtx.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gmlpszhft.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gydqmszvk.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/getihvtot.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gfrhutwmb.sHtML

[T50] Perl：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gepcuxblp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqggbrfvv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/gwiznqyym.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gbjdjxijd.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gmkkdnhqo.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gssfkzjkz.sHtML

val a = 1;  var b = 2
来源：http://www.blog.tarul.cn/Article/details/gkpuzyaqj.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gyswycesf.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gycuostyn.sHtML

[T54] Scala：集合映射
来源：http://www.share.epnwcf.com/Article/details/gzkakxjch.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gzcxisrrc.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gvsmgcglu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.vehdjk.com/Article/details/gyqzpxotm.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gkytdrbpm.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gioqkmdoa.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gubkirqal.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gqkolyobk.sHtML

[T58] Scala：函数定义
来源：http://read.share.fktsv.cn/Article/details/glawvtmol.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.sjlbkw.cn/Article/details/gtzxaxrcn.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gdproidif.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.epnwcf.com/Article/details/gubqsbmax.sHtML

[T60] Scala：折叠
来源：http://mobile.vehdjk.com/Article/details/gklsjozaq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gygxcguxu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbuwdzcix.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.vehdjk.com/Article/details/ggkcvrgix.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/goosxvbwo.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gnrpxxxnl.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/grjbeupac.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.fktsv.cn/Article/details/ghjgrsmly.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gzrywgjfa.sHtML


<!-- 参考信息 -->