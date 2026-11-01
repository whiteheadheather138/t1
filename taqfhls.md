代发 wailian999

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/gmmnvkvxl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.bbcook.cn/Article/details/gklkkeoxn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.vehdjk.com/Article/details/gkapgerkp.sHtML

[R69] 生成随机密码
来源：http://baike.epnwcf.com/Article/details/goeakammt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.vehdjk.com/Article/details/ghbjmqdqt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gpapdlgbo.sHtML

date +%s;  date -d @1700000000
来源：http://blog.sjlbkw.cn/Article/details/gjnoaugks.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gideflbjo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gpagzlgsm.sHtML

[R72] 等待端口就绪
来源：http://www.share.vehdjk.com/Article/details/gldanikfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gejyjirxa.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gptjmdbrt.sHtML

split -l 1000 big.log part_
来源：http://www.share.bbcook.cn/Article/details/gncjlrwjw.sHtML

[R74] 批量重命名
来源：http://3g.vehdjk.com/Article/details/gatiavoqt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.yfazqb.com/Article/details/gxehwffct.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gcqfehaxq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.epnwcf.com/Article/details/giywxezcr.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gkkflsswu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/glrfwcskq.sHtML

[R77] 读取用户输入
来源：http://m.share.sjlbkw.cn/Article/details/gfdclbdpv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/ghzuutjmz.sHtML

[R78] 交互式菜单
来源：http://wap.yfazqb.com/Article/details/ggegvbenp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gwkdwilkb.sHtML

[R79] 解析命令行选项
来源：http://blog.sjlbkw.cn/Article/details/gtnrqpqiv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.vehdjk.com/Article/details/gjsnyigub.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.bbcook.cn/Article/details/gcqrsyngk.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gpfstjxnw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghdwmbtuh.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gslprwnmn.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfzeewvmw.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gwbbbppnw.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/gblvhuyoe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.bbcook.cn/Article/details/gyuwmvbwj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gopxsxzff.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/giqzriclg.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gciiyqgli.sHtML

int x; scanf("%d", &x);
来源：http://www.share.sjlbkw.cn/Article/details/gbnbzhtij.sHtML

[S04] C：字符串复制
来源：http://www.m.share.bbcook.cn/Article/details/gqmsgwjeb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gfrkyuocp.sHtML

[S05] C：字符串长度
来源：http://3g.bbcook.cn/Article/details/gfvmzocyd.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gsrdnjzop.sHtML

[S06] C：字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gnlpvrguy.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/gnwdwjsfo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.tarul.cn/Article/details/gtkdvghef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/gkcalooss.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gcqjjceud.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.tarul.cn/Article/details/gemlwgzxc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.yfazqb.com/Article/details/gxreqgazd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fktsv.cn/Article/details/gzdxmkuvy.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/gnyqencoc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gxttmrlpx.sHtML

[S11] C：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gdgyokrzh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gtazxcagp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/govhbabop.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/ghbmgesen.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/grxztwsse.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gkvcaanlv.sHtML

[S13] C：宏定义
来源：http://3g.bbcook.cn/Article/details/glbgykcko.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.yfazqb.com/Article/details/gatdcpudz.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/glzbjupog.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.epnwcf.com/Article/details/gtbviczfa.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gmjpeobfl.sHtML

(double) a / b
来源：http://mobile.tarul.cn/Article/details/gmjuzfqdq.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/geazjdmic.sHtML

x |= (1 << 3);
来源：http://www.share.epnwcf.com/Article/details/gpqkahhvq.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gesnbcbsv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/gaazowwnj.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gpmamndkk.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/ggjtgfvwe.sHtML

[S19] C：快速排序
来源：http://www.blog.bbcook.cn/Article/details/glglpltzb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gwyzaixps.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/gwvztqlxq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gaiijvzsj.sHtML

[S21] C：字符类别判断
来源：http://www.share.epnwcf.com/Article/details/goqxpeehb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/gypwcbfsv.sHtML

[S22] C：字符串转数字
来源：http://read.share.bbcook.cn/Article/details/gsxgtoiec.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gqewkzgza.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gmdxbhcqe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.sjlbkw.cn/Article/details/ggrgcidvz.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/grmuqmzlv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gvyqnrqtr.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gouruheow.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/gbmlrzpxq.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gqcdpwzvy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.vehdjk.com/Article/details/gordbbrns.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gmlgirupd.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gbkavmudq.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gzdjoirvl.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gmhfpyrtg.sHtML

[S29] C：变参函数
来源：http://mobile.fktsv.cn/Article/details/gsqwaydxz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gwmwmlaar.sHtML

[S30] C：头文件保护
来源：http://read.share.epnwcf.com/Article/details/gixekhsvc.sHtML

#ifndef X_H
来源：http://mobile.epnwcf.com/Article/details/gzokrgxvz.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gfxrynbfi.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gpbiouzrq.sHtML

[S31] C++：Hello World
来源：http://m.share.tarul.cn/Article/details/gpacgzjkw.sHtML

#include <iostream>
来源：http://3g.fktsv.cn/Article/details/gzutmbkvd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.tarul.cn/Article/details/gmsgtpcoh.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjwgfkdoi.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/glibugxhm.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gissplpza.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gkqfvdfzy.sHtML

[S34] C++：遍历 vector
来源：http://baike.epnwcf.com/Article/details/gnvktikiv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjsumzfn.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gqtgyoqzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/glzfeseap.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gshooodma.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gpcilmlhe.sHtML

[S37] C++：set
来源：http://baike.fktsv.cn/Article/details/gjumedktp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.sjlbkw.cn/Article/details/gwyxgtycq.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/gwmtkikmi.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fktsv.cn/Article/details/grjlqykvr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gpaybkltl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/glhujmqbw.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/gelbhhqeb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gnpialmja.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fktsv.cn/Article/details/gbqjifpgk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.bbcook.cn/Article/details/gvpuztyre.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/grgvvayom.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.bbcook.cn/Article/details/gfeetdycu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gwpkakadl.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.yfazqb.com/Article/details/gltxxonpa.sHtML

[S44] C++：引用传参
来源：http://m.share.bbcook.cn/Article/details/grwtxpwfi.sHtML

void inc(int &x) { ++x; }
来源：http://baike.yfazqb.com/Article/details/gjtutoevs.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/ghtirxzaz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.yfazqb.com/Article/details/gswqczaup.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gonnmqqbj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/glfvlfcfu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.yfazqb.com/Article/details/gktrrukch.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gsyrjdcnl.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gopkelncz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/ghwvyvtic.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.tarul.cn/Article/details/gvojzgxmg.sHtML

[S49] C++：写文件
来源：http://www.share.vehdjk.com/Article/details/goekqeqhy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.epnwcf.com/Article/details/gvlaneguj.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gztborflb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gtkbmqfvz.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.vehdjk.com/Article/details/gccmdmrta.sHtML

static_cast<double>(a) / b
来源：http://wap.sjlbkw.cn/Article/details/gpihsainy.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.tarul.cn/Article/details/gzgxavjwh.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gtqkbuanq.sHtML

[S53] C++：移动语义
来源：http://3g.tarul.cn/Article/details/gnyotwhqk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fktsv.cn/Article/details/gxagyhnzp.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gorgukyjh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.vehdjk.com/Article/details/gihelvobq.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gaeqvajth.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gtvzvlkwu.sHtML

[S56] C++：optional
来源：http://blog.tarul.cn/Article/details/gxtoniljl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gfvbwwzhr.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gwsjmjodt.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/godbssmad.sHtML

[S58] C++：命名空间
来源：http://m.share.yfazqb.com/Article/details/gzbwiopft.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gotxqzdrv.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gljsubtud.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fktsv.cn/Article/details/ghexljpxf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/gwgpmohat.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/gtzukeyfa.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghivwthuh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/glztdmkla.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggpmkjaep.sHtML

[T01] Kotlin：Hello World
来源：http://baike.bbcook.cn/Article/details/gczljngkl.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/grfkuvtqx.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gwvhoipby.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fktsv.cn/Article/details/gsfbdykyx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.bbcook.cn/Article/details/gkwqywavg.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gyrvnhwdc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gnbdukjmg.sHtML

val n: String? = null;  n?.length
来源：http://3g.tarul.cn/Article/details/gqrsgvyjb.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gvbidqcbd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.tarul.cn/Article/details/guwjlcgyd.sHtML

[T06] Kotlin：集合映射
来源：http://baike.epnwcf.com/Article/details/gqmmcddlv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.bbcook.cn/Article/details/gupmupoer.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gvsrkjyug.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.tarul.cn/Article/details/grgzfpuzw.sHtML

[T08] Kotlin：数据类
来源：http://blog.bbcook.cn/Article/details/gqaysyyne.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gydhkunaj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gzwvnltop.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fktsv.cn/Article/details/gdgudcnmt.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gpifyxmuh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/gbywjpldr.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/grwxiomca.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.tarul.cn/Article/details/glitgiprf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fktsv.cn/Article/details/grkdkdjdu.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.tarul.cn/Article/details/ggaqgqhnq.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.tarul.cn/Article/details/ghzklmken.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwilzpyrv.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/ghyvadmlz.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gyznezuwd.sHtML

[T15] Kotlin：接口
来源：http://mobile.fktsv.cn/Article/details/ghozvvezf.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.bbcook.cn/Article/details/guprcglvo.sHtML

[T16] Swift：Hello World
来源：http://baike.fktsv.cn/Article/details/gcwxbwpog.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/ggxvqlecs.sHtML

[T17] Swift：变量与常量
来源：http://3g.vehdjk.com/Article/details/gholmjkyf.sHtML

var a = 1;  let b = 2
来源：http://baike.tarul.cn/Article/details/gjgirsozk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gqxgrjkfs.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gcehmucol.sHtML

[T19] Swift：可选绑定
来源：http://baike.yfazqb.com/Article/details/gqoqfhmmd.sHtML

if let n = opt { print(n) }
来源：http://baike.vehdjk.com/Article/details/gdogfebpm.sHtML

[T20] Swift：数组操作
来源：http://www.share.bbcook.cn/Article/details/geharblou.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gxfklcrle.sHtML

[T21] Swift：遍历
来源：http://www.share.tarul.cn/Article/details/glaxhcwaq.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/gsjyrcpdq.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/glaqnuied.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.vehdjk.com/Article/details/gnogvarjx.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/goheaefgk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gktrgatlh.sHtML

[T24] Swift：闭包
来源：http://wap.sjlbkw.cn/Article/details/gffvmczkb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gwgzeuquf.sHtML

[T25] Swift：结构体
来源：http://read.share.fktsv.cn/Article/details/geyaztsks.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gpitopcvt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/gutahnfti.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/gdxntqjiz.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/glzdiogjp.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.epnwcf.com/Article/details/gzbftiugx.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/gvjuouexv.sHtML

enum Color { case red, green }
来源：http://3g.vehdjk.com/Article/details/gwdjokydi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.epnwcf.com/Article/details/gepghbxum.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/gupmjytnt.sHtML

[T30] Swift：协议
来源：http://baike.sjlbkw.cn/Article/details/gtetotskf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/ggbtqsoiv.sHtML

[T31] Lua：Hello World
来源：http://wap.fktsv.cn/Article/details/grbttagsu.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gwbjctzwv.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gipyhfomg.sHtML

local a = 1
来源：http://read.share.fktsv.cn/Article/details/ggphdbpqo.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzqouxku.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gzgelzrzm.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gvuagvjed.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gqznpfcsn.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gfijashqz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.fktsv.cn/Article/details/gxmrikpdg.sHtML

[T36] Lua：函数
来源：http://3g.epnwcf.com/Article/details/gosljoquk.sHtML

function add(a, b) return a + b end
来源：http://blog.epnwcf.com/Article/details/gxvxgrccu.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/geawitbcm.sHtML

"a" .. "b"
来源：http://mobile.tarul.cn/Article/details/gchpamzsx.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gmgxklqcj.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gqgqylfpq.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/gwsvtqdpf.sHtML

string.find(s, "%d+")
来源：http://wap.yfazqb.com/Article/details/gykleiwne.sHtML

[T40] Lua：元表
来源：http://www.m.share.epnwcf.com/Article/details/gyvhqplyz.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gelxhfjgi.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gqqjxnqnb.sHtML

print "Hello\n";
来源：http://www.share.fktsv.cn/Article/details/gltwqynyf.sHtML

[T42] Perl：变量类型
来源：http://blog.bbcook.cn/Article/details/guacpjwpx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.bbcook.cn/Article/details/gzuawbuqq.sHtML

[T43] Perl：字符串插值
来源：http://m.share.tarul.cn/Article/details/ggisvapgj.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gsvoduxft.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gwanyqldl.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/ghabdsfyr.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gtauqafgk.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fktsv.cn/Article/details/gooyjezyx.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/guumudddr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gcjcwercm.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gqekjfnhc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.tarul.cn/Article/details/grehcrrec.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gpsheavdh.sHtML

$s =~ s/old/new/g;
来源：http://wap.vehdjk.com/Article/details/gpyhlcbtr.sHtML

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/giywlabqi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.bbcook.cn/Article/details/gdagiehvp.sHtML

[T50] Perl：逐行读文件
来源：http://blog.tarul.cn/Article/details/gcjbebrxh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gobgfzzlk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gyusxupti.sHtML

[T51] Scala：Hello World
来源：http://www.share.vehdjk.com/Article/details/gcxncvsba.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gfjjjicnc.sHtML

[T52] Scala：变量
来源：http://www.m.share.vehdjk.com/Article/details/gplnmzcjn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gudqdznvd.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/ggrbqxdfo.sHtML

s"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gyzygbwir.sHtML

[T54] Scala：集合映射
来源：http://m.share.tarul.cn/Article/details/gojxozytp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.epnwcf.com/Article/details/grtlgaiki.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gqeguciau.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gmvtevabr.sHtML

[T56] Scala：样例类
来源：http://www.m.share.tarul.cn/Article/details/gtqwsevjd.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gewwhhfyl.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gnmqbirtv.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gqoexwrlt.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwsjeyfv.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgrcwroq.sHtML

[T59] Scala：循环
来源：http://blog.tarul.cn/Article/details/gathlvzgm.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gdjrzurcu.sHtML

[T60] Scala：折叠
来源：http://www.m.share.vehdjk.com/Article/details/gcxrnowic.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.bbcook.cn/Article/details/gxexdlfhw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjobektzs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpjhixpig.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvgofpmcc.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsamexcp.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/gmefogeyj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gzpjzhxrl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gdgxumnvw.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.fktsv.cn/Article/details/gmsnrdlqx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.blog.yfazqb.com/Article/details/gcesjqrfb.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/ghkhbchjj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.yfazqb.com/Article/details/gsmptsiur.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gniididtw.sHtML

list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gobfcdpdu.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.vehdjk.com/Article/details/ghgppnlyz.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gbhvgwmjv.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gkpaminoj.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gygvaldio.sHtML

[U08] Py：展平二维列表
来源：http://3g.bbcook.cn/Article/details/gszycnkqn.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gkxscszjb.sHtML


<!-- 参考信息 -->