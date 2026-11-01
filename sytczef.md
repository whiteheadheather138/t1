代发 wailian999

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/gdjfvhfkm.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/glrlwiumj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gbkyvhgfk.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gklkfmurb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/ggzuknqen.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/gneqdeezb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyylrlhq.sHtML

[R65] 查看端口占用
来源：http://baike.epnwcf.com/Article/details/gncxdwbhl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gangknxea.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/glqvztjtk.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/ggfqtacml.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.tarul.cn/Article/details/glmjexnco.sHtML

openssl rand -hex 16
来源：http://www.m.share.yfazqb.com/Article/details/ghgfqgxgi.sHtML

[R68] 计算文件校验值
来源：http://wap.epnwcf.com/Article/details/gtnwqaskh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.tarul.cn/Article/details/gjxakbbbk.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/ggnobuawv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.epnwcf.com/Article/details/gxdahfiuy.sHtML

[R70] 时间戳与互转
来源：http://blog.fktsv.cn/Article/details/gtoczbrfs.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.yfazqb.com/Article/details/glxoepold.sHtML

[R71] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gxoeoorke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.tarul.cn/Article/details/gcadptdfn.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.sjlbkw.cn/Article/details/gagfffkpu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gavtjptwk.sHtML

[R73] 分割大日志
来源：http://www.m.share.yfazqb.com/Article/details/gvdurfnps.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gavzelgbo.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/geyuvzgxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gfstdjtoe.sHtML

[R75] 导出环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/guknqgbko.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gytbfgbzx.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/grrdkrwwx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.yfazqb.com/Article/details/gughggdbc.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/gpjcnevqs.sHtML

read -rp "请输入: " ans
来源：http://wap.sjlbkw.cn/Article/details/gweamlblc.sHtML

[R78] 交互式菜单
来源：http://www.share.sjlbkw.cn/Article/details/gdrbzoxio.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gcwomezwd.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gcscbxrmh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.yfazqb.com/Article/details/gzpzrktfz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/gnjojlnlu.sHtML

time ./run.sh
来源：http://m.share.vehdjk.com/Article/details/gatbbrdgl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxfjvpksm.sHtML

S. C / C++ 专题
来源：http://wap.epnwcf.com/Article/details/gaoneiglg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/goxiyitxb.sHtML

[S01] C：Hello World
来源：http://wap.yfazqb.com/Article/details/gnignebfd.sHtML

#include <stdio.h>
来源：http://m.share.fktsv.cn/Article/details/gcrqqsnsz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.bbcook.cn/Article/details/ggktfrnbj.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.bbcook.cn/Article/details/giyrkawjd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gibgmufzp.sHtML

[S03] C：读入整数
来源：http://3g.bbcook.cn/Article/details/gmscgmxve.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/gnswegjaa.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fktsv.cn/Article/details/giwhrmycv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gspyoduux.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/gibnmszws.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gznabebud.sHtML

[S06] C：字符串比较
来源：http://read.share.fktsv.cn/Article/details/gbvlxxxyq.sHtML

strcmp(a, b) == 0
来源：http://mobile.yfazqb.com/Article/details/glksyjotm.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gsngcekjs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gtzsfemso.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gptbvzsut.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.yfazqb.com/Article/details/gimvubvqx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.vehdjk.com/Article/details/gktbdzgdq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/ghmtmskgv.sHtML

[S10] C：指针与解引用
来源：http://blog.yfazqb.com/Article/details/gcifhitil.sHtML

int *p = &a;  *p = 5;
来源：http://blog.yfazqb.com/Article/details/gwwxzhqfz.sHtML

[S11] C：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gtrqbqfhx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.epnwcf.com/Article/details/gqaoenxlk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.epnwcf.com/Article/details/gpnzxdbfk.sHtML

fclose(f);
来源：http://baike.vehdjk.com/Article/details/gnzoyuchu.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gnozvxkrw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gnzixaqrc.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/gcozgdegs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fktsv.cn/Article/details/giornqmbf.sHtML

[S14] C：枚举
来源：http://wap.epnwcf.com/Article/details/gvujxgsqa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.yfazqb.com/Article/details/gfqyprizf.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gsqclynbu.sHtML

(double) a / b
来源：http://m.share.tarul.cn/Article/details/gxykzfylk.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gdzlwnits.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/grrlqswsl.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gbeykriri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gttmaqiew.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/gvvvjbpfz.sHtML

int main(int argc, char **argv)
来源：http://m.share.yfazqb.com/Article/details/gaomvbgvy.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/ggntchqro.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/gsssdncsx.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gxttphqxa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gnpoiykwr.sHtML

[S21] C：字符类别判断
来源：http://wap.epnwcf.com/Article/details/gedubgtyq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gymvujmzr.sHtML

[S22] C：字符串转数字
来源：http://blog.vehdjk.com/Article/details/ggtlubtfu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gddberzbe.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gvztywxeh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/grtiasqsi.sHtML

[S24] C：获取本地时间
来源：http://wap.bbcook.cn/Article/details/gcatotlcu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gffyhbwpg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gcucconou.sHtML

memcpy(dst, src, n);
来源：http://m.share.vehdjk.com/Article/details/gazpofibo.sHtML

[S26] C：内存清零
来源：http://blog.yfazqb.com/Article/details/gfhhgaklv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.yfazqb.com/Article/details/gftokmqdt.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/gyvgivqaf.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gxbnkbpny.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gbragzjyk.sHtML

static int counter = 0;
来源：http://wap.vehdjk.com/Article/details/gxzmktbbz.sHtML

[S29] C：变参函数
来源：http://wap.epnwcf.com/Article/details/gjowewvjc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/gpaoxhptt.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/gxnmbfeqv.sHtML

#ifndef X_H
来源：http://3g.fktsv.cn/Article/details/gseyvicye.sHtML

#define X_H
来源：http://baike.tarul.cn/Article/details/gtsyiwzwv.sHtML

#endif
来源：http://mobile.bbcook.cn/Article/details/ghqxelufv.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gzccscueu.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gxdsdetdc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/ghgwxtwdk.sHtML

[S32] C++：字符串
来源：http://www.m.share.epnwcf.com/Article/details/gxzgsxasd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.yfazqb.com/Article/details/gdmucwebl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gahulvmez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gtlpjhpag.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fktsv.cn/Article/details/goyhvxual.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gifwduhoo.sHtML

[S35] C++：map
来源：http://3g.bbcook.cn/Article/details/gtuddebyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gnmxcmppk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.tarul.cn/Article/details/ghhqucmfc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gpuyumvgl.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/guxfqbcgt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/grjmcjnug.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/gqqkxmeaq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gnmkwwwgv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.tarul.cn/Article/details/gsxbfmmih.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fktsv.cn/Article/details/gfmritrrb.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gdwionguw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.tarul.cn/Article/details/gxqhinafa.sHtML

[S41] C++：类与构造函数
来源：http://www.share.tarul.cn/Article/details/gpecnprbf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.vehdjk.com/Article/details/giddnbqem.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fktsv.cn/Article/details/golpvmhvl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/ggjblerxf.sHtML

[S43] C++：智能指针
来源：http://mobile.fktsv.cn/Article/details/gwurkcwvx.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.bbcook.cn/Article/details/gtrwpyrzn.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fktsv.cn/Article/details/gezgbavzs.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.tarul.cn/Article/details/gkjzuyqhn.sHtML

[S45] C++：lambda
来源：http://m.share.tarul.cn/Article/details/galatmrpk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gsvewcred.sHtML

[S46] C++：函数模板
来源：http://wap.fktsv.cn/Article/details/gzzefanmk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fktsv.cn/Article/details/gzokksuzv.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gtdvatshc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gynwkdxlk.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gsasfjsdk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.tarul.cn/Article/details/gzogfzvle.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gnzxgyhpj.sHtML

[S49] C++：写文件
来源：http://blog.yfazqb.com/Article/details/gioajoexf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.tarul.cn/Article/details/gfiehzzsz.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/geysmysnr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gzzzyylnz.sHtML

[S51] C++：显式类型转换
来源：http://baike.epnwcf.com/Article/details/gjxjhozrt.sHtML

static_cast<double>(a) / b
来源：http://m.share.yfazqb.com/Article/details/gevbpkgxl.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gpkimynqf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/gpqtjsitk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fktsv.cn/Article/details/gqiqjbuai.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gdfawvvaz.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/ggfvclmkz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gxwcxhfqf.sHtML

[S55] C++：结构化绑定
来源：http://wap.sjlbkw.cn/Article/details/gnlddtgug.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.sjlbkw.cn/Article/details/gxunwnsvv.sHtML

[S56] C++：optional
来源：http://m.share.vehdjk.com/Article/details/gyxdehlio.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.vehdjk.com/Article/details/gvjdfvjwe.sHtML

[S57] C++：编译期常量
来源：http://www.share.epnwcf.com/Article/details/glsnmgfvk.sHtML

constexpr int N = 10;
来源：http://baike.yfazqb.com/Article/details/gkpeehfxz.sHtML

[S58] C++：命名空间
来源：http://www.share.fktsv.cn/Article/details/gkelridrw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/grezvivct.sHtML

[S59] C++：静态断言
来源：http://baike.sjlbkw.cn/Article/details/gqhehuura.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gdrdecrfg.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.yfazqb.com/Article/details/gtwcmqskl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.vehdjk.com/Article/details/gdhskmugn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyarlihrf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gvantwoax.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gixxwnifb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gaiirvqpj.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gadbhoagb.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/gytoovknp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gujqgwqfv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/goayuocrw.sHtML

"值: $b"
来源：http://www.blog.fktsv.cn/Article/details/ghkfhannd.sHtML

[T04] Kotlin：空安全
来源：http://m.share.bbcook.cn/Article/details/gcbpqkdjr.sHtML

val n: String? = null;  n?.length
来源：http://blog.bbcook.cn/Article/details/goucsqhxv.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gvjgvotjh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gsknriycv.sHtML

[T06] Kotlin：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gtzvnzjfv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.vehdjk.com/Article/details/gjdutehea.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/ghozfkwjt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gfivcpssz.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gdnycmbsp.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gklhcnkyz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gwwbxprqz.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gdbdgtwng.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/ggwbsndeo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.bbcook.cn/Article/details/ghzbgxsdq.sHtML

[T11] Kotlin：协程
来源：http://www.share.epnwcf.com/Article/details/gkqavfyst.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gdgglsujl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.epnwcf.com/Article/details/gfcaknaxr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.tarul.cn/Article/details/grqyamojh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.sjlbkw.cn/Article/details/gdfojvais.sHtML

val m = mapOf("a" to 1)
来源：http://baike.vehdjk.com/Article/details/gywugtpxx.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/ghrinsmrx.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gvjoakwvv.sHtML

[T15] Kotlin：接口
来源：http://www.blog.vehdjk.com/Article/details/gpfmyphlf.sHtML

interface Shape { fun area(): Double }
来源：http://blog.vehdjk.com/Article/details/gtmwlxsuw.sHtML

[T16] Swift：Hello World
来源：http://blog.tarul.cn/Article/details/gfyayztun.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gpvtlarwb.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gkiitkfft.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/gotzymdhh.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/ggquovmai.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/gyvzkgcwv.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gvsctdckq.sHtML

if let n = opt { print(n) }
来源：http://3g.yfazqb.com/Article/details/ghlkbcgzo.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gmpaioemm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gbckloloj.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gxkgdzoin.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gjkgeeboi.sHtML

[T22] Swift：字典
来源：http://www.share.bbcook.cn/Article/details/gtesmmfdt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.vehdjk.com/Article/details/gcxgzodmg.sHtML

[T23] Swift：函数
来源：http://www.blog.fktsv.cn/Article/details/gpumhcmjn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.bbcook.cn/Article/details/guiihdyfi.sHtML

[T24] Swift：闭包
来源：http://www.share.bbcook.cn/Article/details/gthdaupgi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gtsowsrbp.sHtML

[T25] Swift：结构体
来源：http://mobile.vehdjk.com/Article/details/gvzrcnjaq.sHtML

struct P { var x: Int }
来源：http://baike.epnwcf.com/Article/details/gipvzawad.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/ggraiivyo.sHtML

class A: Base { override func f() {} }
来源：http://baike.fktsv.cn/Article/details/gtqvlreex.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gzcymwedf.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fktsv.cn/Article/details/gvbybmgwv.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gqsdkctno.sHtML

enum Color { case red, green }
来源：http://wap.fktsv.cn/Article/details/gyqoftpdl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gixgmbqbv.sHtML

guard let x = opt else { return }
来源：http://read.share.tarul.cn/Article/details/gbdzrujmd.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gaqloaoch.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.yfazqb.com/Article/details/gmomqpdvt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gkfuzdayy.sHtML

print("Hello")
来源：http://mobile.fktsv.cn/Article/details/golrmgzwb.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gekegpytx.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/ghqtsrhwj.sHtML

[T33] Lua：表（数组）
来源：http://baike.bbcook.cn/Article/details/glggurgjy.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fktsv.cn/Article/details/goonvaqii.sHtML

[T34] Lua：遍历表
来源：http://read.share.sjlbkw.cn/Article/details/gwdmhazuj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gjyfvlldg.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/gcormyaye.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.tarul.cn/Article/details/ghoudclwk.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/ghhjtpbff.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gsmdhpboo.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.sjlbkw.cn/Article/details/gimcwunpc.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gcyfzrtsq.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gzjluqyfp.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.yfazqb.com/Article/details/gmnyetman.sHtML

[T39] Lua：模式匹配
来源：http://m.share.epnwcf.com/Article/details/gbmjrogqc.sHtML

string.find(s, "%d+")
来源：http://read.share.vehdjk.com/Article/details/gdmzyogmy.sHtML

[T40] Lua：元表
来源：http://mobile.bbcook.cn/Article/details/gdgajmqdq.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.epnwcf.com/Article/details/gjdhpahxt.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gqeigwxop.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/gexwyypgd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gulunxgql.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gnmmkhjgg.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/grwnfhela.sHtML

"值: $a"
来源：http://baike.epnwcf.com/Article/details/gxexfyvlh.sHtML

[T44] Perl：条件
来源：http://mobile.vehdjk.com/Article/details/glywkiobn.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gykdzaefb.sHtML

[T45] Perl：数组遍历
来源：http://baike.tarul.cn/Article/details/gahfpmlao.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.tarul.cn/Article/details/gzlruujcs.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gqoapveol.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gxetlvawd.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gqrmdvcks.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gppornxxd.sHtML

[T48] Perl：正则替换
来源：http://3g.sjlbkw.cn/Article/details/giilgalkc.sHtML

$s =~ s/old/new/g;
来源：http://blog.fktsv.cn/Article/details/ggsubkuwn.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gdwyhaaku.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/ggqxqymwx.sHtML

[T50] Perl：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gywehkvai.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.sjlbkw.cn/Article/details/gecmjoavs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gframifre.sHtML

[T51] Scala：Hello World
来源：http://3g.vehdjk.com/Article/details/gtmstgfcw.sHtML

println("Hello")
来源：http://m.share.epnwcf.com/Article/details/gsalawshz.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gnediwgqb.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/glaqapdzg.sHtML

[T53] Scala：字符串插值
来源：http://m.share.bbcook.cn/Article/details/grqcdfvfp.sHtML

s"值: $b"
来源：http://mobile.fktsv.cn/Article/details/ghzdcfpmi.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/guwfbxymh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.bbcook.cn/Article/details/grcfghhib.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.vehdjk.com/Article/details/gpttvzujh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.epnwcf.com/Article/details/gkhhhbshx.sHtML

[T56] Scala：样例类
来源：http://baike.sjlbkw.cn/Article/details/gtibefglw.sHtML

case class User(name: String, age: Int)
来源：http://3g.bbcook.cn/Article/details/glcshccgp.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gwnvnkfne.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.epnwcf.com/Article/details/gvilhuxqt.sHtML

[T58] Scala：函数定义
来源：http://blog.yfazqb.com/Article/details/gwcufakkl.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.sjlbkw.cn/Article/details/gaprhmzaj.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gdzzswzmg.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.sjlbkw.cn/Article/details/gurmchffb.sHtML

[T60] Scala：折叠
来源：http://read.share.bbcook.cn/Article/details/gmvlrswqd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/gotbycxgp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcmabarxs.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gidxrvzvs.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glohfydqe.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gebtbtiff.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.sjlbkw.cn/Article/details/gzxumslvi.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.yfazqb.com/Article/details/gpesdrgsk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gncmqhbre.sHtML


<!-- 参考信息 -->