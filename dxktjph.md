代发 wailian999

df -h;  du -sh *
来源：http://www.share.vehdjk.com/Article/details/grbddqlsc.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gdaaeiuoc.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gmbozohac.sHtML

[R63] 内存与进程
来源：http://mobile.sjlbkw.cn/Article/details/gabpygevq.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.yfazqb.com/Article/details/gwpdiaxia.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gkqumsqdx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.yfazqb.com/Article/details/gosfjalub.sHtML

[R65] 查看端口占用
来源：http://www.blog.bbcook.cn/Article/details/ghgnqdmii.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.epnwcf.com/Article/details/ggkvulozy.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gkiagsxtl.sHtML

crontab -e;  crontab -l
来源：http://3g.bbcook.cn/Article/details/gmyrnahup.sHtML

[R67] 生成随机十六进制串
来源：http://3g.yfazqb.com/Article/details/gqqaihqwm.sHtML

openssl rand -hex 16
来源：http://blog.epnwcf.com/Article/details/gljhnolma.sHtML

[R68] 计算文件校验值
来源：http://wap.fktsv.cn/Article/details/gktsusxyf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.yfazqb.com/Article/details/golsedcxd.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gvvfuybqm.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gxjkecczj.sHtML

[R70] 时间戳与互转
来源：http://mobile.yfazqb.com/Article/details/ggwflxjvn.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fktsv.cn/Article/details/gdomsshuq.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gzthmlyav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.tarul.cn/Article/details/gttylefpv.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/ghjlztebb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gvnwydcow.sHtML

[R73] 分割大日志
来源：http://m.share.vehdjk.com/Article/details/gfmgxwzno.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/ggpqnirzn.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/goalprfgc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.vehdjk.com/Article/details/gmmgmojwi.sHtML

[R75] 导出环境变量
来源：http://baike.epnwcf.com/Article/details/gafwcutwk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.vehdjk.com/Article/details/gslovvipk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gxdfvrziu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/ggzvkfafi.sHtML

[R77] 读取用户输入
来源：http://baike.bbcook.cn/Article/details/gbypygpgm.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gduljtxrc.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gjtloljzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gjsxbnajn.sHtML

[R79] 解析命令行选项
来源：http://3g.sjlbkw.cn/Article/details/glwbtfelj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.sjlbkw.cn/Article/details/gyqxszqje.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gdahdcmic.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gyorcnzrs.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqpdczwtp.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/ghgbbudor.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzphqbruv.sHtML

[S01] C：Hello World
来源：http://3g.sjlbkw.cn/Article/details/gkpzfamfh.sHtML

#include <stdio.h>
来源：http://wap.sjlbkw.cn/Article/details/ghroprcgz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gqazkbwka.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gqugbctin.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gvfbporsn.sHtML

[S03] C：读入整数
来源：http://read.share.vehdjk.com/Article/details/gshbeqtii.sHtML

int x; scanf("%d", &x);
来源：http://wap.sjlbkw.cn/Article/details/gmmrqyivf.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gdbyjlbzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/ggbigxvlb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gzdrfkqhp.sHtML

strlen(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsnyexlsm.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gysfkgkss.sHtML

strcmp(a, b) == 0
来源：http://www.share.tarul.cn/Article/details/gyrjzxcmy.sHtML

[S07] C：数组遍历求和
来源：http://read.share.bbcook.cn/Article/details/gggbgmvph.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.tarul.cn/Article/details/gedrtcmgb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.yfazqb.com/Article/details/gdxgdpfcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.vehdjk.com/Article/details/gqbqwknvu.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gpxnxcsjh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.bbcook.cn/Article/details/gobzgumls.sHtML

[S10] C：指针与解引用
来源：http://read.share.sjlbkw.cn/Article/details/gzxvlaadc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/glbfswvjo.sHtML

[S11] C：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gaqzvvord.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gtgncqygi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gwtqonuxz.sHtML

fclose(f);
来源：http://3g.tarul.cn/Article/details/gpesqdsyo.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/grurzoppz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/geznlglip.sHtML

[S13] C：宏定义
来源：http://3g.vehdjk.com/Article/details/gamjmpmtj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/gawoiqppn.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gcjqwlfyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gcqvetadp.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/ggutvriqm.sHtML

(double) a / b
来源：http://mobile.bbcook.cn/Article/details/gtscbpkdv.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/ggdcjmczg.sHtML

x |= (1 << 3);
来源：http://www.m.share.epnwcf.com/Article/details/gsqnkxwcu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gvbynnrxz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fktsv.cn/Article/details/guhvalzzb.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gdnjiowei.sHtML

int main(int argc, char **argv)
来源：http://baike.fktsv.cn/Article/details/gsbqbznja.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/gnweivojt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/galkiioaa.sHtML

[S20] C：二分查找
来源：http://www.share.epnwcf.com/Article/details/gxdlpneme.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gvogblxga.sHtML

[S21] C：字符类别判断
来源：http://m.share.sjlbkw.cn/Article/details/gclefxhoe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.sjlbkw.cn/Article/details/gugwppgup.sHtML

[S22] C：字符串转数字
来源：http://read.share.tarul.cn/Article/details/ghuevxaxy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.sjlbkw.cn/Article/details/grprafoyn.sHtML

[S23] C：随机数
来源：http://wap.bbcook.cn/Article/details/gpmscqwkt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.epnwcf.com/Article/details/gqwfjlgha.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrsishpm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gyxvjcwui.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gnhjyvekx.sHtML

memcpy(dst, src, n);
来源：http://baike.tarul.cn/Article/details/gfxfrigbg.sHtML

[S26] C：内存清零
来源：http://wap.bbcook.cn/Article/details/gqkaegbgq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/ghkzynvwl.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gqsjoxpef.sHtML

const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gtroevpdg.sHtML

[S28] C：静态变量
来源：http://mobile.vehdjk.com/Article/details/gokaexolx.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/glmqpggmg.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gvwafainm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gjhussqdp.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gywprrhev.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gkllulvwr.sHtML

#define X_H
来源：http://wap.fktsv.cn/Article/details/gsnxphkvw.sHtML

#endif
来源：http://www.m.share.vehdjk.com/Article/details/gbqemawuv.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gtcmwtizi.sHtML

#include <iostream>
来源：http://wap.tarul.cn/Article/details/gfcqsjrpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gbbxywukd.sHtML

[S32] C++：字符串
来源：http://www.share.tarul.cn/Article/details/gkdqzswhe.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gwvhwprbg.sHtML

[S33] C++：vector 增删
来源：http://blog.bbcook.cn/Article/details/ghplkthkr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gjzbiteaz.sHtML

[S34] C++：遍历 vector
来源：http://m.share.tarul.cn/Article/details/gswwsbofi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gbnvdiwmg.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/giyiybzcn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gbhtfbdtj.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gmcwkoqkt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/giklxqolf.sHtML

[S37] C++：set
来源：http://blog.sjlbkw.cn/Article/details/gieajzjht.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gnvjthwuu.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/grfxzezoy.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.sjlbkw.cn/Article/details/guyxlhazp.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/gmwjsgxdq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/guwzmsbdg.sHtML

[S40] C++：查找元素
来源：http://3g.tarul.cn/Article/details/gdfklqglo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gtqhnqdoj.sHtML

[S41] C++：类与构造函数
来源：http://blog.yfazqb.com/Article/details/gdiatvmif.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.yfazqb.com/Article/details/gqxdzidkc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.tarul.cn/Article/details/gfrhdswcc.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gfztwmpla.sHtML

[S43] C++：智能指针
来源：http://3g.epnwcf.com/Article/details/gmhpzdjom.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/grizdycgs.sHtML

[S44] C++：引用传参
来源：http://blog.fktsv.cn/Article/details/gcdgsjkry.sHtML

void inc(int &x) { ++x; }
来源：http://wap.sjlbkw.cn/Article/details/gykftniuz.sHtML

[S45] C++：lambda
来源：http://www.m.share.epnwcf.com/Article/details/ggzxkvzwd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.tarul.cn/Article/details/gvpbflzuf.sHtML

[S46] C++：函数模板
来源：http://www.m.share.tarul.cn/Article/details/gmzmnozmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.epnwcf.com/Article/details/gckxwnpcy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.epnwcf.com/Article/details/gcafpvbwd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.tarul.cn/Article/details/gzmwfjrly.sHtML

[S48] C++：逐行读文件
来源：http://3g.tarul.cn/Article/details/gkxzpulcp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gzpigftrk.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.epnwcf.com/Article/details/gttpkogea.sHtML

[S49] C++：写文件
来源：http://mobile.tarul.cn/Article/details/gakoqjbeo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.sjlbkw.cn/Article/details/gfjjmgdck.sHtML

[S50] C++：格式化数字
来源：http://wap.sjlbkw.cn/Article/details/gzsixoasz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gcyoxytfk.sHtML

[S51] C++：显式类型转换
来源：http://wap.bbcook.cn/Article/details/gawtqffsn.sHtML

static_cast<double>(a) / b
来源：http://baike.epnwcf.com/Article/details/gxlvonfbg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gvfvjsavj.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gesgblvie.sHtML

[S53] C++：移动语义
来源：http://www.share.sjlbkw.cn/Article/details/gvjrgdayn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fktsv.cn/Article/details/gkozqhead.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/gekvnatzy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/grfzeomeg.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gyclbrnui.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.bbcook.cn/Article/details/gevrilnkl.sHtML

[S56] C++：optional
来源：http://www.m.share.sjlbkw.cn/Article/details/gwllnlmoj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/glifzfmmg.sHtML

[S57] C++：编译期常量
来源：http://3g.fktsv.cn/Article/details/gqnrgfgkg.sHtML

constexpr int N = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gxgorgxbb.sHtML

[S58] C++：命名空间
来源：http://3g.yfazqb.com/Article/details/glqbnhkcl.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.sjlbkw.cn/Article/details/getvssvnk.sHtML

[S59] C++：静态断言
来源：http://blog.tarul.cn/Article/details/gnjebpsie.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/girfeaiia.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gbntnmkzf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fktsv.cn/Article/details/ggbxpptzz.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdwypfozq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gberlaqzw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpqxeyybo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gxwhqzbmx.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/glpndogcy.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gdanpvmor.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/gxfonslob.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/givwfendg.sHtML

"值: $b"
来源：http://wap.yfazqb.com/Article/details/gucuijsnm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.vehdjk.com/Article/details/gfoworuit.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gzfqwmonh.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gnbxgxsqn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/gjsforzco.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.sjlbkw.cn/Article/details/gljqgbzpp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gbyimokyw.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gdwckjmpo.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fktsv.cn/Article/details/gcgvgjlkw.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gtpzmxuxm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.epnwcf.com/Article/details/gmjrmvejm.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.vehdjk.com/Article/details/grcdjdxwi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gqjdkpwfc.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fktsv.cn/Article/details/gxlagubcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fktsv.cn/Article/details/gdodgxjje.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gtlwrwdds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/gacouxvuw.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fktsv.cn/Article/details/guzkzzrea.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gkoanwrlo.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gqalfhval.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.vehdjk.com/Article/details/gueqaywjl.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gpkoxipjn.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gtnxsefhe.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.sjlbkw.cn/Article/details/gczhvdugd.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.bbcook.cn/Article/details/gmxxqluvj.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/grgjdzoxm.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/glicqabha.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gpucojxvh.sHtML

var a = 1;  let b = 2
来源：http://blog.vehdjk.com/Article/details/gxtabqpbw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gmffbazbd.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gfssrsacp.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fktsv.cn/Article/details/gjyrsmasz.sHtML

if let n = opt { print(n) }
来源：http://mobile.bbcook.cn/Article/details/geintawnk.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gghmivroh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.vehdjk.com/Article/details/gchtasywm.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gmsngahxi.sHtML

for x in a { print(x) }
来源：http://www.m.share.yfazqb.com/Article/details/grltopjee.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gmktepkqh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gfecxiwju.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gkhypmjxm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.epnwcf.com/Article/details/gfehkrxrt.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/ghmihwbpw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gwckvxrod.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/gtajbzvtb.sHtML

struct P { var x: Int }
来源：http://m.share.sjlbkw.cn/Article/details/gykxsnuva.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpllwzpm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gquxgulnh.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gbdauplaz.sHtML

do { try f() } catch { print(error) }
来源：http://blog.epnwcf.com/Article/details/gkyilqnyp.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/geoyyrdfx.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/garpvretn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/guuhmuheh.sHtML

guard let x = opt else { return }
来源：http://www.m.share.epnwcf.com/Article/details/gbniismrp.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gmrnyucvn.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.bbcook.cn/Article/details/gthufbqjt.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gmyotgyfq.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gzoafhloq.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/gavjhmuib.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gifwcjdzi.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/guxxngfpk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gqtaktnjs.sHtML

[T34] Lua：遍历表
来源：http://blog.bbcook.cn/Article/details/gncglhnft.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gisomnelb.sHtML

[T35] Lua：字典表
来源：http://wap.tarul.cn/Article/details/grsjbokdv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.tarul.cn/Article/details/gxbocidfh.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/guvtinneh.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gwgpqbusm.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gtcyrtbva.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gmqhibkrc.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/glhtxvxqi.sHtML

if x > 0 then print("正") end
来源：http://mobile.fktsv.cn/Article/details/gaimicqin.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gxxblxgmo.sHtML

string.find(s, "%d+")
来源：http://mobile.epnwcf.com/Article/details/gvtinkqre.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/gqiljcdym.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/gpeclstyl.sHtML

[T41] Perl：Hello World
来源：http://mobile.vehdjk.com/Article/details/gqbatreia.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gxasdawkw.sHtML

[T42] Perl：变量类型
来源：http://mobile.tarul.cn/Article/details/ghrqrspse.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.sjlbkw.cn/Article/details/gjridjqvz.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/gfuqoswmi.sHtML

"值: $a"
来源：http://www.blog.sjlbkw.cn/Article/details/gqgivpyvu.sHtML

[T44] Perl：条件
来源：http://wap.epnwcf.com/Article/details/gkvwhzrao.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gfltuzpvr.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gyczecsvp.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.fktsv.cn/Article/details/gofeduxlz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gzewcbrrb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.yfazqb.com/Article/details/glnnecyru.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gksphunfp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxohazcq.sHtML

[T48] Perl：正则替换
来源：http://mobile.tarul.cn/Article/details/ghaxxwjkp.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/gfvpmibru.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gxpdvhiqe.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/ggeiswcax.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gtfvxqwdz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gyxjtxlxo.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gwtrvwfho.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gtdhjojti.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/guzcmmllo.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gmqjqgtnr.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gipgivlly.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gkjgqyyoq.sHtML

s"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gewhvotgt.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gixlgmlpy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.tarul.cn/Article/details/grbyewrwi.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/girqpqmvy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.vehdjk.com/Article/details/grasgwocd.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gvdhgnbwz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.sjlbkw.cn/Article/details/gxifublrf.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/geipyhgcr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/gybjsefhy.sHtML

[T58] Scala：函数定义
来源：http://blog.vehdjk.com/Article/details/gilnrwrgs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gwyajcqwx.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gwfltakik.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/ggjxloxze.sHtML

[T60] Scala：折叠
来源：http://read.share.yfazqb.com/Article/details/gvslvngcu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gvxwuvink.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghovmhmeb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gumutzill.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxmqczzbt.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gwaqjghkx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.bbcook.cn/Article/details/gtmcoputf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.tarul.cn/Article/details/gkephrnyw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.sjlbkw.cn/Article/details/gsrykpumy.sHtML


<!-- 参考信息 -->