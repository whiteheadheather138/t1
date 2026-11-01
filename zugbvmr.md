代发 wailian999

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/guypjcfzf.sHtML

[R64] 结束进程
来源：http://wap.epnwcf.com/Article/details/gpuotvjur.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.bbcook.cn/Article/details/gmbkdlssa.sHtML

[R65] 查看端口占用
来源：http://3g.sjlbkw.cn/Article/details/gokgbiptv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.vehdjk.com/Article/details/gtqdkdjze.sHtML

[R66] 定时任务
来源：http://blog.sjlbkw.cn/Article/details/gykqscqcd.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gdneclgjl.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.yfazqb.com/Article/details/gmfrwvfwb.sHtML

openssl rand -hex 16
来源：http://mobile.bbcook.cn/Article/details/gyiyumsnf.sHtML

[R68] 计算文件校验值
来源：http://baike.fktsv.cn/Article/details/gheztnoad.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.bbcook.cn/Article/details/gabviirtz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.epnwcf.com/Article/details/gndlivqmg.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fktsv.cn/Article/details/gzjdpxute.sHtML

[R70] 时间戳与互转
来源：http://read.share.tarul.cn/Article/details/gakxleyiw.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/guetqpfkz.sHtML

[R71] 日期格式化
来源：http://blog.yfazqb.com/Article/details/gthophywh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.epnwcf.com/Article/details/gtyokrrkx.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/gavaglonk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gzshyrubi.sHtML

[R73] 分割大日志
来源：http://baike.sjlbkw.cn/Article/details/giuspwaqv.sHtML

split -l 1000 big.log part_
来源：http://m.share.bbcook.cn/Article/details/ggwouacaa.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gylhiquxm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/gxrjplxio.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/gkxdgclam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gkfshkvsf.sHtML

[R76] 使用临时文件
来源：http://wap.vehdjk.com/Article/details/gvlsnoiji.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.epnwcf.com/Article/details/ghlgatqin.sHtML

[R77] 读取用户输入
来源：http://www.share.epnwcf.com/Article/details/gakdnugor.sHtML

read -rp "请输入: " ans
来源：http://wap.vehdjk.com/Article/details/guoqaqnsl.sHtML

[R78] 交互式菜单
来源：http://baike.bbcook.cn/Article/details/gwritufmr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gwxdydtjp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.vehdjk.com/Article/details/gluvioyrf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.vehdjk.com/Article/details/gbpbkfmku.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/ggxkauyxb.sHtML

time ./run.sh
来源：http://www.blog.bbcook.cn/Article/details/glaruwkat.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gqyjucqkn.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/giaauwxdi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gkcsjrqfp.sHtML

[S01] C：Hello World
来源：http://baike.tarul.cn/Article/details/giabhbdoq.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gzjuqejgc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gmdjqlfxz.sHtML

[S02] C：变量与格式化输出
来源：http://wap.vehdjk.com/Article/details/gjkpjgxmz.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.vehdjk.com/Article/details/gjtohjuvd.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gmlmlzaat.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gtdyrbdsh.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gzacrsxna.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/grtkrhxuh.sHtML

[S05] C：字符串长度
来源：http://wap.fktsv.cn/Article/details/gdwdgfpyy.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gyzxzzljq.sHtML

[S06] C：字符串比较
来源：http://read.share.epnwcf.com/Article/details/gcrkzohah.sHtML

strcmp(a, b) == 0
来源：http://wap.yfazqb.com/Article/details/ggywtbkqt.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gzzpsbagb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.epnwcf.com/Article/details/gematlwtl.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.yfazqb.com/Article/details/ghuvdojwe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.tarul.cn/Article/details/gakrhjvks.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/ggiazdiaw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.sjlbkw.cn/Article/details/gzndzbmaj.sHtML

[S10] C：指针与解引用
来源：http://mobile.vehdjk.com/Article/details/gapqpxvld.sHtML

int *p = &a;  *p = 5;
来源：http://blog.tarul.cn/Article/details/gmminchwq.sHtML

[S11] C：逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gflbrufnd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gjtkqavow.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gsmybsacl.sHtML

fclose(f);
来源：http://www.share.epnwcf.com/Article/details/guwydaaci.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gkanrlfon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gorghmhlp.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/gepylbgsu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fktsv.cn/Article/details/gpkakpdqd.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gpgnvsgtn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gdvltnrle.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gmbyhuahj.sHtML

(double) a / b
来源：http://m.share.yfazqb.com/Article/details/gimcjfcht.sHtML

[S16] C：位操作置位
来源：http://www.m.share.yfazqb.com/Article/details/gwaeiynwm.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/goeseqpbm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gndebttgk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fktsv.cn/Article/details/gysemegtb.sHtML

[S18] C：命令行参数
来源：http://www.share.tarul.cn/Article/details/gjmxknibj.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzshkmey.sHtML

[S19] C：快速排序
来源：http://www.m.share.yfazqb.com/Article/details/gxjmvhccq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbhcnbqy.sHtML

[S20] C：二分查找
来源：http://wap.fktsv.cn/Article/details/gqaoonoet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.epnwcf.com/Article/details/gktwgichm.sHtML

[S21] C：字符类别判断
来源：http://blog.bbcook.cn/Article/details/gplhyyytv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.bbcook.cn/Article/details/gpddqcolc.sHtML

[S22] C：字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gudymjwhx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdkyqbnd.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gacbxxdyd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.bbcook.cn/Article/details/gpajfsrji.sHtML

[S24] C：获取本地时间
来源：http://www.share.epnwcf.com/Article/details/gmjzrekwj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.bbcook.cn/Article/details/gpnjyzxhh.sHtML

[S25] C：内存拷贝
来源：http://wap.epnwcf.com/Article/details/gegpxlrcn.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/gehmgqwxg.sHtML

[S26] C：内存清零
来源：http://wap.fktsv.cn/Article/details/gfovjcbbj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gemexxors.sHtML

[S27] C：定义常量
来源：http://mobile.bbcook.cn/Article/details/gtrysgfzh.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/ggnwggrxv.sHtML

[S28] C：静态变量
来源：http://blog.epnwcf.com/Article/details/gbuhqmkpb.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gvvzzgxcl.sHtML

[S29] C：变参函数
来源：http://www.share.vehdjk.com/Article/details/gdthjgivm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gkjhmftrs.sHtML

[S30] C：头文件保护
来源：http://www.share.tarul.cn/Article/details/gjlncquqb.sHtML

#ifndef X_H
来源：http://read.share.tarul.cn/Article/details/gakelpesi.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gxxuhqcxl.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gfvfhnclp.sHtML

[S31] C++：Hello World
来源：http://wap.epnwcf.com/Article/details/giuduvijg.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gjkpzqrpy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/grunpuali.sHtML

[S32] C++：字符串
来源：http://m.share.bbcook.cn/Article/details/ggjkqbuwc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gvalxccgp.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpfdcvmb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.tarul.cn/Article/details/gsupniibo.sHtML

[S34] C++：遍历 vector
来源：http://m.share.epnwcf.com/Article/details/gbystbtpo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gkpdqipnh.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gdiqshkre.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gycyedsrm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gazbqxfea.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gxtltevaa.sHtML

[S37] C++：set
来源：http://wap.sjlbkw.cn/Article/details/gkfshhcmp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhgvfvbq.sHtML

[S38] C++：排序
来源：http://wap.vehdjk.com/Article/details/gyveqzwdu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gcupccxze.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.yfazqb.com/Article/details/gitcvyxfy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gvdiqcutd.sHtML

[S40] C++：查找元素
来源：http://baike.vehdjk.com/Article/details/gqmankiuu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsljbgvp.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.bbcook.cn/Article/details/ggktxqcju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gmiwjpctv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/ghttnbyae.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.sjlbkw.cn/Article/details/gxkkmvygv.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/ggajrmpar.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gxrztbuko.sHtML

[S44] C++：引用传参
来源：http://blog.tarul.cn/Article/details/gcjrvbltk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gtpodennt.sHtML

[S45] C++：lambda
来源：http://blog.vehdjk.com/Article/details/gbcyddzhh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.tarul.cn/Article/details/gwzmvknbj.sHtML

[S46] C++：函数模板
来源：http://www.blog.vehdjk.com/Article/details/gulpykznc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gcrjrtoxv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.bbcook.cn/Article/details/gmrqwnvio.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.epnwcf.com/Article/details/gabzfdoiy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gykfvhquk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/gkvwopbsy.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gobspmoov.sHtML

[S49] C++：写文件
来源：http://read.share.vehdjk.com/Article/details/gzxndtbin.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.bbcook.cn/Article/details/gxssezhqh.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/gbzkpbgam.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.tarul.cn/Article/details/gbhvmmlgt.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gzvkkoseu.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/gcuvcubyx.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/groazhemr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gblzhzyff.sHtML

[S53] C++：移动语义
来源：http://www.m.share.yfazqb.com/Article/details/gxvnewozy.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.yfazqb.com/Article/details/glirosldu.sHtML

[S54] C++：异常处理
来源：http://www.blog.vehdjk.com/Article/details/gvtkjlspp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.bbcook.cn/Article/details/gsvawawep.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gdmemvtdn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gpwqejbqb.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/guwynoaix.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.tarul.cn/Article/details/gttwoncfl.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gglmhlpmy.sHtML

constexpr int N = 10;
来源：http://3g.vehdjk.com/Article/details/gftdityif.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gwzudaxbt.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gcfcdqydh.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gcpjfttzj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.bbcook.cn/Article/details/genoytilg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.epnwcf.com/Article/details/ghfofhpzx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.yfazqb.com/Article/details/gfpcjxvdf.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvwtkapw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gdezdptci.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbsvzfjom.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gwqjgezct.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gsnlshwmx.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gkfwitjmo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.epnwcf.com/Article/details/gabzgqrnd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fktsv.cn/Article/details/gygbwlqmw.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gocjrrkjs.sHtML

[T04] Kotlin：空安全
来源：http://read.share.vehdjk.com/Article/details/gcxmiqbgo.sHtML

val n: String? = null;  n?.length
来源：http://mobile.bbcook.cn/Article/details/gzlxbgchi.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gkikyphve.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.yfazqb.com/Article/details/ghdidqdtn.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gdredxwnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.vehdjk.com/Article/details/groxhnixn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gwtmjeppp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.sjlbkw.cn/Article/details/gtninofdi.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/glsqudybq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.tarul.cn/Article/details/gvbtpjwwy.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.yfazqb.com/Article/details/gfzivtrbr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.epnwcf.com/Article/details/ghtowupio.sHtML

[T10] Kotlin：默认参数
来源：http://wap.epnwcf.com/Article/details/gwfxnnddw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.tarul.cn/Article/details/glnlqbgxv.sHtML

[T11] Kotlin：协程
来源：http://wap.sjlbkw.cn/Article/details/gutixaahh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.tarul.cn/Article/details/gzunqucvj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.tarul.cn/Article/details/ghcntpmnr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gpwsutveq.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.vehdjk.com/Article/details/guwwcanlp.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gqfzgweiu.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gjwhfqofl.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/giryvuxub.sHtML

[T15] Kotlin：接口
来源：http://3g.vehdjk.com/Article/details/gevptltfv.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.vehdjk.com/Article/details/gmjdkoiwn.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gzbgyhien.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gyygozoyu.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gkcwukqyx.sHtML

var a = 1;  let b = 2
来源：http://wap.yfazqb.com/Article/details/gikbnyufn.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fktsv.cn/Article/details/ggugkwubr.sHtML

"值: \(b)"
来源：http://m.share.fktsv.cn/Article/details/gjgvgvhyz.sHtML

[T19] Swift：可选绑定
来源：http://www.share.bbcook.cn/Article/details/gcdxahezp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/gczpnbyzb.sHtML

[T20] Swift：数组操作
来源：http://mobile.tarul.cn/Article/details/gyjmtuqtl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.tarul.cn/Article/details/gornbmrap.sHtML

[T21] Swift：遍历
来源：http://baike.sjlbkw.cn/Article/details/gcikvkhng.sHtML

for x in a { print(x) }
来源：http://mobile.bbcook.cn/Article/details/gbcvtplui.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gmgxeaqbd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvqbprye.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gaajkxzja.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fktsv.cn/Article/details/gcypggkzb.sHtML

[T24] Swift：闭包
来源：http://mobile.epnwcf.com/Article/details/gacdnkval.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/glislfqhr.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/ggtghbeex.sHtML

struct P { var x: Int }
来源：http://www.blog.fktsv.cn/Article/details/gsriwdjld.sHtML

[T26] Swift：类与重写
来源：http://read.share.vehdjk.com/Article/details/gmjjmqlad.sHtML

class A: Base { override func f() {} }
来源：http://mobile.bbcook.cn/Article/details/gkbrilflq.sHtML

[T27] Swift：错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/girkrwqte.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.tarul.cn/Article/details/gorkbpkxb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/glwofwzoq.sHtML

enum Color { case red, green }
来源：http://mobile.tarul.cn/Article/details/gedcxqxxs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.vehdjk.com/Article/details/gydmdoley.sHtML

guard let x = opt else { return }
来源：http://blog.tarul.cn/Article/details/gltleuobi.sHtML

[T30] Swift：协议
来源：http://mobile.epnwcf.com/Article/details/gbzhquudr.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fktsv.cn/Article/details/gljnptjws.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/gzsqynfli.sHtML

print("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/glnxfuiju.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gloscavzf.sHtML

local a = 1
来源：http://blog.yfazqb.com/Article/details/ggezsixdm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gtwnpkgbd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.epnwcf.com/Article/details/gqcmbeceg.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/guszlqtjv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.yfazqb.com/Article/details/gvktzdref.sHtML

[T35] Lua：字典表
来源：http://www.blog.epnwcf.com/Article/details/gaejnrbrh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/glwnygoie.sHtML

[T36] Lua：函数
来源：http://read.share.vehdjk.com/Article/details/gceckhjwb.sHtML

function add(a, b) return a + b end
来源：http://blog.epnwcf.com/Article/details/gvrfpbeei.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/ghyibenlq.sHtML

"a" .. "b"
来源：http://www.blog.fktsv.cn/Article/details/gmxdcqxwx.sHtML

[T38] Lua：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gmiiaqzmx.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/gnaobsglg.sHtML

[T39] Lua：模式匹配
来源：http://wap.bbcook.cn/Article/details/gbsmpyykg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fktsv.cn/Article/details/gursuhomh.sHtML

[T40] Lua：元表
来源：http://mobile.sjlbkw.cn/Article/details/gdgymqbbn.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.vehdjk.com/Article/details/ggvttdscs.sHtML

[T41] Perl：Hello World
来源：http://baike.bbcook.cn/Article/details/gyfudbzpm.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/glutaybvc.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gvtezpkbr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gfusrhzqt.sHtML

[T43] Perl：字符串插值
来源：http://wap.bbcook.cn/Article/details/gayjgzikx.sHtML

"值: $a"
来源：http://wap.yfazqb.com/Article/details/gxthkjzww.sHtML

[T44] Perl：条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwgfzmom.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.vehdjk.com/Article/details/gdbqeumfd.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gcduecoui.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fktsv.cn/Article/details/gcpfcczcj.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/garzrmrxf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/gtyawrobd.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/geuochsxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gkdumoyaw.sHtML

[T48] Perl：正则替换
来源：http://www.share.epnwcf.com/Article/details/gdqsxykeg.sHtML

$s =~ s/old/new/g;
来源：http://www.share.sjlbkw.cn/Article/details/glvouxgmu.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gwpzgagcy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gepqjtxba.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gawczsvdf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fktsv.cn/Article/details/ghalnlhkv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.vehdjk.com/Article/details/gjpcponzw.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/gcfoyawdj.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gnckfcjxc.sHtML

[T52] Scala：变量
来源：http://www.share.fktsv.cn/Article/details/gpkszhwzc.sHtML

val a = 1;  var b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gcguocafk.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gmremxpsc.sHtML

s"值: $b"
来源：http://www.m.share.vehdjk.com/Article/details/gjuuxrvqm.sHtML

[T54] Scala：集合映射
来源：http://www.blog.bbcook.cn/Article/details/gvkcdomws.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.tarul.cn/Article/details/geircnghp.sHtML

[T55] Scala：集合过滤
来源：http://blog.tarul.cn/Article/details/gmiukrzdr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gsngljpnh.sHtML

[T56] Scala：样例类
来源：http://www.blog.yfazqb.com/Article/details/gxjacbddn.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gzdwdmgtu.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/ghzifjuqr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/golsulijn.sHtML

[T58] Scala：函数定义
来源：http://mobile.vehdjk.com/Article/details/ghaajgidi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.bbcook.cn/Article/details/gegodhduj.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gioxxqoxn.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.bbcook.cn/Article/details/ggxjmdjzb.sHtML

[T60] Scala：折叠
来源：http://mobile.yfazqb.com/Article/details/gduclpjuu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.bbcook.cn/Article/details/gtgammhol.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gurshdwdy.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gorgtiiae.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbmilyajv.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.bbcook.cn/Article/details/gdsecjlko.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.yfazqb.com/Article/details/gccohndlw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.sjlbkw.cn/Article/details/gfimyaygw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.vehdjk.com/Article/details/gcjqsctlw.sHtML

[U03] Py：加载 .env 配置
来源：http://www.blog.yfazqb.com/Article/details/gvvcfcrdx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.tarul.cn/Article/details/gzjtjtbhi.sHtML

[U04] Py：变量调试打印
来源：http://3g.epnwcf.com/Article/details/gqcjmpgrw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.vehdjk.com/Article/details/gmggklvvv.sHtML


<!-- 参考信息 -->