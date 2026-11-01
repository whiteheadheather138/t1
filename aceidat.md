代发 wailian999

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gxzpvptyq.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gnwdutjvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gibrhiogr.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/guspkodhf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/gmtcgwgui.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/gacyvqkqz.sHtML

crontab -e;  crontab -l
来源：http://www.share.fktsv.cn/Article/details/gqtxgxwlu.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.tarul.cn/Article/details/gtjwqkuqd.sHtML

openssl rand -hex 16
来源：http://wap.sjlbkw.cn/Article/details/gftcoxrbm.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/givwmreoh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.bbcook.cn/Article/details/gydbfjvmi.sHtML

[R69] 生成随机密码
来源：http://www.m.share.vehdjk.com/Article/details/gksstpwmg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.sjlbkw.cn/Article/details/gxzkiqeni.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gehhlxmxw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/ggiaehoac.sHtML

[R71] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gteyybyxn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.bbcook.cn/Article/details/gmhkweenl.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/geimoawnr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gpogckrxg.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/gnngryxku.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/gvocvdciu.sHtML

[R74] 批量重命名
来源：http://www.blog.yfazqb.com/Article/details/gvodzlxby.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.vehdjk.com/Article/details/gqlqnensj.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gfbyrziso.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.epnwcf.com/Article/details/gtkcyfqhz.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gjnhvxusd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gpcnlfoiq.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gcpcsdjwu.sHtML

read -rp "请输入: " ans
来源：http://wap.tarul.cn/Article/details/gavwnikiw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gqlxrmuxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gavaeubys.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gyrksxbgz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/geoctbkud.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.bbcook.cn/Article/details/gorkmnibj.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gvmhjbnjk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtthbycve.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/geldkzthx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gciciqfel.sHtML

[S01] C：Hello World
来源：http://blog.epnwcf.com/Article/details/gypklrkrf.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/gisvrwqct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gvtawitff.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.epnwcf.com/Article/details/gjushogmo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gfddqfgyk.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gvkgtfeaj.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/guvfgmpzx.sHtML

[S04] C：字符串复制
来源：http://www.blog.epnwcf.com/Article/details/gtyyxmdsy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.epnwcf.com/Article/details/ggswgajsu.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/gtgvgfxvk.sHtML

strlen(s)
来源：http://m.share.vehdjk.com/Article/details/ggksjmynp.sHtML

[S06] C：字符串比较
来源：http://3g.epnwcf.com/Article/details/gpkksspyr.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkujcyvd.sHtML

[S07] C：数组遍历求和
来源：http://wap.bbcook.cn/Article/details/gyctwzjel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.tarul.cn/Article/details/gmegxixml.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.sjlbkw.cn/Article/details/gsopsrsih.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/glljufaxt.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.vehdjk.com/Article/details/gltmccfzc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/gttrjywhp.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gkhwczgzi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.sjlbkw.cn/Article/details/gvwhyjogr.sHtML

[S11] C：逐行读文件
来源：http://blog.tarul.cn/Article/details/gecrrpwsa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fktsv.cn/Article/details/gfvtmtxmz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.epnwcf.com/Article/details/gcanlhxrw.sHtML

fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gcdbhlwmw.sHtML

[S12] C：写文件
来源：http://3g.sjlbkw.cn/Article/details/ggqwmfala.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gqavnbsis.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gaidaktii.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.epnwcf.com/Article/details/gauotvure.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfrjotu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.tarul.cn/Article/details/gdjmjbnal.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/ggpfvrtzh.sHtML

(double) a / b
来源：http://blog.bbcook.cn/Article/details/gnknczjau.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gqqqlawuh.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/guxxxyhka.sHtML

[S17] C：安全拼接字符串
来源：http://baike.tarul.cn/Article/details/gxjlcaato.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.bbcook.cn/Article/details/guboaigqw.sHtML

[S18] C：命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gaywgxztm.sHtML

int main(int argc, char **argv)
来源：http://blog.epnwcf.com/Article/details/gtocjiesj.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/guyrcigdh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.yfazqb.com/Article/details/gvuzhukcc.sHtML

[S20] C：二分查找
来源：http://baike.fktsv.cn/Article/details/gfewjknrr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gbdvbefhv.sHtML

[S21] C：字符类别判断
来源：http://wap.fktsv.cn/Article/details/gvhptfkys.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.bbcook.cn/Article/details/gnldgqwnn.sHtML

[S22] C：字符串转数字
来源：http://wap.tarul.cn/Article/details/gvddaqvcr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fktsv.cn/Article/details/grjfthtgz.sHtML

[S23] C：随机数
来源：http://3g.yfazqb.com/Article/details/gmxltlxhz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.sjlbkw.cn/Article/details/ggrnehofz.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/ggxiitqds.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/grafqslvx.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gpnolxdny.sHtML

memcpy(dst, src, n);
来源：http://m.share.epnwcf.com/Article/details/gvoiusxxz.sHtML

[S26] C：内存清零
来源：http://baike.bbcook.cn/Article/details/gromttxfy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.epnwcf.com/Article/details/gxhmczlzu.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gdjcnetif.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/gljzjbjbb.sHtML

[S28] C：静态变量
来源：http://www.m.share.epnwcf.com/Article/details/gcodqrpqx.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gcoyolvku.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/goljgveid.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gozaztwix.sHtML

[S30] C：头文件保护
来源：http://www.m.share.yfazqb.com/Article/details/gznuqgubo.sHtML

#ifndef X_H
来源：http://mobile.yfazqb.com/Article/details/gqigfdvwk.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/ghswzoewm.sHtML

#endif
来源：http://read.share.sjlbkw.cn/Article/details/guiawotdm.sHtML

[S31] C++：Hello World
来源：http://www.share.yfazqb.com/Article/details/gztxekjqm.sHtML

#include <iostream>
来源：http://www.share.bbcook.cn/Article/details/giujmdbra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fktsv.cn/Article/details/gojxgdtyo.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gnbjdsjyu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gxvkgwiub.sHtML

[S33] C++：vector 增删
来源：http://read.share.yfazqb.com/Article/details/gneujqeva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/glgmdyamd.sHtML

[S34] C++：遍历 vector
来源：http://read.share.epnwcf.com/Article/details/gyvffpjgr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/gnrgvhepu.sHtML

[S35] C++：map
来源：http://www.blog.epnwcf.com/Article/details/gbqmyypxq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gswplxdlq.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gonntyehz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gxbtznroi.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gcbslmfue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/ghwdbgcoj.sHtML

[S38] C++：排序
来源：http://mobile.yfazqb.com/Article/details/gqymvzrnq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gjxazmrxn.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.sjlbkw.cn/Article/details/ggrfmuwdz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gvzxdfgdw.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/gbnqtphzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.bbcook.cn/Article/details/gviewvlku.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gjqotreuv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.sjlbkw.cn/Article/details/gdjthlhbe.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.vehdjk.com/Article/details/goflpdbnp.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gjudwuuhe.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gjufowyml.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gbwkzscvn.sHtML

[S44] C++：引用传参
来源：http://www.share.tarul.cn/Article/details/gycxapwfw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/gqrkkjzyx.sHtML

[S45] C++：lambda
来源：http://wap.sjlbkw.cn/Article/details/gnzkddkjp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gaxwpwlxd.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gotmvvfir.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfyttuwma.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/guqanfwab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.epnwcf.com/Article/details/gdkvfobuw.sHtML

[S48] C++：逐行读文件
来源：http://3g.epnwcf.com/Article/details/gprtdcrcq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.tarul.cn/Article/details/gtdtlezba.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/gyagszzvr.sHtML

[S49] C++：写文件
来源：http://www.share.yfazqb.com/Article/details/gefjziosc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gbyzmfnac.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/geaflixzw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gbqvqesxu.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gcpyjsger.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/giteftrlp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gjfgncdyk.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.vehdjk.com/Article/details/gsovhaezp.sHtML

[S53] C++：移动语义
来源：http://read.share.bbcook.cn/Article/details/gedsieftw.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.tarul.cn/Article/details/ggudiyrfk.sHtML

[S54] C++：异常处理
来源：http://read.share.sjlbkw.cn/Article/details/gqleijikk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gglhodhex.sHtML

[S55] C++：结构化绑定
来源：http://baike.fktsv.cn/Article/details/gdzwliavh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.tarul.cn/Article/details/gbxzslgpo.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gfwmdvdjm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fktsv.cn/Article/details/gtleokjaz.sHtML

[S57] C++：编译期常量
来源：http://read.share.fktsv.cn/Article/details/gbhofgfmt.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gifugspre.sHtML

[S58] C++：命名空间
来源：http://3g.tarul.cn/Article/details/gswdltchh.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.sjlbkw.cn/Article/details/galxlkwyf.sHtML

[S59] C++：静态断言
来源：http://www.share.epnwcf.com/Article/details/givfamgwv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/gjfixnilx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/giescfcca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.tarul.cn/Article/details/gwaaatrao.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkxsgeuhu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.tarul.cn/Article/details/gyeafxkho.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gettweapn.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/goqklapop.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gegugavrv.sHtML

[T02] Kotlin：变量
来源：http://m.share.fktsv.cn/Article/details/gydxkyocs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.tarul.cn/Article/details/ggzhzshfb.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gyazzsqkr.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gtuvtfmtk.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.tarul.cn/Article/details/gwyfbkeaq.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gcwzngsbg.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gqefzykyl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.sjlbkw.cn/Article/details/gosgqgkxn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.sjlbkw.cn/Article/details/ggnndlesv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.bbcook.cn/Article/details/gsdnbkbff.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gvohfpfib.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/grejikzky.sHtML

[T08] Kotlin：数据类
来源：http://blog.sjlbkw.cn/Article/details/gvlqsnigv.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gdpjuobaq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgxjkuxa.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/goesnmgpd.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/gyhaupirt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.epnwcf.com/Article/details/gpvikahnw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/grpgaeixx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.sjlbkw.cn/Article/details/gxhkcqhfa.sHtML

[T12] Kotlin：解构声明
来源：http://3g.bbcook.cn/Article/details/gqgawcmph.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fktsv.cn/Article/details/gtoqdbskv.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.yfazqb.com/Article/details/giyfapgzu.sHtML

val m = mapOf("a" to 1)
来源：http://baike.yfazqb.com/Article/details/gzaxdusjo.sHtML

[T14] Kotlin：循环
来源：http://mobile.sjlbkw.cn/Article/details/grlltmbnl.sHtML

for (i in 1..10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gweyzbhhg.sHtML

[T15] Kotlin：接口
来源：http://m.share.vehdjk.com/Article/details/gpuvmwnrm.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gaqimezor.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/gaovhnpkg.sHtML

print("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gxqdoxoxy.sHtML

[T17] Swift：变量与常量
来源：http://baike.vehdjk.com/Article/details/gtarjctkb.sHtML

var a = 1;  let b = 2
来源：http://mobile.bbcook.cn/Article/details/gtyvttnor.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.bbcook.cn/Article/details/gyuznprhd.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gzdqpautc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.epnwcf.com/Article/details/gyyjnhppy.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/gvmvkdvdu.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gmroytkop.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gzdbqypwa.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gxunfjxvk.sHtML

for x in a { print(x) }
来源：http://www.m.share.epnwcf.com/Article/details/gmjjlireb.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gzpvzkksv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fktsv.cn/Article/details/gyzroelzf.sHtML

[T23] Swift：函数
来源：http://wap.epnwcf.com/Article/details/gdwudeyxa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gxhsrjahs.sHtML

[T24] Swift：闭包
来源：http://blog.vehdjk.com/Article/details/grbwytiqm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gavfuqrsl.sHtML

[T25] Swift：结构体
来源：http://blog.yfazqb.com/Article/details/gfgagptuj.sHtML

struct P { var x: Int }
来源：http://mobile.tarul.cn/Article/details/gilxgzgql.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/ggthbjmbv.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/gvibficjn.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/gpwgwkmct.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gyyoftixo.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gnebzdapl.sHtML

enum Color { case red, green }
来源：http://mobile.epnwcf.com/Article/details/gpskrcazy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.vehdjk.com/Article/details/gtlwyruze.sHtML

guard let x = opt else { return }
来源：http://wap.sjlbkw.cn/Article/details/gzxhyrvfy.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gfimqhycu.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.epnwcf.com/Article/details/gmcchblxa.sHtML

[T31] Lua：Hello World
来源：http://m.share.fktsv.cn/Article/details/gjpouvsun.sHtML

print("Hello")
来源：http://blog.tarul.cn/Article/details/gsnhwzzbc.sHtML

[T32] Lua：局部变量
来源：http://read.share.epnwcf.com/Article/details/golvnhtmc.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gsnfanrus.sHtML

[T33] Lua：表（数组）
来源：http://mobile.tarul.cn/Article/details/gxupxzxfd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.vehdjk.com/Article/details/guupzqrbb.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gdcyrvvvl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/goveluwar.sHtML

[T35] Lua：字典表
来源：http://www.m.share.vehdjk.com/Article/details/gqxipzpkd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gpojzsipg.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gtyyalabs.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/ggprrhzxf.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.yfazqb.com/Article/details/ggabcthly.sHtML

"a" .. "b"
来源：http://baike.bbcook.cn/Article/details/gqxwxlvnf.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/goqpbqerv.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gdrsfhbom.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gtmmbreim.sHtML

string.find(s, "%d+")
来源：http://baike.fktsv.cn/Article/details/gfwlkaeri.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/ghyyhrvgc.sHtML

setmetatable({}, { __index = base })
来源：http://baike.vehdjk.com/Article/details/ghqwzuyjg.sHtML

[T41] Perl：Hello World
来源：http://www.share.fktsv.cn/Article/details/gtkdgnzvo.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/ggppelapy.sHtML

[T42] Perl：变量类型
来源：http://3g.fktsv.cn/Article/details/ghxzexmcv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gjrxmzrqh.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gknwjktgm.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/gbokaxdfr.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gbywygxyo.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.vehdjk.com/Article/details/gtbuibmkl.sHtML

[T45] Perl：数组遍历
来源：http://m.share.tarul.cn/Article/details/gyzrnmbib.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.sjlbkw.cn/Article/details/gyvccukps.sHtML

[T46] Perl：哈希操作
来源：http://baike.tarul.cn/Article/details/gwrjwexds.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.tarul.cn/Article/details/glxyaoxib.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.bbcook.cn/Article/details/gmnwxlljc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.sjlbkw.cn/Article/details/gfyouaupr.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gmffdryur.sHtML

$s =~ s/old/new/g;
来源：http://www.share.bbcook.cn/Article/details/guvndekqi.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gmwnvarai.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.bbcook.cn/Article/details/gxjhdrcub.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gsoliddrs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.epnwcf.com/Article/details/gbtikmzft.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.yfazqb.com/Article/details/grbchoorr.sHtML

[T51] Scala：Hello World
来源：http://baike.yfazqb.com/Article/details/gtaxmuanp.sHtML

println("Hello")
来源：http://www.m.share.fktsv.cn/Article/details/gbvgaqjcw.sHtML

[T52] Scala：变量
来源：http://mobile.yfazqb.com/Article/details/gellaaari.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gktsipjoe.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/golgtbyqz.sHtML

s"值: $b"
来源：http://www.blog.yfazqb.com/Article/details/gjfskjjah.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gfwjjtfhv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/gghqfsqdt.sHtML

[T55] Scala：集合过滤
来源：http://wap.epnwcf.com/Article/details/goahhgymx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.yfazqb.com/Article/details/gulwbcrot.sHtML

[T56] Scala：样例类
来源：http://3g.vehdjk.com/Article/details/gzamkbdff.sHtML

case class User(name: String, age: Int)
来源：http://3g.tarul.cn/Article/details/gbreeypdh.sHtML

[T57] Scala：模式匹配
来源：http://read.share.epnwcf.com/Article/details/gdwolvuzf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gmmiwymva.sHtML

[T58] Scala：函数定义
来源：http://blog.bbcook.cn/Article/details/goojzgtgg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.yfazqb.com/Article/details/gsibhwpae.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/grlconwiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gcdvqhojt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.yfazqb.com/Article/details/ghqkjliob.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.yfazqb.com/Article/details/guoxvgdjn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gecjrztkx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.vehdjk.com/Article/details/gajwhjwnw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gphieback.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.epnwcf.com/Article/details/gjysqthxx.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.bbcook.cn/Article/details/guytvfkns.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.bbcook.cn/Article/details/gabbaexnm.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.tarul.cn/Article/details/gzodvavez.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gwgnxjowx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.vehdjk.com/Article/details/gfbofzylm.sHtML

[U04] Py：变量调试打印
来源：http://baike.epnwcf.com/Article/details/gszookkwi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gecwymbiu.sHtML


<!-- 参考信息 -->