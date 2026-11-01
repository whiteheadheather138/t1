代发 wailian999

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/ggrnfeoqd.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/ggqvklsam.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/geqzhpvhe.sHtML

[R59] 发 POST JSON
来源：http://blog.yfazqb.com/Article/details/gbmnxehcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gtarckmxm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.tarul.cn/Article/details/gqresycvp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.epnwcf.com/Article/details/gebkspgku.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fktsv.cn/Article/details/gpkmpziuv.sHtML

df -h;  du -sh *
来源：http://blog.bbcook.cn/Article/details/guocmrcnw.sHtML

[R62] 找最占空间的文件
来源：http://baike.yfazqb.com/Article/details/gkonuqvxa.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.epnwcf.com/Article/details/goaeoqcni.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gcseyktch.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gneuceuet.sHtML

[R64] 结束进程
来源：http://wap.fktsv.cn/Article/details/geprugiov.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.bbcook.cn/Article/details/gsfjexsft.sHtML

[R65] 查看端口占用
来源：http://3g.epnwcf.com/Article/details/grsbbobvo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/gkuhuiywy.sHtML

[R66] 定时任务
来源：http://3g.bbcook.cn/Article/details/ghfrddlrx.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gjzlbkzje.sHtML

[R67] 生成随机十六进制串
来源：http://3g.tarul.cn/Article/details/gzwdddkmr.sHtML

openssl rand -hex 16
来源：http://www.blog.bbcook.cn/Article/details/gqrrzwgrn.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gnchlosiq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.vehdjk.com/Article/details/gnbokbihz.sHtML

[R69] 生成随机密码
来源：http://wap.vehdjk.com/Article/details/gxwzpcfel.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/gqbhyvkut.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/glxwahdbo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gjleabbfm.sHtML

[R71] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gurzdkhoa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.sjlbkw.cn/Article/details/gfzhbcmhn.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gwwyhxvmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gdwxtavib.sHtML

[R73] 分割大日志
来源：http://blog.bbcook.cn/Article/details/geiqrarjr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.sjlbkw.cn/Article/details/gjaeqwznr.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gjpkojzgp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.epnwcf.com/Article/details/gwmlafpnm.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gnntitvgp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.sjlbkw.cn/Article/details/gcwjmkkcb.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gfmzkdnsm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gtjiuudsa.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gojccgkpe.sHtML

read -rp "请输入: " ans
来源：http://3g.fktsv.cn/Article/details/gconbeode.sHtML

[R78] 交互式菜单
来源：http://mobile.fktsv.cn/Article/details/gsonmozhy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.tarul.cn/Article/details/gajqeshzn.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/ghmqkoddz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.yfazqb.com/Article/details/gdizoyzqi.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.vehdjk.com/Article/details/geykvpfhn.sHtML

time ./run.sh
来源：http://www.m.share.epnwcf.com/Article/details/ggkifvjwc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzbosjffe.sHtML

S. C / C++ 专题
来源：http://www.share.yfazqb.com/Article/details/giryovmjd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjbrvjpxv.sHtML

[S01] C：Hello World
来源：http://baike.vehdjk.com/Article/details/gfusapyel.sHtML

#include <stdio.h>
来源：http://www.m.share.yfazqb.com/Article/details/gdftisvhh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gytisymth.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/gfobnlymr.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gaitapdlo.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gyicxgsgf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gftrgcihx.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gcnlcnzui.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.vehdjk.com/Article/details/gxsukbdkw.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gtcpfamlv.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gbagdxeld.sHtML

[S06] C：字符串比较
来源：http://m.share.fktsv.cn/Article/details/gwhfnumap.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gloiinimk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fktsv.cn/Article/details/guixfvumk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.sjlbkw.cn/Article/details/gjquhghwf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fktsv.cn/Article/details/gjzaqtxjr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.epnwcf.com/Article/details/gilqpjlkj.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fktsv.cn/Article/details/ggrulfnbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fktsv.cn/Article/details/gxhqyxgpg.sHtML

[S10] C：指针与解引用
来源：http://www.share.tarul.cn/Article/details/grawzuebb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/gmwcrcrkh.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gqjenfrdh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.epnwcf.com/Article/details/gyidigodm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.bbcook.cn/Article/details/gnfhwzuru.sHtML

fclose(f);
来源：http://wap.epnwcf.com/Article/details/gcxhsuqwi.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gcgfsswmm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gpenoajbz.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gwupiaigz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/geqcdwvsq.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/gpgsxheqj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/gakzckgir.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/goyzjslfg.sHtML

(double) a / b
来源：http://www.share.sjlbkw.cn/Article/details/gbkctcdgz.sHtML

[S16] C：位操作置位
来源：http://m.share.fktsv.cn/Article/details/gtxacfedn.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gafpsxagz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.epnwcf.com/Article/details/gjitwjffq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.yfazqb.com/Article/details/glisqwind.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gwrlclhyo.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gbpmabmav.sHtML

[S19] C：快速排序
来源：http://mobile.yfazqb.com/Article/details/gtrwrefwx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gzrljtzsg.sHtML

[S20] C：二分查找
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdoyyjrp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gcnggdmkn.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gaqywcbik.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gedrjwqje.sHtML

[S22] C：字符串转数字
来源：http://3g.tarul.cn/Article/details/geivocmdy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.bbcook.cn/Article/details/gbyxactef.sHtML

[S23] C：随机数
来源：http://www.share.epnwcf.com/Article/details/gvbrcuwpz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.sjlbkw.cn/Article/details/gpvnrypnk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/ghdpczxfe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.sjlbkw.cn/Article/details/gapwtwwkv.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gvjfgolte.sHtML

memcpy(dst, src, n);
来源：http://blog.bbcook.cn/Article/details/ggiiaytah.sHtML

[S26] C：内存清零
来源：http://www.blog.vehdjk.com/Article/details/gtzoonwnc.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/gdcuuvdgt.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gfyamssrl.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gymobqexs.sHtML

[S28] C：静态变量
来源：http://www.blog.tarul.cn/Article/details/gwjkxvsha.sHtML

static int counter = 0;
来源：http://www.blog.bbcook.cn/Article/details/gvwwpaisk.sHtML

[S29] C：变参函数
来源：http://read.share.bbcook.cn/Article/details/grpdovqde.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.vehdjk.com/Article/details/gaqogzwnq.sHtML

[S30] C：头文件保护
来源：http://baike.tarul.cn/Article/details/gxrsxjyjw.sHtML

#ifndef X_H
来源：http://baike.tarul.cn/Article/details/gurwsaxuf.sHtML

#define X_H
来源：http://m.share.sjlbkw.cn/Article/details/gwfipmelk.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gvwndlkmy.sHtML

[S31] C++：Hello World
来源：http://read.share.yfazqb.com/Article/details/gbbskkjwo.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gngtnavau.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gvpouqndp.sHtML

[S32] C++：字符串
来源：http://wap.yfazqb.com/Article/details/gpyvebuyo.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/gxptvzubq.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/gusdjxgrw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fktsv.cn/Article/details/gwjqbbely.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gvfvqeaiz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.tarul.cn/Article/details/gjwlfhjzp.sHtML

[S35] C++：map
来源：http://mobile.epnwcf.com/Article/details/gdpweiheb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/gumbcwoqu.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/gawzoslny.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gujvkaxdd.sHtML

[S37] C++：set
来源：http://baike.yfazqb.com/Article/details/gurshvtdz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gehltenwx.sHtML

[S38] C++：排序
来源：http://baike.epnwcf.com/Article/details/gspwwpojb.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gewywjgik.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gowjjrpxh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.epnwcf.com/Article/details/gwcuccbud.sHtML

[S40] C++：查找元素
来源：http://m.share.yfazqb.com/Article/details/gzvrvmbev.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.tarul.cn/Article/details/gujhgsybd.sHtML

[S41] C++：类与构造函数
来源：http://read.share.bbcook.cn/Article/details/gnckcqcmt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.epnwcf.com/Article/details/gdxbquqvv.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.vehdjk.com/Article/details/gypvhxwke.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.sjlbkw.cn/Article/details/gaspkmoct.sHtML

[S43] C++：智能指针
来源：http://read.share.fktsv.cn/Article/details/gimpnwsyd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gkglkaeki.sHtML

[S44] C++：引用传参
来源：http://baike.yfazqb.com/Article/details/gyoanxeqv.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gbuylaqtz.sHtML

[S45] C++：lambda
来源：http://www.blog.tarul.cn/Article/details/gwfryeayt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gxvdcxupw.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gcdeizefz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gazxngqvp.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gyklwlbhw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.bbcook.cn/Article/details/ggdaswris.sHtML

[S48] C++：逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gwnmebmve.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/giaaijhry.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/glnjbndzz.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/gfyvgwcip.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gfyfwfvtb.sHtML

[S50] C++：格式化数字
来源：http://mobile.epnwcf.com/Article/details/glpapugre.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.yfazqb.com/Article/details/grrzfktxx.sHtML

[S51] C++：显式类型转换
来源：http://mobile.vehdjk.com/Article/details/gofcbexil.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/ghienxvxy.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.yfazqb.com/Article/details/gtnxuradd.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.yfazqb.com/Article/details/gbshimuyb.sHtML

[S53] C++：移动语义
来源：http://m.share.yfazqb.com/Article/details/gcfmiqvsa.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.epnwcf.com/Article/details/gbbgewdck.sHtML

[S54] C++：异常处理
来源：http://www.m.share.epnwcf.com/Article/details/gojcusldy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gunhqnobo.sHtML

[S55] C++：结构化绑定
来源：http://blog.yfazqb.com/Article/details/goordnahc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.epnwcf.com/Article/details/gyyudjbgp.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gghjocdff.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.tarul.cn/Article/details/grtvsvhhm.sHtML

[S57] C++：编译期常量
来源：http://blog.bbcook.cn/Article/details/girumkeud.sHtML

constexpr int N = 10;
来源：http://baike.epnwcf.com/Article/details/gzpisgyme.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/ghjrhtsbe.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.epnwcf.com/Article/details/gcfvyfphh.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gredwwhet.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/glgjtftve.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gspypvzcl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/grecumwmd.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjgwicumb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gwqxqjnuy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfinutkpt.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gbpelevsc.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gxforksfh.sHtML

[T02] Kotlin：变量
来源：http://mobile.sjlbkw.cn/Article/details/gnikxymsd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmurzanp.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.yfazqb.com/Article/details/gaguukwrq.sHtML

"值: $b"
来源：http://baike.epnwcf.com/Article/details/glxnpigmh.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gwdvqlqxf.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.epnwcf.com/Article/details/gxppjrumu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.epnwcf.com/Article/details/gwyhrcbex.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gdtzfslsy.sHtML

[T06] Kotlin：集合映射
来源：http://blog.tarul.cn/Article/details/gczxyerfu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.tarul.cn/Article/details/gslosreao.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/gmpcypwpb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.epnwcf.com/Article/details/gasteljnz.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gqtdvcenq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.yfazqb.com/Article/details/gqzlhrupz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fktsv.cn/Article/details/gooqwdihe.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.sjlbkw.cn/Article/details/ggqnbxxzu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gfwvigubj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fktsv.cn/Article/details/ghdrvadhs.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/giyclbuon.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gtznbtohq.sHtML

[T12] Kotlin：解构声明
来源：http://baike.vehdjk.com/Article/details/gioozlter.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.vehdjk.com/Article/details/gebaoapgh.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.vehdjk.com/Article/details/gopwsuiyv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gqgjlmnxr.sHtML

[T14] Kotlin：循环
来源：http://baike.yfazqb.com/Article/details/gqjykfqsc.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gfrljsktc.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gtotpwaqd.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gbrlkzpue.sHtML

[T16] Swift：Hello World
来源：http://www.share.bbcook.cn/Article/details/gjngxzfbr.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gpjrqygjv.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gvgrlhozq.sHtML

var a = 1;  let b = 2
来源：http://www.share.vehdjk.com/Article/details/gzsrpidzw.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gwndkstye.sHtML

"值: \(b)"
来源：http://www.m.share.vehdjk.com/Article/details/gwlnmyefr.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gafezeran.sHtML

if let n = opt { print(n) }
来源：http://www.share.fktsv.cn/Article/details/gnvjdeunb.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/glfnlklgv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gdfqofoee.sHtML

[T21] Swift：遍历
来源：http://m.share.yfazqb.com/Article/details/glznukvam.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/gtrowzlpd.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gbcpmeiww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gywawyelf.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/ghrmpkinw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gcekokdca.sHtML

[T24] Swift：闭包
来源：http://wap.yfazqb.com/Article/details/geirhaufs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/galzoeonk.sHtML

[T25] Swift：结构体
来源：http://wap.tarul.cn/Article/details/ghrgottxi.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gbwdszwxl.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gbzapcxtr.sHtML

class A: Base { override func f() {} }
来源：http://www.share.tarul.cn/Article/details/gyltjcgft.sHtML

[T27] Swift：错误处理
来源：http://baike.bbcook.cn/Article/details/gbvxyncew.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fktsv.cn/Article/details/grdbcwcip.sHtML

[T28] Swift：枚举
来源：http://3g.sjlbkw.cn/Article/details/gruxkzvma.sHtML

enum Color { case red, green }
来源：http://wap.epnwcf.com/Article/details/gxfcqsdcj.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.sjlbkw.cn/Article/details/gwnmpyaqb.sHtML

guard let x = opt else { return }
来源：http://wap.epnwcf.com/Article/details/gswcepnmd.sHtML

[T30] Swift：协议
来源：http://mobile.tarul.cn/Article/details/gmuqaxiuy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gurynbxrm.sHtML

[T31] Lua：Hello World
来源：http://3g.tarul.cn/Article/details/gpwinupti.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gfpkfzuua.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gfyczkach.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gjrdfpjky.sHtML

[T33] Lua：表（数组）
来源：http://baike.vehdjk.com/Article/details/gzmeholjh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fktsv.cn/Article/details/gupmphbaf.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/gljlmhrov.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.yfazqb.com/Article/details/gnelmsvrq.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/ggpzsajus.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.yfazqb.com/Article/details/glqlgyhej.sHtML

[T36] Lua：函数
来源：http://baike.bbcook.cn/Article/details/gambgpdfz.sHtML

function add(a, b) return a + b end
来源：http://m.share.fktsv.cn/Article/details/guznegtta.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gunthfrrw.sHtML

"a" .. "b"
来源：http://www.share.epnwcf.com/Article/details/gnqekepbs.sHtML

[T38] Lua：条件
来源：http://www.m.share.yfazqb.com/Article/details/guusyayid.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gnmwbntnx.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gziphqmnp.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/grxsphwzr.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gczxigwck.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.bbcook.cn/Article/details/gzceeynle.sHtML

[T41] Perl：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gyxgivurd.sHtML

print "Hello\n";
来源：http://www.m.share.fktsv.cn/Article/details/gbsjikuul.sHtML

[T42] Perl：变量类型
来源：http://3g.tarul.cn/Article/details/gjgccabjk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.vehdjk.com/Article/details/gcibinzdi.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gzrqiyhqx.sHtML

"值: $a"
来源：http://www.share.tarul.cn/Article/details/gaxhfjfsi.sHtML

[T44] Perl：条件
来源：http://read.share.tarul.cn/Article/details/gsdvvhdrd.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/glemqchux.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gxgxdhldn.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fktsv.cn/Article/details/ggkhwwqhc.sHtML

[T46] Perl：哈希操作
来源：http://baike.vehdjk.com/Article/details/gfmxrbcqf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.fktsv.cn/Article/details/giljyblbm.sHtML

[T47] Perl：正则捕获
来源：http://blog.sjlbkw.cn/Article/details/gwptaskfj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.sjlbkw.cn/Article/details/galectwby.sHtML

[T48] Perl：正则替换
来源：http://m.share.yfazqb.com/Article/details/guwibtcxh.sHtML

$s =~ s/old/new/g;
来源：http://3g.epnwcf.com/Article/details/gcdzbrsqj.sHtML

[T49] Perl：函数
来源：http://www.share.vehdjk.com/Article/details/gwqglssee.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.tarul.cn/Article/details/gwcbtxaft.sHtML

[T50] Perl：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gxdcpnuom.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.bbcook.cn/Article/details/gxjwarzxg.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/gzvtwmqtr.sHtML

[T51] Scala：Hello World
来源：http://read.share.fktsv.cn/Article/details/gsdrfwlni.sHtML

println("Hello")
来源：http://www.share.bbcook.cn/Article/details/gryerbjdq.sHtML

[T52] Scala：变量
来源：http://blog.fktsv.cn/Article/details/gcayvwtog.sHtML

val a = 1;  var b = 2
来源：http://mobile.yfazqb.com/Article/details/gcjdxhctt.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gwkksvngo.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gjgztpptm.sHtML

[T54] Scala：集合映射
来源：http://m.share.fktsv.cn/Article/details/gllvkezoi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gpybeoqnh.sHtML

[T55] Scala：集合过滤
来源：http://read.share.epnwcf.com/Article/details/ggcvxxiev.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/gojorulbz.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/godfpzxqr.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gybepavqj.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxkifxqq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.vehdjk.com/Article/details/gezazdsqe.sHtML

[T58] Scala：函数定义
来源：http://blog.fktsv.cn/Article/details/grblphfhr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.sjlbkw.cn/Article/details/gxlgqbyin.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/guzqgnfcl.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.vehdjk.com/Article/details/ghpuehasz.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtcudvui.sHtML


<!-- 参考信息 -->