代发 wailian999

free -h;  ps aux | grep nginx
来源：http://3g.bbcook.cn/Article/details/gtwiwmrnm.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gfmtkrate.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.bbcook.cn/Article/details/grmatuowp.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gptidwvbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqngkpby.sHtML

[R66] 定时任务
来源：http://www.share.vehdjk.com/Article/details/gghvywnwy.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gusrvioub.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gcytxtxcz.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gogggbdaq.sHtML

[R68] 计算文件校验值
来源：http://www.share.yfazqb.com/Article/details/grudqybdp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/ghcyioxzh.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/givaowmhn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gqgfvkwwv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gqmrffwsz.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gieltiaxx.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/grdhnbxeq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gtnkosgcs.sHtML

[R72] 等待端口就绪
来源：http://baike.tarul.cn/Article/details/govbgdpog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/glsrsavfy.sHtML

[R73] 分割大日志
来源：http://3g.fktsv.cn/Article/details/gtbhhsrrc.sHtML

split -l 1000 big.log part_
来源：http://wap.fktsv.cn/Article/details/gtcmbgdub.sHtML

[R74] 批量重命名
来源：http://mobile.tarul.cn/Article/details/gcgqsbrmt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gfylirnkx.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gppzwrybt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gkofhxxvz.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/glzsxyens.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gzmwbbkpk.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/ggcthgoky.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gpfqinizs.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fktsv.cn/Article/details/gxkxvzapl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/gqqqzefyl.sHtML

[R79] 解析命令行选项
来源：http://read.share.bbcook.cn/Article/details/gnkbxcumv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.bbcook.cn/Article/details/ganriitln.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/glyrzurxf.sHtML

time ./run.sh
来源：http://blog.sjlbkw.cn/Article/details/gzarybbcn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goduuddqe.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/gusfxquzy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkvvnddzj.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gxzylqhnz.sHtML

#include <stdio.h>
来源：http://m.share.tarul.cn/Article/details/gkftkmehh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/guwwbfgde.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gmpykehaw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.vehdjk.com/Article/details/gmaezflwy.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gsxcfzpnl.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/globxazcx.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/ghxdsygvh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/giymfliyy.sHtML

[S05] C：字符串长度
来源：http://3g.vehdjk.com/Article/details/gtvkntpjn.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/galkexhpe.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/guvsomnpb.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gpjtrumct.sHtML

[S07] C：数组遍历求和
来源：http://3g.tarul.cn/Article/details/gpqbvdigf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.vehdjk.com/Article/details/ghmfcvmdx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gicipmdxg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.vehdjk.com/Article/details/gtrtfbxnk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.sjlbkw.cn/Article/details/gqamvkwva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/gjksqjycn.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gbhgzbrtd.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.vehdjk.com/Article/details/gulhjdnes.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gzljlsuil.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.vehdjk.com/Article/details/gxkuqgnsk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gtiqkbzzr.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gnyxfhtjr.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gufyucphd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/glvgfjtkr.sHtML

[S13] C：宏定义
来源：http://mobile.tarul.cn/Article/details/ghzdsppgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gvrwppcpw.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/gveftfnmm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.vehdjk.com/Article/details/grktmylka.sHtML

[S15] C：类型转换
来源：http://baike.fktsv.cn/Article/details/gfwobpxut.sHtML

(double) a / b
来源：http://www.m.share.vehdjk.com/Article/details/gxquexgwt.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gtkucmryn.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gwfhplver.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/gcwsghpld.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gicrffxqr.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gsujoelmo.sHtML

int main(int argc, char **argv)
来源：http://blog.vehdjk.com/Article/details/ghmalkzcj.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gzhrgjgzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.tarul.cn/Article/details/gzcmhuatp.sHtML

[S20] C：二分查找
来源：http://3g.sjlbkw.cn/Article/details/gyxpdurwa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gurrlmjzv.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/glbceuyuh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.vehdjk.com/Article/details/gtgpypthm.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gwbukvbpz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gyrtuvbne.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/goxizltfv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/ggoqagyvi.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gjaacdtzt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.vehdjk.com/Article/details/guangolvc.sHtML

[S25] C：内存拷贝
来源：http://3g.tarul.cn/Article/details/gojuxpjzd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.epnwcf.com/Article/details/geynjibuo.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gduwsmjaq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/grszkpbbb.sHtML

[S27] C：定义常量
来源：http://m.share.sjlbkw.cn/Article/details/gqdnscxzu.sHtML

const double PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gokxwnzdt.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/glofmskia.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/ghqnxtzlz.sHtML

[S29] C：变参函数
来源：http://blog.sjlbkw.cn/Article/details/gzbcbadkn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/gfpmcjpfn.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gljcopmfm.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/geifzpiqy.sHtML

#define X_H
来源：http://mobile.sjlbkw.cn/Article/details/gvptvbfbg.sHtML

#endif
来源：http://3g.fktsv.cn/Article/details/gnxfmdhoa.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/ggxfhkukw.sHtML

#include <iostream>
来源：http://read.share.fktsv.cn/Article/details/gtvsxbosi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/grhgzypmy.sHtML

[S32] C++：字符串
来源：http://3g.bbcook.cn/Article/details/gwffqxswp.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.vehdjk.com/Article/details/gqsndagyb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.sjlbkw.cn/Article/details/gdtlbxbdl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gvutsuysv.sHtML

[S34] C++：遍历 vector
来源：http://baike.bbcook.cn/Article/details/grcpjbgzg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gvybwpmeo.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/ghssavlcu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/guyqubniz.sHtML

[S36] C++：unordered_map
来源：http://read.share.vehdjk.com/Article/details/gbuijfgrn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gadgrcnbj.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gcjhnbsmn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.tarul.cn/Article/details/gwgtdaspq.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gmempdrfz.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.bbcook.cn/Article/details/gknjmjozc.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gorrpeyyu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gwxudpbbr.sHtML

[S40] C++：查找元素
来源：http://www.share.tarul.cn/Article/details/gqqatlwjn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gvoowuvvd.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/gzmjvqhuc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.epnwcf.com/Article/details/gtckhrayw.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gxarhsypu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gmgxpffpw.sHtML

[S43] C++：智能指针
来源：http://www.m.share.bbcook.cn/Article/details/gnilefcdw.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gaxaaizws.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gusugtvav.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.epnwcf.com/Article/details/gfdwpauuq.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gdbemcrpx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.epnwcf.com/Article/details/gyyxfdrzn.sHtML

[S46] C++：函数模板
来源：http://read.share.vehdjk.com/Article/details/gonrrgqrl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gqagsypuo.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.vehdjk.com/Article/details/ghhsowhlr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.epnwcf.com/Article/details/gasxmupwr.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gydsndhpj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/guiizmxub.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/ggtgemrjf.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gxtbzuopb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/gbbiakkrd.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gggsdjmld.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.bbcook.cn/Article/details/gsnkojmsk.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gjshepiye.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.vehdjk.com/Article/details/ghxocpieq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/gbfhvtcrb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.sjlbkw.cn/Article/details/gngsjsvdm.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/gdgpwqfzs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.sjlbkw.cn/Article/details/gkugarqdg.sHtML

[S54] C++：异常处理
来源：http://baike.sjlbkw.cn/Article/details/gwhuysdgq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gxtaohbka.sHtML

[S55] C++：结构化绑定
来源：http://mobile.yfazqb.com/Article/details/gmpiexufq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.vehdjk.com/Article/details/gvdazthky.sHtML

[S56] C++：optional
来源：http://wap.fktsv.cn/Article/details/gtxyccerq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.yfazqb.com/Article/details/grktifeig.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gcnthzcvx.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gjavvllow.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/guaarxhwk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.sjlbkw.cn/Article/details/ghonxwkgt.sHtML

[S59] C++：静态断言
来源：http://www.share.yfazqb.com/Article/details/gumcqiohr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/ghjlaqnff.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.bbcook.cn/Article/details/gdzvlfjrm.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.tarul.cn/Article/details/gzvmovgwk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmurylcbo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gzkcaqwng.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghramsefx.sHtML

[T01] Kotlin：Hello World
来源：http://blog.yfazqb.com/Article/details/gotuowvmg.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gllwislaa.sHtML

[T02] Kotlin：变量
来源：http://m.share.yfazqb.com/Article/details/ggdgfkhnu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.tarul.cn/Article/details/gkqvfhqwx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.bbcook.cn/Article/details/gohxknyob.sHtML

"值: $b"
来源：http://www.share.bbcook.cn/Article/details/gyfmjydpx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gdjrlfcai.sHtML

val n: String? = null;  n?.length
来源：http://read.share.vehdjk.com/Article/details/gvslipizs.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/gzipnyhht.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.sjlbkw.cn/Article/details/gklcrovuj.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.vehdjk.com/Article/details/gphszmyeh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqyuduev.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.bbcook.cn/Article/details/gudncards.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.bbcook.cn/Article/details/gkyvhoumh.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gwdfjigfu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.tarul.cn/Article/details/gndkxurhi.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.tarul.cn/Article/details/guyhjepmk.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gtmotkjuw.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gdysxbjct.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.bbcook.cn/Article/details/glzczaqbu.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/grccspwtm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gdhggloph.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gucyzckoq.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gvyrvexfd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvejcjld.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fktsv.cn/Article/details/grglxfhzu.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/glwcapqod.sHtML

for (i in 1..10) println(i)
来源：http://baike.vehdjk.com/Article/details/gfrmsapbp.sHtML

[T15] Kotlin：接口
来源：http://3g.epnwcf.com/Article/details/gumgxgyih.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/groinpsjc.sHtML

[T16] Swift：Hello World
来源：http://baike.epnwcf.com/Article/details/gwkbldywc.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/glecrozel.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/gmdabpxqi.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/glswprbnv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gqtyvtxzg.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gmjgnfbdc.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/giheqznxx.sHtML

if let n = opt { print(n) }
来源：http://blog.vehdjk.com/Article/details/gdbljcwbe.sHtML

[T20] Swift：数组操作
来源：http://blog.tarul.cn/Article/details/ggqolafbb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.sjlbkw.cn/Article/details/giwpaezjl.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/ghipwlxhi.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/geizmhvmw.sHtML

[T22] Swift：字典
来源：http://www.blog.tarul.cn/Article/details/gghwplwpx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/grdhtpkcx.sHtML

[T23] Swift：函数
来源：http://3g.yfazqb.com/Article/details/gxypanmfz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/goqbiydmd.sHtML

[T24] Swift：闭包
来源：http://wap.vehdjk.com/Article/details/ggecbwklk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.yfazqb.com/Article/details/gzxzcvena.sHtML

[T25] Swift：结构体
来源：http://mobile.fktsv.cn/Article/details/gfakvjgvn.sHtML

struct P { var x: Int }
来源：http://baike.tarul.cn/Article/details/gzvavllya.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gjscbtxod.sHtML

class A: Base { override func f() {} }
来源：http://3g.fktsv.cn/Article/details/gfhkunkiv.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gbhtqgavp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.yfazqb.com/Article/details/gbvabwrju.sHtML

[T28] Swift：枚举
来源：http://blog.epnwcf.com/Article/details/gcjvzlmoj.sHtML

enum Color { case red, green }
来源：http://www.m.share.sjlbkw.cn/Article/details/gphnibpwa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gqqdhobdp.sHtML

guard let x = opt else { return }
来源：http://www.m.share.bbcook.cn/Article/details/ggibgjcer.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gmuacusqo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.bbcook.cn/Article/details/gyxdkqrym.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gmmjezogv.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gqialiycd.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gvdzmuplo.sHtML

local a = 1
来源：http://www.blog.tarul.cn/Article/details/gddkhkwad.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gzhejqgfi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/gjlhngyih.sHtML

[T34] Lua：遍历表
来源：http://read.share.bbcook.cn/Article/details/gcfrudogq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gmboqwacb.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gtqgqvvqe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.vehdjk.com/Article/details/gcvxymlgs.sHtML

[T36] Lua：函数
来源：http://wap.vehdjk.com/Article/details/gbdqphygt.sHtML

function add(a, b) return a + b end
来源：http://blog.fktsv.cn/Article/details/gqxzhhupj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gdjrjfeyi.sHtML

"a" .. "b"
来源：http://read.share.sjlbkw.cn/Article/details/goqsrxwek.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/ggkuadlnn.sHtML

if x > 0 then print("正") end
来源：http://wap.sjlbkw.cn/Article/details/gzvjzwvxp.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/gdytniwlc.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gpgsnshjk.sHtML

[T40] Lua：元表
来源：http://www.m.share.fktsv.cn/Article/details/gbdygpwft.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gdpijilsv.sHtML

[T41] Perl：Hello World
来源：http://wap.epnwcf.com/Article/details/gewvrdefl.sHtML

print "Hello\n";
来源：http://www.share.bbcook.cn/Article/details/gdsvpzcyx.sHtML

[T42] Perl：变量类型
来源：http://mobile.bbcook.cn/Article/details/gezbanpzh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.vehdjk.com/Article/details/gbrfpsubp.sHtML

[T43] Perl：字符串插值
来源：http://3g.bbcook.cn/Article/details/gxbhjsumu.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/ghlfnlyan.sHtML

[T44] Perl：条件
来源：http://baike.vehdjk.com/Article/details/ghxzauiow.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gvrvwlvja.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gjxpzxtlw.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/gxbgsshyv.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.vehdjk.com/Article/details/gifccirzi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/ggqtuscay.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gyhrzwngt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/gwjfjrnqi.sHtML

[T48] Perl：正则替换
来源：http://m.share.sjlbkw.cn/Article/details/glrbcvpjd.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gyrblmxmb.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/ggpuyopoo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gaunmipwx.sHtML

[T50] Perl：逐行读文件
来源：http://blog.vehdjk.com/Article/details/glpjaduhz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fktsv.cn/Article/details/gckzxbfcu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.epnwcf.com/Article/details/gcdekobxo.sHtML

[T51] Scala：Hello World
来源：http://3g.epnwcf.com/Article/details/gyizacveh.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gqewjyeej.sHtML

[T52] Scala：变量
来源：http://m.share.epnwcf.com/Article/details/gsxabefod.sHtML

val a = 1;  var b = 2
来源：http://3g.fktsv.cn/Article/details/gjtkjrxfh.sHtML

[T53] Scala：字符串插值
来源：http://wap.epnwcf.com/Article/details/giqudeacv.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gvusunrsn.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/gnthzxpii.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.tarul.cn/Article/details/gqhhytqqc.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gaqmhuyvj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.bbcook.cn/Article/details/gciuyechd.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gtfscfkel.sHtML

case class User(name: String, age: Int)
来源：http://read.share.epnwcf.com/Article/details/gcmbqraqx.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gtsfbssgu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.bbcook.cn/Article/details/gobkifjqf.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/glndwmxwb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.bbcook.cn/Article/details/ggqsevhor.sHtML

[T59] Scala：循环
来源：http://www.m.share.yfazqb.com/Article/details/gfdzsatzz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.yfazqb.com/Article/details/guzyjibwp.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gtnkrbhky.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.vehdjk.com/Article/details/guvlecxnl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpenbvlgu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gsludkghz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gysogzvco.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/guassared.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.sjlbkw.cn/Article/details/gtjnklwni.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gpeaxxmwm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/ggcrtexnr.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/gdngaxdrx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.yfazqb.com/Article/details/gyitshkxp.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gyewjbxtn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.epnwcf.com/Article/details/gnmoowskt.sHtML


<!-- 参考信息 -->