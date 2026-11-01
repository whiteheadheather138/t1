代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.yfazqb.com/Article/details/gtinxthxs.sHtML

[R56] 远程拷贝
来源：http://3g.epnwcf.com/Article/details/gqvwqcqty.sHtML

scp file user@host:/path/
来源：http://baike.bbcook.cn/Article/details/gusnfduak.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/guotoaggm.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gdmkcehra.sHtML

[R58] 下载文件
来源：http://blog.fktsv.cn/Article/details/gmpowxooy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gvltezilh.sHtML

[R59] 发 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gkqtcdzrf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gkurhasut.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gtkipgddh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.epnwcf.com/Article/details/ggjnxhmxt.sHtML

[R61] 磁盘占用
来源：http://www.share.tarul.cn/Article/details/gyszgddbj.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gbwulcwcy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fktsv.cn/Article/details/gdozkwsoj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.yfazqb.com/Article/details/gomjirzsz.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gsdndkpli.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.sjlbkw.cn/Article/details/gwocanjyc.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gbdxhrkpg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.sjlbkw.cn/Article/details/gvslzvlrp.sHtML

[R65] 查看端口占用
来源：http://m.share.epnwcf.com/Article/details/gslmfwfxq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gxwatjxsd.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gpbdmzmid.sHtML

crontab -e;  crontab -l
来源：http://mobile.fktsv.cn/Article/details/gbnwxufne.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.tarul.cn/Article/details/ggrfayuec.sHtML

openssl rand -hex 16
来源：http://3g.fktsv.cn/Article/details/gqbhueoyl.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gazeevztr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.tarul.cn/Article/details/gmtkkkazi.sHtML

[R69] 生成随机密码
来源：http://www.blog.epnwcf.com/Article/details/gywixnyfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.epnwcf.com/Article/details/gxcavnlvu.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/giaeyurjw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/ghvbiilce.sHtML

[R71] 日期格式化
来源：http://wap.yfazqb.com/Article/details/gyufeyibf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gnpogeyrc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gzauztvnj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gjtrktann.sHtML

[R73] 分割大日志
来源：http://www.blog.epnwcf.com/Article/details/gsyjylywj.sHtML

split -l 1000 big.log part_
来源：http://www.blog.epnwcf.com/Article/details/gbxntldfz.sHtML

[R74] 批量重命名
来源：http://m.share.bbcook.cn/Article/details/gshkpmbrl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gevhyzijy.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gwestbith.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.tarul.cn/Article/details/gyhvntajt.sHtML

[R76] 使用临时文件
来源：http://www.share.bbcook.cn/Article/details/gpslrvrnk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fktsv.cn/Article/details/gxclosidf.sHtML

[R77] 读取用户输入
来源：http://blog.fktsv.cn/Article/details/glnjbgvkq.sHtML

read -rp "请输入: " ans
来源：http://m.share.sjlbkw.cn/Article/details/gbwierqvu.sHtML

[R78] 交互式菜单
来源：http://m.share.epnwcf.com/Article/details/gnkyxxouh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fktsv.cn/Article/details/gzbyxsolx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fktsv.cn/Article/details/gttvzxfzk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.epnwcf.com/Article/details/gbrpsovdm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.sjlbkw.cn/Article/details/gklwghheo.sHtML

time ./run.sh
来源：http://mobile.vehdjk.com/Article/details/geogornfg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdgwwrvli.sHtML

S. C / C++ 专题
来源：http://mobile.epnwcf.com/Article/details/gtisjatsb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqccvgnzl.sHtML

[S01] C：Hello World
来源：http://www.m.share.yfazqb.com/Article/details/goximbokt.sHtML

#include <stdio.h>
来源：http://www.blog.sjlbkw.cn/Article/details/gixdhlvrq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fktsv.cn/Article/details/gsymzattu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fktsv.cn/Article/details/gvpfrontd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.bbcook.cn/Article/details/gqnjdzzoa.sHtML

[S03] C：读入整数
来源：http://read.share.epnwcf.com/Article/details/gbtonmjet.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gyaomstzg.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/gszvqbrbl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.yfazqb.com/Article/details/gfqejxwcn.sHtML

[S05] C：字符串长度
来源：http://m.share.epnwcf.com/Article/details/gslowlrpf.sHtML

strlen(s)
来源：http://blog.bbcook.cn/Article/details/gisgftyla.sHtML

[S06] C：字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gdrqeocjv.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/grnpzecuz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.sjlbkw.cn/Article/details/gkvdbrabv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.epnwcf.com/Article/details/gtjgxscyl.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.vehdjk.com/Article/details/gawixtlzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/gemfzoiiw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fktsv.cn/Article/details/gcyibovmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gjgrzqgac.sHtML

[S10] C：指针与解引用
来源：http://read.share.bbcook.cn/Article/details/gbnxzojfo.sHtML

int *p = &a;  *p = 5;
来源：http://3g.tarul.cn/Article/details/guecyngmv.sHtML

[S11] C：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gtrgnbzry.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gvredglwy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.sjlbkw.cn/Article/details/gqegolbyh.sHtML

fclose(f);
来源：http://3g.yfazqb.com/Article/details/gitfmiidr.sHtML

[S12] C：写文件
来源：http://mobile.vehdjk.com/Article/details/gaxgtguua.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.vehdjk.com/Article/details/gugvtcxly.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gtkxdbiqz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.vehdjk.com/Article/details/gkmmqwkqh.sHtML

[S14] C：枚举
来源：http://m.share.yfazqb.com/Article/details/gjbhnnoyc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.tarul.cn/Article/details/gbosikecw.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/ggvfwfqtz.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/gumaqiyxs.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gqzolaogx.sHtML

x |= (1 << 3);
来源：http://baike.tarul.cn/Article/details/gdtcwbcrm.sHtML

[S17] C：安全拼接字符串
来源：http://blog.yfazqb.com/Article/details/gojcfankc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggicxgdul.sHtML

[S18] C：命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/glmirkwei.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fktsv.cn/Article/details/gaqvkihhc.sHtML

[S19] C：快速排序
来源：http://baike.epnwcf.com/Article/details/gzplwgsar.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gpjvsiebk.sHtML

[S20] C：二分查找
来源：http://m.share.bbcook.cn/Article/details/gztkmldnu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gvpoyzrpw.sHtML

[S21] C：字符类别判断
来源：http://wap.tarul.cn/Article/details/gifnilacs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.yfazqb.com/Article/details/gmaiqopgr.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gcysunucg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.sjlbkw.cn/Article/details/gqrvtcfnw.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gtlgiuszs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.yfazqb.com/Article/details/gblipujws.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.vehdjk.com/Article/details/gawyochfx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.yfazqb.com/Article/details/gkusucunh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.tarul.cn/Article/details/gvonccjys.sHtML

memcpy(dst, src, n);
来源：http://baike.vehdjk.com/Article/details/gwcevkucq.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gtfozssgy.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.bbcook.cn/Article/details/gomndeoov.sHtML

[S27] C：定义常量
来源：http://wap.bbcook.cn/Article/details/geujrxgbq.sHtML

const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gixulcmdp.sHtML

[S28] C：静态变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gluskfeyh.sHtML

static int counter = 0;
来源：http://www.share.bbcook.cn/Article/details/gzsggoatw.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gccuozoqi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fktsv.cn/Article/details/gzpwgslia.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gzzfxusym.sHtML

#ifndef X_H
来源：http://www.share.bbcook.cn/Article/details/gdttjryyr.sHtML

#define X_H
来源：http://read.share.epnwcf.com/Article/details/guplzcveu.sHtML

#endif
来源：http://www.share.epnwcf.com/Article/details/gyxfnvujv.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/ghdttrwlo.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/geadihjmj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/ggtrlipyb.sHtML

[S32] C++：字符串
来源：http://mobile.yfazqb.com/Article/details/gcvkhavrn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/giswbwzeg.sHtML

[S33] C++：vector 增删
来源：http://read.share.sjlbkw.cn/Article/details/goesnpeus.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.tarul.cn/Article/details/gzkftkekj.sHtML

[S34] C++：遍历 vector
来源：http://wap.sjlbkw.cn/Article/details/gzvjztkwi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.vehdjk.com/Article/details/glcjenvbl.sHtML

[S35] C++：map
来源：http://www.m.share.yfazqb.com/Article/details/gsduwvxom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gmhyubduh.sHtML

[S36] C++：unordered_map
来源：http://read.share.bbcook.cn/Article/details/gghipqwnu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghelingmr.sHtML

[S37] C++：set
来源：http://wap.bbcook.cn/Article/details/gfsmnfjny.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.sjlbkw.cn/Article/details/getpmqqei.sHtML

[S38] C++：排序
来源：http://www.m.share.fktsv.cn/Article/details/gchqszpuc.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.bbcook.cn/Article/details/gbicqcaqq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.sjlbkw.cn/Article/details/ggvvyjnpj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gatuxcslv.sHtML

[S40] C++：查找元素
来源：http://blog.sjlbkw.cn/Article/details/geryzjfyn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fktsv.cn/Article/details/gdixgxvcw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gfosgikcg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/gpzxlmzjy.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.bbcook.cn/Article/details/gprgnbhty.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gowvolmjz.sHtML

[S43] C++：智能指针
来源：http://blog.fktsv.cn/Article/details/ghkcdefvb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.yfazqb.com/Article/details/gwuwdfafi.sHtML

[S44] C++：引用传参
来源：http://baike.sjlbkw.cn/Article/details/guoognger.sHtML

void inc(int &x) { ++x; }
来源：http://3g.yfazqb.com/Article/details/gizxqhpic.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/ggebknfvx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.vehdjk.com/Article/details/gixhyqyst.sHtML

[S46] C++：函数模板
来源：http://read.share.yfazqb.com/Article/details/gkunlctkf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.tarul.cn/Article/details/gdsrrivmk.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fktsv.cn/Article/details/giftkzkcd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gotiycqml.sHtML

[S48] C++：逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gwbxsxtuz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fktsv.cn/Article/details/gjzmshexw.sHtML

while (std::getline(in, line)) { }
来源：http://wap.tarul.cn/Article/details/gvkdhuctr.sHtML

[S49] C++：写文件
来源：http://blog.vehdjk.com/Article/details/gylhbtxvi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.tarul.cn/Article/details/glgruqprn.sHtML

[S50] C++：格式化数字
来源：http://www.share.epnwcf.com/Article/details/gjylhtrwx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gdlvwhoen.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gdxcepyzm.sHtML

static_cast<double>(a) / b
来源：http://www.blog.sjlbkw.cn/Article/details/ggksyfkzc.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/ghtmywcxk.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gpqkmvydw.sHtML

[S53] C++：移动语义
来源：http://m.share.vehdjk.com/Article/details/gxtdcoyhy.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.tarul.cn/Article/details/grtmbwodc.sHtML

[S54] C++：异常处理
来源：http://www.blog.fktsv.cn/Article/details/gyxiejtmu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.bbcook.cn/Article/details/gyyqxaeiu.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gjoejipyf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fktsv.cn/Article/details/gjrpfpaad.sHtML

[S56] C++：optional
来源：http://blog.bbcook.cn/Article/details/gcvpveufd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.epnwcf.com/Article/details/gxlrrbrld.sHtML

[S57] C++：编译期常量
来源：http://read.share.vehdjk.com/Article/details/gzapklczy.sHtML

constexpr int N = 10;
来源：http://www.blog.bbcook.cn/Article/details/ggtwgeaeu.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/ghauberkn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.yfazqb.com/Article/details/gjhisifkp.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/gemourbfv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gkoxxwdix.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.bbcook.cn/Article/details/gprwlgluu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.yfazqb.com/Article/details/grqawjprt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gstveipzj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.vehdjk.com/Article/details/gquoxqfnl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gumrmfapr.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.bbcook.cn/Article/details/gelrowvos.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gcfdwaojn.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gctzxuydj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/ghfhvgspj.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.bbcook.cn/Article/details/gvpoxwkay.sHtML

"值: $b"
来源：http://m.share.yfazqb.com/Article/details/glrrcieib.sHtML

[T04] Kotlin：空安全
来源：http://read.share.tarul.cn/Article/details/gldppdimc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gxzxcmwmu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.vehdjk.com/Article/details/gtdyvusdk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.bbcook.cn/Article/details/gsjhxsvhn.sHtML

[T06] Kotlin：集合映射
来源：http://wap.yfazqb.com/Article/details/gnuquvzye.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.yfazqb.com/Article/details/ghixsblip.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gxennrdgy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.epnwcf.com/Article/details/ggxbkfdwb.sHtML

[T08] Kotlin：数据类
来源：http://www.share.tarul.cn/Article/details/gtzpvpdhp.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.vehdjk.com/Article/details/gcahnjcud.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.yfazqb.com/Article/details/gebxfedcj.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.epnwcf.com/Article/details/gjzmpwxjh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.bbcook.cn/Article/details/gmjtcekmb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fktsv.cn/Article/details/gceoldqwd.sHtML

[T11] Kotlin：协程
来源：http://www.blog.yfazqb.com/Article/details/gkqvxsisr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.yfazqb.com/Article/details/gqtwgcebp.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.epnwcf.com/Article/details/ggqrqpmdk.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.yfazqb.com/Article/details/ghzjsqwkq.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.vehdjk.com/Article/details/gvizdjexg.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.epnwcf.com/Article/details/ghhpewqec.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fktsv.cn/Article/details/gsqevorxy.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/glktjaytn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.yfazqb.com/Article/details/grpkwejly.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gxmaxabol.sHtML

[T16] Swift：Hello World
来源：http://mobile.vehdjk.com/Article/details/gjfzhnwxp.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gjhdjpoid.sHtML

[T17] Swift：变量与常量
来源：http://read.share.vehdjk.com/Article/details/gomprocci.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gdfghuodb.sHtML

[T18] Swift：字符串插值
来源：http://wap.bbcook.cn/Article/details/gietcbqla.sHtML

"值: \(b)"
来源：http://m.share.vehdjk.com/Article/details/gqdkyvdni.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.epnwcf.com/Article/details/gzvxrrsoi.sHtML

if let n = opt { print(n) }
来源：http://read.share.epnwcf.com/Article/details/gadfjwhhf.sHtML

[T20] Swift：数组操作
来源：http://read.share.yfazqb.com/Article/details/gybjjyioa.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.vehdjk.com/Article/details/gwjjzibbo.sHtML

[T21] Swift：遍历
来源：http://mobile.yfazqb.com/Article/details/gqgdmpopb.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/gnnjbrxbz.sHtML

[T22] Swift：字典
来源：http://read.share.yfazqb.com/Article/details/gozsyrhbf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gcxfnpjss.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gacnbnzrz.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gakqnsopl.sHtML

[T24] Swift：闭包
来源：http://blog.epnwcf.com/Article/details/gnzyclxcd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fktsv.cn/Article/details/gcftvlxap.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gjqnbsgja.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/gnooogusj.sHtML

[T26] Swift：类与重写
来源：http://m.share.yfazqb.com/Article/details/gwcsrzode.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/gomowjjik.sHtML

[T27] Swift：错误处理
来源：http://3g.tarul.cn/Article/details/gdjxvyufp.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.sjlbkw.cn/Article/details/gykqgibju.sHtML

[T28] Swift：枚举
来源：http://wap.vehdjk.com/Article/details/gpevpsgmj.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gbbictlrw.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.tarul.cn/Article/details/gbaathdvu.sHtML

guard let x = opt else { return }
来源：http://3g.tarul.cn/Article/details/glijxebpe.sHtML

[T30] Swift：协议
来源：http://www.m.share.fktsv.cn/Article/details/gmihlcwee.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gbnndmyin.sHtML

[T31] Lua：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gpptjtsfd.sHtML

print("Hello")
来源：http://www.m.share.epnwcf.com/Article/details/ggkfbvkhu.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gpkejjfba.sHtML

local a = 1
来源：http://www.share.vehdjk.com/Article/details/gvlipngak.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.bbcook.cn/Article/details/gaebrjtuw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/glhfgjykb.sHtML

[T34] Lua：遍历表
来源：http://wap.bbcook.cn/Article/details/gnqoxdcsv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/gshqhajik.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/gpsmoyofo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.sjlbkw.cn/Article/details/gqrxiofwk.sHtML

[T36] Lua：函数
来源：http://www.blog.vehdjk.com/Article/details/gutazhecr.sHtML

function add(a, b) return a + b end
来源：http://mobile.tarul.cn/Article/details/gapxiygtu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gyegvzafh.sHtML

"a" .. "b"
来源：http://www.m.share.yfazqb.com/Article/details/grdcwgjcu.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/gdjeskwuc.sHtML

if x > 0 then print("正") end
来源：http://3g.bbcook.cn/Article/details/gytncifeh.sHtML

[T39] Lua：模式匹配
来源：http://www.share.sjlbkw.cn/Article/details/gkvipiejn.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/grhbjhzye.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/gvfjfrpxx.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gvlmywrdd.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/geyxpuvfb.sHtML

print "Hello\n";
来源：http://m.share.fktsv.cn/Article/details/gwldgwqes.sHtML

[T42] Perl：变量类型
来源：http://baike.yfazqb.com/Article/details/geirptljc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.epnwcf.com/Article/details/geogipgti.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gifhvfabk.sHtML

"值: $a"
来源：http://read.share.vehdjk.com/Article/details/gekdsifts.sHtML

[T44] Perl：条件
来源：http://read.share.fktsv.cn/Article/details/gnrwrrusn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gjzndwxfw.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/ggfbiteus.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.yfazqb.com/Article/details/gaespqxfb.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/goblwltvg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.epnwcf.com/Article/details/gxsldscik.sHtML

[T47] Perl：正则捕获
来源：http://baike.vehdjk.com/Article/details/gmzocjcgt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gxgzlnjjc.sHtML

[T48] Perl：正则替换
来源：http://www.share.yfazqb.com/Article/details/gzqjdskkn.sHtML

$s =~ s/old/new/g;
来源：http://mobile.tarul.cn/Article/details/gzaalxxzo.sHtML

[T49] Perl：函数
来源：http://blog.vehdjk.com/Article/details/gbunufjgs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fktsv.cn/Article/details/ghqmjjkbf.sHtML

[T50] Perl：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/gzmwajmwf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gbaekacza.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gykryvcym.sHtML

[T51] Scala：Hello World
来源：http://wap.yfazqb.com/Article/details/gwlwzyojk.sHtML

println("Hello")
来源：http://3g.sjlbkw.cn/Article/details/gbsmgbnso.sHtML

[T52] Scala：变量
来源：http://www.blog.yfazqb.com/Article/details/gnvidmkdg.sHtML

val a = 1;  var b = 2
来源：http://blog.epnwcf.com/Article/details/gdxuysaam.sHtML

[T53] Scala：字符串插值
来源：http://blog.tarul.cn/Article/details/ghgyzhkuy.sHtML

s"值: $b"
来源：http://3g.tarul.cn/Article/details/gipghyjck.sHtML

[T54] Scala：集合映射
来源：http://baike.bbcook.cn/Article/details/gzmictjdx.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.vehdjk.com/Article/details/gvhjjkonp.sHtML

[T55] Scala：集合过滤
来源：http://wap.tarul.cn/Article/details/gmlofnvma.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.bbcook.cn/Article/details/gxhjbnmvq.sHtML

[T56] Scala：样例类
来源：http://www.share.bbcook.cn/Article/details/gjouiafll.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/gzlxhddpc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gihxpxppi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.fktsv.cn/Article/details/gwhsoljho.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gnvtxprqe.sHtML


<!-- 参考信息 -->