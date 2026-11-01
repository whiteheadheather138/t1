代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.bbcook.cn/Article/details/gjbilodsr.sHtML

[R52] 统计行数
来源：http://3g.vehdjk.com/Article/details/gztqdxcdb.sHtML

wc -l a.txt
来源：http://www.blog.bbcook.cn/Article/details/glpsduflf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/grsutoohs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gefwwlrrb.sHtML

[R54] 比较两个文件
来源：http://baike.sjlbkw.cn/Article/details/ggukerafj.sHtML

diff a.txt b.txt
来源：http://www.blog.tarul.cn/Article/details/glgzgqogh.sHtML

[R55] 压缩与解压
来源：http://www.blog.tarul.cn/Article/details/grguvngnn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fktsv.cn/Article/details/gbryxghuu.sHtML

[R56] 远程拷贝
来源：http://blog.fktsv.cn/Article/details/ggfgdmsqk.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gnzrnhtez.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gberaazkp.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/gkprnkcwq.sHtML

[R58] 下载文件
来源：http://read.share.epnwcf.com/Article/details/gboccyess.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.epnwcf.com/Article/details/gxtiipcpv.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gfzkgolfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gsyrdqjif.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gmucnluer.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fktsv.cn/Article/details/gxxoqhzqr.sHtML

[R61] 磁盘占用
来源：http://read.share.sjlbkw.cn/Article/details/gtclgdhfc.sHtML

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/gzxfumrvc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gkafclwqp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.epnwcf.com/Article/details/gpxfrhksj.sHtML

[R63] 内存与进程
来源：http://www.blog.epnwcf.com/Article/details/gfcumvvif.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/ggsnbpowd.sHtML

[R64] 结束进程
来源：http://m.share.bbcook.cn/Article/details/gugltarzo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gfmchdhfg.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gvnqgmpyi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.tarul.cn/Article/details/gxusliinq.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/glksgmqih.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/gzktwbefk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/gtmbjnbkn.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/ggzleqmya.sHtML

[R68] 计算文件校验值
来源：http://baike.epnwcf.com/Article/details/gucfnpijs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.yfazqb.com/Article/details/ghbdjmuwg.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/gjbdgsnqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.bbcook.cn/Article/details/geuepqhru.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwcuxdgu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.epnwcf.com/Article/details/gccljclqp.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/ggoalcusm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/ghekfpmsn.sHtML

[R72] 等待端口就绪
来源：http://m.share.vehdjk.com/Article/details/glyeixdkc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/greyraohj.sHtML

[R73] 分割大日志
来源：http://wap.fktsv.cn/Article/details/gapcoilxs.sHtML

split -l 1000 big.log part_
来源：http://www.blog.tarul.cn/Article/details/gmxwjbmjw.sHtML

[R74] 批量重命名
来源：http://blog.vehdjk.com/Article/details/grfxxvdpa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.tarul.cn/Article/details/gejypslbb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gwtogedgo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fktsv.cn/Article/details/gzvhhnnvs.sHtML

[R76] 使用临时文件
来源：http://wap.sjlbkw.cn/Article/details/grpkbhtyr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/goookybhu.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/glaxfiiim.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/gdnwwggqs.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gemkrtubj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.bbcook.cn/Article/details/gznnjjibi.sHtML

[R79] 解析命令行选项
来源：http://mobile.tarul.cn/Article/details/gidkayzkw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gzojifkaq.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gerblrlfc.sHtML

time ./run.sh
来源：http://www.share.fktsv.cn/Article/details/gzmlalhwy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gebgfqndm.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gedlgpkao.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glxpnwlzx.sHtML

[S01] C：Hello World
来源：http://blog.yfazqb.com/Article/details/guwifhwxz.sHtML

#include <stdio.h>
来源：http://3g.fktsv.cn/Article/details/gkjiorhlr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.sjlbkw.cn/Article/details/gcowiplfw.sHtML

[S02] C：变量与格式化输出
来源：http://baike.yfazqb.com/Article/details/gdghuvkii.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.sjlbkw.cn/Article/details/gwtufdgce.sHtML

[S03] C：读入整数
来源：http://3g.sjlbkw.cn/Article/details/gwfxjuioo.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/gatpfcdvk.sHtML

[S04] C：字符串复制
来源：http://read.share.fktsv.cn/Article/details/glphicrey.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.yfazqb.com/Article/details/gshawfpdf.sHtML

[S05] C：字符串长度
来源：http://mobile.bbcook.cn/Article/details/gabxxyasc.sHtML

strlen(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwhhivnyv.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gqvcgydxh.sHtML

strcmp(a, b) == 0
来源：http://baike.sjlbkw.cn/Article/details/gwbcnotyw.sHtML

[S07] C：数组遍历求和
来源：http://3g.yfazqb.com/Article/details/gunaherwe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.yfazqb.com/Article/details/gfdmdxjxi.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gtighdemr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gwveqcaxi.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fktsv.cn/Article/details/gzhndbcte.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/ggnxpmvpy.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gnacimpqp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.bbcook.cn/Article/details/gzykbrqkg.sHtML

[S11] C：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/glbbrppwq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.sjlbkw.cn/Article/details/gbbtjodng.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/gwovscsao.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gqwlmpilq.sHtML

[S12] C：写文件
来源：http://blog.fktsv.cn/Article/details/gabgyctjz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.bbcook.cn/Article/details/gahbsgwwp.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gqqsmqxof.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.sjlbkw.cn/Article/details/gdmruvnwr.sHtML

[S14] C：枚举
来源：http://www.share.epnwcf.com/Article/details/gukdrjccv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.bbcook.cn/Article/details/gxxzvsyow.sHtML

[S15] C：类型转换
来源：http://read.share.bbcook.cn/Article/details/gymnqavih.sHtML

(double) a / b
来源：http://www.m.share.bbcook.cn/Article/details/guqekzbxi.sHtML

[S16] C：位操作置位
来源：http://baike.bbcook.cn/Article/details/gjvsfumha.sHtML

x |= (1 << 3);
来源：http://wap.bbcook.cn/Article/details/ggmktpjar.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/ggnznjsty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gcjisdpfg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/getznlnbz.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/gkoibiagu.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/grbhwozxd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gxsffktgm.sHtML

[S20] C：二分查找
来源：http://www.blog.yfazqb.com/Article/details/gdkfhukgy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gninyqhhw.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gxzifdtnr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gqlbarumg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gmvnycyfj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.yfazqb.com/Article/details/graruerer.sHtML

[S23] C：随机数
来源：http://baike.epnwcf.com/Article/details/gqlykpvhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.epnwcf.com/Article/details/gzgqmystv.sHtML

[S24] C：获取本地时间
来源：http://baike.sjlbkw.cn/Article/details/glqeaqzse.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gukuewuxr.sHtML

[S25] C：内存拷贝
来源：http://read.share.epnwcf.com/Article/details/gasddekii.sHtML

memcpy(dst, src, n);
来源：http://3g.bbcook.cn/Article/details/gtcyzstrs.sHtML

[S26] C：内存清零
来源：http://3g.vehdjk.com/Article/details/grnylcxks.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fktsv.cn/Article/details/gucexdlfy.sHtML

[S27] C：定义常量
来源：http://mobile.yfazqb.com/Article/details/ggzhhiknt.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gomlqoqbn.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gdvorckxk.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/ggepiiuef.sHtML

[S29] C：变参函数
来源：http://baike.epnwcf.com/Article/details/gxfqusbah.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.sjlbkw.cn/Article/details/ghkjfrfeg.sHtML

[S30] C：头文件保护
来源：http://m.share.vehdjk.com/Article/details/grfkgnpts.sHtML

#ifndef X_H
来源：http://blog.sjlbkw.cn/Article/details/gziaufwpl.sHtML

#define X_H
来源：http://blog.yfazqb.com/Article/details/gxcnifmvn.sHtML

#endif
来源：http://baike.tarul.cn/Article/details/gbduvbdif.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gqmihqrxl.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gehjkkofd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.yfazqb.com/Article/details/ghoinietg.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gagxxuicz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gjavxyoyd.sHtML

[S33] C++：vector 增删
来源：http://wap.tarul.cn/Article/details/gmboywnnj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.yfazqb.com/Article/details/gaddafneo.sHtML

[S34] C++：遍历 vector
来源：http://wap.fktsv.cn/Article/details/gkutcyeew.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.bbcook.cn/Article/details/ghfuqtshj.sHtML

[S35] C++：map
来源：http://read.share.fktsv.cn/Article/details/gctjwumrm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/ghfgilwdn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.sjlbkw.cn/Article/details/gozummyuv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.bbcook.cn/Article/details/geikzivpx.sHtML

[S37] C++：set
来源：http://mobile.sjlbkw.cn/Article/details/gfphsrysa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fktsv.cn/Article/details/gsrgdrtxh.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gspgrxfwi.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/geuvkluow.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/ghwgidwqw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/grmchfutv.sHtML

[S40] C++：查找元素
来源：http://blog.tarul.cn/Article/details/goqbuhzxn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gutdrwezn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.yfazqb.com/Article/details/gjggdxfcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.tarul.cn/Article/details/ggpphqmie.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.yfazqb.com/Article/details/gzagzsufe.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gcjxaziaf.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gvqaecgbn.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.epnwcf.com/Article/details/gmeigiewx.sHtML

[S44] C++：引用传参
来源：http://baike.tarul.cn/Article/details/gzicnxgqb.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grpeymmld.sHtML

[S45] C++：lambda
来源：http://blog.epnwcf.com/Article/details/gutgbcemh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fktsv.cn/Article/details/gasuisvxe.sHtML

[S46] C++：函数模板
来源：http://read.share.fktsv.cn/Article/details/glneypska.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gpvludjgf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.vehdjk.com/Article/details/gckzjrdyq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gahldmjei.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gdwichrfv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gugybsjif.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gmucgxneo.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gtejrbens.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gzvfpthmu.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/glhgcpbpm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gytjjtkih.sHtML

[S51] C++：显式类型转换
来源：http://m.share.vehdjk.com/Article/details/gwxbkitxy.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.bbcook.cn/Article/details/gtfubszij.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/glmmgelkv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.bbcook.cn/Article/details/gaipbuswq.sHtML

[S53] C++：移动语义
来源：http://mobile.epnwcf.com/Article/details/glnsfgszm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.sjlbkw.cn/Article/details/gckervhdv.sHtML

[S54] C++：异常处理
来源：http://mobile.fktsv.cn/Article/details/gvuzuvqdx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.epnwcf.com/Article/details/gcslmupoo.sHtML

[S55] C++：结构化绑定
来源：http://read.share.sjlbkw.cn/Article/details/gdhjapxfg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fktsv.cn/Article/details/gfsmemsrb.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gmeybbzyq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/glsbdtfsf.sHtML

[S57] C++：编译期常量
来源：http://www.share.vehdjk.com/Article/details/gyjdsqrtt.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gxhaxcrhn.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gfwgmlcwl.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.bbcook.cn/Article/details/gfdosbffq.sHtML

[S59] C++：静态断言
来源：http://www.share.tarul.cn/Article/details/ggfhxmowi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.yfazqb.com/Article/details/gacgubode.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.bbcook.cn/Article/details/gfsckmxjo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/glrbeekhe.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwuobsmoo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.tarul.cn/Article/details/ginuunbjx.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/genbqsdtr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fktsv.cn/Article/details/gbemogsjo.sHtML

println("Hello")
来源：http://mobile.vehdjk.com/Article/details/gvgxixtxa.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gkluvspno.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.bbcook.cn/Article/details/gawgvrfik.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.epnwcf.com/Article/details/gwmugwofr.sHtML

"值: $b"
来源：http://3g.tarul.cn/Article/details/ggkmgbpsn.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.sjlbkw.cn/Article/details/gbcbqkblu.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gdeahjtan.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.bbcook.cn/Article/details/gcofezvmr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gnhruzsll.sHtML

[T06] Kotlin：集合映射
来源：http://3g.tarul.cn/Article/details/gofkwaspd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.epnwcf.com/Article/details/gwpqukwyz.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/grajbxulv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.bbcook.cn/Article/details/gzsheoatn.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/grgekukzn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gyjoluyom.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fktsv.cn/Article/details/gtyhxasro.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.bbcook.cn/Article/details/gzdfavrvx.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gdkxlzrnh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/geunlmcin.sHtML

[T11] Kotlin：协程
来源：http://blog.epnwcf.com/Article/details/grdwqipxh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fktsv.cn/Article/details/gcafmiyix.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gvxfgfdvq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.bbcook.cn/Article/details/gmjybujzw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtwkzzsh.sHtML

val m = mapOf("a" to 1)
来源：http://wap.tarul.cn/Article/details/gunkbqlxm.sHtML

[T14] Kotlin：循环
来源：http://baike.tarul.cn/Article/details/gdtnnmucl.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gbmddqpzq.sHtML

[T15] Kotlin：接口
来源：http://www.share.tarul.cn/Article/details/gfwykgsaj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.epnwcf.com/Article/details/gqdqtyxdo.sHtML

[T16] Swift：Hello World
来源：http://read.share.tarul.cn/Article/details/gndnervec.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gxsjfssnp.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fktsv.cn/Article/details/gvgwsztji.sHtML

var a = 1;  let b = 2
来源：http://3g.yfazqb.com/Article/details/gvrnsevgv.sHtML

[T18] Swift：字符串插值
来源：http://wap.tarul.cn/Article/details/gdxpjbpjz.sHtML

"值: \(b)"
来源：http://baike.vehdjk.com/Article/details/gyybubwes.sHtML

[T19] Swift：可选绑定
来源：http://baike.fktsv.cn/Article/details/gxbbmxngh.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/goynfdihx.sHtML

[T20] Swift：数组操作
来源：http://m.share.fktsv.cn/Article/details/gocvdmmly.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.epnwcf.com/Article/details/ggppiaxeg.sHtML

[T21] Swift：遍历
来源：http://www.share.yfazqb.com/Article/details/gcfqbdyjy.sHtML

for x in a { print(x) }
来源：http://3g.yfazqb.com/Article/details/gnqkfwhuj.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/gauhjtqpe.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gphhqtzou.sHtML

[T23] Swift：函数
来源：http://read.share.vehdjk.com/Article/details/gboqyjamn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.yfazqb.com/Article/details/gnjmxyjza.sHtML

[T24] Swift：闭包
来源：http://m.share.sjlbkw.cn/Article/details/gxyqskkyl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gbtnurdlu.sHtML

[T25] Swift：结构体
来源：http://blog.fktsv.cn/Article/details/gbtsknqao.sHtML

struct P { var x: Int }
来源：http://3g.yfazqb.com/Article/details/gfsenbfws.sHtML

[T26] Swift：类与重写
来源：http://www.share.epnwcf.com/Article/details/gblmraqau.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.yfazqb.com/Article/details/geahrfcne.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gsdgzpxwc.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gkefmwkig.sHtML

[T28] Swift：枚举
来源：http://www.m.share.bbcook.cn/Article/details/gyizmjqda.sHtML

enum Color { case red, green }
来源：http://3g.fktsv.cn/Article/details/gplgeiufi.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.bbcook.cn/Article/details/gpbxeceqc.sHtML

guard let x = opt else { return }
来源：http://3g.bbcook.cn/Article/details/gzidvzprr.sHtML

[T30] Swift：协议
来源：http://wap.sjlbkw.cn/Article/details/gzvwmtwzo.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.tarul.cn/Article/details/gepzirdtk.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gjyqkwjxr.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gehbdbdad.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgntklaw.sHtML

local a = 1
来源：http://wap.yfazqb.com/Article/details/glxcnfwqe.sHtML

[T33] Lua：表（数组）
来源：http://wap.bbcook.cn/Article/details/gcuxhshzv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.vehdjk.com/Article/details/gzqplnilg.sHtML

[T34] Lua：遍历表
来源：http://m.share.tarul.cn/Article/details/gcyujtthc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gkypahrko.sHtML

[T35] Lua：字典表
来源：http://m.share.yfazqb.com/Article/details/gjjsfrbyv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.bbcook.cn/Article/details/giaupecah.sHtML

[T36] Lua：函数
来源：http://read.share.fktsv.cn/Article/details/gxgylknsb.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gqdlgdnps.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.tarul.cn/Article/details/gihklknqt.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gidaeqxgx.sHtML

[T38] Lua：条件
来源：http://wap.yfazqb.com/Article/details/gkmgcmvgs.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gmdhsjxxx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gmpqxkdgq.sHtML

string.find(s, "%d+")
来源：http://mobile.tarul.cn/Article/details/gjtrayxby.sHtML

[T40] Lua：元表
来源：http://mobile.fktsv.cn/Article/details/gtxaijqcm.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fktsv.cn/Article/details/gjdvfygob.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gzxallswp.sHtML

print "Hello\n";
来源：http://blog.sjlbkw.cn/Article/details/gymmijhsf.sHtML

[T42] Perl：变量类型
来源：http://m.share.tarul.cn/Article/details/grjwtdons.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.tarul.cn/Article/details/ggdhtfuiz.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gghmqccmz.sHtML

"值: $a"
来源：http://3g.vehdjk.com/Article/details/gojbavunv.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/gtisprhcw.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.bbcook.cn/Article/details/glylmlsdf.sHtML

[T45] Perl：数组遍历
来源：http://3g.bbcook.cn/Article/details/gdcconffn.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.tarul.cn/Article/details/gwzxqaksa.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gcgaazjnp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.vehdjk.com/Article/details/gnnthmvef.sHtML

[T47] Perl：正则捕获
来源：http://3g.sjlbkw.cn/Article/details/gmcdgoloe.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.fktsv.cn/Article/details/goxatlmgd.sHtML

[T48] Perl：正则替换
来源：http://wap.yfazqb.com/Article/details/gxieibams.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/ggjjvipib.sHtML

[T49] Perl：函数
来源：http://m.share.sjlbkw.cn/Article/details/gwahyjnna.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.fktsv.cn/Article/details/grypuwrgu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gtigxxyan.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gxkviwbia.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/gihtiliqs.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzgwbkpan.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gboksmnco.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/grnfumbps.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gnexkyeje.sHtML

[T53] Scala：字符串插值
来源：http://wap.fktsv.cn/Article/details/gwcwvfcsa.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gzhbcpvpy.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gepfqfcdy.sHtML


<!-- 参考信息 -->