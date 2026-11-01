代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/gzgookmnt.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/ghjkfrynz.sHtML

scp file user@host:/path/
来源：http://wap.sjlbkw.cn/Article/details/gkhfptwbs.sHtML

[R57] 远程执行命令
来源：http://wap.bbcook.cn/Article/details/gaqommqfi.sHtML

ssh user@host 'uptime'
来源：http://3g.fktsv.cn/Article/details/ghopdrkcy.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gqircshnt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.yfazqb.com/Article/details/gxqbnrhlq.sHtML

[R59] 发 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gdhehjdee.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fktsv.cn/Article/details/gsnfpmoqx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gfhbcfauj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.sjlbkw.cn/Article/details/giqaeiibe.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/goilogrkb.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gxdqyiwwr.sHtML

[R62] 找最占空间的文件
来源：http://read.share.tarul.cn/Article/details/gogofwbyj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/giivhsgrt.sHtML

[R63] 内存与进程
来源：http://wap.bbcook.cn/Article/details/gveeplyoi.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.sjlbkw.cn/Article/details/gnrfdrnsv.sHtML

[R64] 结束进程
来源：http://www.share.yfazqb.com/Article/details/gicnagtrr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.yfazqb.com/Article/details/gwogrxdsk.sHtML

[R65] 查看端口占用
来源：http://read.share.vehdjk.com/Article/details/gjouqgepq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.epnwcf.com/Article/details/gcspfppqd.sHtML

[R66] 定时任务
来源：http://3g.fktsv.cn/Article/details/gofwqgxkp.sHtML

crontab -e;  crontab -l
来源：http://read.share.yfazqb.com/Article/details/gyitjmcpo.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gfnuhvoyw.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gillfjqjh.sHtML

[R68] 计算文件校验值
来源：http://www.share.epnwcf.com/Article/details/ghoixlbhm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.vehdjk.com/Article/details/gfvpxyqty.sHtML

[R69] 生成随机密码
来源：http://blog.epnwcf.com/Article/details/gwbnxqdvp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/ghzpeusms.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.epnwcf.com/Article/details/gturzodrn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.bbcook.cn/Article/details/gykiylrki.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gnglbxrjx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.bbcook.cn/Article/details/gkifppwkm.sHtML

[R72] 等待端口就绪
来源：http://read.share.bbcook.cn/Article/details/gapjysnce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gmhtessjt.sHtML

[R73] 分割大日志
来源：http://baike.vehdjk.com/Article/details/gvwbnzrlc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fktsv.cn/Article/details/gvcrisxhe.sHtML

[R74] 批量重命名
来源：http://wap.sjlbkw.cn/Article/details/ggotwwllh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gdkxxkoud.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/gqwoegbos.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.sjlbkw.cn/Article/details/gnafwikvw.sHtML

[R76] 使用临时文件
来源：http://read.share.vehdjk.com/Article/details/gfvirtafb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/grzprqcyn.sHtML

[R77] 读取用户输入
来源：http://www.blog.tarul.cn/Article/details/gjwryduqg.sHtML

read -rp "请输入: " ans
来源：http://m.share.vehdjk.com/Article/details/gkzwfbxjp.sHtML

[R78] 交互式菜单
来源：http://www.share.tarul.cn/Article/details/gbogemozl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.sjlbkw.cn/Article/details/gyweblqfm.sHtML

[R79] 解析命令行选项
来源：http://3g.fktsv.cn/Article/details/gzjpjkanv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.vehdjk.com/Article/details/gusyqfmmp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fktsv.cn/Article/details/gppfstgdo.sHtML

time ./run.sh
来源：http://www.m.share.sjlbkw.cn/Article/details/goqmpjadu.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gysscfdqf.sHtML

S. C / C++ 专题
来源：http://wap.yfazqb.com/Article/details/gekonhvun.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gnecyhbta.sHtML

[S01] C：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gnxdothci.sHtML

#include <stdio.h>
来源：http://wap.bbcook.cn/Article/details/glglqylss.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gsleqcbuo.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.vehdjk.com/Article/details/gatrbfzqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/ghpwdkgmf.sHtML

[S03] C：读入整数
来源：http://m.share.sjlbkw.cn/Article/details/getlgzmjc.sHtML

int x; scanf("%d", &x);
来源：http://www.share.epnwcf.com/Article/details/gnpqakeww.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gnbxtlnzi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.yfazqb.com/Article/details/gjhzzjpcm.sHtML

[S05] C：字符串长度
来源：http://mobile.tarul.cn/Article/details/gfgfgwmmd.sHtML

strlen(s)
来源：http://wap.sjlbkw.cn/Article/details/gramumurg.sHtML

[S06] C：字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/glohdilrz.sHtML

strcmp(a, b) == 0
来源：http://blog.tarul.cn/Article/details/gbjcbaakc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fktsv.cn/Article/details/gaowbntkh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fktsv.cn/Article/details/gucvhsuyb.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.sjlbkw.cn/Article/details/giblsgaug.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.sjlbkw.cn/Article/details/gfnkbpbsx.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.yfazqb.com/Article/details/gbvitroul.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.vehdjk.com/Article/details/grdrkiiux.sHtML

[S10] C：指针与解引用
来源：http://www.share.vehdjk.com/Article/details/gefdnejxz.sHtML

int *p = &a;  *p = 5;
来源：http://baike.bbcook.cn/Article/details/gkdwqsprl.sHtML

[S11] C：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gphhdrhdw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.tarul.cn/Article/details/gsraufprt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.epnwcf.com/Article/details/gjykpftiy.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gkjtadpir.sHtML

[S12] C：写文件
来源：http://3g.tarul.cn/Article/details/gqbknelyp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/giyhibdzt.sHtML

[S13] C：宏定义
来源：http://www.share.vehdjk.com/Article/details/gaeefilei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/ggxkpbfub.sHtML

[S14] C：枚举
来源：http://3g.tarul.cn/Article/details/gdkbyyovw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.yfazqb.com/Article/details/gkganrqkp.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gyqhugirm.sHtML

(double) a / b
来源：http://3g.fktsv.cn/Article/details/gwjpgfbwk.sHtML

[S16] C：位操作置位
来源：http://www.share.epnwcf.com/Article/details/gzggpxwvf.sHtML

x |= (1 << 3);
来源：http://m.share.fktsv.cn/Article/details/gftqzkdfs.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gxdwcvyvo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gkuapcnjj.sHtML

[S18] C：命令行参数
来源：http://3g.fktsv.cn/Article/details/gkkjubhcs.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/gtzvmdelk.sHtML

[S19] C：快速排序
来源：http://baike.yfazqb.com/Article/details/galyrcohu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gdovsxxte.sHtML

[S20] C：二分查找
来源：http://read.share.tarul.cn/Article/details/gfxeluaqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gbhaefqju.sHtML

[S21] C：字符类别判断
来源：http://www.blog.vehdjk.com/Article/details/ggzxvaibi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gclrbagxe.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.bbcook.cn/Article/details/gilonufje.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.tarul.cn/Article/details/glzgbauab.sHtML

[S23] C：随机数
来源：http://m.share.fktsv.cn/Article/details/gpmfwapnr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.epnwcf.com/Article/details/gxpgjjjhc.sHtML

[S24] C：获取本地时间
来源：http://baike.tarul.cn/Article/details/gjcfxbsuy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fktsv.cn/Article/details/gzzdiwryz.sHtML

[S25] C：内存拷贝
来源：http://3g.fktsv.cn/Article/details/grouzgwls.sHtML

memcpy(dst, src, n);
来源：http://blog.sjlbkw.cn/Article/details/gjltzogal.sHtML

[S26] C：内存清零
来源：http://www.share.tarul.cn/Article/details/gjvddsclg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/ghqpsdqqu.sHtML

[S27] C：定义常量
来源：http://www.m.share.yfazqb.com/Article/details/gndztjeyn.sHtML

const double PI = 3.14159;
来源：http://wap.fktsv.cn/Article/details/ggmthguyi.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/goornqesz.sHtML

static int counter = 0;
来源：http://baike.vehdjk.com/Article/details/gvqxzchbg.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/gzaqlnmet.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.vehdjk.com/Article/details/gbrqvordz.sHtML

[S30] C：头文件保护
来源：http://m.share.sjlbkw.cn/Article/details/gmjpzqyue.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gqcunpbgb.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gzzqhtvwq.sHtML

#endif
来源：http://wap.vehdjk.com/Article/details/gvilddpld.sHtML

[S31] C++：Hello World
来源：http://wap.tarul.cn/Article/details/gvofkwiun.sHtML

#include <iostream>
来源：http://3g.epnwcf.com/Article/details/gragfxrxw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gnrjrgrju.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gtjdntumk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.sjlbkw.cn/Article/details/goawovxns.sHtML

[S33] C++：vector 增删
来源：http://baike.yfazqb.com/Article/details/gpunokock.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/grokaybje.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gevekrdsh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/gzfilghmc.sHtML

[S35] C++：map
来源：http://www.blog.vehdjk.com/Article/details/gmciwetdh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmsliijy.sHtML

[S36] C++：unordered_map
来源：http://3g.bbcook.cn/Article/details/gbxrtfwtt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.bbcook.cn/Article/details/ghxozeuvh.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gbsgoktcy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gsfnqoenz.sHtML

[S38] C++：排序
来源：http://www.blog.vehdjk.com/Article/details/gpaqvymgt.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/gmoozbxhu.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.epnwcf.com/Article/details/gvkimxwsn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.bbcook.cn/Article/details/gjpajtajk.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gjyzntzqc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gogkqwuuu.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gsoufffdp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.epnwcf.com/Article/details/grarbmsuf.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.sjlbkw.cn/Article/details/grtriewty.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.epnwcf.com/Article/details/gmkyuwtbf.sHtML

[S43] C++：智能指针
来源：http://mobile.bbcook.cn/Article/details/gcygwwdsk.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gkerdodaw.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gkhiishul.sHtML

void inc(int &x) { ++x; }
来源：http://baike.tarul.cn/Article/details/gygakcrup.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gamomsmmx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.yfazqb.com/Article/details/gmjaiktwf.sHtML

[S46] C++：函数模板
来源：http://www.share.bbcook.cn/Article/details/gclarutgv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.bbcook.cn/Article/details/ghubttlnm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.yfazqb.com/Article/details/ghmmtxugz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fktsv.cn/Article/details/gcxpjidzn.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gtqtcjrnx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.bbcook.cn/Article/details/gkmshgreh.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpnuqswd.sHtML

[S49] C++：写文件
来源：http://baike.bbcook.cn/Article/details/gwugezcqb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gqodqjyuo.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/ggfzjhyos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fktsv.cn/Article/details/glrzyoflg.sHtML

[S51] C++：显式类型转换
来源：http://read.share.vehdjk.com/Article/details/gxecrfvff.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gfjrylqpt.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.sjlbkw.cn/Article/details/gtyjedvkt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.epnwcf.com/Article/details/gfxtpkemg.sHtML

[S53] C++：移动语义
来源：http://m.share.epnwcf.com/Article/details/gwfppzxgq.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gkzdrcilh.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/gkatktetr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.yfazqb.com/Article/details/ghhilxxwr.sHtML

[S55] C++：结构化绑定
来源：http://blog.bbcook.cn/Article/details/gjihccozk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gpagpagtv.sHtML

[S56] C++：optional
来源：http://read.share.sjlbkw.cn/Article/details/gfvnmgihn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fktsv.cn/Article/details/gaeoculas.sHtML

[S57] C++：编译期常量
来源：http://www.blog.yfazqb.com/Article/details/gwxxvxkbx.sHtML

constexpr int N = 10;
来源：http://www.share.fktsv.cn/Article/details/gjkigyywh.sHtML

[S58] C++：命名空间
来源：http://m.share.fktsv.cn/Article/details/gjwmfehzg.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.bbcook.cn/Article/details/gmiznmzgs.sHtML

[S59] C++：静态断言
来源：http://blog.bbcook.cn/Article/details/gqkemhdnh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fktsv.cn/Article/details/gamgxozwi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.epnwcf.com/Article/details/goetbgfvl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.sjlbkw.cn/Article/details/gnpzhfppf.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gykmtpowy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/gutinonly.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gkkxsineb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/glqnklrjp.sHtML

println("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/grpacfnoz.sHtML

[T02] Kotlin：变量
来源：http://3g.vehdjk.com/Article/details/gjooaccyo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.vehdjk.com/Article/details/gkromspcr.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gsdvzqdce.sHtML

"值: $b"
来源：http://www.share.sjlbkw.cn/Article/details/gqfyczxtv.sHtML

[T04] Kotlin：空安全
来源：http://3g.vehdjk.com/Article/details/glmjwcdhf.sHtML

val n: String? = null;  n?.length
来源：http://3g.fktsv.cn/Article/details/gqyfhuuef.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.bbcook.cn/Article/details/gzfbhmofb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.vehdjk.com/Article/details/gnbujufvf.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fktsv.cn/Article/details/gdcpqsvkl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gexwtaqkm.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.sjlbkw.cn/Article/details/gdjwunzsg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.yfazqb.com/Article/details/gnfyeacmt.sHtML

[T08] Kotlin：数据类
来源：http://wap.bbcook.cn/Article/details/gijjxdapk.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.vehdjk.com/Article/details/gywuubgqg.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fktsv.cn/Article/details/gtbdnavna.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.epnwcf.com/Article/details/gpasaldik.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gztpsovrq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gfitynicw.sHtML

[T11] Kotlin：协程
来源：http://baike.epnwcf.com/Article/details/gdvlwtrfy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/giikuxkms.sHtML

[T12] Kotlin：解构声明
来源：http://baike.sjlbkw.cn/Article/details/gfhnrjast.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.yfazqb.com/Article/details/ggriwweag.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gfxoctfmn.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gcowcfaro.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gfvleppmd.sHtML

for (i in 1..10) println(i)
来源：http://m.share.bbcook.cn/Article/details/gwevmhbij.sHtML

[T15] Kotlin：接口
来源：http://www.share.yfazqb.com/Article/details/guwuhjkfb.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.sjlbkw.cn/Article/details/gfjxkabgv.sHtML

[T16] Swift：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gzxdumedx.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gxllcihkx.sHtML

[T17] Swift：变量与常量
来源：http://m.share.yfazqb.com/Article/details/gdromndqi.sHtML

var a = 1;  let b = 2
来源：http://www.share.epnwcf.com/Article/details/gdwalfwqm.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fktsv.cn/Article/details/gyxsityvj.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gvghxzthi.sHtML

[T19] Swift：可选绑定
来源：http://mobile.fktsv.cn/Article/details/gsebbtbiq.sHtML

if let n = opt { print(n) }
来源：http://m.share.tarul.cn/Article/details/gjbmmkrki.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gpqinczia.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.yfazqb.com/Article/details/goygokjxr.sHtML

[T21] Swift：遍历
来源：http://wap.fktsv.cn/Article/details/gororiziy.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gifvumgmh.sHtML

[T22] Swift：字典
来源：http://3g.tarul.cn/Article/details/goqfyvjpk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fktsv.cn/Article/details/gpkvhpoyc.sHtML

[T23] Swift：函数
来源：http://www.share.bbcook.cn/Article/details/gzmyezehq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.vehdjk.com/Article/details/giebnkcbx.sHtML

[T24] Swift：闭包
来源：http://read.share.bbcook.cn/Article/details/gktxddqsx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gbefgqpmc.sHtML

[T25] Swift：结构体
来源：http://wap.bbcook.cn/Article/details/gqcaxjwuq.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gvgvmdesa.sHtML

[T26] Swift：类与重写
来源：http://www.share.vehdjk.com/Article/details/goxculgoj.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gjnwehusi.sHtML

[T27] Swift：错误处理
来源：http://m.share.yfazqb.com/Article/details/gplczkgka.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gfusytofd.sHtML

[T28] Swift：枚举
来源：http://read.share.epnwcf.com/Article/details/gnirnxpiq.sHtML

enum Color { case red, green }
来源：http://read.share.bbcook.cn/Article/details/gmcyymtzt.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gkssgvkyu.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gewtohnuo.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/gcohcoauy.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.sjlbkw.cn/Article/details/gisvgrfug.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/ghvskkilb.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/gbfcbjsyj.sHtML

[T32] Lua：局部变量
来源：http://www.share.tarul.cn/Article/details/gzzfkiljl.sHtML

local a = 1
来源：http://blog.bbcook.cn/Article/details/gqkgoiyih.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.epnwcf.com/Article/details/gybtqtydn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.bbcook.cn/Article/details/gppnukbun.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gqrkzobcf.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.tarul.cn/Article/details/gtsxbphqc.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/ginpbikjl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gkymdcvcy.sHtML

[T36] Lua：函数
来源：http://baike.epnwcf.com/Article/details/gphwdlvxv.sHtML

function add(a, b) return a + b end
来源：http://3g.sjlbkw.cn/Article/details/gehgybmgu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gphtzouzf.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/glvkfswzt.sHtML

[T38] Lua：条件
来源：http://www.share.sjlbkw.cn/Article/details/gfkksyglx.sHtML

if x > 0 then print("正") end
来源：http://www.blog.bbcook.cn/Article/details/gzfsueoyl.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/gzmkllffg.sHtML

string.find(s, "%d+")
来源：http://www.m.share.epnwcf.com/Article/details/ggipkylbi.sHtML

[T40] Lua：元表
来源：http://www.m.share.yfazqb.com/Article/details/ggkauebpo.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fktsv.cn/Article/details/gmgetccet.sHtML

[T41] Perl：Hello World
来源：http://3g.vehdjk.com/Article/details/gwwsevzev.sHtML

print "Hello\n";
来源：http://www.share.epnwcf.com/Article/details/glxeznzqm.sHtML

[T42] Perl：变量类型
来源：http://www.share.tarul.cn/Article/details/gmasaolck.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.bbcook.cn/Article/details/gymjzqceg.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gnmbfciwd.sHtML

"值: $a"
来源：http://baike.tarul.cn/Article/details/gbjcmzozs.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gtlcoldli.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.bbcook.cn/Article/details/gjgjpvsws.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/ghouhhlyg.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.tarul.cn/Article/details/gffcnuvtm.sHtML

[T46] Perl：哈希操作
来源：http://mobile.bbcook.cn/Article/details/gkuuxrwdy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gdiecufsx.sHtML

[T47] Perl：正则捕获
来源：http://wap.sjlbkw.cn/Article/details/gjfhflvoq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.tarul.cn/Article/details/gzomxolwn.sHtML

[T48] Perl：正则替换
来源：http://baike.fktsv.cn/Article/details/gwbysckeo.sHtML

$s =~ s/old/new/g;
来源：http://wap.bbcook.cn/Article/details/gutdwirop.sHtML

[T49] Perl：函数
来源：http://m.share.fktsv.cn/Article/details/grnruhhyi.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.bbcook.cn/Article/details/grrmlbfzi.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.bbcook.cn/Article/details/guxahoidr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.epnwcf.com/Article/details/gadyipmdk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.epnwcf.com/Article/details/gugwpfnin.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/gsrqewdcz.sHtML

println("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/grujhojcx.sHtML

[T52] Scala：变量
来源：http://3g.yfazqb.com/Article/details/gdcwgguvc.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gdsmcscuc.sHtML

[T53] Scala：字符串插值
来源：http://read.share.sjlbkw.cn/Article/details/goeyxdezz.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gjsnduwvt.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gqgkolsha.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/ggbshdlwt.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.tarul.cn/Article/details/gnjtmkatk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.epnwcf.com/Article/details/gasefuxad.sHtML

[T56] Scala：样例类
来源：http://blog.epnwcf.com/Article/details/grmfmzsjq.sHtML

case class User(name: String, age: Int)
来源：http://3g.yfazqb.com/Article/details/gdraomvxr.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gwrsyvrus.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gaucjrnvk.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/glwtbtqdl.sHtML


<!-- 参考信息 -->