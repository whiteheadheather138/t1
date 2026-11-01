代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/gqqyvefyq.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/guhbympbr.sHtML

wc -l a.txt
来源：http://wap.yfazqb.com/Article/details/gduihaufu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.yfazqb.com/Article/details/gwwjlseuv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.bbcook.cn/Article/details/gpjbesxcn.sHtML

[R54] 比较两个文件
来源：http://read.share.fktsv.cn/Article/details/gnbtobhnv.sHtML

diff a.txt b.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gcnghhhut.sHtML

[R55] 压缩与解压
来源：http://wap.vehdjk.com/Article/details/gkfkraouv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.sjlbkw.cn/Article/details/gospfoljk.sHtML

[R56] 远程拷贝
来源：http://baike.sjlbkw.cn/Article/details/gdhpokakz.sHtML

scp file user@host:/path/
来源：http://m.share.sjlbkw.cn/Article/details/gcnzrgvld.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/gllynrfin.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gjfxqqtvb.sHtML

[R58] 下载文件
来源：http://wap.vehdjk.com/Article/details/gxplwixow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/geldpjiiu.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbnwtzelj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.bbcook.cn/Article/details/ghdydrvfr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gakvtxprx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.bbcook.cn/Article/details/gznstgaix.sHtML

[R61] 磁盘占用
来源：http://blog.vehdjk.com/Article/details/gjwlcmedq.sHtML

df -h;  du -sh *
来源：http://www.share.bbcook.cn/Article/details/gwyhuhtyu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gldrsgifs.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/gbhvhzmgj.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/ggwdxciuh.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.vehdjk.com/Article/details/gulcbsddm.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gjrzamoxx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.epnwcf.com/Article/details/gbpejhetg.sHtML

[R65] 查看端口占用
来源：http://m.share.tarul.cn/Article/details/gfzrnopoi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.sjlbkw.cn/Article/details/grfmfdrhv.sHtML

[R66] 定时任务
来源：http://3g.sjlbkw.cn/Article/details/gkdnjejhm.sHtML

crontab -e;  crontab -l
来源：http://3g.yfazqb.com/Article/details/gyinhzuog.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gejkqebdu.sHtML

openssl rand -hex 16
来源：http://read.share.bbcook.cn/Article/details/gwivguvhx.sHtML

[R68] 计算文件校验值
来源：http://mobile.bbcook.cn/Article/details/gwdjmsxwu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gltiezrom.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gblqoraes.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.tarul.cn/Article/details/gbgeakntg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/gigtdkfjs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.sjlbkw.cn/Article/details/gnujcrvkm.sHtML

[R71] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gkjzifusr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fktsv.cn/Article/details/gsrbwgrkq.sHtML

[R72] 等待端口就绪
来源：http://m.share.yfazqb.com/Article/details/gmsirnykh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gexpdcsds.sHtML

[R73] 分割大日志
来源：http://read.share.sjlbkw.cn/Article/details/gewfyzgcb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/garcppwwq.sHtML

[R74] 批量重命名
来源：http://www.m.share.vehdjk.com/Article/details/ggbwvgqnw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gpybmduiw.sHtML

[R75] 导出环境变量
来源：http://wap.epnwcf.com/Article/details/gxolmsjqu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/gedjlrovg.sHtML

[R76] 使用临时文件
来源：http://www.share.tarul.cn/Article/details/gcvgothzf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gfgnbydox.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/glpplhury.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/gpaqwxxmx.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/ggzhlhmqd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.vehdjk.com/Article/details/gvjrvsrfh.sHtML

[R79] 解析命令行选项
来源：http://www.share.epnwcf.com/Article/details/gpympqsym.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.bbcook.cn/Article/details/gdkzyzyca.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/ggvmvtirh.sHtML

time ./run.sh
来源：http://m.share.fktsv.cn/Article/details/gdiyjwekr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqrhjcbls.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gjeurxrlh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsijvjhmh.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/gketaysos.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gndydrddo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.vehdjk.com/Article/details/gvlmyicxk.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/guuviovup.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.tarul.cn/Article/details/gmvwoggdf.sHtML

[S03] C：读入整数
来源：http://wap.tarul.cn/Article/details/gnjnloqgx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.yfazqb.com/Article/details/gbuwvkpmm.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/goklmgdbf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.tarul.cn/Article/details/glfpqnayk.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gzvnfbhwa.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/gripsahep.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gifzbfymk.sHtML

strcmp(a, b) == 0
来源：http://wap.tarul.cn/Article/details/gzoasfxdy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/gcmtagkki.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fktsv.cn/Article/details/gogucblpt.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.vehdjk.com/Article/details/gumxmtwrq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/glvtejvqv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.epnwcf.com/Article/details/ggbmznzju.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.bbcook.cn/Article/details/goxgoeplh.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gzhteupki.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.epnwcf.com/Article/details/gebjnepyb.sHtML

[S11] C：逐行读文件
来源：http://3g.fktsv.cn/Article/details/gitxarspz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.vehdjk.com/Article/details/gtzrfyqjg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/gdcrixqjv.sHtML

fclose(f);
来源：http://baike.epnwcf.com/Article/details/gwuzkfrcz.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gymjbwuxn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.epnwcf.com/Article/details/gpldvkkyr.sHtML

[S13] C：宏定义
来源：http://www.share.epnwcf.com/Article/details/gfuptjnfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.bbcook.cn/Article/details/grifkciej.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gnykqkaoz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.vehdjk.com/Article/details/gwxuzqyai.sHtML

[S15] C：类型转换
来源：http://m.share.vehdjk.com/Article/details/gzihynfpl.sHtML

(double) a / b
来源：http://blog.fktsv.cn/Article/details/gbbulwymk.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gswdfnpua.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gkiseqjgw.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gqkguubcs.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/ghenufaoj.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/gpadkuixs.sHtML

int main(int argc, char **argv)
来源：http://3g.tarul.cn/Article/details/gbipuignf.sHtML

[S19] C：快速排序
来源：http://m.share.tarul.cn/Article/details/gakzcuckv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.bbcook.cn/Article/details/gdhkbumbd.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gnjyjqedc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/gfbesprwv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/glhiuppkh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.sjlbkw.cn/Article/details/gyzviokxo.sHtML

[S22] C：字符串转数字
来源：http://wap.yfazqb.com/Article/details/gqmisvvkx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gkivwtfeo.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhdphubu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fktsv.cn/Article/details/gimudaoza.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.tarul.cn/Article/details/gxdlalwtj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.sjlbkw.cn/Article/details/gnzjtxsoi.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gxntzesda.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gouufkeev.sHtML

[S26] C：内存清零
来源：http://wap.vehdjk.com/Article/details/ggvvhtqeu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gpvnxnntw.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gehxlyvmf.sHtML

const double PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gtrybmtdc.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/gqpqtypvy.sHtML

static int counter = 0;
来源：http://wap.tarul.cn/Article/details/goxqnsgmb.sHtML

[S29] C：变参函数
来源：http://www.share.sjlbkw.cn/Article/details/gwlfmanrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.sjlbkw.cn/Article/details/gwagnbbav.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gzvttodnk.sHtML

#ifndef X_H
来源：http://baike.bbcook.cn/Article/details/gftdyvpci.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/gjpomcvrr.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gzrnqwzfd.sHtML

[S31] C++：Hello World
来源：http://read.share.epnwcf.com/Article/details/gpbhsuepq.sHtML

#include <iostream>
来源：http://www.blog.tarul.cn/Article/details/gyhrmdsgg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gydxdtpnz.sHtML

[S32] C++：字符串
来源：http://www.share.sjlbkw.cn/Article/details/gzkuavtug.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.epnwcf.com/Article/details/ggkgazrhj.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsfpndxa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.sjlbkw.cn/Article/details/golpmwwgh.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/grzijbvfn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.epnwcf.com/Article/details/guhcsivga.sHtML

[S35] C++：map
来源：http://read.share.sjlbkw.cn/Article/details/gnasjbgpp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gntjxytor.sHtML

[S36] C++：unordered_map
来源：http://wap.bbcook.cn/Article/details/gozastkry.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gynvogbdx.sHtML

[S37] C++：set
来源：http://read.share.sjlbkw.cn/Article/details/gmywpthjo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gxukjrilb.sHtML

[S38] C++：排序
来源：http://read.share.epnwcf.com/Article/details/gowmdvjxi.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.yfazqb.com/Article/details/gevmleiyg.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.yfazqb.com/Article/details/gsoqmgcty.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.vehdjk.com/Article/details/gpougepsw.sHtML

[S40] C++：查找元素
来源：http://wap.vehdjk.com/Article/details/gziiuxpus.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gyjudluzh.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/goukfhqjx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gctklrzde.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fktsv.cn/Article/details/glxeyrnch.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.vehdjk.com/Article/details/gzrwpyjqd.sHtML

[S43] C++：智能指针
来源：http://m.share.tarul.cn/Article/details/gaqgdppjo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.vehdjk.com/Article/details/gonotfvtr.sHtML

[S44] C++：引用传参
来源：http://blog.vehdjk.com/Article/details/grtaqhqwf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.sjlbkw.cn/Article/details/ghaopovgg.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/ghrzvfduz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gilmyzbxo.sHtML

[S46] C++：函数模板
来源：http://www.blog.bbcook.cn/Article/details/gqitpdhqd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.bbcook.cn/Article/details/gmzoqcenx.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.bbcook.cn/Article/details/gfjdhyscy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gxgylepce.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gklasbvjd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gjayllgte.sHtML

while (std::getline(in, line)) { }
来源：http://wap.epnwcf.com/Article/details/gnypulwnv.sHtML

[S49] C++：写文件
来源：http://m.share.sjlbkw.cn/Article/details/gxsbjdzgw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/giucordtu.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fktsv.cn/Article/details/gpettgvdr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gwjnbcgba.sHtML

[S51] C++：显式类型转换
来源：http://baike.tarul.cn/Article/details/ggediypml.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gbefplofb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.bbcook.cn/Article/details/gmsmzrbqk.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/gcmvdmtjp.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gkdjxgcpc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gllttlpwr.sHtML

[S54] C++：异常处理
来源：http://www.share.epnwcf.com/Article/details/gfxgihked.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.epnwcf.com/Article/details/gctyeczve.sHtML

[S55] C++：结构化绑定
来源：http://baike.bbcook.cn/Article/details/gddklvlft.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.vehdjk.com/Article/details/gplvvcznv.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/gklfvknma.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/gdggtcfbj.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gfyqvuofd.sHtML

constexpr int N = 10;
来源：http://wap.bbcook.cn/Article/details/guukydtcm.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/glnbhoynt.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fktsv.cn/Article/details/gflsyhphr.sHtML

[S59] C++：静态断言
来源：http://3g.epnwcf.com/Article/details/gwxlvmcwr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gpziamvyf.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.tarul.cn/Article/details/gokgmyezg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.yfazqb.com/Article/details/gjikpevsu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/grxnnzxqj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gymewtxpc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzoyfnehl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gegydwplg.sHtML

println("Hello")
来源：http://wap.sjlbkw.cn/Article/details/gnhlouned.sHtML

[T02] Kotlin：变量
来源：http://m.share.bbcook.cn/Article/details/gwdtypqon.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.yfazqb.com/Article/details/gjgpbvvhy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.tarul.cn/Article/details/gdxrhxnfy.sHtML

"值: $b"
来源：http://blog.tarul.cn/Article/details/ghkzjpjgu.sHtML

[T04] Kotlin：空安全
来源：http://3g.yfazqb.com/Article/details/gcursmfri.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/gqqbxnthg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fktsv.cn/Article/details/ggincbccu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/giodwbpad.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.epnwcf.com/Article/details/gtscogodb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fktsv.cn/Article/details/gkczhsgod.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gcaikgdgz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/geabhpclw.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gocxxrqgi.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fktsv.cn/Article/details/gpkrlpfiz.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gnrzyrcra.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.bbcook.cn/Article/details/gzoovvsvc.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gfhbfheut.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.vehdjk.com/Article/details/ghzkxmjss.sHtML

[T11] Kotlin：协程
来源：http://blog.yfazqb.com/Article/details/gunjpcgue.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gaygoyjqm.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.yfazqb.com/Article/details/gunxlnnwj.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.tarul.cn/Article/details/grdfnpmmm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fktsv.cn/Article/details/gfloqpnek.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.tarul.cn/Article/details/graxmwsfa.sHtML

[T14] Kotlin：循环
来源：http://wap.fktsv.cn/Article/details/gfaftsqzq.sHtML

for (i in 1..10) println(i)
来源：http://blog.bbcook.cn/Article/details/guqyyhkhn.sHtML

[T15] Kotlin：接口
来源：http://mobile.vehdjk.com/Article/details/gtuykofem.sHtML

interface Shape { fun area(): Double }
来源：http://wap.vehdjk.com/Article/details/gzxtrrcrf.sHtML

[T16] Swift：Hello World
来源：http://3g.yfazqb.com/Article/details/gqotehnfl.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gnqicavxn.sHtML

[T17] Swift：变量与常量
来源：http://blog.bbcook.cn/Article/details/gubhxayil.sHtML

var a = 1;  let b = 2
来源：http://mobile.sjlbkw.cn/Article/details/gbxyotftk.sHtML

[T18] Swift：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gfusrpxaj.sHtML

"值: \(b)"
来源：http://blog.epnwcf.com/Article/details/geflkesnw.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gqeggpmto.sHtML

if let n = opt { print(n) }
来源：http://m.share.bbcook.cn/Article/details/gczywodll.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.epnwcf.com/Article/details/gkdfvjfuo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/grcsfcwsa.sHtML

[T21] Swift：遍历
来源：http://mobile.tarul.cn/Article/details/grwahxtyh.sHtML

for x in a { print(x) }
来源：http://baike.tarul.cn/Article/details/gyurgaxer.sHtML

[T22] Swift：字典
来源：http://m.share.bbcook.cn/Article/details/gwfvziuap.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.bbcook.cn/Article/details/goykfwyjy.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gknnbjggn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gxepdxakg.sHtML

[T24] Swift：闭包
来源：http://www.blog.bbcook.cn/Article/details/gafyoskcd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.bbcook.cn/Article/details/gofzqltso.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gicsfypzf.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gaigxqdkx.sHtML

[T26] Swift：类与重写
来源：http://baike.sjlbkw.cn/Article/details/gcdxgjwxc.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/ggsjiqamx.sHtML

[T27] Swift：错误处理
来源：http://www.share.bbcook.cn/Article/details/gjdsjolfx.sHtML

do { try f() } catch { print(error) }
来源：http://wap.yfazqb.com/Article/details/gsctqaxaj.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gfzyfdofz.sHtML

enum Color { case red, green }
来源：http://wap.bbcook.cn/Article/details/gogqvsvgp.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gdgrcyjjf.sHtML

guard let x = opt else { return }
来源：http://read.share.yfazqb.com/Article/details/gsclmyozl.sHtML

[T30] Swift：协议
来源：http://mobile.bbcook.cn/Article/details/gkvcgcloi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.vehdjk.com/Article/details/gocvjiqty.sHtML

[T31] Lua：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gxijkqzzl.sHtML

print("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gogjhaawx.sHtML

[T32] Lua：局部变量
来源：http://wap.bbcook.cn/Article/details/gtorafzkp.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/gpdskpafp.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gxzejyyka.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.yfazqb.com/Article/details/gjxpbajqi.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fktsv.cn/Article/details/gssrbdxvc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fktsv.cn/Article/details/gdqndoooo.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gnofrntjd.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.epnwcf.com/Article/details/gkbdobzpl.sHtML

[T36] Lua：函数
来源：http://3g.vehdjk.com/Article/details/gvzoptend.sHtML

function add(a, b) return a + b end
来源：http://www.blog.fktsv.cn/Article/details/grvdttzwj.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gyhqwxwjj.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gajcjdjrr.sHtML

[T38] Lua：条件
来源：http://baike.yfazqb.com/Article/details/gmwthgpuf.sHtML

if x > 0 then print("正") end
来源：http://baike.bbcook.cn/Article/details/glxrslkzl.sHtML

[T39] Lua：模式匹配
来源：http://baike.tarul.cn/Article/details/gikufpuzm.sHtML

string.find(s, "%d+")
来源：http://m.share.fktsv.cn/Article/details/gssrrehtt.sHtML

[T40] Lua：元表
来源：http://3g.vehdjk.com/Article/details/gugnronhn.sHtML

setmetatable({}, { __index = base })
来源：http://3g.fktsv.cn/Article/details/gfdhxuceo.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gzavpohki.sHtML

print "Hello\n";
来源：http://m.share.yfazqb.com/Article/details/giekiowlq.sHtML

[T42] Perl：变量类型
来源：http://baike.sjlbkw.cn/Article/details/glnlgxyxg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gttlzioqj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gomlokdqj.sHtML

"值: $a"
来源：http://baike.bbcook.cn/Article/details/gqxtekgfc.sHtML

[T44] Perl：条件
来源：http://blog.vehdjk.com/Article/details/gzcwxbspg.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.epnwcf.com/Article/details/gysrtenwr.sHtML

[T45] Perl：数组遍历
来源：http://3g.tarul.cn/Article/details/gbtrmyhvw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/grlobfmtt.sHtML

[T46] Perl：哈希操作
来源：http://m.share.epnwcf.com/Article/details/gwtcruwfa.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gumdohcwz.sHtML

[T47] Perl：正则捕获
来源：http://3g.vehdjk.com/Article/details/gnetstucl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.epnwcf.com/Article/details/geirxkzbr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/gqinwtxxl.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gzplxdwmn.sHtML

[T49] Perl：函数
来源：http://3g.vehdjk.com/Article/details/gmhfzuvcd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/gjrjwmhba.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gwukaqqfr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.yfazqb.com/Article/details/gmmevpono.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.tarul.cn/Article/details/gnozytrpz.sHtML

[T51] Scala：Hello World
来源：http://mobile.bbcook.cn/Article/details/gsxiaxwlv.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/gmaiwbzrm.sHtML

[T52] Scala：变量
来源：http://mobile.bbcook.cn/Article/details/gqwoknsmy.sHtML

val a = 1;  var b = 2
来源：http://read.share.yfazqb.com/Article/details/gqowtorcd.sHtML

[T53] Scala：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gdodjlijv.sHtML

s"值: $b"
来源：http://baike.epnwcf.com/Article/details/gjubpkbcc.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gyycgnufx.sHtML


<!-- 参考信息 -->