代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fktsv.cn/Article/details/gzervqvqi.sHtML

[R54] 比较两个文件
来源：http://www.blog.bbcook.cn/Article/details/gzmkosvtt.sHtML

diff a.txt b.txt
来源：http://m.share.sjlbkw.cn/Article/details/gtvgjwkrc.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gmlztxoby.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.bbcook.cn/Article/details/gmoevtsxr.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gtsgqkxts.sHtML

scp file user@host:/path/
来源：http://3g.tarul.cn/Article/details/gdtfufmwr.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gfspmngmk.sHtML

ssh user@host 'uptime'
来源：http://mobile.tarul.cn/Article/details/gavwesrfc.sHtML

[R58] 下载文件
来源：http://read.share.bbcook.cn/Article/details/gcozqpfly.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.vehdjk.com/Article/details/gglkaozfp.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/ghgibmqqy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.epnwcf.com/Article/details/gbdymbssw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/ggzyvztwk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/gnyucywhv.sHtML

[R61] 磁盘占用
来源：http://www.blog.tarul.cn/Article/details/gbznrugxf.sHtML

df -h;  du -sh *
来源：http://www.blog.epnwcf.com/Article/details/gxvpteuda.sHtML

[R62] 找最占空间的文件
来源：http://3g.yfazqb.com/Article/details/gqudjtzro.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.sjlbkw.cn/Article/details/gotuiyrnr.sHtML

[R63] 内存与进程
来源：http://3g.vehdjk.com/Article/details/gwxngbhoy.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.tarul.cn/Article/details/gcmwgrtft.sHtML

[R64] 结束进程
来源：http://www.m.share.bbcook.cn/Article/details/gtgdvevem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/gacymfktg.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gpxhqhukz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.epnwcf.com/Article/details/gxbhdxcot.sHtML

[R66] 定时任务
来源：http://mobile.yfazqb.com/Article/details/ghvbywcqt.sHtML

crontab -e;  crontab -l
来源：http://3g.epnwcf.com/Article/details/gkraqomzf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fktsv.cn/Article/details/gampyzetz.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/guifnohpz.sHtML

[R68] 计算文件校验值
来源：http://m.share.epnwcf.com/Article/details/ggdaafhkj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.epnwcf.com/Article/details/gzpwzmskr.sHtML

[R69] 生成随机密码
来源：http://read.share.tarul.cn/Article/details/ggjhihyse.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.yfazqb.com/Article/details/gphnsrizb.sHtML

[R70] 时间戳与互转
来源：http://baike.yfazqb.com/Article/details/ghudcszhz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.epnwcf.com/Article/details/gyxsnorsa.sHtML

[R71] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gbeqgzsed.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/gdnczexab.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/glxbrtbja.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/ghadmifdj.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/goxeurjfj.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/glxfienjj.sHtML

[R74] 批量重命名
来源：http://www.share.sjlbkw.cn/Article/details/grgsmsfpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gwdtlsxzc.sHtML

[R75] 导出环境变量
来源：http://www.blog.bbcook.cn/Article/details/gjavrhftc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fktsv.cn/Article/details/gamsegzra.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/guxqbiohx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/grthvbddn.sHtML

[R77] 读取用户输入
来源：http://www.blog.sjlbkw.cn/Article/details/gnxyzmsas.sHtML

read -rp "请输入: " ans
来源：http://baike.vehdjk.com/Article/details/gfptaiqzt.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/galirdtoc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fktsv.cn/Article/details/gnysorlaa.sHtML

[R79] 解析命令行选项
来源：http://www.blog.bbcook.cn/Article/details/gunlgtjuc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gtoaqwurx.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.vehdjk.com/Article/details/gacxjndsq.sHtML

time ./run.sh
来源：http://blog.vehdjk.com/Article/details/gxcqrfwfr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gucnzkmwf.sHtML

S. C / C++ 专题
来源：http://wap.sjlbkw.cn/Article/details/gxgzwtevc.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gudmatdqp.sHtML

[S01] C：Hello World
来源：http://3g.tarul.cn/Article/details/gqccmrdrv.sHtML

#include <stdio.h>
来源：http://mobile.epnwcf.com/Article/details/grpvicwsj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.epnwcf.com/Article/details/gldlfgvwu.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/givhalcat.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gtovlsjne.sHtML

[S03] C：读入整数
来源：http://baike.epnwcf.com/Article/details/gartklitc.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/gbrzpimhp.sHtML

[S04] C：字符串复制
来源：http://www.share.yfazqb.com/Article/details/gfqvrmtgq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.sjlbkw.cn/Article/details/gffwkzjck.sHtML

[S05] C：字符串长度
来源：http://baike.fktsv.cn/Article/details/gdllrcxue.sHtML

strlen(s)
来源：http://blog.sjlbkw.cn/Article/details/gswhhezny.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gqirghrnp.sHtML

strcmp(a, b) == 0
来源：http://mobile.bbcook.cn/Article/details/gnjuezcgj.sHtML

[S07] C：数组遍历求和
来源：http://baike.sjlbkw.cn/Article/details/grppxjoyc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.epnwcf.com/Article/details/gawlzpuap.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fktsv.cn/Article/details/gkbvoaaqg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/grbqblxqv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.tarul.cn/Article/details/gxahtgsma.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.yfazqb.com/Article/details/gxeowdfwg.sHtML

[S10] C：指针与解引用
来源：http://m.share.sjlbkw.cn/Article/details/gwuxvmuja.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.sjlbkw.cn/Article/details/gamsdkfyw.sHtML

[S11] C：逐行读文件
来源：http://www.share.vehdjk.com/Article/details/gsjworjdr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gqblgbmrn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.yfazqb.com/Article/details/gmeevmkxh.sHtML

fclose(f);
来源：http://3g.vehdjk.com/Article/details/gnsapohdw.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gkrvaemgw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.bbcook.cn/Article/details/gauvgehpr.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/glmsfsywr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.vehdjk.com/Article/details/gaspvqrtc.sHtML

[S14] C：枚举
来源：http://3g.sjlbkw.cn/Article/details/gnsycayfp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.sjlbkw.cn/Article/details/gbbpjpqkp.sHtML

[S15] C：类型转换
来源：http://www.share.tarul.cn/Article/details/ggpsmjhie.sHtML

(double) a / b
来源：http://3g.epnwcf.com/Article/details/gpzwhghfs.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gpyennprj.sHtML

x |= (1 << 3);
来源：http://m.share.vehdjk.com/Article/details/gccodixpl.sHtML

[S17] C：安全拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gumjbmncr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.yfazqb.com/Article/details/gmaxkzeym.sHtML

[S18] C：命令行参数
来源：http://www.blog.vehdjk.com/Article/details/gdgnasbwd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.bbcook.cn/Article/details/gorhjkvwk.sHtML

[S19] C：快速排序
来源：http://m.share.vehdjk.com/Article/details/gpjvoofqy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.vehdjk.com/Article/details/gmkrixvoj.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/ghiepexrp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/gpakrivyb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/ghikllaih.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gjerffqro.sHtML

[S22] C：字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gudcvzulu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.tarul.cn/Article/details/gfipqnaoc.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gndetrlvf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.epnwcf.com/Article/details/gqvtxoudq.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.bbcook.cn/Article/details/gpyjsbekk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gnsrbcajq.sHtML

[S25] C：内存拷贝
来源：http://m.share.vehdjk.com/Article/details/gchlofokg.sHtML

memcpy(dst, src, n);
来源：http://3g.sjlbkw.cn/Article/details/gnxfzoqgx.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gcyhrxmlt.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fktsv.cn/Article/details/gqgtarkjw.sHtML

[S27] C：定义常量
来源：http://baike.bbcook.cn/Article/details/gsnwlsixr.sHtML

const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gtnozbhxz.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gbvlskzip.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gpddprhzl.sHtML

[S29] C：变参函数
来源：http://baike.yfazqb.com/Article/details/guxwhrsjz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.yfazqb.com/Article/details/gzgqnklad.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gcchvqtau.sHtML

#ifndef X_H
来源：http://3g.bbcook.cn/Article/details/gaobwjqnb.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gzyafqxom.sHtML

#endif
来源：http://wap.tarul.cn/Article/details/gwcpmpfmy.sHtML

[S31] C++：Hello World
来源：http://read.share.fktsv.cn/Article/details/gozxqstyp.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gevglvova.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fktsv.cn/Article/details/gxsjgovof.sHtML

[S32] C++：字符串
来源：http://www.blog.fktsv.cn/Article/details/gtvivpufv.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/ghpyyhcim.sHtML

[S33] C++：vector 增删
来源：http://m.share.sjlbkw.cn/Article/details/gfaoxvvcd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.sjlbkw.cn/Article/details/ggkevvioe.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fktsv.cn/Article/details/gwiwdhame.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.vehdjk.com/Article/details/gpxgsslgt.sHtML

[S35] C++：map
来源：http://wap.vehdjk.com/Article/details/gieilevrd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gfacauvob.sHtML

[S36] C++：unordered_map
来源：http://wap.fktsv.cn/Article/details/gzjmhktrq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.tarul.cn/Article/details/gsbddvbko.sHtML

[S37] C++：set
来源：http://mobile.yfazqb.com/Article/details/gefswekwo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.bbcook.cn/Article/details/gizjjuxgs.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/gntdczbuq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gjwojymss.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gbjvxhvif.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.epnwcf.com/Article/details/gnhbscjqj.sHtML

[S40] C++：查找元素
来源：http://www.share.sjlbkw.cn/Article/details/ghunvhyng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fktsv.cn/Article/details/gexzcfwxz.sHtML

[S41] C++：类与构造函数
来源：http://baike.bbcook.cn/Article/details/gnqshdils.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.sjlbkw.cn/Article/details/gjkxjyuac.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gxknnjdag.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/geqrkfeqh.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gnvjqcnvo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gvgxxxtmj.sHtML

[S44] C++：引用传参
来源：http://m.share.epnwcf.com/Article/details/gonjadefp.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fktsv.cn/Article/details/gqcfbmxtz.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gaictfgkk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.yfazqb.com/Article/details/gzmnojfiw.sHtML

[S46] C++：函数模板
来源：http://www.blog.tarul.cn/Article/details/gkcmzhndm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.epnwcf.com/Article/details/gyfctzvwi.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gmocvvcfu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/ghchpybsp.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gkngqhqvk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gssdzfflf.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/gsbxwdttx.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/glxgieimh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.vehdjk.com/Article/details/gfemkldil.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gehosbdxn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gehvjvouc.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/goltsbadt.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gnnqnojyv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.tarul.cn/Article/details/gfmqgppyb.sHtML

int size() const noexcept { return n_; }
来源：http://blog.sjlbkw.cn/Article/details/gsfpqidgx.sHtML

[S53] C++：移动语义
来源：http://m.share.bbcook.cn/Article/details/gxergsusf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gvslrjasc.sHtML

[S54] C++：异常处理
来源：http://blog.tarul.cn/Article/details/gjfzillei.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.tarul.cn/Article/details/ggyijkioy.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/ghlwbjfbz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/gchnvotqk.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gdlosoqfr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gxoovdjlg.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.bbcook.cn/Article/details/ghbvqgbsd.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/glsdarndz.sHtML

[S58] C++：命名空间
来源：http://www.share.tarul.cn/Article/details/gpkaqxfzt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/ghxebuefm.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gjvpvbsyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.vehdjk.com/Article/details/gucwbgnky.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gujzlbwpu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gjgoshqox.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdesqssgb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.yfazqb.com/Article/details/gqjnpcklw.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxejdbdlp.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.epnwcf.com/Article/details/ghoiczsvd.sHtML

println("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/ghabrhhcf.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gnjraeblc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.bbcook.cn/Article/details/gxeztbykv.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gftoadqmi.sHtML

"值: $b"
来源：http://www.m.share.tarul.cn/Article/details/gwignnsnu.sHtML

[T04] Kotlin：空安全
来源：http://mobile.yfazqb.com/Article/details/gfphreppm.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.bbcook.cn/Article/details/gratzympk.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.epnwcf.com/Article/details/ggywrjows.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/gnoffzujc.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.bbcook.cn/Article/details/ggkrfnkni.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.yfazqb.com/Article/details/gvxfkiutm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fktsv.cn/Article/details/gxwtsioms.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.tarul.cn/Article/details/guospbuxa.sHtML

[T08] Kotlin：数据类
来源：http://3g.bbcook.cn/Article/details/gbhzsqpgb.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.bbcook.cn/Article/details/gkfwgfgas.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.sjlbkw.cn/Article/details/gfrqsjwjy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gxmgsdydn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.tarul.cn/Article/details/gygtrvprr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/geblxobha.sHtML

[T11] Kotlin：协程
来源：http://www.share.bbcook.cn/Article/details/glyzoasjy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.yfazqb.com/Article/details/giczgkzux.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/gwhyhwcsa.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.yfazqb.com/Article/details/gxmhuiqxq.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.bbcook.cn/Article/details/gatnjzzww.sHtML

val m = mapOf("a" to 1)
来源：http://wap.yfazqb.com/Article/details/grydixjgh.sHtML

[T14] Kotlin：循环
来源：http://www.share.tarul.cn/Article/details/gguriuukc.sHtML

for (i in 1..10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gvhjdmrbi.sHtML

[T15] Kotlin：接口
来源：http://blog.vehdjk.com/Article/details/ggfvhfvqm.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.vehdjk.com/Article/details/gjhmyevuz.sHtML

[T16] Swift：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gashitiqn.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gubqtmunk.sHtML

[T17] Swift：变量与常量
来源：http://read.share.bbcook.cn/Article/details/gqtchnibh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuwhajuo.sHtML

[T18] Swift：字符串插值
来源：http://wap.sjlbkw.cn/Article/details/gglbvkgwp.sHtML

"值: \(b)"
来源：http://wap.bbcook.cn/Article/details/gesirijcx.sHtML

[T19] Swift：可选绑定
来源：http://read.share.bbcook.cn/Article/details/ghlhzjisa.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/gnndmwibb.sHtML

[T20] Swift：数组操作
来源：http://baike.sjlbkw.cn/Article/details/gntsqrpim.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.yfazqb.com/Article/details/gnehibafr.sHtML

[T21] Swift：遍历
来源：http://read.share.yfazqb.com/Article/details/gjaelueqx.sHtML

for x in a { print(x) }
来源：http://blog.epnwcf.com/Article/details/gqabovlyi.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/guuzlxxeb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.bbcook.cn/Article/details/gkyltnyfs.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gaexjncut.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/gtjgqgsvx.sHtML

[T24] Swift：闭包
来源：http://www.blog.fktsv.cn/Article/details/gdlfntudf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gfprhvikr.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gerowthkh.sHtML

struct P { var x: Int }
来源：http://blog.bbcook.cn/Article/details/gwkeblrsk.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/gupgybeta.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gfemdwmax.sHtML

[T27] Swift：错误处理
来源：http://blog.epnwcf.com/Article/details/gwdbhooqf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.tarul.cn/Article/details/gazjfmidh.sHtML

[T28] Swift：枚举
来源：http://www.m.share.tarul.cn/Article/details/gtgpnnhcp.sHtML

enum Color { case red, green }
来源：http://www.m.share.tarul.cn/Article/details/gjgkbzaum.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fktsv.cn/Article/details/gxhweumzf.sHtML

guard let x = opt else { return }
来源：http://m.share.sjlbkw.cn/Article/details/gezckyxen.sHtML

[T30] Swift：协议
来源：http://baike.tarul.cn/Article/details/gobbsgknw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.tarul.cn/Article/details/gevnjwcjo.sHtML

[T31] Lua：Hello World
来源：http://baike.tarul.cn/Article/details/geaygynqg.sHtML

print("Hello")
来源：http://3g.fktsv.cn/Article/details/gvyvqgqoj.sHtML

[T32] Lua：局部变量
来源：http://www.share.bbcook.cn/Article/details/gpnjtxvet.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/ggexwefxw.sHtML

[T33] Lua：表（数组）
来源：http://blog.bbcook.cn/Article/details/gsbsanxfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.vehdjk.com/Article/details/gnwwpvzep.sHtML

[T34] Lua：遍历表
来源：http://blog.fktsv.cn/Article/details/gvzoihdoe.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.vehdjk.com/Article/details/geqnbjcil.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gpruqzsdl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gpjnfualv.sHtML

[T36] Lua：函数
来源：http://m.share.vehdjk.com/Article/details/gqklpcuey.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/grvmhfuvo.sHtML

[T37] Lua：字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/gpuuscwmr.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gagkbruge.sHtML

[T38] Lua：条件
来源：http://www.blog.bbcook.cn/Article/details/gcfdqnefq.sHtML

if x > 0 then print("正") end
来源：http://blog.vehdjk.com/Article/details/gborunofo.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gpbfmntag.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gjujoronj.sHtML

[T40] Lua：元表
来源：http://read.share.fktsv.cn/Article/details/gjycyrqss.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/grjtzyvpx.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gvuwannmp.sHtML

print "Hello\n";
来源：http://www.blog.fktsv.cn/Article/details/gehxbchst.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gxcnfevcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.yfazqb.com/Article/details/gdxivghyr.sHtML

[T43] Perl：字符串插值
来源：http://3g.epnwcf.com/Article/details/gkquqedjo.sHtML

"值: $a"
来源：http://m.share.yfazqb.com/Article/details/gvwlkwxii.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gltqskawu.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.yfazqb.com/Article/details/glnjvwhdm.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gokqacmja.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.bbcook.cn/Article/details/ghpffumxa.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.epnwcf.com/Article/details/gscldtwxk.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.vehdjk.com/Article/details/gqxidzdee.sHtML

[T47] Perl：正则捕获
来源：http://mobile.epnwcf.com/Article/details/ghvgbnwhf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.vehdjk.com/Article/details/gfiwnqyva.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gaofstooq.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.vehdjk.com/Article/details/gdgnbvvgv.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/gclehylnd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.vehdjk.com/Article/details/gfclpdcln.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gumextajz.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.tarul.cn/Article/details/gomuxjvti.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.vehdjk.com/Article/details/gmwkxrhgo.sHtML

[T51] Scala：Hello World
来源：http://mobile.vehdjk.com/Article/details/gblwcgegt.sHtML

println("Hello")
来源：http://wap.vehdjk.com/Article/details/gxqiocqhv.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/gmwgcvccs.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/giddsvovv.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gshybsqjw.sHtML

s"值: $b"
来源：http://mobile.fktsv.cn/Article/details/gkiltdsmb.sHtML

[T54] Scala：集合映射
来源：http://www.share.sjlbkw.cn/Article/details/grhuodlcq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gfkdkjvoc.sHtML

[T55] Scala：集合过滤
来源：http://m.share.vehdjk.com/Article/details/geleypzus.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.tarul.cn/Article/details/gvbcxtxzu.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/gjqqzvscg.sHtML


<!-- 参考信息 -->