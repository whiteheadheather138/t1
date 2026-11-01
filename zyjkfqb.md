代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gzbxweiqj.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gayqzdzuo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gohrrdzgk.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gwjbxjgtp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/ghusxsjiw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/geakhefav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.yfazqb.com/Article/details/guskfxfgg.sHtML

[R61] 磁盘占用
来源：http://baike.epnwcf.com/Article/details/gfdvvptfz.sHtML

df -h;  du -sh *
来源：http://baike.vehdjk.com/Article/details/glpmttudc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.bbcook.cn/Article/details/gsfntbchj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gpcxzeqch.sHtML

[R63] 内存与进程
来源：http://www.blog.bbcook.cn/Article/details/gabpymsqh.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gdvwazntj.sHtML

[R64] 结束进程
来源：http://m.share.epnwcf.com/Article/details/gbjwhwebk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fktsv.cn/Article/details/gyilydyro.sHtML

[R65] 查看端口占用
来源：http://baike.tarul.cn/Article/details/gjferycxf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/giiyrangt.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/gccqguzjw.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gddyeaxil.sHtML

[R67] 生成随机十六进制串
来源：http://wap.sjlbkw.cn/Article/details/gebxsixbz.sHtML

openssl rand -hex 16
来源：http://mobile.yfazqb.com/Article/details/gjqnadcrv.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gekpetluj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/gfyodpflq.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gsadlnuul.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.vehdjk.com/Article/details/glwdctpmn.sHtML

[R70] 时间戳与互转
来源：http://baike.tarul.cn/Article/details/gxbqmvrju.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.vehdjk.com/Article/details/gonuxbxlf.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gghidtgoa.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/grletdhot.sHtML

[R72] 等待端口就绪
来源：http://baike.bbcook.cn/Article/details/gkrmxayfr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gwhovmmlz.sHtML

[R73] 分割大日志
来源：http://www.share.vehdjk.com/Article/details/gklrpubkq.sHtML

split -l 1000 big.log part_
来源：http://m.share.yfazqb.com/Article/details/gephpfvum.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gfhysulbj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.yfazqb.com/Article/details/gchpztjpx.sHtML

[R75] 导出环境变量
来源：http://www.m.share.vehdjk.com/Article/details/ggxjsyrbq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/geggtwjaw.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/grjbngtbt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gbmqiqkgr.sHtML

[R77] 读取用户输入
来源：http://www.share.vehdjk.com/Article/details/gobyxbjvd.sHtML

read -rp "请输入: " ans
来源：http://blog.tarul.cn/Article/details/gandssele.sHtML

[R78] 交互式菜单
来源：http://blog.tarul.cn/Article/details/ghtgftler.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fktsv.cn/Article/details/glihizfia.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gscatyvvw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/godgedatt.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gdtajtwke.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gbdneymcg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/goceccdlp.sHtML

S. C / C++ 专题
来源：http://blog.tarul.cn/Article/details/goqtskcul.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gebstvkcc.sHtML

[S01] C：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gwiuesfnb.sHtML

#include <stdio.h>
来源：http://baike.bbcook.cn/Article/details/grpdgwlwt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.yfazqb.com/Article/details/gedxubyfs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.bbcook.cn/Article/details/gqixgkjgs.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gzjrkmehn.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gpozgltsx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fktsv.cn/Article/details/guegrufxf.sHtML

[S04] C：字符串复制
来源：http://m.share.vehdjk.com/Article/details/gzarrpyqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/ghqjxesck.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gggrjynzl.sHtML

strlen(s)
来源：http://www.share.bbcook.cn/Article/details/ggigugriz.sHtML

[S06] C：字符串比较
来源：http://baike.yfazqb.com/Article/details/gjxupulye.sHtML

strcmp(a, b) == 0
来源：http://read.share.fktsv.cn/Article/details/goficyrmy.sHtML

[S07] C：数组遍历求和
来源：http://3g.bbcook.cn/Article/details/guodyulca.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.yfazqb.com/Article/details/ghnkpafld.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.epnwcf.com/Article/details/gwwbiwwkt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.sjlbkw.cn/Article/details/gzrbgjosd.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/gxpbpdsle.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.vehdjk.com/Article/details/gbirzhsqz.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gumyjgcmn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fktsv.cn/Article/details/ghqzcwfji.sHtML

[S11] C：逐行读文件
来源：http://mobile.tarul.cn/Article/details/ghfndgkfy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fktsv.cn/Article/details/gyvvkauef.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gznjnyqzj.sHtML

fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gphaxszvy.sHtML

[S12] C：写文件
来源：http://www.blog.sjlbkw.cn/Article/details/gwugmhyzb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/gdmafloyr.sHtML

[S13] C：宏定义
来源：http://blog.fktsv.cn/Article/details/ghuxvdsuh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.tarul.cn/Article/details/gwsoybxur.sHtML

[S14] C：枚举
来源：http://read.share.bbcook.cn/Article/details/gncdrhdrb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gktbefian.sHtML

[S15] C：类型转换
来源：http://3g.epnwcf.com/Article/details/gowycrnbp.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/ghlictpcy.sHtML

[S16] C：位操作置位
来源：http://mobile.tarul.cn/Article/details/glmfpoqjj.sHtML

x |= (1 << 3);
来源：http://m.share.sjlbkw.cn/Article/details/gcswgpjvc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/grxfqfduq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.vehdjk.com/Article/details/gsvimlglo.sHtML

[S18] C：命令行参数
来源：http://mobile.fktsv.cn/Article/details/gvkibntal.sHtML

int main(int argc, char **argv)
来源：http://wap.sjlbkw.cn/Article/details/gpijfzzor.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gwfisfugp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.vehdjk.com/Article/details/goksvemno.sHtML

[S20] C：二分查找
来源：http://www.blog.bbcook.cn/Article/details/gvtgqyobk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gehslspmv.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gimclwajm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.sjlbkw.cn/Article/details/grwzxnfup.sHtML

[S22] C：字符串转数字
来源：http://3g.fktsv.cn/Article/details/ggxstfbix.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.epnwcf.com/Article/details/gwrpjjjtr.sHtML

[S23] C：随机数
来源：http://www.blog.tarul.cn/Article/details/gjhohtull.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gchvwrldt.sHtML

[S24] C：获取本地时间
来源：http://www.share.yfazqb.com/Article/details/ghegmlxom.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.bbcook.cn/Article/details/ggpeypcoa.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.bbcook.cn/Article/details/ghxvcngok.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/goobedzsk.sHtML

[S26] C：内存清零
来源：http://wap.sjlbkw.cn/Article/details/gjazsugti.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/glvvktwxx.sHtML

[S27] C：定义常量
来源：http://www.blog.sjlbkw.cn/Article/details/gvlobpech.sHtML

const double PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gezrmpbhp.sHtML

[S28] C：静态变量
来源：http://blog.vehdjk.com/Article/details/gzrcikxlo.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/glsuulhar.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/geoankucc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.yfazqb.com/Article/details/glvydptxu.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gthcqimac.sHtML

#ifndef X_H
来源：http://blog.bbcook.cn/Article/details/grdufeqxj.sHtML

#define X_H
来源：http://3g.epnwcf.com/Article/details/ggkpnympu.sHtML

#endif
来源：http://www.share.yfazqb.com/Article/details/glmeqmrpo.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gvlhgsogi.sHtML

#include <iostream>
来源：http://mobile.fktsv.cn/Article/details/ggdnsddrv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.tarul.cn/Article/details/ggqqnxupe.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/gppfvedgi.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.epnwcf.com/Article/details/gtgeuxrzp.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gpgozigdx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.bbcook.cn/Article/details/gyjfbosbb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fktsv.cn/Article/details/gzxiuckee.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.sjlbkw.cn/Article/details/grzuojjha.sHtML

[S35] C++：map
来源：http://www.m.share.bbcook.cn/Article/details/gktgdwkxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/giuippadw.sHtML

[S36] C++：unordered_map
来源：http://blog.vehdjk.com/Article/details/gcneiqztv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.yfazqb.com/Article/details/gxrxuzmne.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gopmjatmp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.yfazqb.com/Article/details/gaqrbfsbf.sHtML

[S38] C++：排序
来源：http://m.share.yfazqb.com/Article/details/gyvmcnyxk.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.bbcook.cn/Article/details/gugogbusb.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gxfjipdhz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.yfazqb.com/Article/details/gwbdusdwf.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gsevmygel.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/ghgetxyek.sHtML

[S41] C++：类与构造函数
来源：http://www.share.vehdjk.com/Article/details/gmgkqublb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.bbcook.cn/Article/details/gmwjcdwyw.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/gnpighzor.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.epnwcf.com/Article/details/gcmybzahx.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gookxsjqq.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.tarul.cn/Article/details/gagwlykne.sHtML

[S44] C++：引用传参
来源：http://www.share.fktsv.cn/Article/details/gwllsdeyy.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gofipwxdi.sHtML

[S45] C++：lambda
来源：http://www.share.fktsv.cn/Article/details/gdodyaxvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.sjlbkw.cn/Article/details/gvdysfuvf.sHtML

[S46] C++：函数模板
来源：http://www.blog.fktsv.cn/Article/details/gcavrlgos.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.yfazqb.com/Article/details/gyeeqitdt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.yfazqb.com/Article/details/gqqtcfyke.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.sjlbkw.cn/Article/details/gogixkrpn.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gouoirupz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gomiuguuz.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.bbcook.cn/Article/details/gujvvistb.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gitkvvioo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.yfazqb.com/Article/details/gyjknkozq.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gscclvqml.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.yfazqb.com/Article/details/gdqlklfer.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gtskbvvdt.sHtML

static_cast<double>(a) / b
来源：http://blog.bbcook.cn/Article/details/ggahrlnkk.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.yfazqb.com/Article/details/gssynzspu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.vehdjk.com/Article/details/gmtmvrghj.sHtML

[S53] C++：移动语义
来源：http://blog.vehdjk.com/Article/details/gztdimljh.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.sjlbkw.cn/Article/details/gykrthfxp.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gvtdrrcjw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.vehdjk.com/Article/details/ghqjipxlx.sHtML

[S55] C++：结构化绑定
来源：http://3g.vehdjk.com/Article/details/gpajfgrfl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gtwopbqlg.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/gmsoxrdpo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gvbzosrjj.sHtML

[S57] C++：编译期常量
来源：http://wap.epnwcf.com/Article/details/gjyvkhsas.sHtML

constexpr int N = 10;
来源：http://blog.sjlbkw.cn/Article/details/gvfxcqmcp.sHtML

[S58] C++：命名空间
来源：http://www.blog.tarul.cn/Article/details/ghmmerayg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gegxzcilo.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/gcywyrbgn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fktsv.cn/Article/details/gqchmvlyr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.yfazqb.com/Article/details/gxsibqlkd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gbhxedmuo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfqrzrezf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gddfacizn.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjasgnouk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/gqoibvdtz.sHtML

println("Hello")
来源：http://mobile.tarul.cn/Article/details/gtyitkhww.sHtML

[T02] Kotlin：变量
来源：http://blog.fktsv.cn/Article/details/gmssqglqd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.vehdjk.com/Article/details/ghkhhmzyp.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.tarul.cn/Article/details/gjzecptyk.sHtML

"值: $b"
来源：http://3g.yfazqb.com/Article/details/gxbgkzmtu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gwfyrdfoe.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gychaaaem.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/gzrgbknlp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gemskmlwy.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.epnwcf.com/Article/details/gexnxlhlv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.epnwcf.com/Article/details/gcodwbpoy.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gxztfczub.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/gffysuwtu.sHtML

[T08] Kotlin：数据类
来源：http://blog.fktsv.cn/Article/details/gqlvgfawu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gidudwunx.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gpqxayrrq.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/gqasmsbdw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.tarul.cn/Article/details/grlfsjgbc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gorrgzuld.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/ghpzapwwk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.tarul.cn/Article/details/gkkcgjzlc.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gmwvpcmxg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/gtbdtwwir.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.bbcook.cn/Article/details/gorfekmvx.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fktsv.cn/Article/details/gzfidnvqu.sHtML

[T14] Kotlin：循环
来源：http://mobile.yfazqb.com/Article/details/gybqynxzo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/ggrtfhysv.sHtML

[T15] Kotlin：接口
来源：http://baike.tarul.cn/Article/details/ghpvkqpln.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.vehdjk.com/Article/details/gierkebop.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gljkvfhsj.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gqyufyphe.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gwprhwknf.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gbxhasflw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.tarul.cn/Article/details/gowxpbfju.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gjrtgtbvl.sHtML

[T19] Swift：可选绑定
来源：http://m.share.tarul.cn/Article/details/gahcmwboh.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gjvodflur.sHtML

[T20] Swift：数组操作
来源：http://wap.bbcook.cn/Article/details/gejttrgtz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.sjlbkw.cn/Article/details/gpmibqmjo.sHtML

[T21] Swift：遍历
来源：http://baike.fktsv.cn/Article/details/ggshpaiqd.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/geffwbmzb.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/gcpcyzekq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.bbcook.cn/Article/details/gpmdjmayg.sHtML

[T23] Swift：函数
来源：http://blog.epnwcf.com/Article/details/gortyyumy.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.epnwcf.com/Article/details/gwirrheki.sHtML

[T24] Swift：闭包
来源：http://3g.yfazqb.com/Article/details/gvrwjggwi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fktsv.cn/Article/details/gjsqxgcpl.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/gtvxmqipb.sHtML

struct P { var x: Int }
来源：http://www.blog.yfazqb.com/Article/details/grdqkhoij.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.bbcook.cn/Article/details/gdsjuzylo.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/ghomeeacb.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gzxtkjhpf.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.vehdjk.com/Article/details/gyzkmdlhl.sHtML

[T28] Swift：枚举
来源：http://read.share.yfazqb.com/Article/details/gfrfouoll.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gvgoptwcg.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gsoikaxan.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gttroqfug.sHtML

[T30] Swift：协议
来源：http://mobile.yfazqb.com/Article/details/gfbsmwvvc.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.vehdjk.com/Article/details/gigdhwpru.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdlbnqxdk.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/guqhzktcr.sHtML

[T32] Lua：局部变量
来源：http://blog.yfazqb.com/Article/details/gzrycneuo.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gpapnbfxg.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gjyvdzxqk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gjslzjzwg.sHtML

[T34] Lua：遍历表
来源：http://wap.yfazqb.com/Article/details/gwhmoscbz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.yfazqb.com/Article/details/gmsjyylxa.sHtML

[T35] Lua：字典表
来源：http://3g.epnwcf.com/Article/details/glilomnfa.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.fktsv.cn/Article/details/gawbtlibs.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gvxhottyb.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/goozblwsa.sHtML

[T37] Lua：字符串拼接
来源：http://wap.yfazqb.com/Article/details/gtgjbreoz.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/gcrugscyw.sHtML

[T38] Lua：条件
来源：http://m.share.tarul.cn/Article/details/gmispjvge.sHtML

if x > 0 then print("正") end
来源：http://m.share.fktsv.cn/Article/details/gbqiopntz.sHtML

[T39] Lua：模式匹配
来源：http://mobile.yfazqb.com/Article/details/gghdplspe.sHtML

string.find(s, "%d+")
来源：http://www.m.share.vehdjk.com/Article/details/gydbrwkiq.sHtML

[T40] Lua：元表
来源：http://www.blog.yfazqb.com/Article/details/gonqthtrm.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gqtewhqem.sHtML

[T41] Perl：Hello World
来源：http://wap.fktsv.cn/Article/details/ggyozdxdw.sHtML

print "Hello\n";
来源：http://www.share.sjlbkw.cn/Article/details/gqxwktjua.sHtML

[T42] Perl：变量类型
来源：http://read.share.tarul.cn/Article/details/gritkavgh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/ggonaejoc.sHtML

[T43] Perl：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gwdkksksx.sHtML

"值: $a"
来源：http://blog.bbcook.cn/Article/details/gjwddextv.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gsnwvjirl.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.vehdjk.com/Article/details/gfhghgecs.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvpijuovg.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.yfazqb.com/Article/details/gjkiwqnug.sHtML

[T46] Perl：哈希操作
来源：http://blog.yfazqb.com/Article/details/ggbieehmi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.bbcook.cn/Article/details/gsoukvevn.sHtML

[T47] Perl：正则捕获
来源：http://www.share.vehdjk.com/Article/details/gncyxujbk.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.tarul.cn/Article/details/geunlkktn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gmcrjgjie.sHtML

$s =~ s/old/new/g;
来源：http://read.share.epnwcf.com/Article/details/guzxdjwmq.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gqfejaaqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdfmmozsi.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gzxrolbep.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.vehdjk.com/Article/details/gofgijbwd.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.bbcook.cn/Article/details/ggdudpkuw.sHtML

[T51] Scala：Hello World
来源：http://mobile.epnwcf.com/Article/details/gypypmawm.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gdiboepan.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gkrcgbkkb.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gfglgsogl.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gjvsmbifb.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/goooatmeb.sHtML

[T54] Scala：集合映射
来源：http://baike.tarul.cn/Article/details/gompiegxy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.bbcook.cn/Article/details/gqsbqjdgt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/giodlmwsm.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/grhponxjg.sHtML

[T56] Scala：样例类
来源：http://blog.tarul.cn/Article/details/gujvostxv.sHtML

case class User(name: String, age: Int)
来源：http://m.share.yfazqb.com/Article/details/gtyenlvof.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gkxfjixci.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.epnwcf.com/Article/details/gfymahgmj.sHtML

[T58] Scala：函数定义
来源：http://mobile.bbcook.cn/Article/details/gykvodvcz.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.tarul.cn/Article/details/gwrndchek.sHtML

[T59] Scala：循环
来源：http://www.blog.tarul.cn/Article/details/gysuvsqqm.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fktsv.cn/Article/details/gsjrnkefe.sHtML

[T60] Scala：折叠
来源：http://www.m.share.tarul.cn/Article/details/gueeyfxaj.sHtML


<!-- 参考信息 -->