代发 wailian999

df -h;  du -sh *
来源：http://www.m.share.yfazqb.com/Article/details/gsjzjznqe.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fktsv.cn/Article/details/gvoaoenth.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gwuusctpe.sHtML

[R63] 内存与进程
来源：http://m.share.vehdjk.com/Article/details/gfbvrzrnd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvmffktc.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gktjcahfr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.sjlbkw.cn/Article/details/gtjdrteci.sHtML

[R65] 查看端口占用
来源：http://mobile.fktsv.cn/Article/details/gakmzikgj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.yfazqb.com/Article/details/gtgedbauq.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/ggceqmkjn.sHtML

crontab -e;  crontab -l
来源：http://m.share.epnwcf.com/Article/details/giiltqons.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.vehdjk.com/Article/details/gxbgfprgo.sHtML

openssl rand -hex 16
来源：http://read.share.yfazqb.com/Article/details/gnrxcbhil.sHtML

[R68] 计算文件校验值
来源：http://wap.vehdjk.com/Article/details/gatbpwhnv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gtoychtdi.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gsuryssga.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gpfjvdeoi.sHtML

[R70] 时间戳与互转
来源：http://wap.vehdjk.com/Article/details/gjbsogmph.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.sjlbkw.cn/Article/details/gdvzyfsyt.sHtML

[R71] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gzqxbnpgi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.vehdjk.com/Article/details/ggirjrhtf.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/ghawkmwqj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/ganagddls.sHtML

[R73] 分割大日志
来源：http://mobile.sjlbkw.cn/Article/details/ghmqzhuqg.sHtML

split -l 1000 big.log part_
来源：http://blog.fktsv.cn/Article/details/gtjqpllbl.sHtML

[R74] 批量重命名
来源：http://www.m.share.yfazqb.com/Article/details/gsiusrlgv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/gfoxpwvvb.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/ghfsjrlbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/ghylhmbje.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/gqlcsebdb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/gbwmydomd.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gksxorhty.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gqrsijddi.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gyseveskn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.bbcook.cn/Article/details/gxbimwpfd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/gtzzhmkak.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.epnwcf.com/Article/details/gzokkysct.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gdldthffn.sHtML

time ./run.sh
来源：http://3g.vehdjk.com/Article/details/gvcfloukh.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzkjtzpxd.sHtML

S. C / C++ 专题
来源：http://blog.fktsv.cn/Article/details/gpartjupb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glbcehlhk.sHtML

[S01] C：Hello World
来源：http://www.blog.vehdjk.com/Article/details/galbjwryp.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/gkyymwnsg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.yfazqb.com/Article/details/gjyijszfz.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fktsv.cn/Article/details/gbwmofcih.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/getnxtbkb.sHtML

[S03] C：读入整数
来源：http://read.share.bbcook.cn/Article/details/gmykervpn.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/ghqqwviud.sHtML

[S04] C：字符串复制
来源：http://baike.yfazqb.com/Article/details/gmpuezckx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gbvkynqal.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fktsv.cn/Article/details/gqdwfjshd.sHtML

strlen(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnkbrdfa.sHtML

[S06] C：字符串比较
来源：http://blog.yfazqb.com/Article/details/gcbfjmivx.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gxgkvynuo.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/guahdyjpm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gxpeoyhyi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.bbcook.cn/Article/details/gavzvydgh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.tarul.cn/Article/details/gwqsrfbqd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.epnwcf.com/Article/details/gmczvnhkj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gutgpcxeb.sHtML

[S10] C：指针与解引用
来源：http://3g.vehdjk.com/Article/details/glweyobbh.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/gcjvmxeyr.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gnknlllyw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gnggfkcor.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gcteaqowf.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/ghojntphx.sHtML

[S12] C：写文件
来源：http://mobile.epnwcf.com/Article/details/ghnhonxfj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.yfazqb.com/Article/details/gizokkwok.sHtML

[S13] C：宏定义
来源：http://m.share.yfazqb.com/Article/details/gjwwakeqy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gseoyqpdf.sHtML

[S14] C：枚举
来源：http://www.blog.bbcook.cn/Article/details/gxskzimiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gttwwwexy.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gkgzupqxj.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gvfcxbjuk.sHtML

[S16] C：位操作置位
来源：http://3g.tarul.cn/Article/details/gvixwlpqv.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/gofkuogcq.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/guvxqgymn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.sjlbkw.cn/Article/details/gkhtwyuht.sHtML

[S18] C：命令行参数
来源：http://m.share.fktsv.cn/Article/details/gfbcmrrap.sHtML

int main(int argc, char **argv)
来源：http://blog.tarul.cn/Article/details/gagrdkwgp.sHtML

[S19] C：快速排序
来源：http://wap.fktsv.cn/Article/details/gqerqxwmx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gaikrmnok.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/gegmafodb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/gwnumacme.sHtML

[S21] C：字符类别判断
来源：http://blog.epnwcf.com/Article/details/gawezuihg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.epnwcf.com/Article/details/gncgwweon.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/grlqabewi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fktsv.cn/Article/details/gaocdgksg.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gzwwjweqq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.tarul.cn/Article/details/glxxwwbya.sHtML

[S24] C：获取本地时间
来源：http://m.share.bbcook.cn/Article/details/gczmnbxbn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrdohjyi.sHtML

[S25] C：内存拷贝
来源：http://blog.fktsv.cn/Article/details/gvacdzfpg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gwogfjqxk.sHtML

[S26] C：内存清零
来源：http://baike.vehdjk.com/Article/details/gmjgwklob.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fktsv.cn/Article/details/gpafmcizt.sHtML

[S27] C：定义常量
来源：http://www.m.share.epnwcf.com/Article/details/gaztzwtbd.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gdvjdlgvs.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gmpabkiry.sHtML

static int counter = 0;
来源：http://mobile.epnwcf.com/Article/details/ggwigxofu.sHtML

[S29] C：变参函数
来源：http://m.share.yfazqb.com/Article/details/gjylygvrj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/gkdelcudx.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gdxfhpeaq.sHtML

#ifndef X_H
来源：http://www.blog.tarul.cn/Article/details/gaqtdmboe.sHtML

#define X_H
来源：http://www.m.share.bbcook.cn/Article/details/godtelepm.sHtML

#endif
来源：http://www.m.share.tarul.cn/Article/details/gusndtpws.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gkhafjmwn.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gkhedeqgg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.yfazqb.com/Article/details/gakuaklgl.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gvgambonc.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gplydqeww.sHtML

[S33] C++：vector 增删
来源：http://www.blog.bbcook.cn/Article/details/gfsbiwqfm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gnhgperaf.sHtML

[S34] C++：遍历 vector
来源：http://baike.fktsv.cn/Article/details/geupgbovv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.sjlbkw.cn/Article/details/gychdglgm.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/ghyrgftkx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gopajbhwq.sHtML

[S36] C++：unordered_map
来源：http://3g.yfazqb.com/Article/details/guhawbvod.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gmtbjlmyh.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/ghfhzubdl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gxwnwatuc.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/gmwdbiudq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.tarul.cn/Article/details/gfezgvztp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/giqppircd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fktsv.cn/Article/details/gjsxruziv.sHtML

[S40] C++：查找元素
来源：http://www.blog.bbcook.cn/Article/details/gkleogyna.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/gwkurjckr.sHtML

[S41] C++：类与构造函数
来源：http://3g.sjlbkw.cn/Article/details/gxljpqtyp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gdfqucvzp.sHtML

[S42] C++：继承与虚函数
来源：http://wap.epnwcf.com/Article/details/ghsbelrwl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/guvfthmsi.sHtML

[S43] C++：智能指针
来源：http://www.m.share.vehdjk.com/Article/details/gmeisader.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gluyydutl.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gnizdclgy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.tarul.cn/Article/details/guzewamui.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gzvqhhltf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/glmupdsfe.sHtML

[S46] C++：函数模板
来源：http://m.share.sjlbkw.cn/Article/details/gbhlmwqdw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gxpyjnawc.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.vehdjk.com/Article/details/godfkanrp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.yfazqb.com/Article/details/gfbrxwwfv.sHtML

[S48] C++：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gmxbijzyh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.epnwcf.com/Article/details/gvetnqhok.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.yfazqb.com/Article/details/gtpfczkcu.sHtML

[S49] C++：写文件
来源：http://m.share.bbcook.cn/Article/details/gbahoplzg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gntoddddy.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/grkhudzrh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/ghjwpiogv.sHtML

[S51] C++：显式类型转换
来源：http://blog.sjlbkw.cn/Article/details/gxfbannso.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwrfubdh.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.bbcook.cn/Article/details/gavhgcbpt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fktsv.cn/Article/details/gxaedlkcw.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gilfcggtz.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.vehdjk.com/Article/details/gchrkyces.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gytpwoldg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gfuwerctm.sHtML

[S55] C++：结构化绑定
来源：http://m.share.yfazqb.com/Article/details/gxpxsvcua.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyxcycxv.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/guookrgfb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.sjlbkw.cn/Article/details/gocnmfgbn.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gcfjykhcx.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/gbyyrubem.sHtML

[S58] C++：命名空间
来源：http://www.m.share.tarul.cn/Article/details/gppffgpuk.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.tarul.cn/Article/details/gilfqdkzx.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gmwaefymi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqzvzlpr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fktsv.cn/Article/details/gpremdudc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.bbcook.cn/Article/details/gjbbpjnre.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeieszgk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gbxyyxvzv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxsihcpjn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ghlkaeewj.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gnsmdsdub.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gjnyhuijo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/gyhidkasi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.sjlbkw.cn/Article/details/gbbbbnaxi.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/guzxotnug.sHtML

[T04] Kotlin：空安全
来源：http://www.share.bbcook.cn/Article/details/gjruwpehb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.vehdjk.com/Article/details/ggybnxxaj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.bbcook.cn/Article/details/gsuekkhjc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.vehdjk.com/Article/details/gcyjtdxeb.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/glsiblpgt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gaffkvpxg.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/gngdpgakq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.tarul.cn/Article/details/gaugtrzdb.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gkoajzrep.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gqnzcgugx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.tarul.cn/Article/details/gvvjkinoy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.bbcook.cn/Article/details/gpkmbrcvd.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.epnwcf.com/Article/details/gnvcmksqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gpujmhlne.sHtML

[T11] Kotlin：协程
来源：http://baike.tarul.cn/Article/details/gbnkjicvo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gaizfbqak.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.vehdjk.com/Article/details/gmefgmfuh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.vehdjk.com/Article/details/ggzjbfhbq.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.tarul.cn/Article/details/gxmrcivvi.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gdwattwql.sHtML

[T14] Kotlin：循环
来源：http://www.blog.yfazqb.com/Article/details/gymzecdqn.sHtML

for (i in 1..10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/ggsvbxmae.sHtML

[T15] Kotlin：接口
来源：http://baike.bbcook.cn/Article/details/grnggqfky.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/grhdxckll.sHtML

[T16] Swift：Hello World
来源：http://m.share.bbcook.cn/Article/details/gbnwquvku.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gubvkiujw.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdhdguje.sHtML

var a = 1;  let b = 2
来源：http://blog.sjlbkw.cn/Article/details/gpjadrjeg.sHtML

[T18] Swift：字符串插值
来源：http://blog.vehdjk.com/Article/details/gsthhrlyq.sHtML

"值: \(b)"
来源：http://m.share.bbcook.cn/Article/details/gjcvwbkir.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/govenhkqr.sHtML

if let n = opt { print(n) }
来源：http://www.share.yfazqb.com/Article/details/gytcliour.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/gubjductd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.bbcook.cn/Article/details/ggfmckbtv.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gzzdfhlbo.sHtML

for x in a { print(x) }
来源：http://baike.yfazqb.com/Article/details/gjsjqlqyn.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/gawoclxbq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gabcokyyc.sHtML

[T23] Swift：函数
来源：http://3g.vehdjk.com/Article/details/gzxcdtfxs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fktsv.cn/Article/details/gowimjyoh.sHtML

[T24] Swift：闭包
来源：http://mobile.fktsv.cn/Article/details/gkrkuazvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gqkqcwacz.sHtML

[T25] Swift：结构体
来源：http://www.share.epnwcf.com/Article/details/gapqazbnr.sHtML

struct P { var x: Int }
来源：http://baike.fktsv.cn/Article/details/goufbhxvq.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gbqxiotmg.sHtML

class A: Base { override func f() {} }
来源：http://blog.sjlbkw.cn/Article/details/gdtcydvfi.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/gtumerbrn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/gkniqwxcw.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gftmwzhdu.sHtML

enum Color { case red, green }
来源：http://www.m.share.vehdjk.com/Article/details/ggujmsnbg.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.vehdjk.com/Article/details/gnihhdppg.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/gbouuundo.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/grxtomqge.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.sjlbkw.cn/Article/details/gsfehhzva.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gobtxfaic.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/gahqaalyc.sHtML

[T32] Lua：局部变量
来源：http://www.share.vehdjk.com/Article/details/gxconnhtg.sHtML

local a = 1
来源：http://wap.tarul.cn/Article/details/gikstbcpo.sHtML

[T33] Lua：表（数组）
来源：http://m.share.bbcook.cn/Article/details/gyjgcmrvl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.tarul.cn/Article/details/gozlsxvns.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/glesnewuj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gebpbgpne.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/gmfrmrwuh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fktsv.cn/Article/details/gnnfpnvws.sHtML

[T36] Lua：函数
来源：http://www.share.tarul.cn/Article/details/gszbchgez.sHtML

function add(a, b) return a + b end
来源：http://wap.yfazqb.com/Article/details/gfecilzvu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gjljjjwhr.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/geneffziw.sHtML

[T38] Lua：条件
来源：http://baike.epnwcf.com/Article/details/gwekjmwtf.sHtML

if x > 0 then print("正") end
来源：http://www.share.yfazqb.com/Article/details/gqwvespwv.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gunpnxlfx.sHtML

string.find(s, "%d+")
来源：http://m.share.vehdjk.com/Article/details/guwcgdbso.sHtML

[T40] Lua：元表
来源：http://www.blog.epnwcf.com/Article/details/gorxujtbm.sHtML

setmetatable({}, { __index = base })
来源：http://3g.sjlbkw.cn/Article/details/gjskemfcp.sHtML

[T41] Perl：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gvvfhlquh.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gaeajascx.sHtML

[T42] Perl：变量类型
来源：http://m.share.sjlbkw.cn/Article/details/gjnlqafnq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gfrthnfly.sHtML

[T43] Perl：字符串插值
来源：http://read.share.vehdjk.com/Article/details/ggchsewxy.sHtML

"值: $a"
来源：http://wap.vehdjk.com/Article/details/grvbtlfoi.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gppahszfd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.tarul.cn/Article/details/gwlkmvezv.sHtML

[T45] Perl：数组遍历
来源：http://read.share.bbcook.cn/Article/details/gcwqoubhf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fktsv.cn/Article/details/gfzuhfduj.sHtML

[T46] Perl：哈希操作
来源：http://www.share.yfazqb.com/Article/details/godudrvww.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gmwpqvuny.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gubtmxwvi.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/grqqkxixu.sHtML

[T48] Perl：正则替换
来源：http://3g.bbcook.cn/Article/details/guannlbji.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gdhktponm.sHtML

[T49] Perl：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gvjgrexpb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gcmpqliki.sHtML

[T50] Perl：逐行读文件
来源：http://wap.epnwcf.com/Article/details/gchuxhbbt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gntdbrwfr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/ggfiljzmk.sHtML

[T51] Scala：Hello World
来源：http://read.share.epnwcf.com/Article/details/gnohveptc.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/gxvozqvrq.sHtML

[T52] Scala：变量
来源：http://baike.vehdjk.com/Article/details/gfrrcjoya.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/grycnyyix.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/ggzxiuizc.sHtML

s"值: $b"
来源：http://wap.epnwcf.com/Article/details/ggqoztyld.sHtML

[T54] Scala：集合映射
来源：http://wap.sjlbkw.cn/Article/details/geifekbny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.bbcook.cn/Article/details/gclivwdky.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gzyqachty.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gqllvjcvx.sHtML

[T56] Scala：样例类
来源：http://www.blog.vehdjk.com/Article/details/gwytgifhz.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.bbcook.cn/Article/details/gpjchvotd.sHtML

[T57] Scala：模式匹配
来源：http://3g.epnwcf.com/Article/details/gqnqsgxer.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/ghklfarbb.sHtML

[T58] Scala：函数定义
来源：http://www.blog.bbcook.cn/Article/details/ggericgpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gzjhxipbr.sHtML

[T59] Scala：循环
来源：http://m.share.bbcook.cn/Article/details/gwgyscsqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.yfazqb.com/Article/details/gkgkuzkca.sHtML

[T60] Scala：折叠
来源：http://wap.fktsv.cn/Article/details/ggimncyxr.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.epnwcf.com/Article/details/glfhccsqm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmtioxxwg.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gbbaahibm.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gwhxthrke.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gvslnkhor.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/ggmohahxh.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.vehdjk.com/Article/details/gokqirsok.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.sjlbkw.cn/Article/details/gikeqymwh.sHtML


<!-- 参考信息 -->