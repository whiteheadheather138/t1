代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.yfazqb.com/Article/details/gjhcrbueu.sHtML

[R58] 下载文件
来源：http://wap.tarul.cn/Article/details/gkcmfijzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.yfazqb.com/Article/details/gcssfazyb.sHtML

[R59] 发 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gkoosbsxv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.bbcook.cn/Article/details/gwqrydhtn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gpxqeqlrm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.epnwcf.com/Article/details/gdotnnvps.sHtML

[R61] 磁盘占用
来源：http://mobile.fktsv.cn/Article/details/gefitfwik.sHtML

df -h;  du -sh *
来源：http://wap.tarul.cn/Article/details/gxphuvctr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gldamxyyi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/geybpxydt.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gimvwrxib.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gmiolduzp.sHtML

[R64] 结束进程
来源：http://read.share.epnwcf.com/Article/details/gzbckoizq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.vehdjk.com/Article/details/ghlezavhj.sHtML

[R65] 查看端口占用
来源：http://www.blog.vehdjk.com/Article/details/golzxdjlx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gdyecotjh.sHtML

[R66] 定时任务
来源：http://baike.yfazqb.com/Article/details/ghttdwamu.sHtML

crontab -e;  crontab -l
来源：http://read.share.bbcook.cn/Article/details/ghsstnizd.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/ghxklyqws.sHtML

openssl rand -hex 16
来源：http://baike.bbcook.cn/Article/details/gwrlxxexp.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gcyiisuha.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fktsv.cn/Article/details/gejpnweje.sHtML

[R69] 生成随机密码
来源：http://read.share.sjlbkw.cn/Article/details/gjkqhmjeo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gxxqmcial.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdlqlnrf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.sjlbkw.cn/Article/details/gotefddwx.sHtML

[R71] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gnvkvxdzn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gmnncdtug.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gktjndxcj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/guudgwsnx.sHtML

[R73] 分割大日志
来源：http://wap.tarul.cn/Article/details/gfemneede.sHtML

split -l 1000 big.log part_
来源：http://baike.tarul.cn/Article/details/gvmlefrmv.sHtML

[R74] 批量重命名
来源：http://mobile.epnwcf.com/Article/details/gzlxgoyoh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gmykrxalv.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gewuwbapo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.tarul.cn/Article/details/gmbchhini.sHtML

[R76] 使用临时文件
来源：http://baike.fktsv.cn/Article/details/gmjpxjykf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gjqyiunil.sHtML

[R77] 读取用户输入
来源：http://m.share.tarul.cn/Article/details/gnsuivhou.sHtML

read -rp "请输入: " ans
来源：http://www.blog.yfazqb.com/Article/details/gbzhrkbkl.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gndtysjez.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gyfxxosgz.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gdnlqvefu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.tarul.cn/Article/details/gdsgeiiis.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdtiaooe.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gwlhjopip.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcovjvsyy.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gyaaaahah.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gggvpqmfz.sHtML

[S01] C：Hello World
来源：http://baike.bbcook.cn/Article/details/gaxnfsszr.sHtML

#include <stdio.h>
来源：http://3g.bbcook.cn/Article/details/gxkenyunl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gaeprprts.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.tarul.cn/Article/details/gbcvjepdi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.epnwcf.com/Article/details/gkqjpkkii.sHtML

[S03] C：读入整数
来源：http://m.share.yfazqb.com/Article/details/gzwfuqapj.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gxyegejar.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/gnbfudixy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.tarul.cn/Article/details/gaugfxdje.sHtML

[S05] C：字符串长度
来源：http://www.share.epnwcf.com/Article/details/ghwacpmsb.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gfucnyhhl.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gekcpiwcl.sHtML

strcmp(a, b) == 0
来源：http://www.share.sjlbkw.cn/Article/details/guatgxnnu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/gjshbuikp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.tarul.cn/Article/details/gqxgomhai.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.yfazqb.com/Article/details/gfxmincbh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.sjlbkw.cn/Article/details/gutipghpo.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gshpthaiu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.vehdjk.com/Article/details/gymkvcmnz.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gvwbhudau.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gjsgowtse.sHtML

[S11] C：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/grgfvmbzk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.yfazqb.com/Article/details/gfmomyagp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.vehdjk.com/Article/details/givkxagml.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/gsyvpefya.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/ghxobdqwl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.vehdjk.com/Article/details/gvkzrpjqp.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/gmaevnxht.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gtxgprgjv.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/gmruumltk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.yfazqb.com/Article/details/gxvfaszve.sHtML

[S15] C：类型转换
来源：http://3g.bbcook.cn/Article/details/gwjrvqacb.sHtML

(double) a / b
来源：http://blog.epnwcf.com/Article/details/ggpzyqfhn.sHtML

[S16] C：位操作置位
来源：http://m.share.vehdjk.com/Article/details/gnlhvyvbq.sHtML

x |= (1 << 3);
来源：http://baike.epnwcf.com/Article/details/gkvuuppou.sHtML

[S17] C：安全拼接字符串
来源：http://blog.epnwcf.com/Article/details/gmmqowcdg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/glhyeychf.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gveqspawk.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gznosvokd.sHtML

[S19] C：快速排序
来源：http://wap.vehdjk.com/Article/details/gzqarevja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gxkfzjppm.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gqknetohm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gkvbfgzak.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.yfazqb.com/Article/details/gfsfspywa.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.epnwcf.com/Article/details/guoekbyne.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gzyqpyvvz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.epnwcf.com/Article/details/ggeinfjon.sHtML

[S23] C：随机数
来源：http://baike.yfazqb.com/Article/details/gmrsfwtdp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.vehdjk.com/Article/details/gdfbkahlh.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gsfwitraj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/guayiphcp.sHtML

[S25] C：内存拷贝
来源：http://mobile.bbcook.cn/Article/details/gillunmkc.sHtML

memcpy(dst, src, n);
来源：http://wap.yfazqb.com/Article/details/grfhptota.sHtML

[S26] C：内存清零
来源：http://www.m.share.bbcook.cn/Article/details/gkoditatq.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.bbcook.cn/Article/details/gmivpwptv.sHtML

[S27] C：定义常量
来源：http://mobile.sjlbkw.cn/Article/details/grqxblmwf.sHtML

const double PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gqmzwnjau.sHtML

[S28] C：静态变量
来源：http://mobile.yfazqb.com/Article/details/gtkyywjuh.sHtML

static int counter = 0;
来源：http://blog.tarul.cn/Article/details/gubdnvmub.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gilhkcycj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.tarul.cn/Article/details/guobvnsme.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/guqsmobdy.sHtML

#ifndef X_H
来源：http://m.share.vehdjk.com/Article/details/gxhybsbrv.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/gixnxnigy.sHtML

#endif
来源：http://www.blog.vehdjk.com/Article/details/gplynxkkv.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gkxvyhjva.sHtML

#include <iostream>
来源：http://mobile.epnwcf.com/Article/details/gihkglrwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.tarul.cn/Article/details/gbhkgrgzp.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gsqjhwjyg.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gozwkobqp.sHtML

[S33] C++：vector 增删
来源：http://read.share.bbcook.cn/Article/details/gjdmgdhlz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.vehdjk.com/Article/details/gwmvsqdiq.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gmfjgbfbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/gnehtyuek.sHtML

[S35] C++：map
来源：http://3g.tarul.cn/Article/details/gxwmkwwlj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/giasuldlw.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/gkddxqmzt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gonhwffod.sHtML

[S37] C++：set
来源：http://www.share.bbcook.cn/Article/details/gtnuiynol.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gxolxpyvn.sHtML

[S38] C++：排序
来源：http://mobile.tarul.cn/Article/details/gzmpegyzo.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gfnyqxach.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gnraeimsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.epnwcf.com/Article/details/gwkitsoac.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gxdmpmbde.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.bbcook.cn/Article/details/gnqyhchyu.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gtaslwosw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gjkrkkagk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbptnblco.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.sjlbkw.cn/Article/details/glbwfpsdv.sHtML

[S43] C++：智能指针
来源：http://read.share.epnwcf.com/Article/details/ghrlugppn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/gzejhdzro.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/gozfhovsb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fktsv.cn/Article/details/goiexhusi.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gzxngindj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.vehdjk.com/Article/details/golgulcdg.sHtML

[S46] C++：函数模板
来源：http://3g.fktsv.cn/Article/details/gtqvashra.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gowsqrwpl.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fktsv.cn/Article/details/gcnygbqlr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.sjlbkw.cn/Article/details/gblttfzoy.sHtML

[S48] C++：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gzyngfryp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fktsv.cn/Article/details/gmawhyycx.sHtML

while (std::getline(in, line)) { }
来源：http://baike.sjlbkw.cn/Article/details/gexwotfzw.sHtML

[S49] C++：写文件
来源：http://blog.bbcook.cn/Article/details/gjevnishl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gokcatiam.sHtML

[S50] C++：格式化数字
来源：http://www.blog.bbcook.cn/Article/details/gxqcwvplk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fktsv.cn/Article/details/grxjmrizy.sHtML

[S51] C++：显式类型转换
来源：http://www.share.sjlbkw.cn/Article/details/gqxbgcqmh.sHtML

static_cast<double>(a) / b
来源：http://www.blog.sjlbkw.cn/Article/details/gfpgiztjf.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/giqwytvkr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gmpfdhseo.sHtML

[S53] C++：移动语义
来源：http://3g.yfazqb.com/Article/details/gskptnfyq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gmdrbclga.sHtML

[S54] C++：异常处理
来源：http://read.share.bbcook.cn/Article/details/gtdzhbgwv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gctfsabnd.sHtML

[S55] C++：结构化绑定
来源：http://3g.tarul.cn/Article/details/gkpaklgou.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gucojhxbw.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/gfrtmrgbt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gcovnozdj.sHtML

[S57] C++：编译期常量
来源：http://www.share.sjlbkw.cn/Article/details/gammcygpo.sHtML

constexpr int N = 10;
来源：http://wap.sjlbkw.cn/Article/details/gwkadkiqt.sHtML

[S58] C++：命名空间
来源：http://wap.yfazqb.com/Article/details/gjqkemrgj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/glelqetqk.sHtML

[S59] C++：静态断言
来源：http://m.share.vehdjk.com/Article/details/gnhndlpzs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/ghzhafrkt.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.tarul.cn/Article/details/gjehmqxwx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gypuafeiq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/goppnypcd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/giszsoesd.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gmenkgasx.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gfnqmvyyx.sHtML

println("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gcptrqqxh.sHtML

[T02] Kotlin：变量
来源：http://www.blog.bbcook.cn/Article/details/gkadbilca.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gkyymsjrv.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.vehdjk.com/Article/details/ghaujcowr.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gqbvsiqgu.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gskhgxbll.sHtML

val n: String? = null;  n?.length
来源：http://read.share.tarul.cn/Article/details/guwoyesca.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gdnaggmkh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.yfazqb.com/Article/details/gbiqasywi.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.bbcook.cn/Article/details/gpyxzxkxg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/gmkwfrvxu.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.vehdjk.com/Article/details/gpgfvvwpb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gekxillwp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.bbcook.cn/Article/details/gbupbmirj.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fktsv.cn/Article/details/gtvxxrrza.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gbllylahf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.sjlbkw.cn/Article/details/gtvxhfjbs.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/gbqhslzqf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.vehdjk.com/Article/details/glvtdmnuy.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.epnwcf.com/Article/details/gvxgpdwuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gfryynwcs.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.yfazqb.com/Article/details/garqxyiug.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.sjlbkw.cn/Article/details/guamtcpzh.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdzndatc.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gqgieucsa.sHtML

[T14] Kotlin：循环
来源：http://www.share.yfazqb.com/Article/details/gbxrficks.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gatwynifr.sHtML

[T15] Kotlin：接口
来源：http://3g.bbcook.cn/Article/details/gyxaeuiho.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fktsv.cn/Article/details/gceelucgp.sHtML

[T16] Swift：Hello World
来源：http://blog.vehdjk.com/Article/details/gjmvkusfn.sHtML

print("Hello")
来源：http://blog.sjlbkw.cn/Article/details/gikjcnlsn.sHtML

[T17] Swift：变量与常量
来源：http://baike.sjlbkw.cn/Article/details/gnajpawgm.sHtML

var a = 1;  let b = 2
来源：http://baike.vehdjk.com/Article/details/gmifqdolb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gmiaxwwer.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gqhghrwfp.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gmslvyqqs.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/glbnhsimh.sHtML

[T20] Swift：数组操作
来源：http://www.blog.vehdjk.com/Article/details/gapwcosdo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.epnwcf.com/Article/details/gkdtqekyb.sHtML

[T21] Swift：遍历
来源：http://blog.fktsv.cn/Article/details/gjyvnyulb.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gqrmqjsis.sHtML

[T22] Swift：字典
来源：http://wap.epnwcf.com/Article/details/gibebrlph.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.bbcook.cn/Article/details/gnyiznlym.sHtML

[T23] Swift：函数
来源：http://m.share.bbcook.cn/Article/details/gqacnbwyg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.bbcook.cn/Article/details/gdtdqgydi.sHtML

[T24] Swift：闭包
来源：http://read.share.yfazqb.com/Article/details/grnkxydyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gdbkleker.sHtML

[T25] Swift：结构体
来源：http://wap.sjlbkw.cn/Article/details/gxextzoch.sHtML

struct P { var x: Int }
来源：http://www.blog.tarul.cn/Article/details/gxncmkavd.sHtML

[T26] Swift：类与重写
来源：http://www.share.fktsv.cn/Article/details/genxtjjdj.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.epnwcf.com/Article/details/gpwjbttjn.sHtML

[T27] Swift：错误处理
来源：http://mobile.fktsv.cn/Article/details/glmlaoneq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gwttmvkjg.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/gyvapqvvi.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gkknqyzgb.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.sjlbkw.cn/Article/details/gvicwskkg.sHtML

guard let x = opt else { return }
来源：http://mobile.vehdjk.com/Article/details/gxqgfybxk.sHtML

[T30] Swift：协议
来源：http://blog.tarul.cn/Article/details/gdkplaztw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gpipzgjgo.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/glalbmwqb.sHtML

print("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gbliicgmp.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gvkyzemwj.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gmmtikpkq.sHtML

[T33] Lua：表（数组）
来源：http://3g.yfazqb.com/Article/details/griewjreo.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gdgnfhjzx.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gjrntyszp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/gzuutakwy.sHtML

[T35] Lua：字典表
来源：http://www.m.share.epnwcf.com/Article/details/gtksnoeoc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/gahakoqnm.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gdtclepol.sHtML

function add(a, b) return a + b end
来源：http://read.share.epnwcf.com/Article/details/gcfngwhft.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.tarul.cn/Article/details/gpifxnxnc.sHtML

"a" .. "b"
来源：http://www.m.share.vehdjk.com/Article/details/gjsscftps.sHtML

[T38] Lua：条件
来源：http://www.share.bbcook.cn/Article/details/govuhogix.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gnhrmotyp.sHtML

[T39] Lua：模式匹配
来源：http://m.share.sjlbkw.cn/Article/details/gtkclwemf.sHtML

string.find(s, "%d+")
来源：http://3g.bbcook.cn/Article/details/gnzsevmdx.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gpqbmxkwf.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.tarul.cn/Article/details/gyxnfbrsn.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gepnejdng.sHtML

print "Hello\n";
来源：http://www.m.share.bbcook.cn/Article/details/gnceqbizm.sHtML

[T42] Perl：变量类型
来源：http://mobile.fktsv.cn/Article/details/grogvbqqh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gdtpzgnbo.sHtML

[T43] Perl：字符串插值
来源：http://baike.fktsv.cn/Article/details/gvswqwqaf.sHtML

"值: $a"
来源：http://www.share.sjlbkw.cn/Article/details/gcbrxzrhc.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/gkelvcnoj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gylxscoab.sHtML

[T45] Perl：数组遍历
来源：http://mobile.fktsv.cn/Article/details/gvroqjpzs.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gcgspsfkx.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.yfazqb.com/Article/details/getmzbxqs.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.tarul.cn/Article/details/gwexpwxht.sHtML

[T47] Perl：正则捕获
来源：http://3g.yfazqb.com/Article/details/glirdstbo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gvldocpyq.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gauxtylag.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.sjlbkw.cn/Article/details/gklbfyoul.sHtML

[T49] Perl：函数
来源：http://wap.fktsv.cn/Article/details/glpkcrola.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gpggkwbzw.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gyueblaib.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.bbcook.cn/Article/details/gqckgaygk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/gzxosewap.sHtML

[T51] Scala：Hello World
来源：http://baike.vehdjk.com/Article/details/gxprkeqau.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gamgvkbaa.sHtML

[T52] Scala：变量
来源：http://3g.sjlbkw.cn/Article/details/gmkpgijgn.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gdomodgaf.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gckctgxts.sHtML

s"值: $b"
来源：http://www.blog.bbcook.cn/Article/details/gmrtiropf.sHtML

[T54] Scala：集合映射
来源：http://www.share.tarul.cn/Article/details/grjpfyiqz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.tarul.cn/Article/details/grlbjzrzl.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gofcosprk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gmanwxyqi.sHtML

[T56] Scala：样例类
来源：http://www.share.vehdjk.com/Article/details/gexcnnfgj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.vehdjk.com/Article/details/gxudyyboq.sHtML

[T57] Scala：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gwfhnemue.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.tarul.cn/Article/details/gxgowzsbz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.yfazqb.com/Article/details/gnkwryqzh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.yfazqb.com/Article/details/gdbxggvnh.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/ggslzcpps.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gwparmkxl.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/gifdhgghs.sHtML


<!-- 参考信息 -->