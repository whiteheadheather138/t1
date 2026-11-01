代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.vehdjk.com/Article/details/gdwomkrti.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/guildraqm.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gcwjykuht.sHtML

[R57] 远程执行命令
来源：http://read.share.fktsv.cn/Article/details/gcjscxnkd.sHtML

ssh user@host 'uptime'
来源：http://baike.bbcook.cn/Article/details/gafttioua.sHtML

[R58] 下载文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gevgcodah.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fktsv.cn/Article/details/gigvsufiw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fktsv.cn/Article/details/gggaadxve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.yfazqb.com/Article/details/ghwprymkl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gdavgewnl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/ghmtwxjhm.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gnhpsuxca.sHtML

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gjntlqqkz.sHtML

[R62] 找最占空间的文件
来源：http://blog.fktsv.cn/Article/details/gpmeerrsl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.yfazqb.com/Article/details/gvehqhyat.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/grjldbfsb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.tarul.cn/Article/details/gndjpppzg.sHtML

[R64] 结束进程
来源：http://blog.yfazqb.com/Article/details/ghyyyqasp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gwhwydvqj.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gikvwhigf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gebgdjnba.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/ggezkecyh.sHtML

crontab -e;  crontab -l
来源：http://read.share.tarul.cn/Article/details/ggbnceaqq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gsggkyrkp.sHtML

openssl rand -hex 16
来源：http://blog.tarul.cn/Article/details/gwhqutjuc.sHtML

[R68] 计算文件校验值
来源：http://m.share.tarul.cn/Article/details/gctwobkjj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.vehdjk.com/Article/details/guidrvcll.sHtML

[R69] 生成随机密码
来源：http://www.blog.yfazqb.com/Article/details/gzxvbzrqm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/gxofwuddy.sHtML

[R70] 时间戳与互转
来源：http://wap.tarul.cn/Article/details/guexrghaw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/gwrkcdgid.sHtML

[R71] 日期格式化
来源：http://baike.tarul.cn/Article/details/gjqhcrzxj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gfejdouki.sHtML

[R72] 等待端口就绪
来源：http://blog.bbcook.cn/Article/details/gupxpbutc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gupucdxxn.sHtML

[R73] 分割大日志
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbixlssj.sHtML

split -l 1000 big.log part_
来源：http://www.share.tarul.cn/Article/details/gnsyuptpr.sHtML

[R74] 批量重命名
来源：http://read.share.bbcook.cn/Article/details/gjnsvrwqv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/gbszdxnwf.sHtML

[R75] 导出环境变量
来源：http://wap.vehdjk.com/Article/details/gqpwcgpfr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fktsv.cn/Article/details/gjkjjwpxf.sHtML

[R76] 使用临时文件
来源：http://www.blog.fktsv.cn/Article/details/gafqziczf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fktsv.cn/Article/details/ggebdpimt.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/grbardfqs.sHtML

read -rp "请输入: " ans
来源：http://read.share.tarul.cn/Article/details/godvrrqkz.sHtML

[R78] 交互式菜单
来源：http://read.share.vehdjk.com/Article/details/gziqhjihv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.yfazqb.com/Article/details/gmnhpckco.sHtML

[R79] 解析命令行选项
来源：http://wap.vehdjk.com/Article/details/ggctrljhn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gwwhhmcny.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gjehcbiwf.sHtML

time ./run.sh
来源：http://www.share.vehdjk.com/Article/details/genekmmxu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/glxpslpya.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gchlfjjtj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gktdeggup.sHtML

[S01] C：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ggfugsija.sHtML

#include <stdio.h>
来源：http://m.share.epnwcf.com/Article/details/gfxyaxgmd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.sjlbkw.cn/Article/details/gwkilqvma.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.yfazqb.com/Article/details/gyvhquimz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gbzxbbkpi.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gklwbtpok.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gyyvyaxcw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.vehdjk.com/Article/details/gzxgokylm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gaxojvazx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gfggpokxb.sHtML

strlen(s)
来源：http://wap.fktsv.cn/Article/details/gepxesttl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgcsmckf.sHtML

strcmp(a, b) == 0
来源：http://m.share.bbcook.cn/Article/details/gbcdcwijv.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/germhuhxu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.bbcook.cn/Article/details/gpucjaxyt.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gclcksmcq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.vehdjk.com/Article/details/gxhwqxzkm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.vehdjk.com/Article/details/gydliiarm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.yfazqb.com/Article/details/gclsxwxnb.sHtML

[S10] C：指针与解引用
来源：http://3g.bbcook.cn/Article/details/gcmpgufbq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.vehdjk.com/Article/details/gyywxnorn.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/geeicelcd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gubcfbhjy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fktsv.cn/Article/details/gwjbvjpuk.sHtML

fclose(f);
来源：http://read.share.epnwcf.com/Article/details/ghddjyiuv.sHtML

[S12] C：写文件
来源：http://www.share.vehdjk.com/Article/details/gjedwdkei.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.vehdjk.com/Article/details/gtjmelcbb.sHtML

[S13] C：宏定义
来源：http://read.share.sjlbkw.cn/Article/details/gkzuhtivk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.epnwcf.com/Article/details/gstxrwrrc.sHtML

[S14] C：枚举
来源：http://www.blog.yfazqb.com/Article/details/gnqstddqo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/ggisyzjfz.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gppjcrsfv.sHtML

(double) a / b
来源：http://baike.tarul.cn/Article/details/gswvigpue.sHtML

[S16] C：位操作置位
来源：http://read.share.epnwcf.com/Article/details/gsyhiuiim.sHtML

x |= (1 << 3);
来源：http://3g.fktsv.cn/Article/details/ggywocniv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gnluekgmj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gdovnihmg.sHtML

[S18] C：命令行参数
来源：http://read.share.tarul.cn/Article/details/gjqeaslfu.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.epnwcf.com/Article/details/gvjcdxrgu.sHtML

[S19] C：快速排序
来源：http://www.share.epnwcf.com/Article/details/gppsjmcai.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/gehxdzduk.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gfhvtnboh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gemqqgqbu.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fktsv.cn/Article/details/gxohqnfef.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.epnwcf.com/Article/details/glzatlgvq.sHtML

[S22] C：字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gecxekazp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.vehdjk.com/Article/details/gsmbcexne.sHtML

[S23] C：随机数
来源：http://blog.tarul.cn/Article/details/gvanzksky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gwqgznlbs.sHtML

[S24] C：获取本地时间
来源：http://read.share.yfazqb.com/Article/details/guhjiiocn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gkkomuuno.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/guvjukgmw.sHtML

memcpy(dst, src, n);
来源：http://m.share.yfazqb.com/Article/details/gncwgsvlo.sHtML

[S26] C：内存清零
来源：http://mobile.vehdjk.com/Article/details/gckarsurz.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gpqjktonb.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gtlwraffr.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gykxxidfb.sHtML

[S28] C：静态变量
来源：http://m.share.tarul.cn/Article/details/gmnoemaal.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/gbkcwrbbj.sHtML

[S29] C：变参函数
来源：http://3g.bbcook.cn/Article/details/gdhvcuvcx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.epnwcf.com/Article/details/gbrekjnnw.sHtML

[S30] C：头文件保护
来源：http://mobile.bbcook.cn/Article/details/gjuwxufvs.sHtML

#ifndef X_H
来源：http://www.m.share.tarul.cn/Article/details/gqahwgzfr.sHtML

#define X_H
来源：http://baike.epnwcf.com/Article/details/gmbgthjdj.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gxxfoxakf.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gofzwnllh.sHtML

#include <iostream>
来源：http://blog.fktsv.cn/Article/details/gewkfeusm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gfcuorqkc.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gyahgnquu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.tarul.cn/Article/details/ggkbskmby.sHtML

[S33] C++：vector 增删
来源：http://mobile.vehdjk.com/Article/details/ggtbculmm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.bbcook.cn/Article/details/gshqxhwqf.sHtML

[S34] C++：遍历 vector
来源：http://www.share.epnwcf.com/Article/details/glyvxvnot.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/guocmdnir.sHtML

[S35] C++：map
来源：http://www.m.share.sjlbkw.cn/Article/details/gddmuxcdm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fktsv.cn/Article/details/gkvxkmako.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gklrrgumo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gfevcjqdy.sHtML

[S37] C++：set
来源：http://www.blog.yfazqb.com/Article/details/gwpaddtmm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/ggzfemsww.sHtML

[S38] C++：排序
来源：http://www.share.yfazqb.com/Article/details/guhmthxaa.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gjnngdmyy.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.tarul.cn/Article/details/geftxdneq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fktsv.cn/Article/details/genpvdydn.sHtML

[S40] C++：查找元素
来源：http://wap.epnwcf.com/Article/details/gcqkdksoe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.bbcook.cn/Article/details/gvksmtmmu.sHtML

[S41] C++：类与构造函数
来源：http://m.share.epnwcf.com/Article/details/glxhwciiv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.sjlbkw.cn/Article/details/gmbssmage.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gntjvtwud.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.yfazqb.com/Article/details/gewzrldnx.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/grxnambbg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmkoyrvl.sHtML

[S44] C++：引用传参
来源：http://www.blog.yfazqb.com/Article/details/gdceniiac.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/ghmwycncu.sHtML

[S45] C++：lambda
来源：http://m.share.sjlbkw.cn/Article/details/gwscgkvhg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/gnxeztymd.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gupqelqll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fktsv.cn/Article/details/geukcphru.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fktsv.cn/Article/details/gattlnowm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.tarul.cn/Article/details/gvrnbeeay.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/ghicxidrg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.yfazqb.com/Article/details/glfzzapot.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gtuwhwgui.sHtML

[S49] C++：写文件
来源：http://www.share.bbcook.cn/Article/details/gyxsnbkgs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.vehdjk.com/Article/details/gbppndrsu.sHtML

[S50] C++：格式化数字
来源：http://wap.yfazqb.com/Article/details/gqgnonbdt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/ghesgapfl.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gwpcwnkvh.sHtML

static_cast<double>(a) / b
来源：http://m.share.bbcook.cn/Article/details/ggifvydzj.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gujefmdvd.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gukkxgmpl.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/gjaazlvoj.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.sjlbkw.cn/Article/details/gvougavfq.sHtML

[S54] C++：异常处理
来源：http://read.share.fktsv.cn/Article/details/gtumfaflq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gqbdnrfiu.sHtML

[S55] C++：结构化绑定
来源：http://wap.yfazqb.com/Article/details/gyjbcwypk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gaplsgozs.sHtML

[S56] C++：optional
来源：http://www.share.sjlbkw.cn/Article/details/gpgzyklnv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gbgedxhob.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gvuquwgvo.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gwwfisyrn.sHtML

[S58] C++：命名空间
来源：http://baike.epnwcf.com/Article/details/gecnswapd.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.vehdjk.com/Article/details/gftwjgurh.sHtML

[S59] C++：静态断言
来源：http://3g.sjlbkw.cn/Article/details/gfrziksfk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.bbcook.cn/Article/details/gdbjnyyhg.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.epnwcf.com/Article/details/gegqmpwge.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fktsv.cn/Article/details/grvluwkss.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdliecqjh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjitbkfb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glyvhzrrw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gwvogjvzu.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/gvlazfypx.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gipecczuh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.vehdjk.com/Article/details/gqwqrpxez.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.tarul.cn/Article/details/gwpgztljg.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gbaagnaqv.sHtML

[T04] Kotlin：空安全
来源：http://wap.bbcook.cn/Article/details/gjlkzacbm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fktsv.cn/Article/details/gexfezutf.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.tarul.cn/Article/details/gzzojulqf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.sjlbkw.cn/Article/details/gffdsaunp.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.epnwcf.com/Article/details/gmqnmtwtt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.vehdjk.com/Article/details/gxebnkkkf.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.epnwcf.com/Article/details/gnosafhno.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.epnwcf.com/Article/details/gjymvpzyq.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/gcozalzpl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gufnbkwvi.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gkinsrexa.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.epnwcf.com/Article/details/gdlictmqs.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.bbcook.cn/Article/details/gkdotpiyv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.sjlbkw.cn/Article/details/gqcwagnyw.sHtML

[T11] Kotlin：协程
来源：http://www.blog.sjlbkw.cn/Article/details/gpjrwzste.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gfgchydsf.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/ggboipsig.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.bbcook.cn/Article/details/ghzwiyptn.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.tarul.cn/Article/details/gojtrblln.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/grwrpzumo.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/gznsptxur.sHtML

for (i in 1..10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gnlqrphoq.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.bbcook.cn/Article/details/gzggdtqiw.sHtML

interface Shape { fun area(): Double }
来源：http://wap.yfazqb.com/Article/details/gmadftldb.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.fktsv.cn/Article/details/gynfjrewr.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gkfoabrhr.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gmewscajp.sHtML

var a = 1;  let b = 2
来源：http://read.share.fktsv.cn/Article/details/ghhthqmgq.sHtML

[T18] Swift：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gukczycjf.sHtML

"值: \(b)"
来源：http://baike.fktsv.cn/Article/details/goomwqfum.sHtML

[T19] Swift：可选绑定
来源：http://mobile.yfazqb.com/Article/details/gwcrgmtdg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.epnwcf.com/Article/details/gchfyyaeh.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gtvepksvs.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/gimujwfeg.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/ghicgtltj.sHtML

for x in a { print(x) }
来源：http://baike.sjlbkw.cn/Article/details/gaoqdwpjt.sHtML

[T22] Swift：字典
来源：http://mobile.yfazqb.com/Article/details/gfvvrqzna.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/guyqjaqqi.sHtML

[T23] Swift：函数
来源：http://www.m.share.epnwcf.com/Article/details/gokvbjzhl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.yfazqb.com/Article/details/gvsqqymfr.sHtML

[T24] Swift：闭包
来源：http://blog.fktsv.cn/Article/details/gagyesbwl.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gjlqssnlm.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gaeaubgko.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/gnbqqlgvo.sHtML

[T26] Swift：类与重写
来源：http://blog.fktsv.cn/Article/details/glgksyalr.sHtML

class A: Base { override func f() {} }
来源：http://wap.sjlbkw.cn/Article/details/ghqjhawxt.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.bbcook.cn/Article/details/grwfmiirc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gruhvyibc.sHtML

[T28] Swift：枚举
来源：http://baike.bbcook.cn/Article/details/gifyrfdam.sHtML

enum Color { case red, green }
来源：http://www.share.epnwcf.com/Article/details/gttxwrxnd.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.sjlbkw.cn/Article/details/gwtptvmcr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fktsv.cn/Article/details/gwpgdwpuz.sHtML

[T30] Swift：协议
来源：http://read.share.epnwcf.com/Article/details/gbmmwonwc.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.yfazqb.com/Article/details/gpywrsonu.sHtML

[T31] Lua：Hello World
来源：http://baike.vehdjk.com/Article/details/gadwjuyti.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/gaenkqnbh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gobcqkbto.sHtML

local a = 1
来源：http://m.share.tarul.cn/Article/details/gremvhlgf.sHtML

[T33] Lua：表（数组）
来源：http://www.share.tarul.cn/Article/details/gzdedkqyd.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fktsv.cn/Article/details/gpbtyyynp.sHtML

[T34] Lua：遍历表
来源：http://read.share.epnwcf.com/Article/details/gfgtqednq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gutqsbfoe.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/gpemyxrpe.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.bbcook.cn/Article/details/glxshjsuo.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gbdxfnjbf.sHtML

function add(a, b) return a + b end
来源：http://baike.bbcook.cn/Article/details/gqmtkchbs.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.vehdjk.com/Article/details/gtgbticzz.sHtML

"a" .. "b"
来源：http://www.share.epnwcf.com/Article/details/gkayrypcz.sHtML

[T38] Lua：条件
来源：http://mobile.epnwcf.com/Article/details/gowhlbhde.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/ggjowlinm.sHtML

[T39] Lua：模式匹配
来源：http://mobile.tarul.cn/Article/details/gaowlmvki.sHtML

string.find(s, "%d+")
来源：http://www.share.bbcook.cn/Article/details/gjoxhpemu.sHtML

[T40] Lua：元表
来源：http://www.m.share.vehdjk.com/Article/details/gyfheenav.sHtML

setmetatable({}, { __index = base })
来源：http://wap.yfazqb.com/Article/details/gislitbfq.sHtML

[T41] Perl：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/geuyulbri.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gkfgbyhxj.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gldvzaxej.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.yfazqb.com/Article/details/gxbnqdsei.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gwlpjsamd.sHtML

"值: $a"
来源：http://www.m.share.vehdjk.com/Article/details/gfyzhoghh.sHtML

[T44] Perl：条件
来源：http://read.share.bbcook.cn/Article/details/gzfpyxntr.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.bbcook.cn/Article/details/gkqkbyrjt.sHtML

[T45] Perl：数组遍历
来源：http://mobile.epnwcf.com/Article/details/grdqtclzp.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.yfazqb.com/Article/details/ggddyvrjp.sHtML

[T46] Perl：哈希操作
来源：http://baike.bbcook.cn/Article/details/giohqwgni.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.tarul.cn/Article/details/goluzrdai.sHtML

[T47] Perl：正则捕获
来源：http://read.share.yfazqb.com/Article/details/gqeiujwma.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gckhxdyes.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gdoxxpjvi.sHtML

$s =~ s/old/new/g;
来源：http://baike.tarul.cn/Article/details/gyfhyogxr.sHtML

[T49] Perl：函数
来源：http://baike.tarul.cn/Article/details/gqvysbsyu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/ggfpjprna.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.bbcook.cn/Article/details/gfbmmszib.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.epnwcf.com/Article/details/giybmlcze.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/gfbziqoei.sHtML

[T51] Scala：Hello World
来源：http://blog.tarul.cn/Article/details/gtbztvevo.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gwiiczujd.sHtML

[T52] Scala：变量
来源：http://m.share.bbcook.cn/Article/details/gbgnfuocl.sHtML

val a = 1;  var b = 2
来源：http://3g.vehdjk.com/Article/details/ghdkiuqge.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gspvhnhzg.sHtML

s"值: $b"
来源：http://wap.bbcook.cn/Article/details/gtirodvzv.sHtML

[T54] Scala：集合映射
来源：http://read.share.epnwcf.com/Article/details/gsrwxfhql.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gglnawsre.sHtML

[T55] Scala：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/grkllesve.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fktsv.cn/Article/details/gdbgvgndz.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/gwhizftym.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gliribpky.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gzgizxlsf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fktsv.cn/Article/details/gbfogjeuj.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gynouzufa.sHtML


<!-- 参考信息 -->