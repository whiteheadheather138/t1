代发 wailian999

openssl rand -hex 16
来源：http://blog.yfazqb.com/Article/details/guzzlfzrz.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/gnchyiimm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.epnwcf.com/Article/details/gfxzpckmy.sHtML

[R69] 生成随机密码
来源：http://wap.tarul.cn/Article/details/gcybkozup.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gnocsdvxb.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gddfrzbdh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.tarul.cn/Article/details/gxdojayic.sHtML

[R71] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gbrhxvwuf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gdfniqtkk.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gjelfhmvf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/ghogsmqnk.sHtML

[R73] 分割大日志
来源：http://www.share.sjlbkw.cn/Article/details/gwmcitzms.sHtML

split -l 1000 big.log part_
来源：http://3g.bbcook.cn/Article/details/gmnkvgaik.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gxwrqsdtm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/grreymoru.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/grvifkzjl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gpkiclwvn.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/gxadxbptn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gniarrtnd.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gvyiurcsp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gdddhzqvn.sHtML

[R78] 交互式菜单
来源：http://baike.sjlbkw.cn/Article/details/glibaozlz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.tarul.cn/Article/details/goqibgqdp.sHtML

[R79] 解析命令行选项
来源：http://baike.tarul.cn/Article/details/grxysjimf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gqamzhrxz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gogckwghp.sHtML

time ./run.sh
来源：http://www.m.share.tarul.cn/Article/details/gmuuvcwsk.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gpudybqxg.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gtalsigey.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gewwelpyy.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gjyeomoxw.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/ghtidmszn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/ghoygftms.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gutrksham.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gbdqydrez.sHtML

[S03] C：读入整数
来源：http://3g.vehdjk.com/Article/details/gqgsxknyf.sHtML

int x; scanf("%d", &x);
来源：http://3g.bbcook.cn/Article/details/gpzcgteff.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/goopllzuy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fktsv.cn/Article/details/gzbivotsk.sHtML

[S05] C：字符串长度
来源：http://3g.epnwcf.com/Article/details/gpfxjskdl.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/guvzdeacr.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/ghmgqqpib.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfkruqkr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/gdvyvcoiz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.vehdjk.com/Article/details/gldmncklx.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.sjlbkw.cn/Article/details/gyikyrwpe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.vehdjk.com/Article/details/gvpmvunxq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.bbcook.cn/Article/details/glcichrln.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.tarul.cn/Article/details/ghxommdnb.sHtML

[S10] C：指针与解引用
来源：http://blog.sjlbkw.cn/Article/details/gvvjoxyar.sHtML

int *p = &a;  *p = 5;
来源：http://blog.epnwcf.com/Article/details/ghpcqlshf.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/goysscoow.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gdyoakxaj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/ghmbxddvl.sHtML

fclose(f);
来源：http://blog.sjlbkw.cn/Article/details/glquwcomg.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gqancsspl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gksspcpst.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gfsnecxva.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gpuxojhxz.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gpvqnkien.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gyxhbyjyo.sHtML

[S15] C：类型转换
来源：http://www.m.share.tarul.cn/Article/details/gmmhrbxne.sHtML

(double) a / b
来源：http://read.share.sjlbkw.cn/Article/details/gjquueyze.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gtmzchosj.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gdsrjmkou.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gqmgljkoc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.sjlbkw.cn/Article/details/ghhgnwsns.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/gjtqsndvp.sHtML

int main(int argc, char **argv)
来源：http://www.share.vehdjk.com/Article/details/guzakndxs.sHtML

[S19] C：快速排序
来源：http://baike.tarul.cn/Article/details/gynqhayrb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gopotgypw.sHtML

[S20] C：二分查找
来源：http://m.share.sjlbkw.cn/Article/details/gjgfxaxgz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gagseyjdy.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gigmqnzwi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.epnwcf.com/Article/details/gsegmjrdx.sHtML

[S22] C：字符串转数字
来源：http://mobile.sjlbkw.cn/Article/details/gwonlxqhk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/gngqeeucn.sHtML

[S23] C：随机数
来源：http://blog.fktsv.cn/Article/details/gbwwuhyoc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.tarul.cn/Article/details/gqvdzcren.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gvbsakwyf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.epnwcf.com/Article/details/gsxqmpbrj.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gmezacyvv.sHtML

memcpy(dst, src, n);
来源：http://baike.sjlbkw.cn/Article/details/glffeccjr.sHtML

[S26] C：内存清零
来源：http://wap.epnwcf.com/Article/details/gqhcohonx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.sjlbkw.cn/Article/details/gjzdjkpdk.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/guduswkxw.sHtML

const double PI = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gdtxhtwlf.sHtML

[S28] C：静态变量
来源：http://m.share.bbcook.cn/Article/details/gpcbhzcvg.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gulcwmftv.sHtML

[S29] C：变参函数
来源：http://blog.fktsv.cn/Article/details/gakpgriwb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.yfazqb.com/Article/details/gzhtzyuks.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/grbxctkaj.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gzzprsnle.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/gxettriqu.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gnaemuhkv.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/geetwbifa.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gfbzsmcbd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.epnwcf.com/Article/details/gljgifklk.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/gogyfhbpt.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gorwidkrn.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/gigjkwfnf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.tarul.cn/Article/details/ggzgzbvod.sHtML

[S34] C++：遍历 vector
来源：http://m.share.yfazqb.com/Article/details/gxwwleyiu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/gdclwcuui.sHtML

[S35] C++：map
来源：http://mobile.bbcook.cn/Article/details/gbfpnfmnj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/glcwslyhc.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/grfbeqyqt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/geiexfaqx.sHtML

[S37] C++：set
来源：http://3g.tarul.cn/Article/details/gtddgwanz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsupnttu.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/gioifhzjn.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.tarul.cn/Article/details/gjxcmuoqf.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.tarul.cn/Article/details/gjezyvuiq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.yfazqb.com/Article/details/gblorynvn.sHtML

[S40] C++：查找元素
来源：http://baike.bbcook.cn/Article/details/gthxbgwnk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.epnwcf.com/Article/details/gfgsdcygd.sHtML

[S41] C++：类与构造函数
来源：http://3g.bbcook.cn/Article/details/glkylpcdm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.tarul.cn/Article/details/gkejqzsrj.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gavkomipy.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/gtfljxayo.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gzfidjofm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/govutgthv.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/ggbwuvafe.sHtML

void inc(int &x) { ++x; }
来源：http://baike.sjlbkw.cn/Article/details/gxgrmtxpu.sHtML

[S45] C++：lambda
来源：http://m.share.yfazqb.com/Article/details/gfommjwsh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.epnwcf.com/Article/details/gdvlbcliv.sHtML

[S46] C++：函数模板
来源：http://mobile.yfazqb.com/Article/details/gtojecdxb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.bbcook.cn/Article/details/gajpugqdi.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/gscledfry.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gasobcvzl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/glcnduqxt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.sjlbkw.cn/Article/details/ginlkpzrt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fktsv.cn/Article/details/givzlwlch.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/giggtjacm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gxwbkbhss.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gjvdrfmrn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.bbcook.cn/Article/details/gbbehohnk.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fktsv.cn/Article/details/glxyhxzem.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gyxouykqv.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gnuxmrfzz.sHtML

int size() const noexcept { return n_; }
来源：http://wap.sjlbkw.cn/Article/details/glrteehjl.sHtML

[S53] C++：移动语义
来源：http://read.share.sjlbkw.cn/Article/details/gvfwvfupo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.tarul.cn/Article/details/gyuhdfttw.sHtML

[S54] C++：异常处理
来源：http://3g.vehdjk.com/Article/details/gqayrnbne.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gzknnwejf.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/gdusgsqjl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.vehdjk.com/Article/details/gmkrjretl.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/gwcaylvpt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gaszetuqi.sHtML

[S57] C++：编译期常量
来源：http://mobile.yfazqb.com/Article/details/gaapsrxly.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gfnmkxpjt.sHtML

[S58] C++：命名空间
来源：http://blog.bbcook.cn/Article/details/gomfovedd.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.epnwcf.com/Article/details/gthwxdrec.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gjesrdhym.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.bbcook.cn/Article/details/gmfoavypr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gcbqcodef.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.vehdjk.com/Article/details/gufjgjojf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghegfohcn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gycqunrai.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjpxwodqh.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gfdltwsll.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gqcixqzha.sHtML

[T02] Kotlin：变量
来源：http://m.share.vehdjk.com/Article/details/gqbffanrt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.bbcook.cn/Article/details/gzmgjlhhj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gvecmzhyc.sHtML

"值: $b"
来源：http://mobile.vehdjk.com/Article/details/gmnmdwlna.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fktsv.cn/Article/details/gcauycvgl.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gpzajgsts.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.yfazqb.com/Article/details/gegstlvpj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/ggvejrwfg.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/ghbfozhmo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.tarul.cn/Article/details/gvpstzhli.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/glsfkrdiv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gotbgbqhk.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gguvrobyt.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.bbcook.cn/Article/details/gcfgtlamu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.yfazqb.com/Article/details/gjbgujhjn.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/ghezpigqt.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.sjlbkw.cn/Article/details/gukkzksue.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/geuoucuvp.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gadrorhzx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.yfazqb.com/Article/details/grncnvlfe.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fktsv.cn/Article/details/gsocxmzsv.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gceqezrmr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.bbcook.cn/Article/details/ggypwbwun.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/gebwxuiga.sHtML

[T14] Kotlin：循环
来源：http://baike.sjlbkw.cn/Article/details/gtzbdyffk.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gbbdgxxpr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gqflgkngs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fktsv.cn/Article/details/gjitwkvxu.sHtML

[T16] Swift：Hello World
来源：http://wap.fktsv.cn/Article/details/gllejmpse.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/grbhmbdqu.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fktsv.cn/Article/details/goaloezkr.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/gqaffarea.sHtML

[T18] Swift：字符串插值
来源：http://blog.fktsv.cn/Article/details/gjeeivose.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gyjoficny.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.bbcook.cn/Article/details/geptvapog.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.tarul.cn/Article/details/gcmaooqkn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.epnwcf.com/Article/details/gzglegjju.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/gvrwvrldj.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/givhvaqtj.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/ggonsxjua.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gnupavyzf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gipohmoxe.sHtML

[T23] Swift：函数
来源：http://wap.bbcook.cn/Article/details/gleesuvpd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.yfazqb.com/Article/details/guljvlsbo.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gsqfwhyjm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/gadtrsvka.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gczgxivbc.sHtML

struct P { var x: Int }
来源：http://www.share.epnwcf.com/Article/details/gfaekosdu.sHtML

[T26] Swift：类与重写
来源：http://mobile.sjlbkw.cn/Article/details/gwbvspxkl.sHtML

class A: Base { override func f() {} }
来源：http://wap.fktsv.cn/Article/details/guaylgddc.sHtML

[T27] Swift：错误处理
来源：http://read.share.bbcook.cn/Article/details/gzhrxbnne.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.sjlbkw.cn/Article/details/gemhewzaf.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/glxblvjqd.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/gnqqmfizp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gbocxugex.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gihqcxzud.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/geubwmbgf.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fktsv.cn/Article/details/gprbvxvmj.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/grascxxfv.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gzgimzxzx.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gsrsqcudx.sHtML

local a = 1
来源：http://blog.vehdjk.com/Article/details/gvgbtjbgv.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gkzqlnoez.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.vehdjk.com/Article/details/gkzfzmoto.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gtlsusdfm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gyixygjgo.sHtML

[T35] Lua：字典表
来源：http://www.m.share.tarul.cn/Article/details/gldbreduo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gzigpeolj.sHtML

[T36] Lua：函数
来源：http://baike.sjlbkw.cn/Article/details/grwndimng.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gvhzcstnc.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gzydjnizb.sHtML

"a" .. "b"
来源：http://blog.yfazqb.com/Article/details/gpxaccmci.sHtML

[T38] Lua：条件
来源：http://www.m.share.yfazqb.com/Article/details/gnhpwlbuu.sHtML

if x > 0 then print("正") end
来源：http://www.share.bbcook.cn/Article/details/gurfshbbp.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/grjczbkxw.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gyxidtimd.sHtML

[T40] Lua：元表
来源：http://www.blog.vehdjk.com/Article/details/gthjmtwbq.sHtML

setmetatable({}, { __index = base })
来源：http://wap.tarul.cn/Article/details/gbdsefvki.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gpeisfomh.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/geqlcifyb.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gvpmkvkok.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gkoevbqtv.sHtML

[T43] Perl：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gtholedcy.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gyrxywdlu.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/gizkwpjti.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/gjhxzdggv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/glqlldwlq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gsdvsgqkw.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/gfxaacjqy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gxjswsupz.sHtML

[T47] Perl：正则捕获
来源：http://blog.epnwcf.com/Article/details/gubktaihl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gvoefepag.sHtML

[T48] Perl：正则替换
来源：http://mobile.epnwcf.com/Article/details/ghetauntc.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gucevchen.sHtML

[T49] Perl：函数
来源：http://www.blog.fktsv.cn/Article/details/grmrzqmuz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gxsqiimhl.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gqflfcltk.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.bbcook.cn/Article/details/ghioircxq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gwwmhxamr.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/ggcmglgkp.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/glualgqvh.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/gkdjhbckf.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/glawiljcs.sHtML

[T53] Scala：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gcnpjkwnu.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gshmkxzic.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gubnwcjrx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gkjurxvxe.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.vehdjk.com/Article/details/grrsokfqj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gefdooqjb.sHtML

[T56] Scala：样例类
来源：http://baike.vehdjk.com/Article/details/gzuqyturc.sHtML

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gjqpmthqz.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/glbeqrzwp.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.yfazqb.com/Article/details/gbtiribyc.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/gexqtsygp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/greefyrrf.sHtML

[T59] Scala：循环
来源：http://www.blog.fktsv.cn/Article/details/gisxcowrh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.bbcook.cn/Article/details/ghlxjbntb.sHtML

[T60] Scala：折叠
来源：http://read.share.sjlbkw.cn/Article/details/gemkxirgg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.bbcook.cn/Article/details/gdplcirci.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ggwprhhsf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/ghvljphjb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpyyvuatw.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.tarul.cn/Article/details/gxiplcefo.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.yfazqb.com/Article/details/gdpsqhkfx.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.yfazqb.com/Article/details/gvkcumwfb.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.tarul.cn/Article/details/gkkraphqf.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.sjlbkw.cn/Article/details/gtfifpohl.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.sjlbkw.cn/Article/details/gbqzfavwq.sHtML

[U04] Py：变量调试打印
来源：http://baike.yfazqb.com/Article/details/gkfsruytc.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.fktsv.cn/Article/details/gqeaaxyar.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.bbcook.cn/Article/details/ghpxfbunh.sHtML

list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/glvtevssz.sHtML

[U06] Py：合并两个字典
来源：http://read.share.bbcook.cn/Article/details/gmppazbos.sHtML

{**a, **b}
来源：http://www.m.share.tarul.cn/Article/details/gvtsavkmy.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxnwtmkw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gxcjtznkb.sHtML

[U08] Py：展平二维列表
来源：http://mobile.tarul.cn/Article/details/gemhipbny.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/gqnhvnedm.sHtML


<!-- 参考信息 -->