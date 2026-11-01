代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gotxdiobl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gsgowhroa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/gewwtpebw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.bbcook.cn/Article/details/gaarrycqj.sHtML

df -h;  du -sh *
来源：http://m.share.sjlbkw.cn/Article/details/govcofrdm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gvzvmqkxo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.sjlbkw.cn/Article/details/gzfxwynpz.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gbqaxqzqz.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.sjlbkw.cn/Article/details/gaeibclul.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/geodfkded.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gdhhpdzpf.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gtiymuoxd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gukgehkvi.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/gorxhdghc.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gotgdaktk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gdxbvwitt.sHtML

openssl rand -hex 16
来源：http://read.share.vehdjk.com/Article/details/gncvjsusr.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gcbzvypmu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gcbsdiwqr.sHtML

[R69] 生成随机密码
来源：http://3g.bbcook.cn/Article/details/gnhigabrn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.tarul.cn/Article/details/gicjgwrrh.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/geexvozaf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.vehdjk.com/Article/details/gcpbapqoi.sHtML

[R71] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/glpyumvxy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.yfazqb.com/Article/details/gprbnavmd.sHtML

[R72] 等待端口就绪
来源：http://www.share.sjlbkw.cn/Article/details/geoeskkyo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gemykpksl.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/gskspdrxo.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fktsv.cn/Article/details/gpmzjfjna.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gzksoazem.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fktsv.cn/Article/details/gidhdrjvc.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gksfwzuxb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/giqffhvpi.sHtML

[R76] 使用临时文件
来源：http://baike.epnwcf.com/Article/details/ggtrsqqcn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gpumnnevz.sHtML

[R77] 读取用户输入
来源：http://blog.sjlbkw.cn/Article/details/gbxbbfzys.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gfmaeuckm.sHtML

[R78] 交互式菜单
来源：http://mobile.bbcook.cn/Article/details/gtutbkoix.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.bbcook.cn/Article/details/gfmhicumm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gwrkfooxh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/gkmxfimvr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gmpolcpko.sHtML

time ./run.sh
来源：http://mobile.epnwcf.com/Article/details/gqbdpjeev.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbcweeymr.sHtML

S. C / C++ 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfrvjict.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gogsueavq.sHtML

[S01] C：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gzwdqgoir.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gtestdttg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gjoqpvtmq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/guqovxclg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/gqkufluro.sHtML

[S03] C：读入整数
来源：http://mobile.vehdjk.com/Article/details/gffbmyran.sHtML

int x; scanf("%d", &x);
来源：http://wap.vehdjk.com/Article/details/gkgwzgdqs.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gklmzzcnw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gbweovfmt.sHtML

[S05] C：字符串长度
来源：http://m.share.tarul.cn/Article/details/grnkwnffh.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/grpvgqrkv.sHtML

[S06] C：字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gorgimgay.sHtML

strcmp(a, b) == 0
来源：http://3g.tarul.cn/Article/details/ggwwtjwrk.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gimhgpmxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fktsv.cn/Article/details/gxqtvxbjo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gokqgfpvv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/gsmecelrz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/gyyabejxe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.epnwcf.com/Article/details/gjitqgabn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.tarul.cn/Article/details/ggmkmivze.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.sjlbkw.cn/Article/details/gyqkcmoga.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gavyrsanm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.epnwcf.com/Article/details/gzfwinpau.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.bbcook.cn/Article/details/gbtthogfz.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gujtwvfnf.sHtML

[S12] C：写文件
来源：http://www.blog.vehdjk.com/Article/details/gyoffqvwy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/ghwbkzlaz.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/gcybgnyan.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.yfazqb.com/Article/details/getuocmwj.sHtML

[S14] C：枚举
来源：http://3g.bbcook.cn/Article/details/goqkertya.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.vehdjk.com/Article/details/gxdepykrw.sHtML

[S15] C：类型转换
来源：http://3g.vehdjk.com/Article/details/gayiljkmv.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/gzomdjtyu.sHtML

[S16] C：位操作置位
来源：http://blog.sjlbkw.cn/Article/details/gfijjlqlt.sHtML

x |= (1 << 3);
来源：http://read.share.tarul.cn/Article/details/gocqhrrvo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gbfhpeyzy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.vehdjk.com/Article/details/gcvekxhbp.sHtML

[S18] C：命令行参数
来源：http://mobile.vehdjk.com/Article/details/gfwtvtpzc.sHtML

int main(int argc, char **argv)
来源：http://baike.tarul.cn/Article/details/ghuynqrtf.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gfponkvhi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gygiegyqh.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/giqcuhtkh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/geludismf.sHtML

[S21] C：字符类别判断
来源：http://3g.fktsv.cn/Article/details/gtwuaxxjv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/guqdcwaam.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/giwwxprjp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gkuructjy.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/ggvqjhrpu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.tarul.cn/Article/details/gnqfajmxi.sHtML

[S24] C：获取本地时间
来源：http://www.share.bbcook.cn/Article/details/gpbqxhdqh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gyqsqmvma.sHtML

[S25] C：内存拷贝
来源：http://baike.fktsv.cn/Article/details/gypnhxypd.sHtML

memcpy(dst, src, n);
来源：http://www.share.bbcook.cn/Article/details/gxvvlvngn.sHtML

[S26] C：内存清零
来源：http://baike.fktsv.cn/Article/details/gheufgrfj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.vehdjk.com/Article/details/grkyqniay.sHtML

[S27] C：定义常量
来源：http://www.share.fktsv.cn/Article/details/gcyksayyt.sHtML

const double PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gkejopndm.sHtML

[S28] C：静态变量
来源：http://3g.bbcook.cn/Article/details/gqixfkmta.sHtML

static int counter = 0;
来源：http://read.share.epnwcf.com/Article/details/gtfctjcom.sHtML

[S29] C：变参函数
来源：http://www.share.yfazqb.com/Article/details/gpiceabnj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gmumwvgzs.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/gviaocvzk.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gvxmmvnqm.sHtML

#define X_H
来源：http://www.m.share.fktsv.cn/Article/details/gwwhlqoog.sHtML

#endif
来源：http://m.share.fktsv.cn/Article/details/ghypjnslq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gcjrjpovm.sHtML

#include <iostream>
来源：http://www.blog.sjlbkw.cn/Article/details/gycmptoiu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.tarul.cn/Article/details/gcpnteipv.sHtML

[S32] C++：字符串
来源：http://blog.tarul.cn/Article/details/gnfyehawf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.yfazqb.com/Article/details/grkglrrmy.sHtML

[S33] C++：vector 增删
来源：http://blog.fktsv.cn/Article/details/gucctfirc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gnfnydwdm.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/gexhkygjg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.bbcook.cn/Article/details/gghdkvulr.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gkueblvaq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gvuxbketc.sHtML

[S36] C++：unordered_map
来源：http://wap.vehdjk.com/Article/details/gxffxpunr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gvmfxrayh.sHtML

[S37] C++：set
来源：http://www.share.epnwcf.com/Article/details/gbkxjrcuz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.vehdjk.com/Article/details/gfsmsxwrb.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/getwnvhzz.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.tarul.cn/Article/details/gywhaccwi.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gsaakakcg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/gekrijkar.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/goetpukmp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.vehdjk.com/Article/details/gpmirayyy.sHtML

[S41] C++：类与构造函数
来源：http://m.share.yfazqb.com/Article/details/geauoxcyy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.tarul.cn/Article/details/gkyqrcpbw.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/ghmkbikyy.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gbvwajafv.sHtML

[S43] C++：智能指针
来源：http://www.share.bbcook.cn/Article/details/gcxygnmag.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gxnqmpcoa.sHtML

[S44] C++：引用传参
来源：http://www.share.vehdjk.com/Article/details/gputrejux.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gxwhrpmxm.sHtML

[S45] C++：lambda
来源：http://wap.yfazqb.com/Article/details/gkeoqynsb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gkealxbdu.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gutgtvdvc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gopjdmnqo.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gsrugkyqp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/giofkjpih.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/glllegaoq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.sjlbkw.cn/Article/details/gdycmkakk.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gzqztcrfy.sHtML

[S49] C++：写文件
来源：http://m.share.epnwcf.com/Article/details/ggkcvsqjf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.yfazqb.com/Article/details/gmllkzyon.sHtML

[S50] C++：格式化数字
来源：http://baike.bbcook.cn/Article/details/ghnomkjph.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.tarul.cn/Article/details/gdbphfqqc.sHtML

[S51] C++：显式类型转换
来源：http://www.share.yfazqb.com/Article/details/gqxianbxf.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gvtxgocyo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.tarul.cn/Article/details/godieucph.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gcheywomx.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fktsv.cn/Article/details/gverkkrux.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gpvfnewlz.sHtML

[S54] C++：异常处理
来源：http://wap.epnwcf.com/Article/details/gguxfyycq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.vehdjk.com/Article/details/gdmscrzou.sHtML

[S55] C++：结构化绑定
来源：http://read.share.bbcook.cn/Article/details/gsbcmylvf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.bbcook.cn/Article/details/gxpjwevvu.sHtML

[S56] C++：optional
来源：http://www.share.bbcook.cn/Article/details/gjvpnltpw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.vehdjk.com/Article/details/gwtaredjq.sHtML

[S57] C++：编译期常量
来源：http://baike.vehdjk.com/Article/details/gcqmsyppm.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gybjkvlzi.sHtML

[S58] C++：命名空间
来源：http://mobile.fktsv.cn/Article/details/gxfpvavvg.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.bbcook.cn/Article/details/gyzxqzewz.sHtML

[S59] C++：静态断言
来源：http://3g.bbcook.cn/Article/details/gjcqopedn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.bbcook.cn/Article/details/gxedrgset.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fktsv.cn/Article/details/ghxprfqwk.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/gxlladzpm.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/ghycoavsi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.sjlbkw.cn/Article/details/gdnylfkwg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gimvxwmgq.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/gxxpxlirf.sHtML

println("Hello")
来源：http://m.share.fktsv.cn/Article/details/gfyympnvc.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gcramjeka.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gmkiccvfx.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.vehdjk.com/Article/details/ghjhbunok.sHtML

"值: $b"
来源：http://3g.bbcook.cn/Article/details/ggwijnhuh.sHtML

[T04] Kotlin：空安全
来源：http://baike.bbcook.cn/Article/details/gnjbfrxgb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.tarul.cn/Article/details/gjlgfrmdo.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gsshqsxqx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/godwfyhvs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.sjlbkw.cn/Article/details/giqgfkylt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.yfazqb.com/Article/details/grztqcohl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gkrjgudyg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/gsczkmzfc.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.sjlbkw.cn/Article/details/gltrxegak.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.vehdjk.com/Article/details/gbofltajo.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.epnwcf.com/Article/details/ggzapgohj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.vehdjk.com/Article/details/gknnnvquo.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.yfazqb.com/Article/details/gyhygcsjo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/gijjjiieb.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gubimdefa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.yfazqb.com/Article/details/geycvsjcb.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.tarul.cn/Article/details/gmsxjizfy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/glumqqujn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.sjlbkw.cn/Article/details/ghmjoccub.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gotafqtss.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/giyufyeyr.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fktsv.cn/Article/details/goodladsa.sHtML

[T15] Kotlin：接口
来源：http://baike.epnwcf.com/Article/details/ggeynnjyk.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/ganrtobut.sHtML

[T16] Swift：Hello World
来源：http://baike.tarul.cn/Article/details/gxxpvswds.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/guuftivoz.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/ggxykzlng.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gnnhmenwx.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gwdksjtlt.sHtML

"值: \(b)"
来源：http://blog.fktsv.cn/Article/details/gddezxafs.sHtML

[T19] Swift：可选绑定
来源：http://blog.epnwcf.com/Article/details/gwzmoapmj.sHtML

if let n = opt { print(n) }
来源：http://blog.epnwcf.com/Article/details/gjrbkuexx.sHtML

[T20] Swift：数组操作
来源：http://www.share.fktsv.cn/Article/details/gjosdnmip.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/gaizexind.sHtML

[T21] Swift：遍历
来源：http://read.share.tarul.cn/Article/details/godaidwib.sHtML

for x in a { print(x) }
来源：http://3g.epnwcf.com/Article/details/geesmserg.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gaehchogn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.vehdjk.com/Article/details/grfkequcx.sHtML

[T23] Swift：函数
来源：http://mobile.epnwcf.com/Article/details/gnrkhvuqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gxiiwbtlq.sHtML

[T24] Swift：闭包
来源：http://m.share.tarul.cn/Article/details/gxhrwtmqy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.bbcook.cn/Article/details/gpryugbuz.sHtML

[T25] Swift：结构体
来源：http://m.share.tarul.cn/Article/details/gtlabrytc.sHtML

struct P { var x: Int }
来源：http://blog.vehdjk.com/Article/details/gmhmdazvr.sHtML

[T26] Swift：类与重写
来源：http://baike.yfazqb.com/Article/details/gdckekjcj.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gfagbedhc.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/gywdwjwts.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gwttroezd.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/gmcyafisx.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gqmtrbufp.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/ghxbyzwql.sHtML

guard let x = opt else { return }
来源：http://baike.vehdjk.com/Article/details/gxudswfzk.sHtML

[T30] Swift：协议
来源：http://baike.fktsv.cn/Article/details/gbnlgkqgu.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/gsfpwjgms.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gvflslmon.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gzhjozkdi.sHtML

[T32] Lua：局部变量
来源：http://wap.epnwcf.com/Article/details/govpcuilu.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/gsxzdinkp.sHtML

[T33] Lua：表（数组）
来源：http://read.share.tarul.cn/Article/details/gflhsamgh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.bbcook.cn/Article/details/gfxljowgr.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.bbcook.cn/Article/details/gvybfrxry.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.yfazqb.com/Article/details/gmoffexod.sHtML

[T35] Lua：字典表
来源：http://www.share.sjlbkw.cn/Article/details/glyzusdyu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gqdpzzxos.sHtML

[T36] Lua：函数
来源：http://mobile.sjlbkw.cn/Article/details/gybfdkxci.sHtML

function add(a, b) return a + b end
来源：http://www.share.sjlbkw.cn/Article/details/gnrbfylbh.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gqxgrxsec.sHtML

"a" .. "b"
来源：http://www.share.yfazqb.com/Article/details/gexgvsbqp.sHtML

[T38] Lua：条件
来源：http://baike.bbcook.cn/Article/details/gtpbmcauw.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gdidylnpo.sHtML

[T39] Lua：模式匹配
来源：http://blog.vehdjk.com/Article/details/gooxzmdeq.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gsrvgchzd.sHtML

[T40] Lua：元表
来源：http://baike.tarul.cn/Article/details/gwkhyfjgf.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/ggsypddcz.sHtML

[T41] Perl：Hello World
来源：http://3g.fktsv.cn/Article/details/gjcgadayx.sHtML

print "Hello\n";
来源：http://m.share.vehdjk.com/Article/details/gcqgjobjv.sHtML

[T42] Perl：变量类型
来源：http://blog.tarul.cn/Article/details/gkkbfobwx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.tarul.cn/Article/details/guiutrcbi.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gsaovtfzk.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gevevvdyk.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gjjvspcdn.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gbxigimwy.sHtML

[T45] Perl：数组遍历
来源：http://m.share.epnwcf.com/Article/details/gnbfuqbvi.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.vehdjk.com/Article/details/gcwqwgnga.sHtML

[T46] Perl：哈希操作
来源：http://baike.epnwcf.com/Article/details/gtvdsleum.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fktsv.cn/Article/details/ghfjycsdz.sHtML

[T47] Perl：正则捕获
来源：http://mobile.tarul.cn/Article/details/gssgsxgat.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/guehgladw.sHtML

[T48] Perl：正则替换
来源：http://blog.fktsv.cn/Article/details/glkblcfjn.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gbqruyuga.sHtML

[T49] Perl：函数
来源：http://read.share.bbcook.cn/Article/details/gqnyoaehl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gnxhedtji.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gghmksvlv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/ggkqzptuu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.vehdjk.com/Article/details/gitgsetyl.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gvxepdqqh.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gkrilwnxy.sHtML

[T52] Scala：变量
来源：http://www.share.bbcook.cn/Article/details/gbbjvctqc.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.bbcook.cn/Article/details/gwxpkbyxz.sHtML

[T53] Scala：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gbolavrjz.sHtML

s"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gixawbpax.sHtML

[T54] Scala：集合映射
来源：http://wap.yfazqb.com/Article/details/gmnkrjkng.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gnnyfggxy.sHtML

[T55] Scala：集合过滤
来源：http://mobile.vehdjk.com/Article/details/gxtijafjv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/gwrygmjmd.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gncuasjhz.sHtML

case class User(name: String, age: Int)
来源：http://www.share.tarul.cn/Article/details/gzstssukk.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.vehdjk.com/Article/details/ggefkkjie.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/gjpjgkwch.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gjegdtmuk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.tarul.cn/Article/details/ghzfmsvfn.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gwugbaixc.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.yfazqb.com/Article/details/gfubqjbvt.sHtML

[T60] Scala：折叠
来源：http://mobile.tarul.cn/Article/details/gzuhfcxjy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.bbcook.cn/Article/details/gcfpppdjj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdvgvfraf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gymikruvv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gstaggwfd.sHtML


<!-- 参考信息 -->