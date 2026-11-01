代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.yfazqb.com/Article/details/gtvlufama.sHtML

[R58] 下载文件
来源：http://mobile.bbcook.cn/Article/details/gvbhrgemq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/gmglgvaee.sHtML

[R59] 发 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gjnfqrkwd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.vehdjk.com/Article/details/gyugzrxeq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/ggzlnjyaz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gmrerzfyf.sHtML

[R61] 磁盘占用
来源：http://www.blog.vehdjk.com/Article/details/gsgfnpval.sHtML

df -h;  du -sh *
来源：http://www.share.epnwcf.com/Article/details/gumvjracw.sHtML

[R62] 找最占空间的文件
来源：http://baike.sjlbkw.cn/Article/details/gxrndhozd.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.yfazqb.com/Article/details/gdcegcjcd.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gnzordguf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.bbcook.cn/Article/details/gosaiqgcc.sHtML

[R64] 结束进程
来源：http://www.share.sjlbkw.cn/Article/details/ggexlfkog.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.vehdjk.com/Article/details/ghzxpwgkk.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gtmwdvsvk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gmnutagjr.sHtML

[R66] 定时任务
来源：http://mobile.vehdjk.com/Article/details/gbywdkcuq.sHtML

crontab -e;  crontab -l
来源：http://wap.bbcook.cn/Article/details/gucngjsji.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fktsv.cn/Article/details/gjzqumvgq.sHtML

openssl rand -hex 16
来源：http://wap.bbcook.cn/Article/details/gzrmovlop.sHtML

[R68] 计算文件校验值
来源：http://mobile.vehdjk.com/Article/details/gdqhvynwb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/gdmdnwfro.sHtML

[R69] 生成随机密码
来源：http://wap.epnwcf.com/Article/details/gnxcaktjg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/gqplgopff.sHtML

[R70] 时间戳与互转
来源：http://wap.fktsv.cn/Article/details/gmaqfdkhf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gbmtomfqn.sHtML

[R71] 日期格式化
来源：http://wap.tarul.cn/Article/details/ggabphvvv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fktsv.cn/Article/details/gttjrcsre.sHtML

[R72] 等待端口就绪
来源：http://wap.vehdjk.com/Article/details/gwlejcjcu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gndkgfxch.sHtML

[R73] 分割大日志
来源：http://baike.yfazqb.com/Article/details/ggfviievg.sHtML

split -l 1000 big.log part_
来源：http://read.share.tarul.cn/Article/details/gombyphzy.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gobdwygfa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.sjlbkw.cn/Article/details/ggisbbggg.sHtML

[R75] 导出环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gqyjwapoc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gsitzsmru.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/gojbnzraz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.yfazqb.com/Article/details/gflhlpsnu.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/glmwrnvkm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.epnwcf.com/Article/details/gxofekgab.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gvckpjddv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.sjlbkw.cn/Article/details/gxfakqqjv.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gytznwavk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.tarul.cn/Article/details/gefsmjhhb.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.tarul.cn/Article/details/gyocsabhx.sHtML

time ./run.sh
来源：http://m.share.tarul.cn/Article/details/gdrzksmqm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gniyyztje.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gyhweblmc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/godsqwklm.sHtML

[S01] C：Hello World
来源：http://mobile.vehdjk.com/Article/details/gegxpiamo.sHtML

#include <stdio.h>
来源：http://baike.epnwcf.com/Article/details/ghswajjvb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fktsv.cn/Article/details/gojumeiax.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gzaijdpsl.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gwboprcrw.sHtML

[S03] C：读入整数
来源：http://m.share.epnwcf.com/Article/details/gjvmurtdb.sHtML

int x; scanf("%d", &x);
来源：http://www.share.vehdjk.com/Article/details/ghoybdbrw.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/ggdffezoo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.yfazqb.com/Article/details/goorouppf.sHtML

[S05] C：字符串长度
来源：http://3g.fktsv.cn/Article/details/gnegcxifq.sHtML

strlen(s)
来源：http://www.m.share.fktsv.cn/Article/details/gcrqgefdm.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gihiqpggq.sHtML

strcmp(a, b) == 0
来源：http://www.share.epnwcf.com/Article/details/gmepojmcx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.epnwcf.com/Article/details/gnmklpkwh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/grjsrvtak.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gbojqhwil.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gtprjkuqr.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gqnkonetl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.sjlbkw.cn/Article/details/gfrcadhdi.sHtML

[S10] C：指针与解引用
来源：http://www.blog.vehdjk.com/Article/details/glagrvtjr.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gwqpoymrw.sHtML

[S11] C：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gzdrtucpu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.yfazqb.com/Article/details/grjquambk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.vehdjk.com/Article/details/ggtgfoguv.sHtML

fclose(f);
来源：http://wap.fktsv.cn/Article/details/gaysxodep.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/geoljnikg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.bbcook.cn/Article/details/goanqlchc.sHtML

[S13] C：宏定义
来源：http://wap.bbcook.cn/Article/details/gvdrhohbu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.bbcook.cn/Article/details/gdtzgpzms.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gcbdupxkq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/greebadyz.sHtML

[S15] C：类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gtmpbzfjg.sHtML

(double) a / b
来源：http://baike.epnwcf.com/Article/details/gbarxdedz.sHtML

[S16] C：位操作置位
来源：http://m.share.bbcook.cn/Article/details/gscgwovrg.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gqozeujyi.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.tarul.cn/Article/details/ggtitgdgc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fktsv.cn/Article/details/glvpmkpqe.sHtML

[S18] C：命令行参数
来源：http://baike.tarul.cn/Article/details/gzdpkeuui.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gbopwecez.sHtML

[S19] C：快速排序
来源：http://www.share.sjlbkw.cn/Article/details/gibmhctfh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gpuxuqgcz.sHtML

[S20] C：二分查找
来源：http://www.blog.epnwcf.com/Article/details/gtcxvzyel.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gtrunchuq.sHtML

[S21] C：字符类别判断
来源：http://baike.vehdjk.com/Article/details/gjlxuzpxf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/gfcyrodxd.sHtML

[S22] C：字符串转数字
来源：http://www.share.tarul.cn/Article/details/gbicsisfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.sjlbkw.cn/Article/details/gmtnjktuc.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/ggonfppwc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.yfazqb.com/Article/details/gcgweyfov.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gnpkppafz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.epnwcf.com/Article/details/ghczbxbdw.sHtML

[S25] C：内存拷贝
来源：http://m.share.epnwcf.com/Article/details/gcpgazkor.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gssrftltl.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gqurtwpqu.sHtML

memset(a, 0, sizeof a);
来源：http://baike.yfazqb.com/Article/details/gbklucxhc.sHtML

[S27] C：定义常量
来源：http://wap.tarul.cn/Article/details/glctnpakg.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/glbwbxtsx.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gjtimjzzy.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/gseextcnk.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gsrarrmgn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.yfazqb.com/Article/details/gigjmndle.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gdlowclpr.sHtML

#ifndef X_H
来源：http://m.share.bbcook.cn/Article/details/gksylgxfc.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/guiajkmze.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gjwwouphi.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gomwscdhv.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gyjxnsamn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fktsv.cn/Article/details/gfnqrindh.sHtML

[S32] C++：字符串
来源：http://3g.tarul.cn/Article/details/gcbyabftf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.bbcook.cn/Article/details/gpcfulgzy.sHtML

[S33] C++：vector 增删
来源：http://baike.sjlbkw.cn/Article/details/gtqluoeih.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.yfazqb.com/Article/details/giwulitap.sHtML

[S34] C++：遍历 vector
来源：http://m.share.sjlbkw.cn/Article/details/gahnpnqpn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fktsv.cn/Article/details/gicsznnbs.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gadeydmal.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gdmdfesmh.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gwwyreagl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/goiytkofz.sHtML

[S37] C++：set
来源：http://blog.epnwcf.com/Article/details/gmpwmcuru.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/gzgrudkki.sHtML

[S38] C++：排序
来源：http://wap.fktsv.cn/Article/details/gqwhfdigu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gxpyaocrs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gagjcqfdi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.epnwcf.com/Article/details/glkcilalt.sHtML

[S40] C++：查找元素
来源：http://mobile.epnwcf.com/Article/details/gkfyopbiy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.bbcook.cn/Article/details/gvxmxgfbo.sHtML

[S41] C++：类与构造函数
来源：http://blog.epnwcf.com/Article/details/gklidyqxy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gpwhysnvh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/gnjvtxqsm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gjdwjfcou.sHtML

[S43] C++：智能指针
来源：http://blog.yfazqb.com/Article/details/goeoxtebr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gejrelezf.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/grgzawidq.sHtML

void inc(int &x) { ++x; }
来源：http://wap.vehdjk.com/Article/details/gccmicbml.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gerxhjglp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gkfzefbkj.sHtML

[S46] C++：函数模板
来源：http://m.share.bbcook.cn/Article/details/gvueojwij.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gnjehxoyg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.bbcook.cn/Article/details/gogwwwbuj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.yfazqb.com/Article/details/gobalpirv.sHtML

[S48] C++：逐行读文件
来源：http://baike.yfazqb.com/Article/details/gjprmyvwg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.vehdjk.com/Article/details/gkirnfeyp.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.epnwcf.com/Article/details/glqxkadrw.sHtML

[S49] C++：写文件
来源：http://baike.yfazqb.com/Article/details/grximyogy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fktsv.cn/Article/details/gchwurtyn.sHtML

[S50] C++：格式化数字
来源：http://read.share.tarul.cn/Article/details/gdkjypyzf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.tarul.cn/Article/details/grpduzdlq.sHtML

[S51] C++：显式类型转换
来源：http://3g.bbcook.cn/Article/details/gszeabzky.sHtML

static_cast<double>(a) / b
来源：http://read.share.yfazqb.com/Article/details/gtbzzdnzi.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.bbcook.cn/Article/details/gsfwxmthp.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.sjlbkw.cn/Article/details/gzxtnaxyg.sHtML

[S53] C++：移动语义
来源：http://blog.sjlbkw.cn/Article/details/grbsfrtgo.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gtccapnte.sHtML

[S54] C++：异常处理
来源：http://baike.sjlbkw.cn/Article/details/gxopwmhde.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.vehdjk.com/Article/details/govxfglbl.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.sjlbkw.cn/Article/details/gimojrdol.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gvtjoykzp.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gnkahinle.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fktsv.cn/Article/details/gtsaohqct.sHtML

[S57] C++：编译期常量
来源：http://3g.sjlbkw.cn/Article/details/ggihyokmh.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/guvqxekux.sHtML

[S58] C++：命名空间
来源：http://mobile.yfazqb.com/Article/details/gamvelpez.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gfwslxuks.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gknezwtcs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/gpplewgfb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.tarul.cn/Article/details/gdxaexalf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gpiakxbzg.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gvyisvdch.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gggbkiseb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcjsirchx.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ghizkmoyk.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gltkfljhh.sHtML

[T02] Kotlin：变量
来源：http://blog.tarul.cn/Article/details/gbvqqghuj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fktsv.cn/Article/details/gqacwfvus.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.yfazqb.com/Article/details/gmivcundq.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gspxrfpdg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gnqvcdwxw.sHtML

val n: String? = null;  n?.length
来源：http://www.share.vehdjk.com/Article/details/gdwlinxpd.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gymyyqdvs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fktsv.cn/Article/details/gqbgmvvlc.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fktsv.cn/Article/details/gcahzljkq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gkjgxqvzw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.bbcook.cn/Article/details/gxxukaeum.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.sjlbkw.cn/Article/details/gzzbhmlbf.sHtML

[T08] Kotlin：数据类
来源：http://wap.vehdjk.com/Article/details/glakhhxml.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gyisczcqe.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gluibxsqj.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/gzmxmgcrt.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fktsv.cn/Article/details/gkjjmmxon.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gdnebobmo.sHtML

[T11] Kotlin：协程
来源：http://mobile.sjlbkw.cn/Article/details/gkwypdduf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.yfazqb.com/Article/details/gnoabwsjh.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.yfazqb.com/Article/details/gaohnhcol.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fktsv.cn/Article/details/glhmcotse.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gjuharusb.sHtML

val m = mapOf("a" to 1)
来源：http://blog.vehdjk.com/Article/details/geqfrrirk.sHtML

[T14] Kotlin：循环
来源：http://3g.epnwcf.com/Article/details/gtfbhptfe.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/giqvpqtok.sHtML

[T15] Kotlin：接口
来源：http://m.share.sjlbkw.cn/Article/details/gdmlbpxxa.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/ggulxvxhl.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/geknareiw.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gkifofung.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.vehdjk.com/Article/details/gagxayccp.sHtML

var a = 1;  let b = 2
来源：http://wap.bbcook.cn/Article/details/gvuwfvndy.sHtML

[T18] Swift：字符串插值
来源：http://read.share.tarul.cn/Article/details/gyctttwns.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/glqysqdnc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gdofgdwic.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gnzbtmtpu.sHtML

[T20] Swift：数组操作
来源：http://read.share.epnwcf.com/Article/details/gqmqaezgj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.bbcook.cn/Article/details/gdgsmpakr.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gzykipgqz.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gnynvhxxv.sHtML

[T22] Swift：字典
来源：http://www.share.yfazqb.com/Article/details/gyrlwahkr.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.fktsv.cn/Article/details/gwheextgw.sHtML

[T23] Swift：函数
来源：http://read.share.epnwcf.com/Article/details/glefjfyfb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.yfazqb.com/Article/details/gyowzmrrm.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/ggerbiloc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gwuhndjni.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gezdkiiwb.sHtML

struct P { var x: Int }
来源：http://read.share.bbcook.cn/Article/details/gnegnqrhv.sHtML

[T26] Swift：类与重写
来源：http://m.share.bbcook.cn/Article/details/gdrmfgenj.sHtML

class A: Base { override func f() {} }
来源：http://www.share.sjlbkw.cn/Article/details/ghhtidyei.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gqslfosam.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.vehdjk.com/Article/details/gqfwhgagc.sHtML

[T28] Swift：枚举
来源：http://mobile.bbcook.cn/Article/details/ghzsndcga.sHtML

enum Color { case red, green }
来源：http://www.m.share.bbcook.cn/Article/details/gmxhozdrv.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.sjlbkw.cn/Article/details/gcfvskglu.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/gloytjeve.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gnvmvukea.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.bbcook.cn/Article/details/gjnnxvzbq.sHtML

[T31] Lua：Hello World
来源：http://baike.epnwcf.com/Article/details/giqtszggm.sHtML

print("Hello")
来源：http://www.share.tarul.cn/Article/details/gelocufbz.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrnfwaeo.sHtML

local a = 1
来源：http://baike.bbcook.cn/Article/details/gwnwseggi.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/glbsnrcnp.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gjsnmkssr.sHtML

[T34] Lua：遍历表
来源：http://wap.vehdjk.com/Article/details/gfliuxydm.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/gpdljgsog.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gsqmznaeg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.tarul.cn/Article/details/gqrvsfpxo.sHtML

[T36] Lua：函数
来源：http://3g.fktsv.cn/Article/details/gscgiasjj.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gfivbzxmj.sHtML

[T37] Lua：字符串拼接
来源：http://3g.tarul.cn/Article/details/gmekzfuoj.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gdwtmwfck.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gtottsmgk.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/gphkswbyc.sHtML

[T39] Lua：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gahodizjx.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gyhukaonw.sHtML

[T40] Lua：元表
来源：http://www.blog.epnwcf.com/Article/details/gcyuofkui.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gqdwovfea.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gasyhzbyz.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gkgyopkgl.sHtML

[T42] Perl：变量类型
来源：http://read.share.fktsv.cn/Article/details/gbkxrfexd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gawhmovhx.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/ggewtypte.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gpunvhypj.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gfygpmgrx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.vehdjk.com/Article/details/grccehwut.sHtML

[T45] Perl：数组遍历
来源：http://www.share.yfazqb.com/Article/details/gbymmxmhn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/gtavlebbj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.tarul.cn/Article/details/gjkjvdhom.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmrhzfdd.sHtML

[T47] Perl：正则捕获
来源：http://blog.tarul.cn/Article/details/gstmninol.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.yfazqb.com/Article/details/gesfmuvuo.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gxiwpyykq.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gssjgnbcj.sHtML

[T49] Perl：函数
来源：http://3g.sjlbkw.cn/Article/details/gnqshkhva.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/glqeqytry.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fktsv.cn/Article/details/glzcryyft.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.tarul.cn/Article/details/gshbvcshl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtesgguz.sHtML

[T51] Scala：Hello World
来源：http://read.share.tarul.cn/Article/details/gdyixreui.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gwnmjyvkv.sHtML

[T52] Scala：变量
来源：http://mobile.vehdjk.com/Article/details/gbbsdldov.sHtML

val a = 1;  var b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gjfqhxetw.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/gsaaajnkt.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gniudkffm.sHtML

[T54] Scala：集合映射
来源：http://blog.bbcook.cn/Article/details/gtzgriduj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gvgtovowl.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gqnsifmcw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gespxfrlc.sHtML

[T56] Scala：样例类
来源：http://www.m.share.vehdjk.com/Article/details/gcvyziemt.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gdlxifiyt.sHtML

[T57] Scala：模式匹配
来源：http://baike.epnwcf.com/Article/details/goxfmbyxf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.bbcook.cn/Article/details/gjncmoywl.sHtML

[T58] Scala：函数定义
来源：http://m.share.sjlbkw.cn/Article/details/grdklygko.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gewcfifnq.sHtML

[T59] Scala：循环
来源：http://blog.bbcook.cn/Article/details/gjxhhhoyi.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gcevvwddy.sHtML

[T60] Scala：折叠
来源：http://baike.sjlbkw.cn/Article/details/gacjkszht.sHtML


<!-- 参考信息 -->