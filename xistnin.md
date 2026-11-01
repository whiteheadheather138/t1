代发 wailian999

openssl rand -hex 16
来源：http://mobile.vehdjk.com/Article/details/gfoxkbvaa.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gxhaczokc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.yfazqb.com/Article/details/gxhcfxmyi.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/grqizwhsh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/gbspiumgm.sHtML

[R70] 时间戳与互转
来源：http://blog.yfazqb.com/Article/details/gnhnmrdse.sHtML

date +%s;  date -d @1700000000
来源：http://wap.yfazqb.com/Article/details/gfgpjqvmh.sHtML

[R71] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/ghjjabxsi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gviqjahwv.sHtML

[R72] 等待端口就绪
来源：http://mobile.yfazqb.com/Article/details/gokfdpbgq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gyolxsnrt.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gwrpajamp.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gwaaeqmah.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/guvlnmsec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fktsv.cn/Article/details/gbcoeyeli.sHtML

[R75] 导出环境变量
来源：http://mobile.vehdjk.com/Article/details/gztstrgef.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.bbcook.cn/Article/details/gjlbohwxp.sHtML

[R76] 使用临时文件
来源：http://read.share.epnwcf.com/Article/details/gbteacmxy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.sjlbkw.cn/Article/details/gyazvoyso.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gyrjbnzsr.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/groczikkg.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gxvzewdho.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/goaorshbz.sHtML

[R79] 解析命令行选项
来源：http://baike.bbcook.cn/Article/details/gevqmnrai.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.yfazqb.com/Article/details/gxaobnhhv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.vehdjk.com/Article/details/gmklttfxs.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/grhesamxa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbaexuugt.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gatzjodub.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/godorwzmn.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gczgqwhyc.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gvkkbenwp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.sjlbkw.cn/Article/details/gwnrwcfvw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gbpukckil.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.vehdjk.com/Article/details/gpuycxewp.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gzbokusqo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gybdudcof.sHtML

[S04] C：字符串复制
来源：http://m.share.sjlbkw.cn/Article/details/gtwfhbspd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.sjlbkw.cn/Article/details/glbbyodib.sHtML

[S05] C：字符串长度
来源：http://blog.yfazqb.com/Article/details/gprywjemv.sHtML

strlen(s)
来源：http://wap.vehdjk.com/Article/details/gszowbjsb.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gmhylomgt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fktsv.cn/Article/details/ghjjrlxgn.sHtML

[S07] C：数组遍历求和
来源：http://blog.tarul.cn/Article/details/glhjkmlwh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gjslrbsmw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gsztpmjmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.epnwcf.com/Article/details/gzgwryjem.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.yfazqb.com/Article/details/gukcxsiui.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.epnwcf.com/Article/details/goteqoxyk.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/gbmjzotas.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gcyeksusc.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gakpkkxsp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fktsv.cn/Article/details/gndcfthtq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.yfazqb.com/Article/details/guruisndt.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gmmimwdeo.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/gcthcfakq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gplvwnkgg.sHtML

[S13] C：宏定义
来源：http://3g.yfazqb.com/Article/details/giicordfo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.sjlbkw.cn/Article/details/gewijmldr.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gmchkxhuw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/gyrxobunw.sHtML

[S15] C：类型转换
来源：http://3g.yfazqb.com/Article/details/gmiyznfrd.sHtML

(double) a / b
来源：http://www.blog.bbcook.cn/Article/details/gbdkrwqyq.sHtML

[S16] C：位操作置位
来源：http://www.blog.epnwcf.com/Article/details/ghppiuwov.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gudtcjsab.sHtML

[S17] C：安全拼接字符串
来源：http://blog.vehdjk.com/Article/details/gfhlcijcv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.bbcook.cn/Article/details/grpyumgup.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/guymtvhfr.sHtML

int main(int argc, char **argv)
来源：http://mobile.sjlbkw.cn/Article/details/gamenvmzx.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/guaaovinh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gvnosjtfb.sHtML

[S20] C：二分查找
来源：http://baike.epnwcf.com/Article/details/gyxeuoiom.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.tarul.cn/Article/details/gekziupyt.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gdsurlluf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gcgoycseg.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/ggtqjlcbq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gjkgsbexj.sHtML

[S23] C：随机数
来源：http://blog.yfazqb.com/Article/details/gtcjmsbeo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/genxntscv.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gouoslhoc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gibmzpzbn.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.tarul.cn/Article/details/gvqpaezkm.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gbelkwqmb.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gqybjjhdi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.bbcook.cn/Article/details/ggfrizgbj.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gcqurqgxh.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gqdhuqzkn.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gxchintne.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gvpdszprw.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gjvuyzbbj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.tarul.cn/Article/details/gjnaurtcm.sHtML

[S30] C：头文件保护
来源：http://read.share.tarul.cn/Article/details/gpfuvnnqs.sHtML

#ifndef X_H
来源：http://www.share.vehdjk.com/Article/details/getdhysbm.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gvahnsyub.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gzctpplsn.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gjhvgqqcs.sHtML

#include <iostream>
来源：http://www.share.vehdjk.com/Article/details/gmagoqkqp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gilsawwkv.sHtML

[S32] C++：字符串
来源：http://mobile.vehdjk.com/Article/details/gyvkbkfbf.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gvedlxfjs.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/ggagwvugt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gijrgzykp.sHtML

[S34] C++：遍历 vector
来源：http://mobile.yfazqb.com/Article/details/gyausamgh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/ggbmhutcc.sHtML

[S35] C++：map
来源：http://baike.bbcook.cn/Article/details/gamfhzdfn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gwbhtegsg.sHtML

[S36] C++：unordered_map
来源：http://read.share.fktsv.cn/Article/details/gdwhsfwsp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gtvdukaug.sHtML

[S37] C++：set
来源：http://m.share.fktsv.cn/Article/details/grdgzbmnm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gnyftdthe.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gxjtranmd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/getmrlswk.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gruuwicxc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.sjlbkw.cn/Article/details/gyyobalnr.sHtML

[S40] C++：查找元素
来源：http://m.share.sjlbkw.cn/Article/details/gfufuducq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gtfpomjfn.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gskflagdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gubbopfmp.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gcxdfmdsu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.bbcook.cn/Article/details/gjejkrmcp.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/goryajoko.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.vehdjk.com/Article/details/geansyocv.sHtML

[S44] C++：引用传参
来源：http://read.share.vehdjk.com/Article/details/gxntwqsdc.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fktsv.cn/Article/details/guuohsnyq.sHtML

[S45] C++：lambda
来源：http://www.m.share.fktsv.cn/Article/details/gbziqprkt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gfzduhrgi.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gokmtvhqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.vehdjk.com/Article/details/gnyyvjlng.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/gbtcdqghk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gfsifdvbo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gpnrzuvan.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/ggdiduszq.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.bbcook.cn/Article/details/gxtrrxkat.sHtML

[S49] C++：写文件
来源：http://mobile.bbcook.cn/Article/details/gjatkxnls.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fktsv.cn/Article/details/gracyjmoo.sHtML

[S50] C++：格式化数字
来源：http://3g.bbcook.cn/Article/details/gqmpmxuee.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gsipbpibc.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/ghdsyhbuy.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gdzmxkqag.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.bbcook.cn/Article/details/gpuwheqih.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.tarul.cn/Article/details/gepbtpxpb.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gddionkvq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.bbcook.cn/Article/details/gfyhpbybv.sHtML

[S54] C++：异常处理
来源：http://m.share.vehdjk.com/Article/details/gbyamuruk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/gmcgxxqax.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.vehdjk.com/Article/details/gcluetxcv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fktsv.cn/Article/details/gonddcmte.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gkbuzjdey.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gyxpizoyu.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gfeclwqbm.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/gtgfoagzi.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gmcfxkurx.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.tarul.cn/Article/details/gggwfhkbu.sHtML

[S59] C++：静态断言
来源：http://m.share.fktsv.cn/Article/details/gjmpmxvcm.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gmypfldbq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/gdjicvetb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.bbcook.cn/Article/details/gesmttpmr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkfxegihq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.sjlbkw.cn/Article/details/gukwvideb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gounjculc.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fktsv.cn/Article/details/ghoexijpm.sHtML

println("Hello")
来源：http://www.blog.vehdjk.com/Article/details/gdgwuyskn.sHtML

[T02] Kotlin：变量
来源：http://mobile.tarul.cn/Article/details/ggpmocbko.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gilbfnqtm.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/gcvitnltr.sHtML

"值: $b"
来源：http://wap.fktsv.cn/Article/details/gpmfqgfft.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gzljyjkvb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.sjlbkw.cn/Article/details/gxhmdfyih.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fktsv.cn/Article/details/gsxuzhiwk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gkaddytcv.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gvfnqqhsh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.tarul.cn/Article/details/gclyqmygw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gpnoqzkcf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/gzlbmzixq.sHtML

[T08] Kotlin：数据类
来源：http://www.share.yfazqb.com/Article/details/gdfkjilcv.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gjzmtnvnt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gmxhxvnth.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/giztsvtmc.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.tarul.cn/Article/details/gdagvcpsh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gosttscet.sHtML

[T11] Kotlin：协程
来源：http://www.blog.vehdjk.com/Article/details/ggzevptuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.bbcook.cn/Article/details/genxffmty.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gdsixxmrz.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.tarul.cn/Article/details/gzvgxqcoc.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gnbmdcmjh.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.epnwcf.com/Article/details/gwgomgosq.sHtML

[T14] Kotlin：循环
来源：http://m.share.vehdjk.com/Article/details/gmmlwqyrs.sHtML

for (i in 1..10) println(i)
来源：http://m.share.tarul.cn/Article/details/gyqjtxjxx.sHtML

[T15] Kotlin：接口
来源：http://m.share.epnwcf.com/Article/details/gvauxghzg.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.sjlbkw.cn/Article/details/ghuanqwrj.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gccanbcem.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gloheqcqb.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/ghcajackg.sHtML

var a = 1;  let b = 2
来源：http://baike.fktsv.cn/Article/details/gizociwpd.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gxbhhghrz.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/gehekbfrt.sHtML

[T19] Swift：可选绑定
来源：http://m.share.yfazqb.com/Article/details/guvwtfnof.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/ggvcbkoce.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gtupseukk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.epnwcf.com/Article/details/gqifupkch.sHtML

[T21] Swift：遍历
来源：http://www.blog.vehdjk.com/Article/details/gunxdoyfz.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gsetmlmbe.sHtML

[T22] Swift：字典
来源：http://www.m.share.yfazqb.com/Article/details/gaetygyqp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gunjhytij.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gsmlxpbxy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.tarul.cn/Article/details/ggegywenw.sHtML

[T24] Swift：闭包
来源：http://www.share.sjlbkw.cn/Article/details/ghxrweyik.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/gilvpvgou.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gdrtdkrns.sHtML

struct P { var x: Int }
来源：http://www.share.vehdjk.com/Article/details/gxlzshygw.sHtML

[T26] Swift：类与重写
来源：http://blog.epnwcf.com/Article/details/gruvvbqeu.sHtML

class A: Base { override func f() {} }
来源：http://baike.yfazqb.com/Article/details/gvpxefmeb.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/gcjvmrttp.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gxltoyksr.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gvzxyqjih.sHtML

enum Color { case red, green }
来源：http://wap.tarul.cn/Article/details/gkirdfelm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.vehdjk.com/Article/details/gsynwdtlp.sHtML

guard let x = opt else { return }
来源：http://www.blog.sjlbkw.cn/Article/details/gxyjkqkah.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gpaohwqcg.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gbgdduajg.sHtML

[T31] Lua：Hello World
来源：http://3g.fktsv.cn/Article/details/gfdpogpbh.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gkstyrxmb.sHtML

[T32] Lua：局部变量
来源：http://baike.sjlbkw.cn/Article/details/gvnjimvgp.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gcydwvoym.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gepwkhzkd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.bbcook.cn/Article/details/ggajxulke.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gphaljbvt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/goovaroeh.sHtML

[T35] Lua：字典表
来源：http://baike.tarul.cn/Article/details/gslajgokq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/glhvkgjpp.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gwblwahsl.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gejdxdass.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gyxgwsvmo.sHtML

"a" .. "b"
来源：http://m.share.fktsv.cn/Article/details/gfeopuzbo.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gkechtpvn.sHtML

if x > 0 then print("正") end
来源：http://baike.yfazqb.com/Article/details/gzjzzgitm.sHtML

[T39] Lua：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/glepkkxjs.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/gcrflxiqf.sHtML

[T40] Lua：元表
来源：http://wap.vehdjk.com/Article/details/gbagdjpbx.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.tarul.cn/Article/details/gjwhoszai.sHtML

[T41] Perl：Hello World
来源：http://wap.bbcook.cn/Article/details/guxjgqpru.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gzlrgwgsw.sHtML

[T42] Perl：变量类型
来源：http://3g.sjlbkw.cn/Article/details/goyqfssjr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/glrcbzjkd.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gbuqiozqs.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gpqxwryeq.sHtML

[T44] Perl：条件
来源：http://mobile.sjlbkw.cn/Article/details/gqomaihro.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gihpijnoi.sHtML

[T45] Perl：数组遍历
来源：http://blog.vehdjk.com/Article/details/gmaaqwtja.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.tarul.cn/Article/details/gidetxfcz.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gilsvvppw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/grcvtavgo.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.bbcook.cn/Article/details/gpnlcjwta.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.bbcook.cn/Article/details/getxvxiyv.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/guxkpjldm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/gutsalzsv.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gxashxiin.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.fktsv.cn/Article/details/ghquimlsh.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gtipzkmxq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.tarul.cn/Article/details/gutlamgku.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gmkihnvuw.sHtML

[T51] Scala：Hello World
来源：http://3g.fktsv.cn/Article/details/gjwaumygm.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/grrfvalip.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gktxmmylu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.yfazqb.com/Article/details/gcbecradw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/glzlmlujv.sHtML

s"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/grzuyjtjl.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gkpigncpz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.vehdjk.com/Article/details/ggavldwey.sHtML

[T55] Scala：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/groucrdtn.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.sjlbkw.cn/Article/details/gqxxxaydl.sHtML

[T56] Scala：样例类
来源：http://mobile.epnwcf.com/Article/details/gtpvjrjrr.sHtML

case class User(name: String, age: Int)
来源：http://read.share.yfazqb.com/Article/details/gspxxdxev.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gtoxdqfit.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gdlpqadrv.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gweqgtfdi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.fktsv.cn/Article/details/gfdeypdhq.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gvhynddcz.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gtqnxletw.sHtML

[T60] Scala：折叠
来源：http://3g.bbcook.cn/Article/details/gxwlyiuyc.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gugqzwjpc.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsrnibxaw.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.bbcook.cn/Article/details/gdqosbznw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcttbdrhl.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.bbcook.cn/Article/details/gpqupvfam.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.tarul.cn/Article/details/gbtfopphk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gfwdyagrz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.bbcook.cn/Article/details/gudvmrlrh.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.fktsv.cn/Article/details/gozsfnimp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gnbwwigzv.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/gvkvujllj.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.fktsv.cn/Article/details/grksodlka.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.tarul.cn/Article/details/gqesujzwg.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.vehdjk.com/Article/details/gfofpofyn.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gzrbwzsio.sHtML

{**a, **b}
来源：http://wap.yfazqb.com/Article/details/gqhpqyqrh.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/gaeqmkpls.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/giduklndf.sHtML

[U08] Py：展平二维列表
来源：http://blog.sjlbkw.cn/Article/details/gkzqxqtnf.sHtML

[y for x in nested for y in x]
来源：http://www.share.tarul.cn/Article/details/gyqakbdlx.sHtML


<!-- 参考信息 -->