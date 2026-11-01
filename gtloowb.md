代发 wailian999

openssl rand -hex 16
来源：http://read.share.fktsv.cn/Article/details/grjhaiapj.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gtuddhapv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.sjlbkw.cn/Article/details/giazqlbmd.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gacmphuiy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.epnwcf.com/Article/details/gssbllisz.sHtML

[R70] 时间戳与互转
来源：http://baike.bbcook.cn/Article/details/gnjoofbgy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/ghaqfccat.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gaxnavyyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gglbwtuhe.sHtML

[R72] 等待端口就绪
来源：http://read.share.sjlbkw.cn/Article/details/gboeyllvq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gpinukqms.sHtML

[R73] 分割大日志
来源：http://baike.fktsv.cn/Article/details/gshfpxsvf.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gquowixzu.sHtML

[R74] 批量重命名
来源：http://blog.epnwcf.com/Article/details/gekmsazpw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.vehdjk.com/Article/details/gptxehaud.sHtML

[R75] 导出环境变量
来源：http://read.share.vehdjk.com/Article/details/gnkfulmxl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fktsv.cn/Article/details/gxcihtdrc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.epnwcf.com/Article/details/gibeityqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gpazlmefa.sHtML

[R77] 读取用户输入
来源：http://www.blog.fktsv.cn/Article/details/gqabohbmv.sHtML

read -rp "请输入: " ans
来源：http://read.share.bbcook.cn/Article/details/gajlamqoq.sHtML

[R78] 交互式菜单
来源：http://wap.sjlbkw.cn/Article/details/goxsyihwj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.sjlbkw.cn/Article/details/gmlevzsxw.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/glgdodtqe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fktsv.cn/Article/details/gexjrqofi.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gtccfxtsu.sHtML

time ./run.sh
来源：http://mobile.sjlbkw.cn/Article/details/guhnrxlyn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggpnyfakz.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gedmldlqy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gkqngiine.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/ghgrkoclc.sHtML

#include <stdio.h>
来源：http://www.blog.yfazqb.com/Article/details/gnxbaafsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gwanyoiex.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.tarul.cn/Article/details/gdqflvlyz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gksbvbgxk.sHtML

[S03] C：读入整数
来源：http://wap.sjlbkw.cn/Article/details/gozmjmmrf.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gjlfnkocz.sHtML

[S04] C：字符串复制
来源：http://www.blog.vehdjk.com/Article/details/gxgochdwq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.vehdjk.com/Article/details/gktswqtvr.sHtML

[S05] C：字符串长度
来源：http://www.blog.sjlbkw.cn/Article/details/gvmjhwefl.sHtML

strlen(s)
来源：http://wap.yfazqb.com/Article/details/ghevcexmh.sHtML

[S06] C：字符串比较
来源：http://www.share.yfazqb.com/Article/details/gmrgcagei.sHtML

strcmp(a, b) == 0
来源：http://m.share.epnwcf.com/Article/details/govacelyz.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gtmgxkzvt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/gfofpzjnf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gsimgmejo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.bbcook.cn/Article/details/glverkjma.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/guxjragzn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/gebhwznis.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/gznbfsdyc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gzrdbxptu.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gdietvyax.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.bbcook.cn/Article/details/gfqwdmqdl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/gdfiiylav.sHtML

fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/grhnjylqn.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfbfnzxkv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.tarul.cn/Article/details/gibibdhut.sHtML

[S13] C：宏定义
来源：http://www.m.share.vehdjk.com/Article/details/gpxnfgkaz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/gjlvfjjce.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gbjrrecno.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fktsv.cn/Article/details/gkqomajfu.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gfjufylku.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/gxglukxvx.sHtML

[S16] C：位操作置位
来源：http://www.share.vehdjk.com/Article/details/gmdgfjvfc.sHtML

x |= (1 << 3);
来源：http://mobile.tarul.cn/Article/details/gschuhsvc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fktsv.cn/Article/details/gbisipcse.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.yfazqb.com/Article/details/gumxfflfb.sHtML

[S18] C：命令行参数
来源：http://www.share.fktsv.cn/Article/details/gviwajusx.sHtML

int main(int argc, char **argv)
来源：http://mobile.tarul.cn/Article/details/ggnffqrec.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gwjkdsjic.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gnlnjsbek.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gsscpgkvy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gkivdndan.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/grmyxffvo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.epnwcf.com/Article/details/genrfapnn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gepgceocx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.tarul.cn/Article/details/gslclxvck.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/ghsnhdenp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkqjksme.sHtML

[S24] C：获取本地时间
来源：http://3g.epnwcf.com/Article/details/gbavkhhwc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gdzwppagj.sHtML

[S25] C：内存拷贝
来源：http://wap.yfazqb.com/Article/details/geubdzeou.sHtML

memcpy(dst, src, n);
来源：http://3g.vehdjk.com/Article/details/gydjnhjfg.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gadlpnjyo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.bbcook.cn/Article/details/gdnfxrfqo.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/ggxjjyodr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gcbcoksww.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/gicwmyebd.sHtML

static int counter = 0;
来源：http://www.share.sjlbkw.cn/Article/details/gtbltpwve.sHtML

[S29] C：变参函数
来源：http://www.blog.yfazqb.com/Article/details/gzozoypqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.sjlbkw.cn/Article/details/grhtkifla.sHtML

[S30] C：头文件保护
来源：http://mobile.fktsv.cn/Article/details/gxylklapv.sHtML

#ifndef X_H
来源：http://read.share.bbcook.cn/Article/details/ghpwryavc.sHtML

#define X_H
来源：http://m.share.yfazqb.com/Article/details/gbeegbchi.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gpaspbuop.sHtML

[S31] C++：Hello World
来源：http://baike.epnwcf.com/Article/details/gwzjydjpg.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gxeaekktg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/gcpsxgyqm.sHtML

[S32] C++：字符串
来源：http://www.share.epnwcf.com/Article/details/gnfwjsjku.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gzmhrlpjy.sHtML

[S33] C++：vector 增删
来源：http://3g.tarul.cn/Article/details/gwpzmkhcx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gxehdeasu.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gbeuyxfyt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.tarul.cn/Article/details/gbbemxfwm.sHtML

[S35] C++：map
来源：http://mobile.vehdjk.com/Article/details/gwhajekth.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/glfeypbwc.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gvcslxyrg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gvmlnauac.sHtML

[S37] C++：set
来源：http://wap.fktsv.cn/Article/details/glrjgqqii.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gjhuenakj.sHtML

[S38] C++：排序
来源：http://www.blog.fktsv.cn/Article/details/gygghfmsm.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.bbcook.cn/Article/details/gnrtuqbwn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fktsv.cn/Article/details/gflmeoxue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.sjlbkw.cn/Article/details/gjjdtflme.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gmymardee.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.yfazqb.com/Article/details/grpikxpas.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gtcxbzpsn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fktsv.cn/Article/details/gvtjdjiet.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/ggdxbueqs.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gnjsejpqu.sHtML

[S43] C++：智能指针
来源：http://baike.vehdjk.com/Article/details/gqwjffhdq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fktsv.cn/Article/details/gzirsnsig.sHtML

[S44] C++：引用传参
来源：http://www.m.share.bbcook.cn/Article/details/ghesmlnef.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/gvylrcgou.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gdvvxlqeh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.vehdjk.com/Article/details/gwbtnmyqb.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gxwidaysv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/ghflfvxfr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fktsv.cn/Article/details/ggkengpax.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.yfazqb.com/Article/details/gejhfgshy.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/grwprffqs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.yfazqb.com/Article/details/gajboeqds.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fktsv.cn/Article/details/gntsdvacs.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gsidwrvgt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gzjhqfpoi.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/geoymyywj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gihvssycd.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gwgedlbyj.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gvaulyqgi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.epnwcf.com/Article/details/gitgmkdvd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.yfazqb.com/Article/details/gpqygjqxi.sHtML

[S53] C++：移动语义
来源：http://www.m.share.sjlbkw.cn/Article/details/gpejckshf.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gbszyqptc.sHtML

[S54] C++：异常处理
来源：http://m.share.tarul.cn/Article/details/ghxtuwlmf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gnzwbvwhq.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gzvknlvdz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.sjlbkw.cn/Article/details/ggphwuczu.sHtML

[S56] C++：optional
来源：http://m.share.sjlbkw.cn/Article/details/gdlsiafvq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gjaehiupo.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fktsv.cn/Article/details/gmgubrkcz.sHtML

constexpr int N = 10;
来源：http://3g.fktsv.cn/Article/details/gkpetvxfs.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gmbdvajke.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gkferrcoq.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/godzsttgd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gpdybpush.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.sjlbkw.cn/Article/details/gqdauwkrc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.yfazqb.com/Article/details/ghpiapyxh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghtxiwnjk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gojrhkqnw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqyouodjt.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gvebydaje.sHtML

println("Hello")
来源：http://www.share.epnwcf.com/Article/details/gfkujfcld.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gneqqpbfp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/galdwobgy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.tarul.cn/Article/details/gantvzxvt.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gagogbevu.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/gkrwqptaa.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gnlihymma.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gddhzvxwx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gkvoxctep.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gnpiodkle.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.yfazqb.com/Article/details/gcdkulgxs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gyzempciz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gxvshnziz.sHtML

[T08] Kotlin：数据类
来源：http://3g.fktsv.cn/Article/details/glwsixtri.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.epnwcf.com/Article/details/gsmphbzlx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.epnwcf.com/Article/details/gbighdkjv.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.bbcook.cn/Article/details/ggqhdjpgh.sHtML

[T10] Kotlin：默认参数
来源：http://wap.bbcook.cn/Article/details/gtjrqyanh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.yfazqb.com/Article/details/gexhizavo.sHtML

[T11] Kotlin：协程
来源：http://www.share.yfazqb.com/Article/details/gxwzmezcm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gfcowxohx.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gohvscijr.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gbsonphnr.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.tarul.cn/Article/details/gogsuwahz.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gytjgzjsz.sHtML

[T14] Kotlin：循环
来源：http://baike.vehdjk.com/Article/details/gukhwqxhg.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/gekrvijfn.sHtML

[T15] Kotlin：接口
来源：http://m.share.fktsv.cn/Article/details/gxkpjhbvk.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/ggnytlwrc.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gimuxasux.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gfbjxeoml.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gvpgflyhb.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/gxpsoizup.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gliidkbzt.sHtML

"值: \(b)"
来源：http://3g.epnwcf.com/Article/details/gjfyuvtyb.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gzdwaumxu.sHtML

if let n = opt { print(n) }
来源：http://wap.sjlbkw.cn/Article/details/gvdnsarwz.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/ghetpshhr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.yfazqb.com/Article/details/gfpukjqwh.sHtML

[T21] Swift：遍历
来源：http://www.share.epnwcf.com/Article/details/gxtfoqzel.sHtML

for x in a { print(x) }
来源：http://read.share.sjlbkw.cn/Article/details/gszdhrdmx.sHtML

[T22] Swift：字典
来源：http://www.m.share.tarul.cn/Article/details/gqujxlxkd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/gbsurkpct.sHtML

[T23] Swift：函数
来源：http://wap.fktsv.cn/Article/details/gkiphcctw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gyqyuwgel.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gdnsjjopk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gstalhvrg.sHtML

[T25] Swift：结构体
来源：http://blog.epnwcf.com/Article/details/gihzcqnbb.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gesujfvhi.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gcyjnjzlg.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gkxglqeyk.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gmwvscrmb.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gnrbnmjhr.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gschkwrsg.sHtML

enum Color { case red, green }
来源：http://www.m.share.fktsv.cn/Article/details/gabyuvfsd.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.tarul.cn/Article/details/goddpmnda.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/gauwextxz.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gkcaxtewu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.vehdjk.com/Article/details/gagrghsad.sHtML

[T31] Lua：Hello World
来源：http://read.share.bbcook.cn/Article/details/gafxzycoa.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gqcqpqwrw.sHtML

[T32] Lua：局部变量
来源：http://baike.epnwcf.com/Article/details/gdurfleny.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/gzzkocvon.sHtML

[T33] Lua：表（数组）
来源：http://3g.bbcook.cn/Article/details/gyezujwlp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gvbqpveec.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gzxayvdue.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gocoaqnjr.sHtML

[T35] Lua：字典表
来源：http://baike.fktsv.cn/Article/details/geznpfgla.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gnamvnmyq.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gvtbpkbvf.sHtML

function add(a, b) return a + b end
来源：http://www.blog.bbcook.cn/Article/details/gaagqwmpy.sHtML

[T37] Lua：字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gxmkbpazh.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/goaoxnykc.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gdsuopzwc.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gaoatbzbc.sHtML

[T39] Lua：模式匹配
来源：http://m.share.bbcook.cn/Article/details/gqldxfkvw.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gemmelziu.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gexzzwfjl.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gsfpmrewn.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/gfkgvjnpc.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gqnpyokpv.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/gscgijxkm.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.sjlbkw.cn/Article/details/ghywjyupq.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gembfmsul.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gwbdxpbbf.sHtML

[T44] Perl：条件
来源：http://wap.bbcook.cn/Article/details/gtmqjmldl.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.yfazqb.com/Article/details/grqmqpjvx.sHtML

[T45] Perl：数组遍历
来源：http://blog.fktsv.cn/Article/details/gcbolecla.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/gbfjhxdfe.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gaimoplhf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gyeeqgtsz.sHtML

[T47] Perl：正则捕获
来源：http://baike.fktsv.cn/Article/details/ggiqkwzrh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gpezblggx.sHtML

[T48] Perl：正则替换
来源：http://www.share.sjlbkw.cn/Article/details/gdjzivkvd.sHtML

$s =~ s/old/new/g;
来源：http://mobile.bbcook.cn/Article/details/gbmqreylq.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gkliqzqsn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gdqiuflcz.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxdpgppb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fktsv.cn/Article/details/gekktasqq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.yfazqb.com/Article/details/glezumncj.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gmyyajfol.sHtML

println("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gotikhkmf.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/gcjlbkqif.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gvpnyegpr.sHtML

[T53] Scala：字符串插值
来源：http://3g.yfazqb.com/Article/details/gvkxrnqjx.sHtML

s"值: $b"
来源：http://m.share.tarul.cn/Article/details/gqbuiyhai.sHtML

[T54] Scala：集合映射
来源：http://mobile.epnwcf.com/Article/details/gpbuwhdow.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/gduyoqmli.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gqfdwjdnf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gjpfgkjwj.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gttmzkamt.sHtML

case class User(name: String, age: Int)
来源：http://baike.epnwcf.com/Article/details/ganckgmsi.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gwgghufbu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.epnwcf.com/Article/details/ghtlaqjaz.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fktsv.cn/Article/details/gxmynidqh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.bbcook.cn/Article/details/gwvwrgbgl.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/gfvgfvwvu.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gbzvthnwf.sHtML

[T60] Scala：折叠
来源：http://www.blog.yfazqb.com/Article/details/gzdqyebzw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.epnwcf.com/Article/details/gdshiawcm.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/guxaiowlu.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gjwzpeeuc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdrachtna.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gugjjyoiz.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.vehdjk.com/Article/details/gxqkqzmrj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://3g.yfazqb.com/Article/details/gdcplxfew.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.sjlbkw.cn/Article/details/gyyntrieh.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.bbcook.cn/Article/details/gjrtdfxlb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/gzouhwcxd.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/gcnxltxre.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.bbcook.cn/Article/details/glwizmenk.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.sjlbkw.cn/Article/details/gralmeybk.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/ghgvlqwfm.sHtML

[U06] Py：合并两个字典
来源：http://baike.vehdjk.com/Article/details/gahxusdfb.sHtML

{**a, **b}
来源：http://read.share.vehdjk.com/Article/details/gzwprtugm.sHtML

[U07] Py：反转字典键值
来源：http://wap.bbcook.cn/Article/details/gipqpvgph.sHtML

{v: k for k, v in d.items()}
来源：http://wap.epnwcf.com/Article/details/gnglfovdw.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gonhvyyje.sHtML

[y for x in nested for y in x]
来源：http://3g.bbcook.cn/Article/details/gddvaaohj.sHtML


<!-- 参考信息 -->