代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gzjyhoyic.sHtML

[R66] 定时任务
来源：http://baike.bbcook.cn/Article/details/gxxeinixt.sHtML

crontab -e;  crontab -l
来源：http://mobile.tarul.cn/Article/details/gbnmwwoog.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.epnwcf.com/Article/details/gegcbcwxd.sHtML

openssl rand -hex 16
来源：http://baike.epnwcf.com/Article/details/gyeadqbvu.sHtML

[R68] 计算文件校验值
来源：http://3g.bbcook.cn/Article/details/gjllrvrtm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.vehdjk.com/Article/details/gthqdxfgm.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gyljbbnwl.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.vehdjk.com/Article/details/gejmlxist.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gvyxglrvt.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.sjlbkw.cn/Article/details/gnlxuqotd.sHtML

[R71] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gqmvgdmwj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gnwbqzika.sHtML

[R72] 等待端口就绪
来源：http://www.share.tarul.cn/Article/details/gmcflnxtf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gbliwnxzz.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gqjqgkvcu.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/geypzcfqo.sHtML

[R74] 批量重命名
来源：http://read.share.sjlbkw.cn/Article/details/goncujhsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/gvlizecus.sHtML

[R75] 导出环境变量
来源：http://mobile.tarul.cn/Article/details/grcdnxqiz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.vehdjk.com/Article/details/grnzeorko.sHtML

[R76] 使用临时文件
来源：http://wap.bbcook.cn/Article/details/gjevlphgz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gditxnmqi.sHtML

[R77] 读取用户输入
来源：http://mobile.yfazqb.com/Article/details/gmyyixyoa.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/gotlynzxd.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gwktedjie.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.yfazqb.com/Article/details/gvqxnzmka.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/gptdkovfh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fktsv.cn/Article/details/ghtfhwoll.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fktsv.cn/Article/details/guszlzlmn.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gqoewfdep.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gknvzcqih.sHtML

S. C / C++ 专题
来源：http://mobile.tarul.cn/Article/details/glovhsdut.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjmlfghkq.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gkinrivcn.sHtML

#include <stdio.h>
来源：http://www.m.share.tarul.cn/Article/details/gscrjyezt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fktsv.cn/Article/details/ggcxdvmoo.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.vehdjk.com/Article/details/gvojcchrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/glkoaocvr.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gzbrbwgqu.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.vehdjk.com/Article/details/goijrhjde.sHtML

[S04] C：字符串复制
来源：http://blog.tarul.cn/Article/details/gcttfxths.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.epnwcf.com/Article/details/gncirojvg.sHtML

[S05] C：字符串长度
来源：http://blog.epnwcf.com/Article/details/gvxfmvnnm.sHtML

strlen(s)
来源：http://mobile.bbcook.cn/Article/details/gfycospuu.sHtML

[S06] C：字符串比较
来源：http://www.blog.tarul.cn/Article/details/ghupmvnap.sHtML

strcmp(a, b) == 0
来源：http://www.blog.bbcook.cn/Article/details/guuexbtep.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gczhmrxhu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.sjlbkw.cn/Article/details/guqiqsrdm.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/ghwzgyifh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.vehdjk.com/Article/details/gefrgutis.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gcapvueiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gjckqrdpd.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gneoboiql.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fktsv.cn/Article/details/gvzmwoase.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gjwbtpumd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.yfazqb.com/Article/details/gojwgzrdw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gsrfafkrp.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/ggufnfnht.sHtML

[S12] C：写文件
来源：http://blog.yfazqb.com/Article/details/gxfypejwe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.epnwcf.com/Article/details/gazceexpl.sHtML

[S13] C：宏定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzgdzrmw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.bbcook.cn/Article/details/gzkdpddyn.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gphwblvsw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.bbcook.cn/Article/details/gyqahkcjl.sHtML

[S15] C：类型转换
来源：http://read.share.tarul.cn/Article/details/geahhnxjf.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gawrhafar.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/ggrvabmpn.sHtML

x |= (1 << 3);
来源：http://wap.vehdjk.com/Article/details/goccmpgim.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gipjktqvw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gyiytmiab.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gkoeyexpv.sHtML

int main(int argc, char **argv)
来源：http://3g.epnwcf.com/Article/details/gnrqnfjlf.sHtML

[S19] C：快速排序
来源：http://3g.sjlbkw.cn/Article/details/ghmnrmayw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gxdogfgpf.sHtML

[S20] C：二分查找
来源：http://www.share.yfazqb.com/Article/details/gayfixzpg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gfmzeskzn.sHtML

[S21] C：字符类别判断
来源：http://wap.vehdjk.com/Article/details/gbrpxsflk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.vehdjk.com/Article/details/gfcosyfsl.sHtML

[S22] C：字符串转数字
来源：http://baike.epnwcf.com/Article/details/gwrxrwsaz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/gohvxsabp.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gqifhymwa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fktsv.cn/Article/details/gnbwuhoem.sHtML

[S24] C：获取本地时间
来源：http://blog.yfazqb.com/Article/details/gvzdqvjak.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.vehdjk.com/Article/details/gfcwxrmbk.sHtML

[S25] C：内存拷贝
来源：http://baike.yfazqb.com/Article/details/gtdyutazv.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/gfxwprpkf.sHtML

[S26] C：内存清零
来源：http://www.m.share.epnwcf.com/Article/details/gcifaaeyz.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gfadvgrnd.sHtML

[S27] C：定义常量
来源：http://3g.yfazqb.com/Article/details/gghfqiurh.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gjsxtfgyt.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gkgonifyi.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gcihjzjuf.sHtML

[S29] C：变参函数
来源：http://blog.vehdjk.com/Article/details/gsilwjskn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.tarul.cn/Article/details/glwnwjqpp.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gpzxsmzxz.sHtML

#ifndef X_H
来源：http://read.share.fktsv.cn/Article/details/gnrphqhzj.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gyrwzltup.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gfrgcglcs.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/gajjgvgby.sHtML

#include <iostream>
来源：http://3g.vehdjk.com/Article/details/grfitmqkn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.sjlbkw.cn/Article/details/georrauki.sHtML

[S32] C++：字符串
来源：http://wap.epnwcf.com/Article/details/gmsyugmyp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/gfaknqzhy.sHtML

[S33] C++：vector 增删
来源：http://mobile.fktsv.cn/Article/details/gknnkhrmv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/glihutwbn.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gonkjsllm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.tarul.cn/Article/details/gugtfoild.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/geduvzibf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gikuahfgz.sHtML

[S36] C++：unordered_map
来源：http://baike.epnwcf.com/Article/details/gpgoncvng.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gsbyykpky.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gsaywkcyi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/grxuaujlg.sHtML

[S38] C++：排序
来源：http://www.m.share.epnwcf.com/Article/details/grbmpdfjh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gzvxuzeny.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.epnwcf.com/Article/details/gpoqbjkjp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/ggyqgiwtj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.epnwcf.com/Article/details/gyklkazqt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.epnwcf.com/Article/details/grpctnggb.sHtML

[S41] C++：类与构造函数
来源：http://wap.tarul.cn/Article/details/gnbqpruid.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.tarul.cn/Article/details/gsfrsodny.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.tarul.cn/Article/details/ggmslydxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuiureht.sHtML

[S43] C++：智能指针
来源：http://read.share.bbcook.cn/Article/details/gakcntjyj.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.sjlbkw.cn/Article/details/gbjwscnjn.sHtML

[S44] C++：引用传参
来源：http://m.share.sjlbkw.cn/Article/details/gzwdlrfud.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.tarul.cn/Article/details/gkhnskvpq.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gvmvsuafc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fktsv.cn/Article/details/gjkmagyjc.sHtML

[S46] C++：函数模板
来源：http://read.share.bbcook.cn/Article/details/gjvyxpwjy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gmyqlgwac.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/ghorxhszv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gabyfdxzv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gmbhyxafp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gaykqmvej.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/goxbtxgsx.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gdgzdejrt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gcivenrnv.sHtML

[S50] C++：格式化数字
来源：http://read.share.bbcook.cn/Article/details/gtnkxyoou.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gqrbzsnvf.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gfnezofdx.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/googgocxx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/gvavxkslq.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gmhewqedn.sHtML

[S53] C++：移动语义
来源：http://mobile.tarul.cn/Article/details/gqehircba.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gfrdkrcwm.sHtML

[S54] C++：异常处理
来源：http://mobile.sjlbkw.cn/Article/details/gmhbbozmw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/ghxkyevoz.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fktsv.cn/Article/details/guebskwgr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.sjlbkw.cn/Article/details/guepbzrwm.sHtML

[S56] C++：optional
来源：http://blog.yfazqb.com/Article/details/gdaxlwvof.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/grzbufmjw.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/gylnqtvtx.sHtML

constexpr int N = 10;
来源：http://blog.fktsv.cn/Article/details/gdfzpyfdp.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gaydhkqdr.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fktsv.cn/Article/details/gopntpfrp.sHtML

[S59] C++：静态断言
来源：http://www.m.share.bbcook.cn/Article/details/grosgdovb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fktsv.cn/Article/details/giebxnlsl.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gtkvszxvx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.epnwcf.com/Article/details/giidommxu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gzlymygsu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.sjlbkw.cn/Article/details/gavxjxhnq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gycivobnc.sHtML

[T01] Kotlin：Hello World
来源：http://wap.tarul.cn/Article/details/gaqfrelsw.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gpnmjigae.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gezmjpdyg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.sjlbkw.cn/Article/details/gyrcoznwr.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.bbcook.cn/Article/details/gbcfguaje.sHtML

"值: $b"
来源：http://3g.epnwcf.com/Article/details/ghpgaxogp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/glqvvoegv.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gxqkkftfc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/gwzioykrs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.yfazqb.com/Article/details/ghqbdkima.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/grgmefppm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/guauywwsr.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/ggauylmnt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.epnwcf.com/Article/details/gsfbqvjna.sHtML

[T08] Kotlin：数据类
来源：http://blog.tarul.cn/Article/details/ggdfkczwp.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.sjlbkw.cn/Article/details/gnhxvigcv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.bbcook.cn/Article/details/gqlgxfoiu.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.vehdjk.com/Article/details/gmyygkucm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fktsv.cn/Article/details/gflmwvndv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/gucpqkigj.sHtML

[T11] Kotlin：协程
来源：http://blog.sjlbkw.cn/Article/details/gussldhjy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.bbcook.cn/Article/details/gkqyfjbbe.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gztrlrkbx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/ghaqprspd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.epnwcf.com/Article/details/gcbutxtwx.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gyvopgbxr.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gkmrdgiay.sHtML

for (i in 1..10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gpflezeqi.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gtsmghjla.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gtyyphdti.sHtML

[T16] Swift：Hello World
来源：http://mobile.epnwcf.com/Article/details/gdvdwphlj.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gkkigdpyr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gqxqmpgzs.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gicsdnarn.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/guldlkihv.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/ghamhydsp.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gulpsrdfl.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gecrhwkjl.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gdldjabmi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.sjlbkw.cn/Article/details/glrahczrm.sHtML

[T21] Swift：遍历
来源：http://wap.sjlbkw.cn/Article/details/gffkhyxbw.sHtML

for x in a { print(x) }
来源：http://read.share.vehdjk.com/Article/details/gtvhvdzeh.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/glpwcdxcz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.vehdjk.com/Article/details/gfxyyexsp.sHtML

[T23] Swift：函数
来源：http://www.m.share.tarul.cn/Article/details/getqmukfs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.tarul.cn/Article/details/gcltdcped.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/goqelztel.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fktsv.cn/Article/details/gzdgwhcuf.sHtML

[T25] Swift：结构体
来源：http://read.share.yfazqb.com/Article/details/gtfrqxsvm.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gvbbajtrg.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gmretgtnx.sHtML

class A: Base { override func f() {} }
来源：http://3g.vehdjk.com/Article/details/gyuqmpyqm.sHtML

[T27] Swift：错误处理
来源：http://mobile.vehdjk.com/Article/details/gzzevxhmc.sHtML

do { try f() } catch { print(error) }
来源：http://baike.bbcook.cn/Article/details/gczffmekv.sHtML

[T28] Swift：枚举
来源：http://www.share.vehdjk.com/Article/details/gbguocxsd.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gozzosips.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/gercxejnh.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/gxcsuaykv.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gfoduwgoe.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.epnwcf.com/Article/details/gzfyewgci.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/gaaclynmo.sHtML

print("Hello")
来源：http://wap.tarul.cn/Article/details/gmznbglly.sHtML

[T32] Lua：局部变量
来源：http://read.share.tarul.cn/Article/details/gxsdhfiqh.sHtML

local a = 1
来源：http://read.share.epnwcf.com/Article/details/gwflkhsco.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gcmbxskup.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.epnwcf.com/Article/details/gyrhkvjym.sHtML

[T34] Lua：遍历表
来源：http://m.share.vehdjk.com/Article/details/gkkuivekq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.epnwcf.com/Article/details/gfdywvwht.sHtML

[T35] Lua：字典表
来源：http://m.share.fktsv.cn/Article/details/gjudjdovf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/gslmasfce.sHtML

[T36] Lua：函数
来源：http://wap.sjlbkw.cn/Article/details/gfrwmfapi.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gnqrlqbfo.sHtML

[T37] Lua：字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gveqiubkn.sHtML

"a" .. "b"
来源：http://blog.tarul.cn/Article/details/ggngiwaar.sHtML

[T38] Lua：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gapfphhit.sHtML

if x > 0 then print("正") end
来源：http://mobile.yfazqb.com/Article/details/gnlnekesv.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gtadipjiu.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gxupozcsf.sHtML

[T40] Lua：元表
来源：http://www.share.yfazqb.com/Article/details/gdtfzliew.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gkaileujg.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gmiuoszze.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gnmwvdewl.sHtML

[T42] Perl：变量类型
来源：http://read.share.sjlbkw.cn/Article/details/gobamwfat.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gvufsuamb.sHtML

[T43] Perl：字符串插值
来源：http://wap.vehdjk.com/Article/details/gcppxqsnd.sHtML

"值: $a"
来源：http://3g.bbcook.cn/Article/details/gtzuywtzt.sHtML

[T44] Perl：条件
来源：http://blog.sjlbkw.cn/Article/details/ggrlkgnaw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/gbqekxtfx.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.bbcook.cn/Article/details/giustayof.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gnvhjcrsn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.sjlbkw.cn/Article/details/gythswfah.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.vehdjk.com/Article/details/gyrljecpw.sHtML

[T47] Perl：正则捕获
来源：http://read.share.sjlbkw.cn/Article/details/gevidbfov.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.yfazqb.com/Article/details/gkojhdcbs.sHtML

[T48] Perl：正则替换
来源：http://www.share.tarul.cn/Article/details/gohozejbl.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/grvhjaxqx.sHtML

[T49] Perl：函数
来源：http://mobile.bbcook.cn/Article/details/gpnlkstyi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/gmrpesrud.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gfsxrrwtu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gfldoefik.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/gulsqazgp.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gjxjguqsm.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/gcvsjktsu.sHtML

[T52] Scala：变量
来源：http://m.share.vehdjk.com/Article/details/guymtkgrq.sHtML

val a = 1;  var b = 2
来源：http://www.blog.epnwcf.com/Article/details/gjqalikur.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gnelxertg.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gbpssxsra.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gvvfyzksm.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.sjlbkw.cn/Article/details/gdndynapn.sHtML

[T55] Scala：集合过滤
来源：http://read.share.bbcook.cn/Article/details/gjxpozjuy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gkzlehxtw.sHtML

[T56] Scala：样例类
来源：http://read.share.vehdjk.com/Article/details/gjfjvidnf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.bbcook.cn/Article/details/gdbgjakwn.sHtML

[T57] Scala：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gojduiprk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gvxhzpdlk.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/galvdkzhg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gtlwvcltt.sHtML

[T59] Scala：循环
来源：http://mobile.vehdjk.com/Article/details/gxblmzpth.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.tarul.cn/Article/details/gzpdyuonl.sHtML

[T60] Scala：折叠
来源：http://www.share.yfazqb.com/Article/details/guodhzcye.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.tarul.cn/Article/details/gaivyuuzd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gulpaykni.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/givjnokxe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqwfozbnh.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gfuzkqbid.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gjsirvvfw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.tarul.cn/Article/details/gscsgwmxu.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gzgzpgsuy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gmfsersgh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://read.share.fktsv.cn/Article/details/ggwduartj.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gfdgdqdio.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.vehdjk.com/Article/details/ghjpfkmnc.sHtML

[U05] Py：列表去重且保序
来源：http://wap.vehdjk.com/Article/details/gnfynxegk.sHtML

list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gdkfpahgw.sHtML

[U06] Py：合并两个字典
来源：http://baike.tarul.cn/Article/details/gylfitonx.sHtML

{**a, **b}
来源：http://m.share.epnwcf.com/Article/details/gbibwzbli.sHtML


<!-- 参考信息 -->