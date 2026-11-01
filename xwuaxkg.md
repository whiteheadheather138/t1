代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.epnwcf.com/Article/details/gxgauqxnb.sHtML

[R56] 远程拷贝
来源：http://3g.fktsv.cn/Article/details/gnftlvznl.sHtML

scp file user@host:/path/
来源：http://www.share.epnwcf.com/Article/details/getbwynqn.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gebsunmqr.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/ghvckgxyj.sHtML

[R58] 下载文件
来源：http://read.share.sjlbkw.cn/Article/details/gvfvdcfrz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fktsv.cn/Article/details/gkuvkvyog.sHtML

[R59] 发 POST JSON
来源：http://m.share.epnwcf.com/Article/details/gtabefrau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.vehdjk.com/Article/details/gusedigmi.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.tarul.cn/Article/details/govnmjvvy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fktsv.cn/Article/details/geeyqxlyq.sHtML

[R61] 磁盘占用
来源：http://mobile.vehdjk.com/Article/details/grdohquva.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gycsxopjm.sHtML

[R62] 找最占空间的文件
来源：http://wap.yfazqb.com/Article/details/gawuqzhqh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gqqqrujqr.sHtML

[R63] 内存与进程
来源：http://wap.epnwcf.com/Article/details/gcsedqgbj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.tarul.cn/Article/details/glhqdnhlk.sHtML

[R64] 结束进程
来源：http://blog.bbcook.cn/Article/details/gutmwlxiy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.tarul.cn/Article/details/golckqqrs.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gmuqypyws.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gjcaihlkx.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/gwcfehchl.sHtML

crontab -e;  crontab -l
来源：http://mobile.bbcook.cn/Article/details/gchlsmlaz.sHtML

[R67] 生成随机十六进制串
来源：http://blog.yfazqb.com/Article/details/gubjkkuaw.sHtML

openssl rand -hex 16
来源：http://3g.tarul.cn/Article/details/gdfurbwrj.sHtML

[R68] 计算文件校验值
来源：http://mobile.sjlbkw.cn/Article/details/gocscpcez.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.yfazqb.com/Article/details/gnhcflnlp.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/gpdrtiege.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.bbcook.cn/Article/details/gbvsbhicj.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fktsv.cn/Article/details/ghvuldmad.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fktsv.cn/Article/details/gdetrjnbw.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gknqxhgtr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fktsv.cn/Article/details/gficabude.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/ghqjuncsr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gtjdaxnms.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/glypbdguo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrrvxhwn.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/ghslmoebh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/ggommgwoa.sHtML

[R75] 导出环境变量
来源：http://mobile.fktsv.cn/Article/details/ghnripjep.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/grcgobieq.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/ghfbxcbjp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/gzdupdvhh.sHtML

[R77] 读取用户输入
来源：http://read.share.tarul.cn/Article/details/gpipjushn.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gcorppzpi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.epnwcf.com/Article/details/gvfquvnni.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.vehdjk.com/Article/details/gmsrjmzst.sHtML

[R79] 解析命令行选项
来源：http://baike.vehdjk.com/Article/details/gzuobkgcr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/glymzmxqr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gndomkdpc.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/gscmwwvcl.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glgqxqvnj.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/ghozlhzba.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtmajpgvf.sHtML

[S01] C：Hello World
来源：http://blog.tarul.cn/Article/details/gkchketvs.sHtML

#include <stdio.h>
来源：http://www.m.share.fktsv.cn/Article/details/glzgsiptu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjavfnzxs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.vehdjk.com/Article/details/gujcbfuwb.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.bbcook.cn/Article/details/glvtwqpau.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gunhkwjbe.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gtqufcxbn.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/grqtrtxoz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/glsfouctg.sHtML

[S05] C：字符串长度
来源：http://wap.yfazqb.com/Article/details/gvbzqvzlm.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gwdqzeclf.sHtML

[S06] C：字符串比较
来源：http://wap.yfazqb.com/Article/details/gnhzwjzav.sHtML

strcmp(a, b) == 0
来源：http://read.share.yfazqb.com/Article/details/ghzrcpbqe.sHtML

[S07] C：数组遍历求和
来源：http://www.share.yfazqb.com/Article/details/gmtwsagtv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.tarul.cn/Article/details/gvbysiafn.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.vehdjk.com/Article/details/gidtajmji.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gynhwnmxs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gwlhqkwsb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.yfazqb.com/Article/details/gcyjxthao.sHtML

[S10] C：指针与解引用
来源：http://m.share.vehdjk.com/Article/details/gealguftu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gyapgbmkm.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gezqbtxtd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.epnwcf.com/Article/details/gzrutthcq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gbizlrwiz.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gseqkqjcz.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gsjziaorg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gbfntbhbz.sHtML

[S13] C：宏定义
来源：http://mobile.fktsv.cn/Article/details/gdoonskyk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.epnwcf.com/Article/details/gwridzwdx.sHtML

[S14] C：枚举
来源：http://www.blog.vehdjk.com/Article/details/gadxouswi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gntdivdhr.sHtML

[S15] C：类型转换
来源：http://mobile.yfazqb.com/Article/details/gpckqvmfq.sHtML

(double) a / b
来源：http://www.share.vehdjk.com/Article/details/gteiaibrz.sHtML

[S16] C：位操作置位
来源：http://mobile.yfazqb.com/Article/details/gmufkldni.sHtML

x |= (1 << 3);
来源：http://read.share.vehdjk.com/Article/details/gzndepnar.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/ghjithnya.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gtmovyhxm.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gtrnrewqh.sHtML

int main(int argc, char **argv)
来源：http://m.share.vehdjk.com/Article/details/gtnkambrn.sHtML

[S19] C：快速排序
来源：http://wap.tarul.cn/Article/details/ggdecuchn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gfokdtcao.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gkduzdgsi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gravikivo.sHtML

[S21] C：字符类别判断
来源：http://mobile.sjlbkw.cn/Article/details/gdgaixfqj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gcbyzflvn.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gtwajvywj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.yfazqb.com/Article/details/gytpzetnk.sHtML

[S23] C：随机数
来源：http://read.share.fktsv.cn/Article/details/gkpdnybju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.tarul.cn/Article/details/gfzwaeeqd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/goqypskxi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.yfazqb.com/Article/details/gupxewuul.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gvlwoluwm.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gdjzmpbfk.sHtML

[S26] C：内存清零
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrtpmxem.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.vehdjk.com/Article/details/gqzodovyb.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gyvgcwtir.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/glxlhxgra.sHtML

[S28] C：静态变量
来源：http://www.share.tarul.cn/Article/details/gsoqeqnqo.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/gqghaqsxo.sHtML

[S29] C：变参函数
来源：http://m.share.bbcook.cn/Article/details/ghltbzxau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.epnwcf.com/Article/details/giaomzsng.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fktsv.cn/Article/details/gzaeqqfrr.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gsmpslxip.sHtML

#define X_H
来源：http://www.blog.epnwcf.com/Article/details/gcnjbyose.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/gyqbaunid.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gvshuhbgf.sHtML

#include <iostream>
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgswhywc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fktsv.cn/Article/details/ggwfrmhdj.sHtML

[S32] C++：字符串
来源：http://www.share.bbcook.cn/Article/details/gpgncrzsc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.epnwcf.com/Article/details/gdfftqmth.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gtahjcnsa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fktsv.cn/Article/details/gihnpxkww.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.yfazqb.com/Article/details/ghostszlx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.epnwcf.com/Article/details/gfzonpcsn.sHtML

[S35] C++：map
来源：http://wap.fktsv.cn/Article/details/gyhwqhawz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gunhllvnf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gniqlcdwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gglykjlgo.sHtML

[S37] C++：set
来源：http://mobile.bbcook.cn/Article/details/gphotwpxx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.epnwcf.com/Article/details/gwreqvjsw.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gqjxbhfip.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.epnwcf.com/Article/details/gqxjhohwr.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gczhjuouh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fktsv.cn/Article/details/gddtionql.sHtML

[S40] C++：查找元素
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcznucsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gfalbxcgf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.bbcook.cn/Article/details/gcxendhdk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gyyxwwzqi.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.epnwcf.com/Article/details/gvlhykzbz.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gapioleaw.sHtML

[S43] C++：智能指针
来源：http://mobile.yfazqb.com/Article/details/gdukhvigm.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gmoclacgi.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/gaabunuju.sHtML

void inc(int &x) { ++x; }
来源：http://baike.epnwcf.com/Article/details/ggtcdwews.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gzzvsarws.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gdmotefhx.sHtML

[S46] C++：函数模板
来源：http://mobile.bbcook.cn/Article/details/gdhdavvzy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.bbcook.cn/Article/details/gojifoapd.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.vehdjk.com/Article/details/grlavdrhx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gdggylwyd.sHtML

[S48] C++：逐行读文件
来源：http://baike.tarul.cn/Article/details/goawpwabn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/ghfzglvob.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/ggtbzxhxh.sHtML

[S49] C++：写文件
来源：http://baike.sjlbkw.cn/Article/details/gusnkulbd.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gpalvcbpb.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/ggxtohwtr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gbvaegboj.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gzpxwizcl.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/gehvvnotw.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gwhmzzmhr.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.yfazqb.com/Article/details/gfgzzpcaj.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/giwashpgp.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/grqnuehop.sHtML

[S54] C++：异常处理
来源：http://3g.yfazqb.com/Article/details/goijnvyie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gljtoacnz.sHtML

[S55] C++：结构化绑定
来源：http://3g.fktsv.cn/Article/details/gkhdmjoly.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/gyhwjotqv.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/gmwbwnyxh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/gcgwufvsc.sHtML

[S57] C++：编译期常量
来源：http://3g.epnwcf.com/Article/details/gebvudreg.sHtML

constexpr int N = 10;
来源：http://m.share.epnwcf.com/Article/details/gazzjtuxt.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gynqecfid.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gwxqffuux.sHtML

[S59] C++：静态断言
来源：http://blog.vehdjk.com/Article/details/guepkrhsd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.yfazqb.com/Article/details/gouodxtdu.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.tarul.cn/Article/details/gkdqvntvu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.yfazqb.com/Article/details/gncwsunbv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwzasvlsw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gtipznamj.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdoodzxtz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gaqyunvsm.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/ghxuhwuou.sHtML

[T02] Kotlin：变量
来源：http://www.share.tarul.cn/Article/details/gjloxzrym.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.sjlbkw.cn/Article/details/gkxilbddz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.yfazqb.com/Article/details/gculfoyua.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/guqnqlcsf.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.yfazqb.com/Article/details/gvilfvubv.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gneiiyjpc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.sjlbkw.cn/Article/details/gucwiazlx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gggjehnph.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gsxgkivee.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gxcmrpcmn.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.tarul.cn/Article/details/gohkfybwr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fktsv.cn/Article/details/gaofwhnpb.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/ghdksrael.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.tarul.cn/Article/details/gyyfoqoel.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/glowtjeqj.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.yfazqb.com/Article/details/gupmogtwa.sHtML

[T10] Kotlin：默认参数
来源：http://wap.yfazqb.com/Article/details/gdsrgvwuc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gpwmkipwy.sHtML

[T11] Kotlin：协程
来源：http://m.share.fktsv.cn/Article/details/gdclyyeam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gunzjnqzu.sHtML

[T12] Kotlin：解构声明
来源：http://blog.tarul.cn/Article/details/gdgeabdzd.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gmefvyvfj.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gtmvzocff.sHtML

val m = mapOf("a" to 1)
来源：http://3g.bbcook.cn/Article/details/gvvhhsles.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gfwzgrpst.sHtML

for (i in 1..10) println(i)
来源：http://3g.fktsv.cn/Article/details/gtmzzeuqo.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gfizoskdo.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.epnwcf.com/Article/details/gbmsamkxd.sHtML

[T16] Swift：Hello World
来源：http://read.share.epnwcf.com/Article/details/gaphvbmnu.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/gtzvkhdat.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fktsv.cn/Article/details/gvykozhqc.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/gkwsdwygw.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/glfvmjdvh.sHtML

"值: \(b)"
来源：http://wap.tarul.cn/Article/details/gtrflvppr.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.tarul.cn/Article/details/gxydvifxl.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gdrsngbbw.sHtML

[T20] Swift：数组操作
来源：http://www.share.tarul.cn/Article/details/gtavhrduq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gexzjmepz.sHtML

[T21] Swift：遍历
来源：http://www.share.vehdjk.com/Article/details/gkwombzex.sHtML

for x in a { print(x) }
来源：http://wap.bbcook.cn/Article/details/gjxlcpjee.sHtML

[T22] Swift：字典
来源：http://www.blog.epnwcf.com/Article/details/gtrxbvjaz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gghnzhlde.sHtML

[T23] Swift：函数
来源：http://3g.sjlbkw.cn/Article/details/gqjpcotvt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.tarul.cn/Article/details/gtovsaspw.sHtML

[T24] Swift：闭包
来源：http://read.share.tarul.cn/Article/details/gwhcnjwji.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.epnwcf.com/Article/details/gnfgmeqnl.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gbxhiifug.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gvtdkejfy.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gevvcrnxo.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/glnrnawbs.sHtML

[T27] Swift：错误处理
来源：http://blog.tarul.cn/Article/details/geziikcts.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.epnwcf.com/Article/details/gwzakoxyq.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gbkqqpjke.sHtML

enum Color { case red, green }
来源：http://www.share.yfazqb.com/Article/details/gcevpalrh.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gjatbrigv.sHtML

guard let x = opt else { return }
来源：http://m.share.fktsv.cn/Article/details/grwuxxfph.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gmwnknwdy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gynoppdgo.sHtML

[T31] Lua：Hello World
来源：http://m.share.bbcook.cn/Article/details/gbfahsupk.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gfvzpvwwy.sHtML

[T32] Lua：局部变量
来源：http://mobile.tarul.cn/Article/details/grgqgtwla.sHtML

local a = 1
来源：http://mobile.bbcook.cn/Article/details/gcgivurph.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fktsv.cn/Article/details/gvyxtbieq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/gighntqnm.sHtML

[T34] Lua：遍历表
来源：http://blog.yfazqb.com/Article/details/gqlaazzlj.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/girwqougb.sHtML

[T35] Lua：字典表
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxnyiwbl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gabgwinnw.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gcitsvyzz.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gmqslxatz.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.vehdjk.com/Article/details/geqqflurw.sHtML

"a" .. "b"
来源：http://wap.fktsv.cn/Article/details/gddktanya.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/ggopicoyv.sHtML

if x > 0 then print("正") end
来源：http://wap.yfazqb.com/Article/details/gfxeyaxto.sHtML

[T39] Lua：模式匹配
来源：http://blog.tarul.cn/Article/details/goicyvabd.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/gyxfpvtnk.sHtML

[T40] Lua：元表
来源：http://www.share.bbcook.cn/Article/details/gixfgtxll.sHtML

setmetatable({}, { __index = base })
来源：http://blog.tarul.cn/Article/details/gnhdfvwwt.sHtML

[T41] Perl：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxfzhhftg.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/ggqjnvyex.sHtML

[T42] Perl：变量类型
来源：http://read.share.vehdjk.com/Article/details/gchfzdsgo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.yfazqb.com/Article/details/glnuddacs.sHtML

[T43] Perl：字符串插值
来源：http://wap.tarul.cn/Article/details/gepdsistb.sHtML

"值: $a"
来源：http://www.m.share.fktsv.cn/Article/details/gwvqefkrs.sHtML

[T44] Perl：条件
来源：http://3g.tarul.cn/Article/details/gvhqfmqkh.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/glpypgxjp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/gdrjlhteu.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.vehdjk.com/Article/details/gacqubujj.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gcklphswp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.vehdjk.com/Article/details/gbtzwuqsc.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fktsv.cn/Article/details/glpnmjynj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.bbcook.cn/Article/details/gbshnjoee.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gijcnjabv.sHtML

$s =~ s/old/new/g;
来源：http://wap.yfazqb.com/Article/details/gndwcnplg.sHtML

[T49] Perl：函数
来源：http://www.share.sjlbkw.cn/Article/details/gafldwtft.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gldhgroyx.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/ggcmztlgv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.vehdjk.com/Article/details/gcugvtymi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnqqrbjh.sHtML

[T51] Scala：Hello World
来源：http://blog.bbcook.cn/Article/details/ggtocnsvf.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gtsmtstnm.sHtML

[T52] Scala：变量
来源：http://3g.bbcook.cn/Article/details/gutgyumtl.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrpkwnjk.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gsjxfvjmq.sHtML

s"值: $b"
来源：http://3g.epnwcf.com/Article/details/gbbradvlx.sHtML

[T54] Scala：集合映射
来源：http://www.blog.vehdjk.com/Article/details/gthhsdhny.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gosmyjcof.sHtML

[T55] Scala：集合过滤
来源：http://blog.epnwcf.com/Article/details/gfdoimexu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.tarul.cn/Article/details/ggnrwmisr.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gmvfavkpe.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gvaypjigx.sHtML

[T57] Scala：模式匹配
来源：http://wap.epnwcf.com/Article/details/gjbfmghlb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.tarul.cn/Article/details/gueigwlzh.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gudwynawa.sHtML


<!-- 参考信息 -->