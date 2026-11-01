代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.epnwcf.com/Article/details/gnkupcizd.sHtML

[R54] 比较两个文件
来源：http://www.share.vehdjk.com/Article/details/ggtbufbal.sHtML

diff a.txt b.txt
来源：http://mobile.yfazqb.com/Article/details/gjhbuvvgv.sHtML

[R55] 压缩与解压
来源：http://www.share.sjlbkw.cn/Article/details/gbcrgudyn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gknvljeet.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/ghnjkiosi.sHtML

scp file user@host:/path/
来源：http://blog.bbcook.cn/Article/details/gkrxlfgsw.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gvhrcrkqp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.vehdjk.com/Article/details/ggsyruhfv.sHtML

[R58] 下载文件
来源：http://www.share.tarul.cn/Article/details/gvyolqlpe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/gcsgskzzs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/goqwcqqeb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.vehdjk.com/Article/details/gqlldnwtu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.vehdjk.com/Article/details/gnbxwympd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.vehdjk.com/Article/details/gasolivqf.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/grmnupjim.sHtML

df -h;  du -sh *
来源：http://www.blog.vehdjk.com/Article/details/gzmascmeh.sHtML

[R62] 找最占空间的文件
来源：http://blog.yfazqb.com/Article/details/gtldxsisv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.vehdjk.com/Article/details/gniardhre.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gdojfefny.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gnidnudtk.sHtML

[R64] 结束进程
来源：http://read.share.vehdjk.com/Article/details/gxsckxhvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.bbcook.cn/Article/details/ggspkcjvc.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/gpihvxaez.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gezuzxaeb.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/glwpzurge.sHtML

crontab -e;  crontab -l
来源：http://blog.vehdjk.com/Article/details/gqbraisja.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gefmekxpb.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/gyaneqqho.sHtML

[R68] 计算文件校验值
来源：http://baike.sjlbkw.cn/Article/details/ggjhskees.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.tarul.cn/Article/details/ggizzckcy.sHtML

[R69] 生成随机密码
来源：http://m.share.fktsv.cn/Article/details/gcrytiobn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.epnwcf.com/Article/details/goiijkkal.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/gslgmtovf.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/gwxhzxvip.sHtML

[R71] 日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gcbycbqdh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.sjlbkw.cn/Article/details/goewspffs.sHtML

[R72] 等待端口就绪
来源：http://baike.epnwcf.com/Article/details/gqatncreb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/ginbbysjd.sHtML

[R73] 分割大日志
来源：http://blog.tarul.cn/Article/details/gnsihwqtf.sHtML

split -l 1000 big.log part_
来源：http://www.share.sjlbkw.cn/Article/details/gvocgloee.sHtML

[R74] 批量重命名
来源：http://www.blog.sjlbkw.cn/Article/details/gudqtbaql.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gumxzbrpy.sHtML

[R75] 导出环境变量
来源：http://3g.sjlbkw.cn/Article/details/gbhkxgvjg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gawwmpmut.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gqeosfiuw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gqwlxguiu.sHtML

[R77] 读取用户输入
来源：http://wap.epnwcf.com/Article/details/gliwjouee.sHtML

read -rp "请输入: " ans
来源：http://www.blog.sjlbkw.cn/Article/details/girjtjmpu.sHtML

[R78] 交互式菜单
来源：http://mobile.vehdjk.com/Article/details/gqdbbvfxc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.vehdjk.com/Article/details/gxrobfjfh.sHtML

[R79] 解析命令行选项
来源：http://mobile.bbcook.cn/Article/details/gkwkhinyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/geqxnhqhy.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gyfocuoio.sHtML

time ./run.sh
来源：http://m.share.epnwcf.com/Article/details/gfguozxrt.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gwnjhkvaa.sHtML

S. C / C++ 专题
来源：http://www.share.bbcook.cn/Article/details/gdgdnlfwg.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ghrmdqzwh.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/gzenuwnjx.sHtML

#include <stdio.h>
来源：http://www.blog.fktsv.cn/Article/details/gmoqyukyp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gklyalotn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.tarul.cn/Article/details/ghugjncnv.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/geotbhovm.sHtML

[S03] C：读入整数
来源：http://wap.yfazqb.com/Article/details/gvvchnkfu.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/grmzmnzjs.sHtML

[S04] C：字符串复制
来源：http://wap.epnwcf.com/Article/details/gpbhusmct.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.epnwcf.com/Article/details/gxidyqwkr.sHtML

[S05] C：字符串长度
来源：http://www.share.yfazqb.com/Article/details/gleedwopo.sHtML

strlen(s)
来源：http://www.blog.fktsv.cn/Article/details/gcsqzewiy.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gkfrkfain.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/gbhcpigfs.sHtML

[S07] C：数组遍历求和
来源：http://m.share.sjlbkw.cn/Article/details/gfqhgqvff.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.epnwcf.com/Article/details/gwxdecnua.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gypdvbvbp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gedculdhp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gycttwshz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.vehdjk.com/Article/details/gtfcbgfqo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.yfazqb.com/Article/details/gzdivjqzm.sHtML

int *p = &a;  *p = 5;
来源：http://blog.bbcook.cn/Article/details/gjqwgxeoh.sHtML

[S11] C：逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/gcesbgcqe.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.sjlbkw.cn/Article/details/gsjvwwsqx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/glgdqvvfm.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gdalptkoo.sHtML

[S12] C：写文件
来源：http://blog.epnwcf.com/Article/details/gmnbcigti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.vehdjk.com/Article/details/glahbwxxn.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/gylomztav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fktsv.cn/Article/details/gspgsouiw.sHtML

[S14] C：枚举
来源：http://www.m.share.bbcook.cn/Article/details/geczvmghy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.yfazqb.com/Article/details/gwzthtrmb.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gjnpsqypi.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gydjegabm.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/ghtwkcaat.sHtML

x |= (1 << 3);
来源：http://read.share.fktsv.cn/Article/details/gwjtybatg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.yfazqb.com/Article/details/gddxqlzns.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.vehdjk.com/Article/details/gdfduurlb.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/ghwmjikpa.sHtML

int main(int argc, char **argv)
来源：http://wap.vehdjk.com/Article/details/ghjtfmjha.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gsugytvpk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fktsv.cn/Article/details/goqhfudno.sHtML

[S20] C：二分查找
来源：http://www.blog.fktsv.cn/Article/details/gtrdhkfot.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/gitbjcyrv.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/gfisrksad.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/gdmbszjsq.sHtML

[S22] C：字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gahjzwoux.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.vehdjk.com/Article/details/gilpgnfyx.sHtML

[S23] C：随机数
来源：http://m.share.tarul.cn/Article/details/gaycawivq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.tarul.cn/Article/details/gekptfcig.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gzhkiukez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.yfazqb.com/Article/details/gyskuorul.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gtphqjgjr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrtmhasv.sHtML

[S26] C：内存清零
来源：http://read.share.bbcook.cn/Article/details/gddxtynmd.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.vehdjk.com/Article/details/glcrvgejh.sHtML

[S27] C：定义常量
来源：http://blog.sjlbkw.cn/Article/details/gnbmommtg.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gtxywufjw.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gongoayeq.sHtML

static int counter = 0;
来源：http://www.m.share.tarul.cn/Article/details/gpcdwyggx.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gfzsodceb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gvfkjshmv.sHtML

[S30] C：头文件保护
来源：http://3g.bbcook.cn/Article/details/gskwelumn.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gcxkvjklb.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gthtqyarj.sHtML

#endif
来源：http://read.share.bbcook.cn/Article/details/gcchtyqat.sHtML

[S31] C++：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/ggpllvhpn.sHtML

#include <iostream>
来源：http://www.m.share.tarul.cn/Article/details/gydrsykrt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.vehdjk.com/Article/details/gbzcczpqm.sHtML

[S32] C++：字符串
来源：http://baike.fktsv.cn/Article/details/guayrckft.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.vehdjk.com/Article/details/ghfdwauhz.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/gcaizixoy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.sjlbkw.cn/Article/details/gplwdzapt.sHtML

[S34] C++：遍历 vector
来源：http://wap.epnwcf.com/Article/details/gbplmqznp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.sjlbkw.cn/Article/details/gkfggvgrx.sHtML

[S35] C++：map
来源：http://www.blog.fktsv.cn/Article/details/gtknzggky.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gpvvpyeal.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/grnvqovbr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gqqwruerz.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gxywdwcyr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gcuahfpda.sHtML

[S38] C++：排序
来源：http://wap.bbcook.cn/Article/details/gvmsgmwah.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fktsv.cn/Article/details/gsdwfvgvy.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.epnwcf.com/Article/details/gpinyijil.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.yfazqb.com/Article/details/ginqpfzqi.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gouqwqzxh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.bbcook.cn/Article/details/gcipbtrir.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gouxfyexi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fktsv.cn/Article/details/gbgpcbwuc.sHtML

[S42] C++：继承与虚函数
来源：http://baike.vehdjk.com/Article/details/gcmrxgpag.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/goohxfann.sHtML

[S43] C++：智能指针
来源：http://mobile.tarul.cn/Article/details/gikkfjqlh.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/glhzdtlnx.sHtML

[S44] C++：引用传参
来源：http://wap.epnwcf.com/Article/details/ghrkgauis.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gaizqfxfo.sHtML

[S45] C++：lambda
来源：http://mobile.epnwcf.com/Article/details/ghwvqsdni.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fktsv.cn/Article/details/ghyhtdrgz.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gscsuqgqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.vehdjk.com/Article/details/glqjhhsie.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.tarul.cn/Article/details/gqkjaardr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/gkpxlfcmr.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gmzmcobyi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gostpozgw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.yfazqb.com/Article/details/gijpiyqkp.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gzaonmyka.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gbsjvhyst.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gkbnldteb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gasnqhtzp.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gxwsoqiiv.sHtML

static_cast<double>(a) / b
来源：http://www.share.fktsv.cn/Article/details/gxiucezcp.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gphoxcqfh.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gkuguldlc.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gezejovyl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fktsv.cn/Article/details/gybafwmyn.sHtML

[S54] C++：异常处理
来源：http://3g.tarul.cn/Article/details/gydsyqsfp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.vehdjk.com/Article/details/gwkrziwou.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/ghdtccxbw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.yfazqb.com/Article/details/gcfywajor.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gvxduzhza.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.bbcook.cn/Article/details/gxuajlzqk.sHtML

[S57] C++：编译期常量
来源：http://www.blog.sjlbkw.cn/Article/details/ghivmbjos.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gkgmaafoo.sHtML

[S58] C++：命名空间
来源：http://m.share.sjlbkw.cn/Article/details/gzsabupal.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.sjlbkw.cn/Article/details/gjggvosix.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/ggujprenp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.tarul.cn/Article/details/gcstiqmdo.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.vehdjk.com/Article/details/gfpiyirdn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.bbcook.cn/Article/details/gbjqgkmph.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gaqkkvcif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.tarul.cn/Article/details/gaotjgcxg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gcwlirpuj.sHtML

[T01] Kotlin：Hello World
来源：http://blog.yfazqb.com/Article/details/gcxkwyqog.sHtML

println("Hello")
来源：http://wap.epnwcf.com/Article/details/ghozzvbob.sHtML

[T02] Kotlin：变量
来源：http://read.share.fktsv.cn/Article/details/gepglzekh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.yfazqb.com/Article/details/gnudqgate.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fktsv.cn/Article/details/gjxnedptq.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gprzdxsuh.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gkwnuxwtc.sHtML

val n: String? = null;  n?.length
来源：http://wap.tarul.cn/Article/details/gpyfcaqpf.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gptxxoadv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.vehdjk.com/Article/details/gbeemzuql.sHtML

[T06] Kotlin：集合映射
来源：http://wap.vehdjk.com/Article/details/gpauyzcnc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/gegzzpooq.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.yfazqb.com/Article/details/gwjjqafxs.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gekkycuwt.sHtML

[T08] Kotlin：数据类
来源：http://baike.fktsv.cn/Article/details/gwmifmxcz.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.yfazqb.com/Article/details/gpqebonga.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.sjlbkw.cn/Article/details/gpwalkmbw.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gqlqpfncq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.sjlbkw.cn/Article/details/gplhevpyf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.vehdjk.com/Article/details/ggbkjvjsf.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gmejnuqtw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.vehdjk.com/Article/details/gwkpfwxfg.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gbljkvjyd.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fktsv.cn/Article/details/gbputogkg.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/ganvnhlpv.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gfodtrzty.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gnfzelapl.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gpbqbbbwm.sHtML

[T15] Kotlin：接口
来源：http://www.blog.epnwcf.com/Article/details/gqvifobru.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.tarul.cn/Article/details/gynlqnwbi.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gcghllnrg.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/giubclrdk.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.tarul.cn/Article/details/gupfyfpzv.sHtML

var a = 1;  let b = 2
来源：http://wap.tarul.cn/Article/details/gzkhpelvq.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gwmtgycyx.sHtML

"值: \(b)"
来源：http://wap.vehdjk.com/Article/details/gvsluamkk.sHtML

[T19] Swift：可选绑定
来源：http://www.share.yfazqb.com/Article/details/gapjjojcj.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.bbcook.cn/Article/details/grotawayi.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/gwuaaapay.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.bbcook.cn/Article/details/ghcykliau.sHtML

[T21] Swift：遍历
来源：http://www.share.bbcook.cn/Article/details/gleopmveg.sHtML

for x in a { print(x) }
来源：http://3g.tarul.cn/Article/details/gxlvornti.sHtML

[T22] Swift：字典
来源：http://wap.tarul.cn/Article/details/gdllkwnbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.tarul.cn/Article/details/gdomiyemq.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gglfyawyc.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fktsv.cn/Article/details/gdckhcpio.sHtML

[T24] Swift：闭包
来源：http://3g.epnwcf.com/Article/details/gubgphvct.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gzkueqaif.sHtML

[T25] Swift：结构体
来源：http://wap.yfazqb.com/Article/details/giqqlemtp.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gwbodxerl.sHtML

[T26] Swift：类与重写
来源：http://read.share.sjlbkw.cn/Article/details/gwmhqdgvr.sHtML

class A: Base { override func f() {} }
来源：http://3g.epnwcf.com/Article/details/gtduyiflt.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/gknfjlkqm.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gdfdbzaeb.sHtML

[T28] Swift：枚举
来源：http://blog.vehdjk.com/Article/details/galndbouw.sHtML

enum Color { case red, green }
来源：http://www.blog.bbcook.cn/Article/details/gjqritmiw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.vehdjk.com/Article/details/gddiohgzm.sHtML

guard let x = opt else { return }
来源：http://www.share.tarul.cn/Article/details/gqdcivvcw.sHtML

[T30] Swift：协议
来源：http://www.share.yfazqb.com/Article/details/gnguivjio.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gaidcvvti.sHtML

[T31] Lua：Hello World
来源：http://read.share.yfazqb.com/Article/details/grvhzccvp.sHtML

print("Hello")
来源：http://baike.tarul.cn/Article/details/gqegphuni.sHtML

[T32] Lua：局部变量
来源：http://3g.vehdjk.com/Article/details/giquqvrdw.sHtML

local a = 1
来源：http://www.m.share.yfazqb.com/Article/details/ggglctplb.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gckzwdcce.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.bbcook.cn/Article/details/ghnzrzbkt.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/gqjfxadnl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.vehdjk.com/Article/details/gpvxmdrhe.sHtML

[T35] Lua：字典表
来源：http://mobile.fktsv.cn/Article/details/ghngmmfpe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/gajegpxdw.sHtML

[T36] Lua：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpqvupnm.sHtML

function add(a, b) return a + b end
来源：http://blog.bbcook.cn/Article/details/gzhhacrhw.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/ghngyhuon.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gmldyrwqe.sHtML

[T38] Lua：条件
来源：http://blog.tarul.cn/Article/details/grxowvbjp.sHtML

if x > 0 then print("正") end
来源：http://3g.epnwcf.com/Article/details/gvxhikccs.sHtML

[T39] Lua：模式匹配
来源：http://blog.bbcook.cn/Article/details/gfrfbuzsr.sHtML

string.find(s, "%d+")
来源：http://mobile.epnwcf.com/Article/details/grkgyrpqi.sHtML

[T40] Lua：元表
来源：http://www.blog.tarul.cn/Article/details/gprcqnefz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.epnwcf.com/Article/details/ghmndoxvl.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gjvycswxr.sHtML

print "Hello\n";
来源：http://baike.epnwcf.com/Article/details/gbktnwsgd.sHtML

[T42] Perl：变量类型
来源：http://wap.sjlbkw.cn/Article/details/gmkmrwbvg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.vehdjk.com/Article/details/gzadbnxyg.sHtML

[T43] Perl：字符串插值
来源：http://3g.tarul.cn/Article/details/gvagjzrhc.sHtML

"值: $a"
来源：http://www.blog.bbcook.cn/Article/details/gzcvejdez.sHtML

[T44] Perl：条件
来源：http://www.m.share.yfazqb.com/Article/details/geztupxxu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.bbcook.cn/Article/details/gdzeebjqs.sHtML

[T45] Perl：数组遍历
来源：http://www.share.epnwcf.com/Article/details/gqxxixqpy.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.yfazqb.com/Article/details/giaytspnm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.bbcook.cn/Article/details/guxbwhsvr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.bbcook.cn/Article/details/ghgatxslj.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fktsv.cn/Article/details/gssqsmfbh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.blog.bbcook.cn/Article/details/gekhpryhp.sHtML

[T48] Perl：正则替换
来源：http://wap.fktsv.cn/Article/details/glkkmrogg.sHtML

$s =~ s/old/new/g;
来源：http://mobile.vehdjk.com/Article/details/gubeuojae.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/guzcalfob.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gtlfcqolx.sHtML

[T50] Perl：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gzugvofqt.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gdcteyjrl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.epnwcf.com/Article/details/ghwqndsid.sHtML

[T51] Scala：Hello World
来源：http://mobile.yfazqb.com/Article/details/gpwljyvii.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/gocqnxswp.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gahdnokox.sHtML

val a = 1;  var b = 2
来源：http://baike.yfazqb.com/Article/details/gkopntscq.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gtfmbzbnh.sHtML

s"值: $b"
来源：http://m.share.fktsv.cn/Article/details/gwfqyztfo.sHtML

[T54] Scala：集合映射
来源：http://mobile.fktsv.cn/Article/details/geihjztuo.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/grpyzdltm.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.bbcook.cn/Article/details/gqsjuvtne.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.bbcook.cn/Article/details/gktvppogy.sHtML

[T56] Scala：样例类
来源：http://wap.bbcook.cn/Article/details/gqmksrwbs.sHtML


<!-- 参考信息 -->