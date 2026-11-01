代发 wailian999

ssh user@host 'uptime'
来源：http://read.share.tarul.cn/Article/details/gnthudown.sHtML

[R58] 下载文件
来源：http://baike.sjlbkw.cn/Article/details/gpxovkmny.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.bbcook.cn/Article/details/gknnsftkl.sHtML

[R59] 发 POST JSON
来源：http://wap.tarul.cn/Article/details/gkfusvzqf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.sjlbkw.cn/Article/details/garltgkew.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gfqksjaot.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.tarul.cn/Article/details/ghcfmkxez.sHtML

[R61] 磁盘占用
来源：http://m.share.fktsv.cn/Article/details/gbpuqjgzb.sHtML

df -h;  du -sh *
来源：http://www.share.tarul.cn/Article/details/gtzytepgg.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gtvzesprx.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/glvaroiwz.sHtML

[R63] 内存与进程
来源：http://www.blog.epnwcf.com/Article/details/gieldjqdr.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.vehdjk.com/Article/details/gllhrnllr.sHtML

[R64] 结束进程
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnwqqrqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.epnwcf.com/Article/details/ghfvurcuq.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvdhdsga.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.epnwcf.com/Article/details/goayxvjbz.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gpnohfwpj.sHtML

crontab -e;  crontab -l
来源：http://blog.bbcook.cn/Article/details/gfczpmifc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gshyttmry.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/gjzlitqhc.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gvsruvkpn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gblqcqqck.sHtML

[R69] 生成随机密码
来源：http://baike.yfazqb.com/Article/details/gfxxqurbj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gjurunmro.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gdufribhn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.tarul.cn/Article/details/gjpjhoqsb.sHtML

[R71] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gabhfpnus.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.yfazqb.com/Article/details/glonqxyml.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gtncvztvp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gdjzaoxvr.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gqawrgzps.sHtML

split -l 1000 big.log part_
来源：http://www.blog.yfazqb.com/Article/details/gtrdhiinv.sHtML

[R74] 批量重命名
来源：http://www.blog.bbcook.cn/Article/details/gvyvalyov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.tarul.cn/Article/details/gnwawmdyj.sHtML

[R75] 导出环境变量
来源：http://3g.tarul.cn/Article/details/gvdvsgihp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fktsv.cn/Article/details/gxwmqbajh.sHtML

[R76] 使用临时文件
来源：http://blog.yfazqb.com/Article/details/goozxnurs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/giwbdbfey.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gfeefrxsh.sHtML

read -rp "请输入: " ans
来源：http://baike.yfazqb.com/Article/details/gaftwbsxl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gkerpeuvo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gvzfvjelq.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/gfddhmluf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.bbcook.cn/Article/details/ggckiwzwv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.epnwcf.com/Article/details/gbkjdjosa.sHtML

time ./run.sh
来源：http://mobile.yfazqb.com/Article/details/gtgoemhdc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtzruqrwt.sHtML

S. C / C++ 专题
来源：http://read.share.bbcook.cn/Article/details/gnjapesjn.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqzkgbwmb.sHtML

[S01] C：Hello World
来源：http://wap.vehdjk.com/Article/details/gqvpjljpy.sHtML

#include <stdio.h>
来源：http://3g.epnwcf.com/Article/details/gbzkyitqy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gdkspghvd.sHtML

[S02] C：变量与格式化输出
来源：http://wap.sjlbkw.cn/Article/details/gptxhftcr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.sjlbkw.cn/Article/details/gtyjviwnq.sHtML

[S03] C：读入整数
来源：http://www.blog.yfazqb.com/Article/details/ggzlnvnal.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gfaytqhco.sHtML

[S04] C：字符串复制
来源：http://www.blog.sjlbkw.cn/Article/details/ghrmrmvjj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fktsv.cn/Article/details/gpcruengc.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/ggmbysgaz.sHtML

strlen(s)
来源：http://www.blog.epnwcf.com/Article/details/gvocmjufn.sHtML

[S06] C：字符串比较
来源：http://blog.vehdjk.com/Article/details/gpimibdyu.sHtML

strcmp(a, b) == 0
来源：http://baike.vehdjk.com/Article/details/gcqhsbaps.sHtML

[S07] C：数组遍历求和
来源：http://m.share.bbcook.cn/Article/details/gqxqjydpu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/gbuimewpy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.bbcook.cn/Article/details/gogetiexc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gpccbfqmv.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gtnmwgeqa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/gtlhvrxud.sHtML

[S10] C：指针与解引用
来源：http://mobile.yfazqb.com/Article/details/gxikufvkb.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gkqvzydps.sHtML

[S11] C：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/guuorygue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fktsv.cn/Article/details/ghugslstx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.tarul.cn/Article/details/gxicvpprq.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/ghaikubpt.sHtML

[S12] C：写文件
来源：http://read.share.fktsv.cn/Article/details/guteqjare.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fktsv.cn/Article/details/gyuzmyrwd.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gssohkjkm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.tarul.cn/Article/details/gekvpwlok.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/glkhqlxia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gchzqgnmr.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gumjwmode.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/gmwvhwtyi.sHtML

[S16] C：位操作置位
来源：http://3g.fktsv.cn/Article/details/gpgugrknj.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gffgxbarc.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gjpkzhlnk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gbzgtfuue.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/glnibhzyu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gjfxtrpvb.sHtML

[S19] C：快速排序
来源：http://www.share.vehdjk.com/Article/details/ggfkgbfsn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/grelozmnz.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gbrcpzrcp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.bbcook.cn/Article/details/goegrmhnw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.sjlbkw.cn/Article/details/grziuirqa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fktsv.cn/Article/details/ggplozyhu.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gsddhbrus.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gowherzil.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/giiwijwfb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/guhyzqhwm.sHtML

[S24] C：获取本地时间
来源：http://www.share.sjlbkw.cn/Article/details/gzkxvhomk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fktsv.cn/Article/details/genzklbcx.sHtML

[S25] C：内存拷贝
来源：http://mobile.epnwcf.com/Article/details/gojtgidpa.sHtML

memcpy(dst, src, n);
来源：http://m.share.fktsv.cn/Article/details/goyeorgup.sHtML

[S26] C：内存清零
来源：http://mobile.epnwcf.com/Article/details/ggrgoyaey.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gleoydkki.sHtML

[S27] C：定义常量
来源：http://3g.vehdjk.com/Article/details/gvfsseghl.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/ghklwctja.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gjsgadtir.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gpzvgpksm.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gpglakccc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fktsv.cn/Article/details/gejulldiy.sHtML

[S30] C：头文件保护
来源：http://www.share.yfazqb.com/Article/details/gnwvuvmii.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gdvakkqcs.sHtML

#define X_H
来源：http://www.m.share.tarul.cn/Article/details/gctrtjyum.sHtML

#endif
来源：http://m.share.epnwcf.com/Article/details/gbreuinqj.sHtML

[S31] C++：Hello World
来源：http://www.blog.fktsv.cn/Article/details/grecapqkw.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gcwnacbil.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.epnwcf.com/Article/details/gvnmkvfxd.sHtML

[S32] C++：字符串
来源：http://baike.epnwcf.com/Article/details/ggjkmbqkj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/gymyonwyy.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gehvszpac.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.sjlbkw.cn/Article/details/ghjykyrsw.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.bbcook.cn/Article/details/gxkhjimoz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fktsv.cn/Article/details/ggponfnth.sHtML

[S35] C++：map
来源：http://www.blog.tarul.cn/Article/details/guaevcvia.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/ggzooawli.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gdrbezonj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fktsv.cn/Article/details/granvjhfn.sHtML

[S37] C++：set
来源：http://m.share.sjlbkw.cn/Article/details/gvsaelvnh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.sjlbkw.cn/Article/details/gzrambxft.sHtML

[S38] C++：排序
来源：http://blog.fktsv.cn/Article/details/gxacaxgoe.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.bbcook.cn/Article/details/gfjmvjhkn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.epnwcf.com/Article/details/grvkpsgue.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gfznjqqrc.sHtML

[S40] C++：查找元素
来源：http://www.share.vehdjk.com/Article/details/gtnrrklco.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.tarul.cn/Article/details/gflbcpqhq.sHtML

[S41] C++：类与构造函数
来源：http://wap.fktsv.cn/Article/details/gvhpdkbih.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/gcybgghkl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/gzpwkxpja.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.sjlbkw.cn/Article/details/goyhgkiqu.sHtML

[S43] C++：智能指针
来源：http://read.share.sjlbkw.cn/Article/details/gkakzqghi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.tarul.cn/Article/details/gzabrqapj.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gqxlfibro.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/gwrewkgam.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gubsyrpkz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.epnwcf.com/Article/details/gfuktvpou.sHtML

[S46] C++：函数模板
来源：http://www.share.vehdjk.com/Article/details/grheffpgp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.vehdjk.com/Article/details/gkvjqfeer.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/glxurpexm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/glnsnkzjw.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gulnsbano.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gnsvhyusa.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.vehdjk.com/Article/details/glqvmofjr.sHtML

[S49] C++：写文件
来源：http://wap.yfazqb.com/Article/details/gzsvrkfcj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gsldsfgjs.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/guysibthc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gcfgjkbam.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gvwgjwutw.sHtML

static_cast<double>(a) / b
来源：http://read.share.epnwcf.com/Article/details/gkoejvovn.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.epnwcf.com/Article/details/guveeicie.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fktsv.cn/Article/details/gnrvogwlm.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gayyotdao.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gcrixhrag.sHtML

[S54] C++：异常处理
来源：http://www.blog.bbcook.cn/Article/details/gzqdoejxn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gfkpvzofi.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gdvbiyelg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gfdaslwbv.sHtML

[S56] C++：optional
来源：http://www.share.tarul.cn/Article/details/gosfmdrzk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.bbcook.cn/Article/details/gleaiqtpr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/gimbpscjv.sHtML

constexpr int N = 10;
来源：http://www.blog.vehdjk.com/Article/details/gozfqretz.sHtML

[S58] C++：命名空间
来源：http://wap.epnwcf.com/Article/details/glojmdyev.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/gmknuuovz.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gydjaftzo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.tarul.cn/Article/details/ggbwjcwur.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fktsv.cn/Article/details/gbrxggenj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gobbnoaig.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdsrqqbjy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.vehdjk.com/Article/details/gmuqksjfb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gqxshbsqc.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.epnwcf.com/Article/details/gudlbmqew.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gsgjsrtjr.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gginwjdtb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.yfazqb.com/Article/details/golluxxuy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.vehdjk.com/Article/details/geyjwbojv.sHtML

"值: $b"
来源：http://3g.vehdjk.com/Article/details/gvuqdyzsa.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gsgksjptd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.tarul.cn/Article/details/gxanfvrvp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gxnjivbmj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.vehdjk.com/Article/details/gbtiakdba.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gnftmdhnb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gcwdvhrch.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/glgexsyqt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.bbcook.cn/Article/details/gixidprjk.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/gqntpvrge.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gycksgwxc.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gdemdivew.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gscicpgwg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.bbcook.cn/Article/details/gpqifofzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/ghenrhwmf.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gycxywrsd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.epnwcf.com/Article/details/gfpikyfcc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.sjlbkw.cn/Article/details/gadrsswjf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.vehdjk.com/Article/details/gxpailltr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/gktpkunww.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.tarul.cn/Article/details/gyeherwot.sHtML

[T14] Kotlin：循环
来源：http://mobile.bbcook.cn/Article/details/gicqiiitg.sHtML

for (i in 1..10) println(i)
来源：http://blog.vehdjk.com/Article/details/gfkyipthn.sHtML

[T15] Kotlin：接口
来源：http://read.share.yfazqb.com/Article/details/gbdjhujfh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gbbyjymlg.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/gmbvblpks.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/ggpohmjam.sHtML

[T17] Swift：变量与常量
来源：http://wap.yfazqb.com/Article/details/gsufmvdta.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fktsv.cn/Article/details/ggkdelkhl.sHtML

[T18] Swift：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gdiuozcbz.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gkptymsuu.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/glcogdoud.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gfilccano.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gmuskkndh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gkajxzsno.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/gfqlqzpto.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gtzqyndva.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gvgulureb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gihpwwzgf.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gnxyjtpsg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.bbcook.cn/Article/details/ghknlcrvf.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gxxwgxgwc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.vehdjk.com/Article/details/gcxzybcuw.sHtML

[T25] Swift：结构体
来源：http://www.share.vehdjk.com/Article/details/glqvhrjvz.sHtML

struct P { var x: Int }
来源：http://baike.bbcook.cn/Article/details/grzvrfxrg.sHtML

[T26] Swift：类与重写
来源：http://3g.bbcook.cn/Article/details/giandmhgb.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/ggzmxxkjb.sHtML

[T27] Swift：错误处理
来源：http://read.share.vehdjk.com/Article/details/goknhgyvm.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/gllzjwjud.sHtML

[T28] Swift：枚举
来源：http://read.share.vehdjk.com/Article/details/gcmniimrr.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/gqngcnnlr.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gqowwolaz.sHtML

guard let x = opt else { return }
来源：http://www.blog.vehdjk.com/Article/details/ggwvmejnl.sHtML

[T30] Swift：协议
来源：http://3g.bbcook.cn/Article/details/gsvavkjib.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fktsv.cn/Article/details/gxgridocm.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gudyphjrl.sHtML

print("Hello")
来源：http://m.share.fktsv.cn/Article/details/gyrauegut.sHtML

[T32] Lua：局部变量
来源：http://3g.bbcook.cn/Article/details/ghwexbqwx.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/goeverayr.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fktsv.cn/Article/details/gzumfwmwx.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.tarul.cn/Article/details/gghojncqr.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gqqwfkale.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.sjlbkw.cn/Article/details/gddmmlfvv.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/ghhqwsath.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.yfazqb.com/Article/details/gzgfrrtje.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/grhprpjyj.sHtML

function add(a, b) return a + b end
来源：http://www.blog.yfazqb.com/Article/details/gjfjkbjim.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/ggkrjhijf.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gpspvtyll.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gvoosenxx.sHtML

if x > 0 then print("正") end
来源：http://wap.fktsv.cn/Article/details/ghewwordz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gtvheqsrg.sHtML

string.find(s, "%d+")
来源：http://www.share.vehdjk.com/Article/details/gcbuaaadw.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gjhkqrplm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gjeuutqcb.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/genbatrnp.sHtML

print "Hello\n";
来源：http://read.share.vehdjk.com/Article/details/godzhqapx.sHtML

[T42] Perl：变量类型
来源：http://www.blog.sjlbkw.cn/Article/details/gdaofmkip.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/gvjfjxqxm.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gecukejhh.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/gouuucqri.sHtML

[T44] Perl：条件
来源：http://baike.epnwcf.com/Article/details/glmbfttzw.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.epnwcf.com/Article/details/gqhwkiaus.sHtML

[T45] Perl：数组遍历
来源：http://www.share.tarul.cn/Article/details/gbdfgetks.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.epnwcf.com/Article/details/gpxdgockz.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/grzzzypgy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.tarul.cn/Article/details/gtkgjdwin.sHtML

[T47] Perl：正则捕获
来源：http://read.share.vehdjk.com/Article/details/gcosstrtp.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/gimhrvkrh.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/ggfblcxfb.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gizwrfgyc.sHtML

[T49] Perl：函数
来源：http://wap.epnwcf.com/Article/details/geaiwlxbl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gugytrqvd.sHtML

[T50] Perl：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gxtypllty.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gsflgebam.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gigdzmmen.sHtML

[T51] Scala：Hello World
来源：http://m.share.fktsv.cn/Article/details/gpwmdioac.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gdczcvfax.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gcmgrkrhw.sHtML

val a = 1;  var b = 2
来源：http://baike.fktsv.cn/Article/details/gyoymydah.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gvwtrdepw.sHtML

s"值: $b"
来源：http://wap.yfazqb.com/Article/details/gbukepxgf.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gsannptxf.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.tarul.cn/Article/details/gqlqzikcs.sHtML

[T55] Scala：集合过滤
来源：http://baike.vehdjk.com/Article/details/gdifqvjbi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.tarul.cn/Article/details/gydywteiw.sHtML

[T56] Scala：样例类
来源：http://baike.bbcook.cn/Article/details/gxjaiauxj.sHtML

case class User(name: String, age: Int)
来源：http://blog.vehdjk.com/Article/details/gxurzmsqn.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gblztwiay.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gtvkdbzmq.sHtML

[T58] Scala：函数定义
来源：http://www.share.epnwcf.com/Article/details/gfibykjhb.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gegnsddwf.sHtML

[T59] Scala：循环
来源：http://3g.epnwcf.com/Article/details/gapvtjuaw.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.bbcook.cn/Article/details/gmevtsprl.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gdzenbraj.sHtML


<!-- 参考信息 -->