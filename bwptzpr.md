代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.epnwcf.com/Article/details/gejbdrkeb.sHtML

[R66] 定时任务
来源：http://read.share.yfazqb.com/Article/details/grynehrqi.sHtML

crontab -e;  crontab -l
来源：http://wap.epnwcf.com/Article/details/gihrbiuuf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gouunamdv.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gjrfrxdyl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/gkvvlrvyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gfxynunai.sHtML

[R69] 生成随机密码
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgsprfbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gumpoisyo.sHtML

[R70] 时间戳与互转
来源：http://www.share.sjlbkw.cn/Article/details/gfzdikhve.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gvrboqaoz.sHtML

[R71] 日期格式化
来源：http://m.share.tarul.cn/Article/details/grjlxqlcf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gfqegxnyu.sHtML

[R72] 等待端口就绪
来源：http://3g.tarul.cn/Article/details/gyfyqbzce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gdrvzqqsx.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/gmybrucyn.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gpfqfgwwa.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/grgrrkcfv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.bbcook.cn/Article/details/ggjmiumsn.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gfdockmki.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gdtjelsin.sHtML

[R76] 使用临时文件
来源：http://www.blog.epnwcf.com/Article/details/ghlucepdb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.tarul.cn/Article/details/gtnkkehht.sHtML

[R77] 读取用户输入
来源：http://baike.yfazqb.com/Article/details/glynrmowp.sHtML

read -rp "请输入: " ans
来源：http://baike.tarul.cn/Article/details/genmhgilf.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gjadcskff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.yfazqb.com/Article/details/gzewfetic.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/grgwzvofj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/gxjyzlpdp.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gbwkdkfjt.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/gkcsknnpd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghccuxlpq.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/gfgkowhvu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/godvudlew.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gljsrgueg.sHtML

#include <stdio.h>
来源：http://read.share.epnwcf.com/Article/details/gcwxcbpvv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.epnwcf.com/Article/details/gntbzatca.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gvvicaght.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.sjlbkw.cn/Article/details/gkkuklzll.sHtML

[S03] C：读入整数
来源：http://wap.fktsv.cn/Article/details/gtazengfs.sHtML

int x; scanf("%d", &x);
来源：http://www.share.bbcook.cn/Article/details/gshkroldu.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/gstspqtbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.bbcook.cn/Article/details/gpzrfmjmc.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gjlqeeuxy.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gncfsphbn.sHtML

[S06] C：字符串比较
来源：http://www.share.fktsv.cn/Article/details/gfpnohjck.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/ghriyzdxd.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gpywevide.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.sjlbkw.cn/Article/details/gfaofexqk.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/glilhsrcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fktsv.cn/Article/details/gkflfzjxr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gregddcjq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.bbcook.cn/Article/details/gjudfdcqi.sHtML

[S10] C：指针与解引用
来源：http://baike.yfazqb.com/Article/details/gwpccvulk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gvvzsojym.sHtML

[S11] C：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gxmkvropv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/gqtgyjnne.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gxweefxfb.sHtML

fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqijibag.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/ginvrfwlr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gfjpgvwqf.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gqtqtlfnt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gvvxnhzpe.sHtML

[S14] C：枚举
来源：http://www.blog.fktsv.cn/Article/details/gargxgwff.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gyvxlhoff.sHtML

[S15] C：类型转换
来源：http://wap.sjlbkw.cn/Article/details/gssaomarj.sHtML

(double) a / b
来源：http://www.share.fktsv.cn/Article/details/gixglxzbq.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/ggaiqgyet.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gqfijwvpj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gcvukwskv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.tarul.cn/Article/details/gfyyiegju.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gutwkkula.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsixvyswc.sHtML

[S19] C：快速排序
来源：http://blog.tarul.cn/Article/details/glfedzcxu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gtmdqxkhj.sHtML

[S20] C：二分查找
来源：http://wap.sjlbkw.cn/Article/details/gcjkbvpoo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gsgacwqin.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gylsiinjz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/gqslozeso.sHtML

[S22] C：字符串转数字
来源：http://www.blog.tarul.cn/Article/details/gvmavkpmg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.yfazqb.com/Article/details/gemydortf.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/goinrqnlj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fktsv.cn/Article/details/gotkleirq.sHtML

[S24] C：获取本地时间
来源：http://baike.bbcook.cn/Article/details/gcvzgfahe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fktsv.cn/Article/details/gdwhjbdvr.sHtML

[S25] C：内存拷贝
来源：http://m.share.yfazqb.com/Article/details/gjytevixx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.bbcook.cn/Article/details/gqexmarcz.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gsqcnqxgl.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.tarul.cn/Article/details/gjgvxdcfw.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/ggpdzjhns.sHtML

const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gtnifxovv.sHtML

[S28] C：静态变量
来源：http://baike.sjlbkw.cn/Article/details/grlmfctxp.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gwlhcqwht.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gprrnlary.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.bbcook.cn/Article/details/gtfyxqasv.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gidskjmnx.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gkedzqyhk.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gscaqprrd.sHtML

#endif
来源：http://read.share.tarul.cn/Article/details/gzlqlgngl.sHtML

[S31] C++：Hello World
来源：http://blog.yfazqb.com/Article/details/gyqmnktjn.sHtML

#include <iostream>
来源：http://www.share.fktsv.cn/Article/details/ghoalbkgi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/glydiwczt.sHtML

[S32] C++：字符串
来源：http://baike.bbcook.cn/Article/details/gxsnjhvlh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.vehdjk.com/Article/details/gfqiclfkq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.yfazqb.com/Article/details/gqtofbohq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gqeqaeuza.sHtML

[S34] C++：遍历 vector
来源：http://m.share.vehdjk.com/Article/details/gadcqjdmr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.epnwcf.com/Article/details/gpsyoaeiv.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/gdzqbdvvj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gbtyhoylb.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gapjfuuwk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gpmjxtrkx.sHtML

[S37] C++：set
来源：http://www.m.share.fktsv.cn/Article/details/gorrkdcye.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.sjlbkw.cn/Article/details/gytdphzrz.sHtML

[S38] C++：排序
来源：http://www.share.bbcook.cn/Article/details/gwtgmuadt.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gicglazpy.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/givozvuis.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzlxvfbx.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gftqulhss.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/godyznksd.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fktsv.cn/Article/details/gcudvpnis.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.vehdjk.com/Article/details/gkwnqtehx.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/giodobpfk.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fktsv.cn/Article/details/gplfaupcu.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gsvlxxzun.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/ggduogzhu.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gfqyudwwi.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.epnwcf.com/Article/details/giyzdlbqp.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gxybealzc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/guztcszol.sHtML

[S46] C++：函数模板
来源：http://blog.bbcook.cn/Article/details/gcdninxkp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gnscfpfib.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fktsv.cn/Article/details/guxvcfdlj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.epnwcf.com/Article/details/gtbwenhyj.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/ghnufsnge.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.vehdjk.com/Article/details/ggtfolyom.sHtML

while (std::getline(in, line)) { }
来源：http://wap.yfazqb.com/Article/details/gobzgetbh.sHtML

[S49] C++：写文件
来源：http://blog.fktsv.cn/Article/details/geezpiudf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.epnwcf.com/Article/details/gimvhjchg.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.tarul.cn/Article/details/gzlxqdjyc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.bbcook.cn/Article/details/giuvsjhoo.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gokbxlkkf.sHtML

static_cast<double>(a) / b
来源：http://read.share.bbcook.cn/Article/details/gpsjcnkvy.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.vehdjk.com/Article/details/gizmjgowh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gnkdecjil.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gldkhnwfh.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/ghjcwklxb.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/gszvvonry.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gzjdulbsx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/ghsseksjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gwevhvqzs.sHtML

[S56] C++：optional
来源：http://baike.vehdjk.com/Article/details/gpzwqgtoz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fktsv.cn/Article/details/gdlynwfzh.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gglniglqu.sHtML

constexpr int N = 10;
来源：http://www.blog.yfazqb.com/Article/details/giuwllxnc.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/grpdewuad.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.epnwcf.com/Article/details/gbiztbhkl.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gdavwpypk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.vehdjk.com/Article/details/gpueqspap.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/gwarrzglt.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/gwfsbnfeb.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/godtmkrya.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/ghlpqhcbe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwookzpdb.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gzmxmvbef.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/geymwxgkn.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gkcomzvht.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.sjlbkw.cn/Article/details/gbqcblbbh.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.bbcook.cn/Article/details/gyxebfzdb.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/ghqznvuvp.sHtML

[T04] Kotlin：空安全
来源：http://baike.epnwcf.com/Article/details/gqvppkhvy.sHtML

val n: String? = null;  n?.length
来源：http://baike.yfazqb.com/Article/details/gjiuvgpkk.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/grvrofvht.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.bbcook.cn/Article/details/gzkuinemh.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.yfazqb.com/Article/details/gimuuaeso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.vehdjk.com/Article/details/gvgnigqom.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fktsv.cn/Article/details/guyadkuqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/gjuzerucs.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gvyicixes.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gosvdidua.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/ggjlpiltd.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gxwzrugke.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gnorgswmi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gwvcldsuv.sHtML

[T11] Kotlin：协程
来源：http://m.share.sjlbkw.cn/Article/details/grkcifefm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gpsfkiyhb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/ggbvvwrta.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gtemausyv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.epnwcf.com/Article/details/guejmytlz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/grobmsejx.sHtML

[T14] Kotlin：循环
来源：http://m.share.epnwcf.com/Article/details/goqwntdzz.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gsntxdyhg.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gtfjcjunq.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gnzdtvgtx.sHtML

[T16] Swift：Hello World
来源：http://read.share.vehdjk.com/Article/details/gcdijdozn.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gzforjyze.sHtML

[T17] Swift：变量与常量
来源：http://baike.epnwcf.com/Article/details/gfhqblkzt.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gxlfywmdz.sHtML

[T18] Swift：字符串插值
来源：http://read.share.vehdjk.com/Article/details/glzsdywic.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gcpxrthxm.sHtML

[T19] Swift：可选绑定
来源：http://blog.yfazqb.com/Article/details/gobdczbxv.sHtML

if let n = opt { print(n) }
来源：http://www.blog.yfazqb.com/Article/details/gwxpwlrmp.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gdwybweba.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gyzcppvpb.sHtML

[T21] Swift：遍历
来源：http://www.share.fktsv.cn/Article/details/gkqtcgnel.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gebgakmsy.sHtML

[T22] Swift：字典
来源：http://3g.fktsv.cn/Article/details/giggxzmdr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gdfprtsar.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/gotsqeuro.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.vehdjk.com/Article/details/gocymmfuq.sHtML

[T24] Swift：闭包
来源：http://mobile.bbcook.cn/Article/details/gkgxotrmc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gwdmefoiw.sHtML

[T25] Swift：结构体
来源：http://3g.sjlbkw.cn/Article/details/gqphbhfjn.sHtML

struct P { var x: Int }
来源：http://read.share.epnwcf.com/Article/details/goyekpuoa.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gjqhwookw.sHtML

class A: Base { override func f() {} }
来源：http://blog.tarul.cn/Article/details/ggmcuvzae.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gfqbpcpfx.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gzxzlzvyn.sHtML

[T28] Swift：枚举
来源：http://m.share.yfazqb.com/Article/details/gabqmzzjr.sHtML

enum Color { case red, green }
来源：http://www.blog.yfazqb.com/Article/details/gdcanoccr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.bbcook.cn/Article/details/gqdbjuzir.sHtML

guard let x = opt else { return }
来源：http://baike.yfazqb.com/Article/details/gubfxdqvy.sHtML

[T30] Swift：协议
来源：http://read.share.sjlbkw.cn/Article/details/gdotvfawm.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.bbcook.cn/Article/details/ggjdduokk.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gwnipzpzl.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gabyxskeb.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gliijffwy.sHtML

local a = 1
来源：http://www.m.share.tarul.cn/Article/details/gwjvgejcj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.sjlbkw.cn/Article/details/glzmuhnct.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.tarul.cn/Article/details/gdlixnksx.sHtML

[T34] Lua：遍历表
来源：http://baike.yfazqb.com/Article/details/gshazspip.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.sjlbkw.cn/Article/details/gniwhxegs.sHtML

[T35] Lua：字典表
来源：http://www.blog.tarul.cn/Article/details/gsnjyvykf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/gpxtrijqk.sHtML

[T36] Lua：函数
来源：http://blog.sjlbkw.cn/Article/details/gouxkbiks.sHtML

function add(a, b) return a + b end
来源：http://wap.fktsv.cn/Article/details/gpubvfgpd.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gvrbddiyc.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/goommnbnj.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/gebiytlpf.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gkozuuucq.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/geahjnecz.sHtML

string.find(s, "%d+")
来源：http://www.share.yfazqb.com/Article/details/gvfyhcocj.sHtML

[T40] Lua：元表
来源：http://3g.epnwcf.com/Article/details/gieszynyi.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gqzpfazhd.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gyflxrefj.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gcmkwycak.sHtML

[T42] Perl：变量类型
来源：http://blog.sjlbkw.cn/Article/details/gmbljybck.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.sjlbkw.cn/Article/details/gwyapvtux.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gejnjytju.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/giziowgnj.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/gcrzvjtnp.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.yfazqb.com/Article/details/ghjhvssuk.sHtML

[T45] Perl：数组遍历
来源：http://blog.bbcook.cn/Article/details/gtgynchoy.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/ghfzlmjpr.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/gvsxnwuxu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/gkztnhucx.sHtML

[T47] Perl：正则捕获
来源：http://baike.tarul.cn/Article/details/gnarsgvzp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.tarul.cn/Article/details/ghudrncrj.sHtML

[T48] Perl：正则替换
来源：http://m.share.bbcook.cn/Article/details/gnvssjxym.sHtML

$s =~ s/old/new/g;
来源：http://3g.sjlbkw.cn/Article/details/ghixmvcxk.sHtML

[T49] Perl：函数
来源：http://m.share.yfazqb.com/Article/details/giwcafrst.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/ghtttmjab.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gfcxmcbuk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.sjlbkw.cn/Article/details/ggqlrmkqf.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.yfazqb.com/Article/details/gboszrewm.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gynzvjhji.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gumzucsmc.sHtML

[T52] Scala：变量
来源：http://m.share.sjlbkw.cn/Article/details/gmpjlzfsi.sHtML

val a = 1;  var b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gxnfneqoo.sHtML

[T53] Scala：字符串插值
来源：http://baike.vehdjk.com/Article/details/gehhycbrf.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gdyqueoyx.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/garkjrxzo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/grwtwqkwa.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gsvavwyek.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gazdqrztq.sHtML

[T56] Scala：样例类
来源：http://read.share.bbcook.cn/Article/details/ghgvguqko.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/gzvjuriau.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/grytxibey.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/giaosefap.sHtML

[T58] Scala：函数定义
来源：http://3g.fktsv.cn/Article/details/gdsxwzaxu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gviyiangv.sHtML

[T59] Scala：循环
来源：http://baike.bbcook.cn/Article/details/gvrvenuoz.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/gacgrjtpg.sHtML

[T60] Scala：折叠
来源：http://m.share.bbcook.cn/Article/details/gaocsfgiw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gdrkzciby.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gllqsjryf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fktsv.cn/Article/details/gsryegnzb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gswwgxacl.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.epnwcf.com/Article/details/gbmzogmna.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.yfazqb.com/Article/details/gojzzmkge.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpbbafhj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.vehdjk.com/Article/details/gjsacpflz.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.tarul.cn/Article/details/ggnouhwot.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.fktsv.cn/Article/details/gdooirrri.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gadfomxmk.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.tarul.cn/Article/details/gspehvmya.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.yfazqb.com/Article/details/gfphtjdgx.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gepvrxsae.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/gvmzuhijr.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/gvxptosqu.sHtML


<!-- 参考信息 -->