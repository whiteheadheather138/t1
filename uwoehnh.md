代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.bbcook.cn/Article/details/gffxakgsi.sHtML

[R56] 远程拷贝
来源：http://blog.tarul.cn/Article/details/gujyvbuig.sHtML

scp file user@host:/path/
来源：http://www.blog.yfazqb.com/Article/details/gvzehseas.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gmardsctg.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/ggnutektf.sHtML

[R58] 下载文件
来源：http://www.blog.bbcook.cn/Article/details/ginoqsdbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.tarul.cn/Article/details/glnediudm.sHtML

[R59] 发 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/gvnhtumun.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fktsv.cn/Article/details/gvvqxajsq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gvcjttxrj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.sjlbkw.cn/Article/details/gorglxkek.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gteorijho.sHtML

df -h;  du -sh *
来源：http://3g.fktsv.cn/Article/details/gswdoqabd.sHtML

[R62] 找最占空间的文件
来源：http://wap.fktsv.cn/Article/details/gpotvvjhw.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gwkjfaqcp.sHtML

[R63] 内存与进程
来源：http://baike.sjlbkw.cn/Article/details/gabpnvnfo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/ggkanpvnk.sHtML

[R64] 结束进程
来源：http://mobile.fktsv.cn/Article/details/gyzfzjyca.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.tarul.cn/Article/details/gigfccggb.sHtML

[R65] 查看端口占用
来源：http://mobile.yfazqb.com/Article/details/gjgcvvqxu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.vehdjk.com/Article/details/goqrhgyhl.sHtML

[R66] 定时任务
来源：http://www.share.yfazqb.com/Article/details/gmirdsvhd.sHtML

crontab -e;  crontab -l
来源：http://wap.sjlbkw.cn/Article/details/gucsahjmf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.vehdjk.com/Article/details/gpgyhsgcq.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gweybsjrx.sHtML

[R68] 计算文件校验值
来源：http://mobile.tarul.cn/Article/details/gambfavsm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gohsrntpa.sHtML

[R69] 生成随机密码
来源：http://3g.vehdjk.com/Article/details/ggwwsyxts.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.bbcook.cn/Article/details/ggyauswlj.sHtML

[R70] 时间戳与互转
来源：http://blog.bbcook.cn/Article/details/gxwzboube.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.tarul.cn/Article/details/gfvjqgasn.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gcanxxxkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.bbcook.cn/Article/details/guwzhcxia.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gdlnzgmoh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.vehdjk.com/Article/details/gktdjysqe.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/gayhwoqtb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gzvsgzkzh.sHtML

[R74] 批量重命名
来源：http://m.share.tarul.cn/Article/details/gorfvbkul.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gmjvjotgo.sHtML

[R75] 导出环境变量
来源：http://baike.vehdjk.com/Article/details/gajpxnurk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.tarul.cn/Article/details/gaahflqvh.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gdryyyqfe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.yfazqb.com/Article/details/gpkzayiud.sHtML

[R77] 读取用户输入
来源：http://www.m.share.epnwcf.com/Article/details/gbxoigcgj.sHtML

read -rp "请输入: " ans
来源：http://read.share.yfazqb.com/Article/details/gpfpnrexf.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gnrhryvqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.tarul.cn/Article/details/gqcgctsqa.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/gtowqofmx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.epnwcf.com/Article/details/geqnkclsd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fktsv.cn/Article/details/gamiposmj.sHtML

time ./run.sh
来源：http://www.share.bbcook.cn/Article/details/glkjenqxe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaqsunmmt.sHtML

S. C / C++ 专题
来源：http://3g.fktsv.cn/Article/details/gnigxbvsp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfsmnbqhl.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/ggmvyjfow.sHtML

#include <stdio.h>
来源：http://www.share.tarul.cn/Article/details/gsghycvai.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.epnwcf.com/Article/details/gdzaqtapw.sHtML

[S02] C：变量与格式化输出
来源：http://3g.sjlbkw.cn/Article/details/gcxdtxxhu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.epnwcf.com/Article/details/gezbfwdvn.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gzlpktoko.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/gibhavnpl.sHtML

[S04] C：字符串复制
来源：http://www.share.epnwcf.com/Article/details/gibjlpamt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.epnwcf.com/Article/details/gwodlfbde.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gflkaajfn.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gsagpmoor.sHtML

[S06] C：字符串比较
来源：http://blog.bbcook.cn/Article/details/gxgxuqgzx.sHtML

strcmp(a, b) == 0
来源：http://mobile.vehdjk.com/Article/details/galafysun.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.sjlbkw.cn/Article/details/grsndwvnd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.yfazqb.com/Article/details/gdgceitud.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.epnwcf.com/Article/details/gjpnehplk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gevwwfhtc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/geyjflrkv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.epnwcf.com/Article/details/gedesfuae.sHtML

[S10] C：指针与解引用
来源：http://mobile.fktsv.cn/Article/details/gomlttgrg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fktsv.cn/Article/details/gjmgmykrt.sHtML

[S11] C：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gqdjlvoly.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gzqpwktdb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.bbcook.cn/Article/details/gvbdamgbx.sHtML

fclose(f);
来源：http://read.share.tarul.cn/Article/details/gteetniug.sHtML

[S12] C：写文件
来源：http://www.m.share.bbcook.cn/Article/details/ggcqydnnh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gtoaokiwz.sHtML

[S13] C：宏定义
来源：http://m.share.tarul.cn/Article/details/giejvqeqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.bbcook.cn/Article/details/gggeildig.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/glkwftbif.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.sjlbkw.cn/Article/details/gvfmuyexg.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gxghvjxcj.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/gekrhjpal.sHtML

[S16] C：位操作置位
来源：http://3g.sjlbkw.cn/Article/details/gkziivefy.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gtqdwupyi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/ghzryneyq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.sjlbkw.cn/Article/details/gslrnghnw.sHtML

[S18] C：命令行参数
来源：http://baike.vehdjk.com/Article/details/glapsorys.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/goufltdvn.sHtML

[S19] C：快速排序
来源：http://www.m.share.vehdjk.com/Article/details/gvsapwjbg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.epnwcf.com/Article/details/gmvfcpreo.sHtML

[S20] C：二分查找
来源：http://baike.vehdjk.com/Article/details/gpvoqgemi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gznqjcdhw.sHtML

[S21] C：字符类别判断
来源：http://www.share.vehdjk.com/Article/details/gboehwtsk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/ghuvsxzbc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.yfazqb.com/Article/details/gqwlzajpr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gnuukjtwj.sHtML

[S23] C：随机数
来源：http://mobile.sjlbkw.cn/Article/details/gjwvnfacd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.bbcook.cn/Article/details/grcciyovf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gzcdfgfhu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fktsv.cn/Article/details/gkoyisxxg.sHtML

[S25] C：内存拷贝
来源：http://wap.fktsv.cn/Article/details/gsmggcbtt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/guhhsaast.sHtML

[S26] C：内存清零
来源：http://m.share.epnwcf.com/Article/details/geuktwdov.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/grkeuajag.sHtML

[S27] C：定义常量
来源：http://baike.yfazqb.com/Article/details/gtzpobigp.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gxhulkdyn.sHtML

[S28] C：静态变量
来源：http://read.share.bbcook.cn/Article/details/gwanxtuxo.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/ghsxtneyp.sHtML

[S29] C：变参函数
来源：http://www.m.share.epnwcf.com/Article/details/gbdvfsyvq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gvibriiaq.sHtML

[S30] C：头文件保护
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqgbucfs.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gjckeikey.sHtML

#define X_H
来源：http://baike.yfazqb.com/Article/details/gdykqexnr.sHtML

#endif
来源：http://baike.vehdjk.com/Article/details/gbriunxlm.sHtML

[S31] C++：Hello World
来源：http://mobile.bbcook.cn/Article/details/gbwoilpgd.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/grfragjtl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gxqhkuvgs.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gwgosexha.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.epnwcf.com/Article/details/gvumfmxnz.sHtML

[S33] C++：vector 增删
来源：http://mobile.yfazqb.com/Article/details/grsmovajf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fktsv.cn/Article/details/garlfuuyi.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.tarul.cn/Article/details/gcicypbuz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/grccjuudv.sHtML

[S35] C++：map
来源：http://www.share.vehdjk.com/Article/details/gpkiretoo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/glrtcxqso.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/gxfbemofs.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gbcwaqpze.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gfdhgdwxy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.bbcook.cn/Article/details/gskzhndfu.sHtML

[S38] C++：排序
来源：http://mobile.sjlbkw.cn/Article/details/gnoxxoflx.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.tarul.cn/Article/details/gedklaktp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.vehdjk.com/Article/details/gqobonwnf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.vehdjk.com/Article/details/gaapwuhwy.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gjgcuthfx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fktsv.cn/Article/details/gyqrkdbpn.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fktsv.cn/Article/details/gtufzdlpm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.sjlbkw.cn/Article/details/gcmmakluz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gmvataore.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gjtdtider.sHtML

[S43] C++：智能指针
来源：http://www.blog.sjlbkw.cn/Article/details/gtvfjxqrq.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.tarul.cn/Article/details/grmoeaxkw.sHtML

[S44] C++：引用传参
来源：http://m.share.vehdjk.com/Article/details/gtxyyzbid.sHtML

void inc(int &x) { ++x; }
来源：http://3g.tarul.cn/Article/details/gztefwczr.sHtML

[S45] C++：lambda
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnvcncfq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.sjlbkw.cn/Article/details/gjekrrnhk.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gobodahcg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.tarul.cn/Article/details/gyibrdgvm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.sjlbkw.cn/Article/details/goepmdypf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.sjlbkw.cn/Article/details/gzmeusdmn.sHtML

[S48] C++：逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gzmffxonu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.vehdjk.com/Article/details/gcvuwghwf.sHtML

while (std::getline(in, line)) { }
来源：http://baike.tarul.cn/Article/details/gqozdfzeh.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/gkmehbzgr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gsddmsqwc.sHtML

[S50] C++：格式化数字
来源：http://blog.bbcook.cn/Article/details/gebiewqvh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gybomsrvc.sHtML

[S51] C++：显式类型转换
来源：http://m.share.sjlbkw.cn/Article/details/gxhwuplxv.sHtML

static_cast<double>(a) / b
来源：http://www.blog.bbcook.cn/Article/details/gtchyzjqx.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.tarul.cn/Article/details/gcgviduyu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/gsqlclixx.sHtML

[S53] C++：移动语义
来源：http://wap.bbcook.cn/Article/details/gufpzcbrk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/gwurjadbu.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gjmwyrjkq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.bbcook.cn/Article/details/ggkgmuprm.sHtML

[S55] C++：结构化绑定
来源：http://baike.yfazqb.com/Article/details/gtlkecvdo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.epnwcf.com/Article/details/gfklceemn.sHtML

[S56] C++：optional
来源：http://m.share.fktsv.cn/Article/details/ghadlwvzs.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.tarul.cn/Article/details/ghzgfssnr.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gzvlfcgya.sHtML

constexpr int N = 10;
来源：http://www.share.epnwcf.com/Article/details/gxinylqau.sHtML

[S58] C++：命名空间
来源：http://www.share.epnwcf.com/Article/details/grbrqmkde.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gxmlvbphd.sHtML

[S59] C++：静态断言
来源：http://www.m.share.vehdjk.com/Article/details/gftfvguun.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/ghhzwvltx.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.sjlbkw.cn/Article/details/gehonzrju.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gzyceamtt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/guzibqarn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/giqpddgjh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkdxmtlbm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.epnwcf.com/Article/details/gvaizlait.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/ggljvisaa.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gdkgthgiu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gdetgllvz.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fktsv.cn/Article/details/ghorycpfk.sHtML

"值: $b"
来源：http://www.m.share.yfazqb.com/Article/details/gxqzirldb.sHtML

[T04] Kotlin：空安全
来源：http://blog.epnwcf.com/Article/details/gpfuheady.sHtML

val n: String? = null;  n?.length
来源：http://wap.vehdjk.com/Article/details/gwjemeokj.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.tarul.cn/Article/details/gzpmezurb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.epnwcf.com/Article/details/gybzlzogb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/ghkeptnlx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/geuaezsus.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gzqqabwrp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.tarul.cn/Article/details/gpsqkympc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.epnwcf.com/Article/details/gmrxsqxua.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gwnafvbnt.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.vehdjk.com/Article/details/gklqoxjku.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/grmaozcgl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.tarul.cn/Article/details/gprcosbib.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.sjlbkw.cn/Article/details/gmyopihjf.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gjzeorjig.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.vehdjk.com/Article/details/gbdxlkiqv.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.epnwcf.com/Article/details/gmmysbjgl.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.bbcook.cn/Article/details/gabqpefoc.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.sjlbkw.cn/Article/details/gmhbmsgzu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/ggqcqwlbn.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gvytsdbvu.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/gfrkrbexp.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gtloyijtp.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.sjlbkw.cn/Article/details/gwgiivbsh.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gdrdjdlmt.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gtuaoqcpt.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gabswdhsa.sHtML

var a = 1;  let b = 2
来源：http://www.share.bbcook.cn/Article/details/ggrezkjsd.sHtML

[T18] Swift：字符串插值
来源：http://3g.tarul.cn/Article/details/gvunaacdf.sHtML

"值: \(b)"
来源：http://baike.yfazqb.com/Article/details/gxwzectqr.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/gzsiztwqb.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gttxbxdom.sHtML

[T20] Swift：数组操作
来源：http://www.share.epnwcf.com/Article/details/gzdzjigcu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.sjlbkw.cn/Article/details/gecrcqmvd.sHtML

[T21] Swift：遍历
来源：http://blog.yfazqb.com/Article/details/glqqktwnx.sHtML

for x in a { print(x) }
来源：http://www.m.share.epnwcf.com/Article/details/gnthanmxj.sHtML

[T22] Swift：字典
来源：http://blog.vehdjk.com/Article/details/gegwdfoxh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.tarul.cn/Article/details/gflnnbngi.sHtML

[T23] Swift：函数
来源：http://www.blog.sjlbkw.cn/Article/details/gprsvrjzq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gqdfeclnm.sHtML

[T24] Swift：闭包
来源：http://wap.bbcook.cn/Article/details/glndqtwkw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.bbcook.cn/Article/details/gisqbscxg.sHtML

[T25] Swift：结构体
来源：http://www.m.share.tarul.cn/Article/details/gpxbjecng.sHtML

struct P { var x: Int }
来源：http://www.share.fktsv.cn/Article/details/gveygrcsg.sHtML

[T26] Swift：类与重写
来源：http://wap.vehdjk.com/Article/details/gdbcpnyix.sHtML

class A: Base { override func f() {} }
来源：http://3g.bbcook.cn/Article/details/ggybnriei.sHtML

[T27] Swift：错误处理
来源：http://www.share.fktsv.cn/Article/details/getlhsqic.sHtML

do { try f() } catch { print(error) }
来源：http://3g.bbcook.cn/Article/details/guvrcdbdc.sHtML

[T28] Swift：枚举
来源：http://baike.yfazqb.com/Article/details/ghrkknwcu.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gqiwofonl.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.yfazqb.com/Article/details/gnfvepkjx.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/grcdhqlkt.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gqjippbtu.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gbaismepk.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/gjzblxmtn.sHtML

print("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/ggozheeox.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/giatnueix.sHtML

local a = 1
来源：http://3g.epnwcf.com/Article/details/gazadrhmk.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gcebhgopu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.yfazqb.com/Article/details/glcthftsf.sHtML

[T34] Lua：遍历表
来源：http://blog.tarul.cn/Article/details/gjfuthvib.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/geesakpnl.sHtML

[T35] Lua：字典表
来源：http://m.share.epnwcf.com/Article/details/gstucjykg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/glcqsgcva.sHtML

[T36] Lua：函数
来源：http://3g.yfazqb.com/Article/details/gdncwnzsj.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gxgjcritl.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/gubycwaxa.sHtML

"a" .. "b"
来源：http://3g.fktsv.cn/Article/details/gfnomwmbp.sHtML

[T38] Lua：条件
来源：http://www.m.share.bbcook.cn/Article/details/gjmjkgndw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.epnwcf.com/Article/details/gapixfopd.sHtML

[T39] Lua：模式匹配
来源：http://3g.vehdjk.com/Article/details/glzanncli.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gifyskznu.sHtML

[T40] Lua：元表
来源：http://www.blog.sjlbkw.cn/Article/details/gkpwfulex.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/gedpclsrs.sHtML

[T41] Perl：Hello World
来源：http://m.share.epnwcf.com/Article/details/gnyppxskd.sHtML

print "Hello\n";
来源：http://wap.yfazqb.com/Article/details/gznxfwssn.sHtML

[T42] Perl：变量类型
来源：http://www.blog.tarul.cn/Article/details/gbtqnlssu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/gsdamfmoz.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/glcgacitd.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/gbjjjkwxe.sHtML

[T44] Perl：条件
来源：http://blog.bbcook.cn/Article/details/guuwzqauf.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.vehdjk.com/Article/details/gnfjqjtfa.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/gwtxuobzb.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gfvpartlz.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gybuuzlgm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.epnwcf.com/Article/details/grticgxco.sHtML

[T47] Perl：正则捕获
来源：http://blog.vehdjk.com/Article/details/gyopmjcvw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.yfazqb.com/Article/details/giddzruhi.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gjvwndxfg.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.tarul.cn/Article/details/gmgzidzqs.sHtML

[T49] Perl：函数
来源：http://baike.epnwcf.com/Article/details/gzuqvizpu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.tarul.cn/Article/details/gwtahewhx.sHtML

[T50] Perl：逐行读文件
来源：http://baike.tarul.cn/Article/details/gtzdkqxsu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.yfazqb.com/Article/details/gcyjgfsgx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/goojuiljp.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gmqjllvrl.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/gkzafelvf.sHtML

[T52] Scala：变量
来源：http://read.share.epnwcf.com/Article/details/gobhfhqqu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/ghleuzcht.sHtML

[T53] Scala：字符串插值
来源：http://baike.yfazqb.com/Article/details/gdquerepf.sHtML

s"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gfavwxnbu.sHtML

[T54] Scala：集合映射
来源：http://read.share.bbcook.cn/Article/details/gwvajfuqq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.bbcook.cn/Article/details/ggndctvhl.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gzmnjpkjc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gaeyaeiko.sHtML

[T56] Scala：样例类
来源：http://m.share.fktsv.cn/Article/details/gmsruetst.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fktsv.cn/Article/details/guzefdpvu.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gwnlqaixa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.epnwcf.com/Article/details/gczxyqkht.sHtML

[T58] Scala：函数定义
来源：http://wap.tarul.cn/Article/details/gelzinqmb.sHtML


<!-- 参考信息 -->