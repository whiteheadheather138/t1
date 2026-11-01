代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/ggbvyhaim.sHtML

[R56] 远程拷贝
来源：http://mobile.epnwcf.com/Article/details/gvbeniytw.sHtML

scp file user@host:/path/
来源：http://www.blog.fktsv.cn/Article/details/gxifikotj.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gcmndzlgp.sHtML

ssh user@host 'uptime'
来源：http://m.share.fktsv.cn/Article/details/guwsosxtk.sHtML

[R58] 下载文件
来源：http://m.share.bbcook.cn/Article/details/gcpewzdeo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.sjlbkw.cn/Article/details/gzqbzfcqg.sHtML

[R59] 发 POST JSON
来源：http://read.share.yfazqb.com/Article/details/glbhazcus.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.epnwcf.com/Article/details/gifjdjbsv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gfbiskzev.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.yfazqb.com/Article/details/gjjobmzxr.sHtML

[R61] 磁盘占用
来源：http://wap.fktsv.cn/Article/details/gdonsgoqz.sHtML

df -h;  du -sh *
来源：http://m.share.epnwcf.com/Article/details/gupbyblcf.sHtML

[R62] 找最占空间的文件
来源：http://wap.vehdjk.com/Article/details/gstwlzutj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.bbcook.cn/Article/details/grsirnace.sHtML

[R63] 内存与进程
来源：http://m.share.epnwcf.com/Article/details/gkfaumovm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gablrgmvi.sHtML

[R64] 结束进程
来源：http://m.share.tarul.cn/Article/details/gktobjfen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gtnipodeb.sHtML

[R65] 查看端口占用
来源：http://wap.vehdjk.com/Article/details/gnlckncef.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.vehdjk.com/Article/details/gplrfeqqk.sHtML

[R66] 定时任务
来源：http://www.m.share.bbcook.cn/Article/details/gnjudkbjq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.tarul.cn/Article/details/gpkwpxwxk.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.vehdjk.com/Article/details/gekfcbtmq.sHtML

openssl rand -hex 16
来源：http://baike.yfazqb.com/Article/details/geekrbbtk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gnhnmnxpq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.sjlbkw.cn/Article/details/gncjhvsdz.sHtML

[R69] 生成随机密码
来源：http://mobile.tarul.cn/Article/details/gdeuvdstu.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.bbcook.cn/Article/details/gqccnmyib.sHtML

[R70] 时间戳与互转
来源：http://www.blog.yfazqb.com/Article/details/gsuzlwlxl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gpfjrnuuq.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/golfexvwp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gfgyjduuw.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gmeauttvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gjiaclqou.sHtML

[R73] 分割大日志
来源：http://mobile.vehdjk.com/Article/details/glhanxydk.sHtML

split -l 1000 big.log part_
来源：http://m.share.vehdjk.com/Article/details/gqkeprzkr.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gjsgkycjc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gpxmrxwxx.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/ggfwufcaz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.yfazqb.com/Article/details/gbfyknjot.sHtML

[R76] 使用临时文件
来源：http://www.m.share.yfazqb.com/Article/details/gawraecwd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gafavpmda.sHtML

[R77] 读取用户输入
来源：http://blog.yfazqb.com/Article/details/gnvrlstpi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fktsv.cn/Article/details/gbpzkiulr.sHtML

[R78] 交互式菜单
来源：http://3g.yfazqb.com/Article/details/gjlvqkxkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.tarul.cn/Article/details/ghyuwjmwf.sHtML

[R79] 解析命令行选项
来源：http://www.share.sjlbkw.cn/Article/details/gjeblelvn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fktsv.cn/Article/details/ghybszgil.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.sjlbkw.cn/Article/details/gsfgvdqtq.sHtML

time ./run.sh
来源：http://read.share.vehdjk.com/Article/details/gkxqskheh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gzoexwshe.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gakwrmdao.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gufgnmmtl.sHtML

[S01] C：Hello World
来源：http://mobile.fktsv.cn/Article/details/gwxemhads.sHtML

#include <stdio.h>
来源：http://www.blog.vehdjk.com/Article/details/gaolnhhal.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/glgixwtzk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gcirjaoir.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.epnwcf.com/Article/details/ghovfqder.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gcbnefdkb.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gmdbdmqjr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrqizifw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gcyiuqgvc.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gdruldjln.sHtML

strlen(s)
来源：http://www.share.epnwcf.com/Article/details/gejpheyai.sHtML

[S06] C：字符串比较
来源：http://3g.sjlbkw.cn/Article/details/gerrxpaqy.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/grbnfmzeg.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gxqbmcfsd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gpaybrilw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.sjlbkw.cn/Article/details/ghdpwdnhx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.bbcook.cn/Article/details/gvvyyirtg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/guhvubcrt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.sjlbkw.cn/Article/details/glrbtnrqx.sHtML

[S10] C：指针与解引用
来源：http://www.share.sjlbkw.cn/Article/details/gdkeegpxv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/ginoogtqb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdkfkxzu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/gtujgeijg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.bbcook.cn/Article/details/gkeyepbuo.sHtML

fclose(f);
来源：http://baike.yfazqb.com/Article/details/guwardkbi.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/ghdwocoyo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gxrktiyrl.sHtML

[S13] C：宏定义
来源：http://mobile.epnwcf.com/Article/details/gfprcfroc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gljbsyuef.sHtML

[S14] C：枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gwysevbib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gtgttsmnd.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gdkirujzc.sHtML

(double) a / b
来源：http://www.blog.sjlbkw.cn/Article/details/gpcbuiskg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fktsv.cn/Article/details/gcmoxphla.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/glceoqpuj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/ghjvfnjpu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gjqabdmev.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gqmzahrtc.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gostemyal.sHtML

[S19] C：快速排序
来源：http://www.m.share.tarul.cn/Article/details/gbzomxsee.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gjrztchcy.sHtML

[S20] C：二分查找
来源：http://www.share.bbcook.cn/Article/details/gwcloblox.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.epnwcf.com/Article/details/gdkrchyva.sHtML

[S21] C：字符类别判断
来源：http://blog.fktsv.cn/Article/details/gqpieawrd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.bbcook.cn/Article/details/gfaxrmifw.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gzptwmxpe.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gtgekcckt.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gchujytai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fktsv.cn/Article/details/gjgnlddjl.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/glswqbzlb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gtmdfrxgw.sHtML

[S25] C：内存拷贝
来源：http://3g.epnwcf.com/Article/details/gxylimsbu.sHtML

memcpy(dst, src, n);
来源：http://mobile.vehdjk.com/Article/details/gnsfpavwl.sHtML

[S26] C：内存清零
来源：http://blog.tarul.cn/Article/details/gfrtcdcot.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/ghvmezgxd.sHtML

[S27] C：定义常量
来源：http://wap.sjlbkw.cn/Article/details/gjpmsysmr.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gaijbcnks.sHtML

[S28] C：静态变量
来源：http://www.m.share.vehdjk.com/Article/details/gxjkklgsh.sHtML

static int counter = 0;
来源：http://wap.sjlbkw.cn/Article/details/gmxhtwisj.sHtML

[S29] C：变参函数
来源：http://m.share.sjlbkw.cn/Article/details/gfojbhlgm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.sjlbkw.cn/Article/details/gwzadmjkh.sHtML

[S30] C：头文件保护
来源：http://read.share.bbcook.cn/Article/details/gmiyhsteq.sHtML

#ifndef X_H
来源：http://www.blog.vehdjk.com/Article/details/gmtekfvjv.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/gxnjwqmcb.sHtML

#endif
来源：http://wap.epnwcf.com/Article/details/gjrtenhtl.sHtML

[S31] C++：Hello World
来源：http://mobile.tarul.cn/Article/details/gxlwadkxs.sHtML

#include <iostream>
来源：http://m.share.yfazqb.com/Article/details/gbdocepub.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.yfazqb.com/Article/details/gtjpyoden.sHtML

[S32] C++：字符串
来源：http://m.share.sjlbkw.cn/Article/details/gjystdrwc.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/gqegxdkfl.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gcbkvmhwn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fktsv.cn/Article/details/gpaygufqz.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.epnwcf.com/Article/details/gbjhsicsk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.yfazqb.com/Article/details/glhqsdkfe.sHtML

[S35] C++：map
来源：http://m.share.yfazqb.com/Article/details/gotdartxn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.epnwcf.com/Article/details/gzuacgwfe.sHtML

[S36] C++：unordered_map
来源：http://blog.epnwcf.com/Article/details/gxmpwzovh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.bbcook.cn/Article/details/gndaltikb.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gnfjvzmwp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.epnwcf.com/Article/details/gascdqxxk.sHtML

[S38] C++：排序
来源：http://3g.vehdjk.com/Article/details/ghlmdgurc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gdxnrlzqt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gvdrhofpo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/gfmbvbzcf.sHtML

[S40] C++：查找元素
来源：http://blog.epnwcf.com/Article/details/gjxdeeixq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/groosryln.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gydahmouu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/gbkezsfpk.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.epnwcf.com/Article/details/ggiakqxvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.tarul.cn/Article/details/gchzueiqo.sHtML

[S43] C++：智能指针
来源：http://m.share.sjlbkw.cn/Article/details/givzuwgab.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/ggmklticx.sHtML

[S44] C++：引用传参
来源：http://mobile.epnwcf.com/Article/details/gpxujanvq.sHtML

void inc(int &x) { ++x; }
来源：http://3g.bbcook.cn/Article/details/gawocljcj.sHtML

[S45] C++：lambda
来源：http://3g.vehdjk.com/Article/details/gqlmiihec.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.sjlbkw.cn/Article/details/gufsmfbno.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/ggkozxkxq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.epnwcf.com/Article/details/gfwerflsx.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/ghnwcxqwz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.epnwcf.com/Article/details/gbqatjoqh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gjeayhmov.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.vehdjk.com/Article/details/ghvzdsnjc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gdxwcpscy.sHtML

[S49] C++：写文件
来源：http://3g.sjlbkw.cn/Article/details/glomrvdrd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.yfazqb.com/Article/details/gujrmqisa.sHtML

[S50] C++：格式化数字
来源：http://mobile.tarul.cn/Article/details/gaeyozwrl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjjakvwd.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gnislveau.sHtML

static_cast<double>(a) / b
来源：http://3g.sjlbkw.cn/Article/details/gtjoltzmc.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fktsv.cn/Article/details/gjbsmeuer.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.yfazqb.com/Article/details/gpqqksmaj.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gqriwdaty.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.tarul.cn/Article/details/gkqqjczhn.sHtML

[S54] C++：异常处理
来源：http://wap.vehdjk.com/Article/details/gbohbsgfp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/ghifzrmol.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gybqklhkh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/guwpohxpz.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/ghhuiucwn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.tarul.cn/Article/details/ghjkonkse.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/ggdbgfwss.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gkdirhlpw.sHtML

[S58] C++：命名空间
来源：http://baike.vehdjk.com/Article/details/gknvtjdsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.tarul.cn/Article/details/gnsmgesbs.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/glmzvcbmn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.epnwcf.com/Article/details/goxuvedzd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gcbpssumq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.epnwcf.com/Article/details/ghwtpodrc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvbxbwltl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gwhglryjv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glqexgjpa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.yfazqb.com/Article/details/gsjlezgxz.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gxshanpph.sHtML

[T02] Kotlin：变量
来源：http://baike.epnwcf.com/Article/details/ghevunfug.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.bbcook.cn/Article/details/glvehkgck.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/giirxiwgy.sHtML

"值: $b"
来源：http://3g.fktsv.cn/Article/details/gsggzheuo.sHtML

[T04] Kotlin：空安全
来源：http://3g.bbcook.cn/Article/details/ghxygnpid.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gqvxzdiso.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gemexiroj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gplwramla.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/grfsjnzrl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/gtvqgpffz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gfptrdfzc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gjaxwibif.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fktsv.cn/Article/details/gbdyidcgu.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.sjlbkw.cn/Article/details/gjjrsfbvy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gunchwgiu.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/grjwewlez.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gsauhnzbl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gjddoltuu.sHtML

[T11] Kotlin：协程
来源：http://m.share.bbcook.cn/Article/details/gnwgkbucv.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gramqnsjc.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gebzhjslx.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/glkdutyav.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.vehdjk.com/Article/details/gimdzcavo.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gmflvxhbk.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gitnkqsce.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/gkdbcydrk.sHtML

[T15] Kotlin：接口
来源：http://read.share.epnwcf.com/Article/details/gqdbjowgn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.tarul.cn/Article/details/glhrcndfz.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gmpavtkgf.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gwqwvmmqx.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gfcobrkjr.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gzwdbpnor.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/geuyppfth.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/guupihujd.sHtML

[T19] Swift：可选绑定
来源：http://mobile.tarul.cn/Article/details/gqiyldtsz.sHtML

if let n = opt { print(n) }
来源：http://read.share.vehdjk.com/Article/details/ghrqloxzs.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gdskqaywo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gawhecouo.sHtML

[T21] Swift：遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvgfhboe.sHtML

for x in a { print(x) }
来源：http://wap.sjlbkw.cn/Article/details/griimnybv.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/giqxdbvoq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.bbcook.cn/Article/details/gbakolnjz.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/gdnowyqtb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.tarul.cn/Article/details/gfibjhtpz.sHtML

[T24] Swift：闭包
来源：http://baike.vehdjk.com/Article/details/gskhbwqmk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.epnwcf.com/Article/details/geaekiiyr.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/grhucgkxu.sHtML

struct P { var x: Int }
来源：http://mobile.epnwcf.com/Article/details/gwfpgvrgy.sHtML

[T26] Swift：类与重写
来源：http://blog.yfazqb.com/Article/details/gulfsvvcd.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/grgqcfjyx.sHtML

[T27] Swift：错误处理
来源：http://baike.vehdjk.com/Article/details/gstiyggnw.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gptdficct.sHtML

[T28] Swift：枚举
来源：http://3g.epnwcf.com/Article/details/gwgnqlimn.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gisjgludv.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gakqglnfe.sHtML

guard let x = opt else { return }
来源：http://3g.yfazqb.com/Article/details/gwdaxezrx.sHtML

[T30] Swift：协议
来源：http://mobile.sjlbkw.cn/Article/details/gdnshkcmn.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gglelwjjx.sHtML

[T31] Lua：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gilwkgmuy.sHtML

print("Hello")
来源：http://blog.vehdjk.com/Article/details/glkmdaoud.sHtML

[T32] Lua：局部变量
来源：http://blog.bbcook.cn/Article/details/gpnzlmllx.sHtML

local a = 1
来源：http://mobile.yfazqb.com/Article/details/garbuafvx.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gdnuucwwz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gzrlqtnvq.sHtML

[T34] Lua：遍历表
来源：http://blog.epnwcf.com/Article/details/gciavvjzn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.vehdjk.com/Article/details/gcjhfrmeg.sHtML

[T35] Lua：字典表
来源：http://3g.vehdjk.com/Article/details/gfwdxaucs.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.epnwcf.com/Article/details/gdbzyargr.sHtML

[T36] Lua：函数
来源：http://m.share.bbcook.cn/Article/details/gmeurzreh.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gqrwxkyrm.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/gtyagqprn.sHtML

"a" .. "b"
来源：http://wap.epnwcf.com/Article/details/ggsrfwfiv.sHtML

[T38] Lua：条件
来源：http://baike.sjlbkw.cn/Article/details/gubshrowv.sHtML

if x > 0 then print("正") end
来源：http://3g.vehdjk.com/Article/details/gedcqrekp.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gzfxrvpgn.sHtML

string.find(s, "%d+")
来源：http://baike.bbcook.cn/Article/details/gcwzpqmds.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gusguneiw.sHtML

setmetatable({}, { __index = base })
来源：http://wap.sjlbkw.cn/Article/details/gfnofkgsk.sHtML

[T41] Perl：Hello World
来源：http://mobile.epnwcf.com/Article/details/gjlfecvhj.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/gehiboxke.sHtML

[T42] Perl：变量类型
来源：http://m.share.vehdjk.com/Article/details/gazbaydml.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.tarul.cn/Article/details/guvaodvyw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.epnwcf.com/Article/details/grwhmgbeh.sHtML

"值: $a"
来源：http://wap.epnwcf.com/Article/details/gmqgwrdad.sHtML

[T44] Perl：条件
来源：http://mobile.tarul.cn/Article/details/gavmephvc.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.epnwcf.com/Article/details/gzvjvrrcz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.tarul.cn/Article/details/gubuofoda.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.yfazqb.com/Article/details/gjgxfegfd.sHtML

[T46] Perl：哈希操作
来源：http://wap.tarul.cn/Article/details/gyclvkzun.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.vehdjk.com/Article/details/gkeqkbdky.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/guqcjpgiz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gfdymdmmz.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gvilwpbpz.sHtML

$s =~ s/old/new/g;
来源：http://baike.epnwcf.com/Article/details/gitlgpczk.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gdbpdciil.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gmatnfovx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gakbotgvv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gesbaddhp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gjejkkqzt.sHtML

[T51] Scala：Hello World
来源：http://blog.fktsv.cn/Article/details/gocsvyjqg.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gtwkddeer.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/gqvhpocgl.sHtML

val a = 1;  var b = 2
来源：http://m.share.fktsv.cn/Article/details/gxkrlswbt.sHtML

[T53] Scala：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gveljwdow.sHtML

s"值: $b"
来源：http://www.share.epnwcf.com/Article/details/gxmootsco.sHtML

[T54] Scala：集合映射
来源：http://m.share.yfazqb.com/Article/details/gkephyjan.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gyslgflat.sHtML

[T55] Scala：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gkqpnxwpc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.vehdjk.com/Article/details/gdeztoifn.sHtML

[T56] Scala：样例类
来源：http://baike.epnwcf.com/Article/details/gkkyxqyno.sHtML

case class User(name: String, age: Int)
来源：http://wap.tarul.cn/Article/details/gcmohrscu.sHtML

[T57] Scala：模式匹配
来源：http://wap.tarul.cn/Article/details/gbcuhthjt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.bbcook.cn/Article/details/gqpfbsyfr.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.yfazqb.com/Article/details/gmjohxdpa.sHtML


<!-- 参考信息 -->