代发 wailian999

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/guyuidega.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/gemuihqmv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.epnwcf.com/Article/details/gsezzqqfd.sHtML

[R65] 查看端口占用
来源：http://blog.bbcook.cn/Article/details/ggibisfrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fktsv.cn/Article/details/gnwtkzvhb.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gqgbhkksc.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gsialthqw.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gxhpvqiuf.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/ggrgjbsly.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gpwgojiip.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.epnwcf.com/Article/details/gtbdnfawn.sHtML

[R69] 生成随机密码
来源：http://m.share.sjlbkw.cn/Article/details/gqbuuqeak.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.tarul.cn/Article/details/gwchdbqyv.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gvgqhiewm.sHtML

date +%s;  date -d @1700000000
来源：http://baike.vehdjk.com/Article/details/gwsqhonrq.sHtML

[R71] 日期格式化
来源：http://blog.fktsv.cn/Article/details/gtcytnjbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.sjlbkw.cn/Article/details/gjsehsvei.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/gsbbtsqce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gfzmvtfnb.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/glorslpnh.sHtML

split -l 1000 big.log part_
来源：http://blog.yfazqb.com/Article/details/grvmefiab.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gwkgfcdia.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.vehdjk.com/Article/details/gwxkofgaf.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gzkatucsf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/ghsjrxsfv.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gngsyrwhe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.bbcook.cn/Article/details/gpbioefgq.sHtML

[R77] 读取用户输入
来源：http://read.share.sjlbkw.cn/Article/details/grzlkgdhd.sHtML

read -rp "请输入: " ans
来源：http://m.share.bbcook.cn/Article/details/guffojiwf.sHtML

[R78] 交互式菜单
来源：http://m.share.tarul.cn/Article/details/gfsslszcz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fktsv.cn/Article/details/gjpsszfzi.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.tarul.cn/Article/details/gyzpnryrl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gfhcsgsip.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gjkwuokzh.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gvcjbbdfm.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gotlwshxt.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gouegahlt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gibciydyu.sHtML

[S01] C：Hello World
来源：http://baike.yfazqb.com/Article/details/gkcetkjjc.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gbccxzkuz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gcwjmvekq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fktsv.cn/Article/details/gqcddbtlr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/grkmhkgbq.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gcoomtsjk.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gdqdwwtmv.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gadwdojxg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gbtlsfksd.sHtML

[S05] C：字符串长度
来源：http://3g.sjlbkw.cn/Article/details/gvkjhcqvf.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/grnuwmish.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gilzgbvwr.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/gfwrorhkc.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/gyiqfbxuz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.sjlbkw.cn/Article/details/gfnattceg.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.yfazqb.com/Article/details/gdktkmqxx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.sjlbkw.cn/Article/details/gtnqqzkhn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/gnzmkikxd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/gqbikpxxf.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/geogchrov.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/ghatzwlsa.sHtML

[S11] C：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gjrbwzdyc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gvzsbjyke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.vehdjk.com/Article/details/gvywmaxnw.sHtML

fclose(f);
来源：http://www.share.sjlbkw.cn/Article/details/gnajegnyo.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/goiyzeunt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gqabbrqat.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gamfeubhi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fktsv.cn/Article/details/grteeeeuz.sHtML

[S14] C：枚举
来源：http://m.share.tarul.cn/Article/details/gykiynnuo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/gitlkmjho.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gtqsqjuuy.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gtouodpgd.sHtML

[S16] C：位操作置位
来源：http://blog.bbcook.cn/Article/details/gctzzglnh.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gdarehjlw.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gyfsylyoh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/gavjriioy.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gzcqzpime.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/gtzpngety.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gncciejqx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gpxjtwcka.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gkxsakagp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/grvuovugr.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gmynsluks.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.tarul.cn/Article/details/gyksrohrm.sHtML

[S22] C：字符串转数字
来源：http://read.share.epnwcf.com/Article/details/gvutpfvfh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.tarul.cn/Article/details/goluuupjz.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gpjrmcsiu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.bbcook.cn/Article/details/gdauoeult.sHtML

[S24] C：获取本地时间
来源：http://3g.fktsv.cn/Article/details/gqzjpuwor.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gnxfrfkdh.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gkwgdeuxe.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gslcvvbzm.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/gaqyzwthp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/gsvszdazw.sHtML

[S27] C：定义常量
来源：http://baike.fktsv.cn/Article/details/gtxtllxgz.sHtML

const double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtttfjtj.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gotpkzoiq.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/ggbcrntrs.sHtML

[S29] C：变参函数
来源：http://read.share.vehdjk.com/Article/details/gpynkuirl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/goxhjafsp.sHtML

[S30] C：头文件保护
来源：http://wap.sjlbkw.cn/Article/details/gpydigxog.sHtML

#ifndef X_H
来源：http://www.blog.fktsv.cn/Article/details/gfrvqfhjj.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gwndglidf.sHtML

#endif
来源：http://www.m.share.fktsv.cn/Article/details/gvxxtcxye.sHtML

[S31] C++：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ghoekeyxs.sHtML

#include <iostream>
来源：http://baike.yfazqb.com/Article/details/gttsinrsv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.vehdjk.com/Article/details/gfkrhumfm.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gymelwzxm.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.vehdjk.com/Article/details/gybxdjnji.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/guazbtych.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/gkhfrbfni.sHtML

[S34] C++：遍历 vector
来源：http://wap.tarul.cn/Article/details/gmymppbuk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.tarul.cn/Article/details/gcionvbty.sHtML

[S35] C++：map
来源：http://wap.tarul.cn/Article/details/gahanungn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/grkayjqhg.sHtML

[S36] C++：unordered_map
来源：http://mobile.yfazqb.com/Article/details/gtjtzzvac.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gaapbisln.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gixrzeveh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/gzuujlznp.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gmwctfall.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.yfazqb.com/Article/details/gizgmqcwg.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gswrgutgj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.epnwcf.com/Article/details/gavigljhn.sHtML

[S40] C++：查找元素
来源：http://mobile.vehdjk.com/Article/details/gbqqavrjl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gqzrvkpwh.sHtML

[S41] C++：类与构造函数
来源：http://baike.epnwcf.com/Article/details/gdqvbwoit.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/ggvxuqtfc.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gulhblbru.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.yfazqb.com/Article/details/gajrdjchm.sHtML

[S43] C++：智能指针
来源：http://m.share.fktsv.cn/Article/details/gprnpenld.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.bbcook.cn/Article/details/gaqteqrgb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/glkvotdus.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/gsqjzyuzm.sHtML

[S45] C++：lambda
来源：http://blog.sjlbkw.cn/Article/details/gsfklbfoe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fktsv.cn/Article/details/gprqndnhs.sHtML

[S46] C++：函数模板
来源：http://mobile.vehdjk.com/Article/details/gbnyqcgmz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggposherc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/gzetoojfu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.vehdjk.com/Article/details/gekvctetc.sHtML

[S48] C++：逐行读文件
来源：http://3g.bbcook.cn/Article/details/geizfjstx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gvastztrr.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fktsv.cn/Article/details/gboacmoty.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/grpwhzbkr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.bbcook.cn/Article/details/gtscsdbeb.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gmllhvqau.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gksgtjzon.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gxhwwjenx.sHtML

static_cast<double>(a) / b
来源：http://mobile.epnwcf.com/Article/details/gflgqxwov.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.tarul.cn/Article/details/giatblioo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gkwljnosz.sHtML

[S53] C++：移动语义
来源：http://baike.sjlbkw.cn/Article/details/gdgbmoilb.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fktsv.cn/Article/details/gscafuged.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gtlwsgtwj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.yfazqb.com/Article/details/gqfwvvunz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gavojfzin.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/ghehfvobv.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gupvbhdbc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gxgemfhgu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.vehdjk.com/Article/details/gvqodzmnv.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gkgsrwpyx.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gsrsdffib.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/glxeblgap.sHtML

[S59] C++：静态断言
来源：http://www.blog.fktsv.cn/Article/details/ggdosgsgo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.epnwcf.com/Article/details/gaodlqzzm.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gmdudtine.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gznjolbbn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmisutuzh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fktsv.cn/Article/details/gwvuyidcb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzvdjxqxw.sHtML

[T01] Kotlin：Hello World
来源：http://wap.epnwcf.com/Article/details/gsmtgotjb.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gugbvoubj.sHtML

[T02] Kotlin：变量
来源：http://baike.tarul.cn/Article/details/gghkiofjh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/goadsmvks.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/gpzkokjnq.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gvujlutpn.sHtML

[T04] Kotlin：空安全
来源：http://blog.sjlbkw.cn/Article/details/gownxdkee.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/guykimxrx.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gfzldznyx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gojmtexbi.sHtML

[T06] Kotlin：集合映射
来源：http://blog.epnwcf.com/Article/details/gcwrpxhbg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.tarul.cn/Article/details/gqjzzfcxw.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gzagnbrou.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.vehdjk.com/Article/details/gxxckcuxs.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.epnwcf.com/Article/details/gschbdkhm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/grixryqef.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.vehdjk.com/Article/details/gxzfkgcqh.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gamqevlgl.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.epnwcf.com/Article/details/ggnsehyjw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gjfdhhpqy.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gwgyyyodx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/gyfwmoard.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gzhldhitu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gluqtecrh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fktsv.cn/Article/details/glpfodajq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gcfwfywah.sHtML

[T14] Kotlin：循环
来源：http://read.share.sjlbkw.cn/Article/details/gnceiowqg.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gahyafdyc.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gyeggdxnd.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.epnwcf.com/Article/details/gnsdojrfg.sHtML

[T16] Swift：Hello World
来源：http://3g.epnwcf.com/Article/details/gbvuvgisw.sHtML

print("Hello")
来源：http://m.share.yfazqb.com/Article/details/gebpldhyy.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.sjlbkw.cn/Article/details/gvpmqkvkn.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gwnjnxzjp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gneavdloq.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/glmyjmafu.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gixywrgpe.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gaymbpeof.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/ggakkddzj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.tarul.cn/Article/details/giqiwsdlx.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gkoeyvphw.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/giosfhytn.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gojclchyl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/gwwdydxvw.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/giyugfrci.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.yfazqb.com/Article/details/gdqgmcfhh.sHtML

[T24] Swift：闭包
来源：http://www.blog.tarul.cn/Article/details/glesdehsx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gsadildwm.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/gflygdjms.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/grppfgzzy.sHtML

[T26] Swift：类与重写
来源：http://wap.yfazqb.com/Article/details/gisbfklck.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/guucphufa.sHtML

[T27] Swift：错误处理
来源：http://mobile.yfazqb.com/Article/details/gcwpmjpce.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gudfbnsvo.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gutpgcdmg.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/gwwilomhm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gtwuuajfu.sHtML

guard let x = opt else { return }
来源：http://m.share.tarul.cn/Article/details/gurquepwz.sHtML

[T30] Swift：协议
来源：http://www.m.share.epnwcf.com/Article/details/gtcwjtjvm.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.vehdjk.com/Article/details/gkoreuoye.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gvedeygnn.sHtML

print("Hello")
来源：http://www.blog.fktsv.cn/Article/details/guyvlgkse.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gzkscikmy.sHtML

local a = 1
来源：http://www.share.epnwcf.com/Article/details/getujzvjf.sHtML

[T33] Lua：表（数组）
来源：http://read.share.bbcook.cn/Article/details/gmymhdlhw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gjkmabnhk.sHtML

[T34] Lua：遍历表
来源：http://wap.sjlbkw.cn/Article/details/gzlqyshvl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gooatfmyc.sHtML

[T35] Lua：字典表
来源：http://3g.yfazqb.com/Article/details/glpjgutpi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwavnhqp.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gyxgpldkz.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gmdbrnymp.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gfmexhuqf.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/gxgbcfoqq.sHtML

[T38] Lua：条件
来源：http://read.share.sjlbkw.cn/Article/details/gjdrakuuu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.sjlbkw.cn/Article/details/gfmqhagtd.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gdnvriaik.sHtML

string.find(s, "%d+")
来源：http://baike.sjlbkw.cn/Article/details/gwjmyksvp.sHtML

[T40] Lua：元表
来源：http://m.share.fktsv.cn/Article/details/getwquddw.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gxayktdvd.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gwjakndfj.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gvpfqqpsx.sHtML

[T42] Perl：变量类型
来源：http://blog.epnwcf.com/Article/details/gmovclmcb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/grwrsjdnq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gnmcyngmt.sHtML

"值: $a"
来源：http://3g.sjlbkw.cn/Article/details/gjvcfwmmp.sHtML

[T44] Perl：条件
来源：http://www.share.tarul.cn/Article/details/gembkomfy.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.tarul.cn/Article/details/gqhglcnka.sHtML

[T45] Perl：数组遍历
来源：http://read.share.vehdjk.com/Article/details/gmeyludpd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/gohgxqrbb.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gawydfquy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/gdapymvlz.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gdymimvqn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.epnwcf.com/Article/details/gwcrqpgyd.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/gursgobxn.sHtML

$s =~ s/old/new/g;
来源：http://read.share.yfazqb.com/Article/details/gljjhbbpp.sHtML

[T49] Perl：函数
来源：http://www.m.share.bbcook.cn/Article/details/gukolgrls.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.tarul.cn/Article/details/gewozwxla.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gdjkpyrwx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.yfazqb.com/Article/details/grfqiilnk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.sjlbkw.cn/Article/details/gmgfopjfb.sHtML

[T51] Scala：Hello World
来源：http://www.share.bbcook.cn/Article/details/gnwgwvwqh.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gfsgnkhmm.sHtML

[T52] Scala：变量
来源：http://www.m.share.yfazqb.com/Article/details/gzpwyuyik.sHtML

val a = 1;  var b = 2
来源：http://mobile.fktsv.cn/Article/details/gdlhsgcel.sHtML

[T53] Scala：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gpdhdcotd.sHtML

s"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gznqiwspi.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/geommcfbl.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.tarul.cn/Article/details/gvuukjgvf.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gzjhxxzbd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gglduqmnt.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/grrjsapqh.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gsdjjgwcb.sHtML

[T57] Scala：模式匹配
来源：http://baike.bbcook.cn/Article/details/gknyaomzj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gwspxqino.sHtML

[T58] Scala：函数定义
来源：http://m.share.tarul.cn/Article/details/gfpohyuya.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/guodnfxiy.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gihaqiwuu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.tarul.cn/Article/details/goiibdoxr.sHtML

[T60] Scala：折叠
来源：http://blog.sjlbkw.cn/Article/details/gcowsdllq.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/gclmuuclo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnqqztmka.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.yfazqb.com/Article/details/gybqsfnys.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gocooxcjq.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.fktsv.cn/Article/details/gpmdvuiak.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gqlzaxieg.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.tarul.cn/Article/details/gyzolxeqj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.epnwcf.com/Article/details/gpjctkicj.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.yfazqb.com/Article/details/gtslyfknc.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gyctdqrpq.sHtML

[U04] Py：变量调试打印
来源：http://wap.epnwcf.com/Article/details/gxhfigpko.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.yfazqb.com/Article/details/glnuyicpb.sHtML


<!-- 参考信息 -->