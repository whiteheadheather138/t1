代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.sjlbkw.cn/Article/details/geuzjjefu.sHtML

[R66] 定时任务
来源：http://read.share.tarul.cn/Article/details/glltojnmf.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/ggwbvswzk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gvkcultns.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/grdapuztm.sHtML

[R68] 计算文件校验值
来源：http://www.blog.yfazqb.com/Article/details/grmlfnpxb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.tarul.cn/Article/details/galkrkxqa.sHtML

[R69] 生成随机密码
来源：http://www.share.vehdjk.com/Article/details/guppwmhgu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.tarul.cn/Article/details/gkresslbr.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/ggnvoixiu.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gyvlbtlwk.sHtML

[R71] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/ghfhiidqy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gwlmwaqgz.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gndqaosod.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gspqpuqbq.sHtML

[R73] 分割大日志
来源：http://read.share.vehdjk.com/Article/details/gqobmlkry.sHtML

split -l 1000 big.log part_
来源：http://mobile.tarul.cn/Article/details/gchuwewxn.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/ghanxvevq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gtouetzvl.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gdcleabyk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.epnwcf.com/Article/details/gjzeqkgha.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gvkrrfplq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.vehdjk.com/Article/details/guelrsefw.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gwghvurbo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfjjuvja.sHtML

[R78] 交互式菜单
来源：http://www.blog.sjlbkw.cn/Article/details/ghhmolrck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.tarul.cn/Article/details/gyfszcmso.sHtML

[R79] 解析命令行选项
来源：http://mobile.yfazqb.com/Article/details/gguwwjdgj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gvtmesbgh.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/guxpvcqdn.sHtML

time ./run.sh
来源：http://www.m.share.bbcook.cn/Article/details/gqhnziobg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gsbalwtlx.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/goebrapui.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjionwjcv.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gkudckqve.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/gnhtqisqo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.vehdjk.com/Article/details/glvqhnxdo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gppevoiwe.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.tarul.cn/Article/details/gegiaaqss.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gnahegctu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gwplxuoja.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/glnwhapov.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gxbynefyz.sHtML

[S05] C：字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gxfcldqjn.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gbwrflsjs.sHtML

[S06] C：字符串比较
来源：http://www.share.tarul.cn/Article/details/gpvgtnwaz.sHtML

strcmp(a, b) == 0
来源：http://m.share.yfazqb.com/Article/details/guwvbeimt.sHtML

[S07] C：数组遍历求和
来源：http://wap.yfazqb.com/Article/details/gtvyacqnh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.epnwcf.com/Article/details/giiwgvcvf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.epnwcf.com/Article/details/gdeknraiw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/gfgmfwdsg.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.tarul.cn/Article/details/giayytuax.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.tarul.cn/Article/details/glarxwnej.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gfkqkcvhr.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fktsv.cn/Article/details/goircnzbm.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/geyuypsom.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/gfdhpizru.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gxldjpsgf.sHtML

fclose(f);
来源：http://www.blog.yfazqb.com/Article/details/gokelmhwm.sHtML

[S12] C：写文件
来源：http://3g.epnwcf.com/Article/details/gtaswmzgb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.tarul.cn/Article/details/gjgnmsfhu.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gxrjwepfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/grrorimkr.sHtML

[S14] C：枚举
来源：http://3g.epnwcf.com/Article/details/gsjafwvls.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/guvuqxuyd.sHtML

[S15] C：类型转换
来源：http://www.share.bbcook.cn/Article/details/ggpnmlqpv.sHtML

(double) a / b
来源：http://m.share.bbcook.cn/Article/details/glfedbegn.sHtML

[S16] C：位操作置位
来源：http://m.share.sjlbkw.cn/Article/details/ghmxcxnaw.sHtML

x |= (1 << 3);
来源：http://m.share.epnwcf.com/Article/details/gevcgrcoh.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.vehdjk.com/Article/details/grryqgrkl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/gknpmyhwm.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gzvyeytcu.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gbcokapfe.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gujxxjbjq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/ghkrqlhqn.sHtML

[S20] C：二分查找
来源：http://blog.yfazqb.com/Article/details/ggnkoygpn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.yfazqb.com/Article/details/gmifzdywa.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gyblqleco.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.bbcook.cn/Article/details/gczopjbrh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gbfuhaohc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gttclyxll.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gidmsipvo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gselyrmlw.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fktsv.cn/Article/details/gizbwenff.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gbymmpiov.sHtML

[S25] C：内存拷贝
来源：http://3g.bbcook.cn/Article/details/gklfgrwgs.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gbfqcapyc.sHtML

[S26] C：内存清零
来源：http://read.share.sjlbkw.cn/Article/details/gkfedylha.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/gtkovejpq.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/gjoxiyjeg.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gttoafxus.sHtML

[S28] C：静态变量
来源：http://3g.sjlbkw.cn/Article/details/ghbprtsye.sHtML

static int counter = 0;
来源：http://www.share.fktsv.cn/Article/details/gtwlnwqsu.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/ghzeatadm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fktsv.cn/Article/details/gpoflggyz.sHtML

[S30] C：头文件保护
来源：http://www.blog.yfazqb.com/Article/details/gsqakdzoj.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gxdbkicox.sHtML

#define X_H
来源：http://wap.tarul.cn/Article/details/gfibbawos.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gutnsovjs.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gicbhcoxb.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gdtlbjbrd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.sjlbkw.cn/Article/details/grzpbavdw.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gcctomkke.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gbajttrqz.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gqbxvpoaf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.sjlbkw.cn/Article/details/gimytuxfm.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gpweweklk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gnkkvbplh.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gekpjkppi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gomawmznd.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gyfurcdog.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.vehdjk.com/Article/details/gklnbapcy.sHtML

[S37] C++：set
来源：http://blog.yfazqb.com/Article/details/ghhdaazjj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.yfazqb.com/Article/details/geyelrsqt.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gtkjmcpzs.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.vehdjk.com/Article/details/gvxlvbpav.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.epnwcf.com/Article/details/guexzmmbv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gknyaqzgg.sHtML

[S40] C++：查找元素
来源：http://mobile.yfazqb.com/Article/details/gqbxzqkgi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gdztxgdfz.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.tarul.cn/Article/details/gmrvlpurq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fktsv.cn/Article/details/gvamcusxi.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gjnqomhuk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fktsv.cn/Article/details/gmjyqlupr.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gmsaumxtp.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.epnwcf.com/Article/details/gkgcskjbv.sHtML

[S44] C++：引用传参
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfudrzcf.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gymmkbvja.sHtML

[S45] C++：lambda
来源：http://m.share.epnwcf.com/Article/details/glswzumpg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.bbcook.cn/Article/details/gvvhkydsw.sHtML

[S46] C++：函数模板
来源：http://m.share.yfazqb.com/Article/details/gaqbdbjtd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/gvefbcvfy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gyndachtv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.sjlbkw.cn/Article/details/govjdiwcg.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gxaghqddh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gaenxcsib.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gziclzmap.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gstgrjnie.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/gklbpqyrx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/geulbxqqx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gmsldyhum.sHtML

[S51] C++：显式类型转换
来源：http://baike.bbcook.cn/Article/details/gpnvyhobx.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gzbynebpt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.yfazqb.com/Article/details/gxqgzjpfl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gmylfnorf.sHtML

[S53] C++：移动语义
来源：http://mobile.bbcook.cn/Article/details/gaekvhzba.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gqpjaoluc.sHtML

[S54] C++：异常处理
来源：http://blog.sjlbkw.cn/Article/details/guvatqibe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gcbynjskc.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/glqeumqxl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/gotnojeuo.sHtML

[S56] C++：optional
来源：http://read.share.tarul.cn/Article/details/gosxgrblq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.bbcook.cn/Article/details/gdkksinyu.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/greechewf.sHtML

constexpr int N = 10;
来源：http://baike.fktsv.cn/Article/details/gwhtrymzb.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gujvlsnna.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gzvwcbpdh.sHtML

[S59] C++：静态断言
来源：http://m.share.yfazqb.com/Article/details/gckxejjnu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.yfazqb.com/Article/details/guefomoyv.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gqadqfiwl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.tarul.cn/Article/details/gxnoropxb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvjeakdem.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gikzrajca.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gysntvity.sHtML

[T01] Kotlin：Hello World
来源：http://baike.tarul.cn/Article/details/glsovkjmh.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gswblqkvi.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gteooxtyv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/grevtatdj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gkyejizqx.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gdvvabfzl.sHtML

[T04] Kotlin：空安全
来源：http://baike.tarul.cn/Article/details/gjktfuykv.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/gkfxpauby.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.vehdjk.com/Article/details/gyixlkibl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/giwusbcch.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fktsv.cn/Article/details/gnxzggyxc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.tarul.cn/Article/details/ghejabsem.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/ghvyxchhs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gajtcbfyq.sHtML

[T08] Kotlin：数据类
来源：http://wap.tarul.cn/Article/details/gxdyngxqd.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gugubyiyv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fktsv.cn/Article/details/gmjknljch.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fktsv.cn/Article/details/gyalxfqgi.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gpclkndqx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.tarul.cn/Article/details/grhmfgkjz.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/guaxjwpzx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/glgyxaimd.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/gxmjtsued.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gcxlnyvjt.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.epnwcf.com/Article/details/gjukiqgul.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/ggxbdxjae.sHtML

[T14] Kotlin：循环
来源：http://3g.tarul.cn/Article/details/glphwbacm.sHtML

for (i in 1..10) println(i)
来源：http://read.share.vehdjk.com/Article/details/gkjezhuhb.sHtML

[T15] Kotlin：接口
来源：http://mobile.sjlbkw.cn/Article/details/grcqmbusg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.sjlbkw.cn/Article/details/gjyfzqpvp.sHtML

[T16] Swift：Hello World
来源：http://baike.bbcook.cn/Article/details/grtmelgcm.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/ggdvpniit.sHtML

[T17] Swift：变量与常量
来源：http://3g.tarul.cn/Article/details/geokapgpq.sHtML

var a = 1;  let b = 2
来源：http://m.share.vehdjk.com/Article/details/gclbhrqyl.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gocfgcsow.sHtML

"值: \(b)"
来源：http://mobile.yfazqb.com/Article/details/gawiywpph.sHtML

[T19] Swift：可选绑定
来源：http://read.share.tarul.cn/Article/details/gkcnioras.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gijurowfg.sHtML

[T20] Swift：数组操作
来源：http://www.blog.bbcook.cn/Article/details/gufasvncn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.bbcook.cn/Article/details/gffzezhgl.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/glvrdldtj.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gsubtafvg.sHtML

[T22] Swift：字典
来源：http://read.share.vehdjk.com/Article/details/goenqqptd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.epnwcf.com/Article/details/gzyzswqgv.sHtML

[T23] Swift：函数
来源：http://baike.epnwcf.com/Article/details/gzsheqfgm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.epnwcf.com/Article/details/gudtteivd.sHtML

[T24] Swift：闭包
来源：http://mobile.sjlbkw.cn/Article/details/gvjhcjose.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/ggnsxcxzk.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/grxmwfihg.sHtML

struct P { var x: Int }
来源：http://m.share.tarul.cn/Article/details/gxlftjeho.sHtML

[T26] Swift：类与重写
来源：http://baike.fktsv.cn/Article/details/gakgcbdib.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gbikccikq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.yfazqb.com/Article/details/gqslajafx.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gtldhevgx.sHtML

[T28] Swift：枚举
来源：http://m.share.vehdjk.com/Article/details/gredbmzww.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/goqqobdvh.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/ghacjuisj.sHtML

guard let x = opt else { return }
来源：http://read.share.vehdjk.com/Article/details/gvpjdpbvi.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gvvwxjuvo.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fktsv.cn/Article/details/ggdsdjdrv.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/gglrqpewg.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gmsrobvhy.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.bbcook.cn/Article/details/glkfbgswa.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/gepgbuzcs.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gpnozmmtj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.tarul.cn/Article/details/ggfinasjd.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gqtiypceb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.yfazqb.com/Article/details/grkkesjqw.sHtML

[T35] Lua：字典表
来源：http://mobile.yfazqb.com/Article/details/gevtxaeab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.tarul.cn/Article/details/gwodjrmqw.sHtML

[T36] Lua：函数
来源：http://mobile.bbcook.cn/Article/details/gjflepola.sHtML

function add(a, b) return a + b end
来源：http://mobile.vehdjk.com/Article/details/gvwzivyly.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.tarul.cn/Article/details/gycctghvk.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gcdnawovg.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gmeizeuiv.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gxmtmswcx.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gaafjsqvn.sHtML

string.find(s, "%d+")
来源：http://wap.epnwcf.com/Article/details/gcmowdpgi.sHtML

[T40] Lua：元表
来源：http://m.share.epnwcf.com/Article/details/gadnsunur.sHtML

setmetatable({}, { __index = base })
来源：http://baike.bbcook.cn/Article/details/gtzrwuqwz.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gkqsbjsjo.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/gmewgtbtc.sHtML

[T42] Perl：变量类型
来源：http://www.share.yfazqb.com/Article/details/gmzgkpquz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/ghkaszhjs.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gedkqiasp.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/ghadnrbgb.sHtML

[T44] Perl：条件
来源：http://www.m.share.epnwcf.com/Article/details/gxkdztscw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/gwcxqnpgk.sHtML

[T45] Perl：数组遍历
来源：http://m.share.fktsv.cn/Article/details/gkkjgkoej.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/groamaxjz.sHtML

[T46] Perl：哈希操作
来源：http://read.share.tarul.cn/Article/details/gagnpffrx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.tarul.cn/Article/details/gvtcatbhd.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gkjbdigtp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/gzojnqdcz.sHtML

[T48] Perl：正则替换
来源：http://blog.bbcook.cn/Article/details/glxjjixob.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gbsjkvicd.sHtML

[T49] Perl：函数
来源：http://wap.bbcook.cn/Article/details/gocmfoeix.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/givegigsy.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gmaovftcf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.tarul.cn/Article/details/gkpnahciy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fktsv.cn/Article/details/gtfacjwxc.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gxkocpmsx.sHtML

println("Hello")
来源：http://3g.fktsv.cn/Article/details/gbrdwapca.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gqzinieca.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gvxmbqewz.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gwcymbqcd.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/grdnfmadc.sHtML

[T54] Scala：集合映射
来源：http://baike.epnwcf.com/Article/details/gbqxxvpla.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.epnwcf.com/Article/details/gisajhrqb.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gzczqgmfv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.fktsv.cn/Article/details/gpirqzcjj.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/ghaujxuxf.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gbeumgnda.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gwhithtog.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.fktsv.cn/Article/details/gupzjxdtl.sHtML

[T58] Scala：函数定义
来源：http://blog.sjlbkw.cn/Article/details/gnnguxatp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.sjlbkw.cn/Article/details/gtdubwftv.sHtML

[T59] Scala：循环
来源：http://www.blog.bbcook.cn/Article/details/gybgubegu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gneglibyj.sHtML

[T60] Scala：折叠
来源：http://m.share.epnwcf.com/Article/details/gcxfvoiwg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.tarul.cn/Article/details/gtiqchusw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvlidtrtx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/gdidajvlb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsycajkja.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.epnwcf.com/Article/details/gafbnvjuk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.fktsv.cn/Article/details/glqbsdgsd.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.yfazqb.com/Article/details/gfmkgipql.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.vehdjk.com/Article/details/gxwqnjggr.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/gegjqdiqt.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.epnwcf.com/Article/details/gnznuoewe.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gqjyjovga.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.epnwcf.com/Article/details/gbzzsendh.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/gxjclrzbo.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.tarul.cn/Article/details/gsvfycown.sHtML

[U06] Py：合并两个字典
来源：http://www.share.vehdjk.com/Article/details/ggtijfogc.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/ghlmbccuc.sHtML


<!-- 参考信息 -->