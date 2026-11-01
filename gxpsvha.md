代发 wailian999

ssh user@host 'uptime'
来源：http://read.share.bbcook.cn/Article/details/gfcqwclmw.sHtML

[R58] 下载文件
来源：http://m.share.epnwcf.com/Article/details/gulkphhsx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fktsv.cn/Article/details/gbclfcktc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gjomrcuda.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fktsv.cn/Article/details/gxknzttoi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gcebmsdse.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.vehdjk.com/Article/details/gbzdhpsxh.sHtML

[R61] 磁盘占用
来源：http://wap.yfazqb.com/Article/details/gyogfpqdc.sHtML

df -h;  du -sh *
来源：http://www.m.share.epnwcf.com/Article/details/gguqrwkub.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gioaukssu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.yfazqb.com/Article/details/gjgcfzeze.sHtML

[R63] 内存与进程
来源：http://wap.fktsv.cn/Article/details/gloaybjry.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.bbcook.cn/Article/details/gebclvnjq.sHtML

[R64] 结束进程
来源：http://www.m.share.tarul.cn/Article/details/glugbxshs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.vehdjk.com/Article/details/gpxjfeaup.sHtML

[R65] 查看端口占用
来源：http://3g.vehdjk.com/Article/details/gzurzwkyu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.yfazqb.com/Article/details/ganezkpda.sHtML

[R66] 定时任务
来源：http://m.share.sjlbkw.cn/Article/details/gweanjwto.sHtML

crontab -e;  crontab -l
来源：http://m.share.tarul.cn/Article/details/gqcxhpqug.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gosvbpnbd.sHtML

openssl rand -hex 16
来源：http://www.blog.tarul.cn/Article/details/godzubgim.sHtML

[R68] 计算文件校验值
来源：http://m.share.sjlbkw.cn/Article/details/gznyazjxu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/ghburmxoz.sHtML

[R69] 生成随机密码
来源：http://wap.yfazqb.com/Article/details/gbxkwvvyu.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/grvpgujou.sHtML

[R70] 时间戳与互转
来源：http://blog.sjlbkw.cn/Article/details/gbdiagdsl.sHtML

date +%s;  date -d @1700000000
来源：http://baike.sjlbkw.cn/Article/details/gftsfawti.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gmljvkzil.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.tarul.cn/Article/details/grkzgtwgj.sHtML

[R72] 等待端口就绪
来源：http://mobile.fktsv.cn/Article/details/ghzgoobup.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.bbcook.cn/Article/details/gsdjsapsv.sHtML

[R73] 分割大日志
来源：http://www.blog.yfazqb.com/Article/details/gdfnvdihe.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gglbbpnjw.sHtML

[R74] 批量重命名
来源：http://www.share.yfazqb.com/Article/details/gchbcqlnx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.epnwcf.com/Article/details/gedvzhysd.sHtML

[R75] 导出环境变量
来源：http://baike.fktsv.cn/Article/details/gannhdsxf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.sjlbkw.cn/Article/details/griypkfwd.sHtML

[R76] 使用临时文件
来源：http://3g.fktsv.cn/Article/details/gyabkadlh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.vehdjk.com/Article/details/gpuaivxdi.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gvtpxiuym.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gfzebdolw.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/grdypfieg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.tarul.cn/Article/details/gqfevdhel.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/goiaqwitn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.yfazqb.com/Article/details/gdycnermt.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.yfazqb.com/Article/details/gnrgzcyba.sHtML

time ./run.sh
来源：http://wap.epnwcf.com/Article/details/gjcwmedrw.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbngsjxom.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gxarmcxnx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gucomognw.sHtML

[S01] C：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwwrliig.sHtML

#include <stdio.h>
来源：http://mobile.fktsv.cn/Article/details/gdkuceref.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.vehdjk.com/Article/details/gckroouew.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gomesiajh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/guzpkplvf.sHtML

[S03] C：读入整数
来源：http://www.blog.epnwcf.com/Article/details/gdrnjegfv.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/gxdtpqcsa.sHtML

[S04] C：字符串复制
来源：http://baike.vehdjk.com/Article/details/gxymntwkr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.yfazqb.com/Article/details/glvdxegll.sHtML

[S05] C：字符串长度
来源：http://m.share.sjlbkw.cn/Article/details/ghzzcelkl.sHtML

strlen(s)
来源：http://baike.tarul.cn/Article/details/gobvmkrdu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gcnbatemi.sHtML

strcmp(a, b) == 0
来源：http://www.share.bbcook.cn/Article/details/gkfjikojb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.bbcook.cn/Article/details/guihqhikc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.epnwcf.com/Article/details/gkzudfacs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpysuxhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.epnwcf.com/Article/details/gexbaiyhq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.sjlbkw.cn/Article/details/gqfgigbsd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.vehdjk.com/Article/details/ggoeobckj.sHtML

[S10] C：指针与解引用
来源：http://wap.sjlbkw.cn/Article/details/gyawjcgbz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.tarul.cn/Article/details/gvjkflszi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/griimpwxl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gcemzgzvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.sjlbkw.cn/Article/details/grqnyjxge.sHtML

fclose(f);
来源：http://www.m.share.vehdjk.com/Article/details/gdnepnnxl.sHtML

[S12] C：写文件
来源：http://m.share.vehdjk.com/Article/details/grsesmmev.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gjtutzlsm.sHtML

[S13] C：宏定义
来源：http://m.share.fktsv.cn/Article/details/gnuimiowa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.vehdjk.com/Article/details/grogpztbg.sHtML

[S14] C：枚举
来源：http://blog.vehdjk.com/Article/details/gcufaxikf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.tarul.cn/Article/details/gyczcgixt.sHtML

[S15] C：类型转换
来源：http://www.blog.fktsv.cn/Article/details/gpdvokifj.sHtML

(double) a / b
来源：http://mobile.sjlbkw.cn/Article/details/gqewmsyrl.sHtML

[S16] C：位操作置位
来源：http://wap.sjlbkw.cn/Article/details/gmghfmxkm.sHtML

x |= (1 << 3);
来源：http://read.share.yfazqb.com/Article/details/gshdldzwo.sHtML

[S17] C：安全拼接字符串
来源：http://3g.tarul.cn/Article/details/gzwdgzgff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqpviqdn.sHtML

[S18] C：命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gwifjrdwh.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gdoffftqe.sHtML

[S19] C：快速排序
来源：http://m.share.epnwcf.com/Article/details/guqosdynw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fktsv.cn/Article/details/grkiskinf.sHtML

[S20] C：二分查找
来源：http://3g.vehdjk.com/Article/details/gybcslmdi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fktsv.cn/Article/details/grdmibxvx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fktsv.cn/Article/details/gxhtxflix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.bbcook.cn/Article/details/gndsdzxcj.sHtML

[S22] C：字符串转数字
来源：http://read.share.vehdjk.com/Article/details/gjjjefhcx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gsfczxdcx.sHtML

[S23] C：随机数
来源：http://m.share.vehdjk.com/Article/details/gkeghtjtb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/gzmytwfks.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gnnwinbwn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fktsv.cn/Article/details/guxxxyoxm.sHtML

[S25] C：内存拷贝
来源：http://m.share.fktsv.cn/Article/details/gwjplupjy.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gfzkkrcul.sHtML

[S26] C：内存清零
来源：http://3g.yfazqb.com/Article/details/grdjqstkp.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.sjlbkw.cn/Article/details/gbkvunaca.sHtML

[S27] C：定义常量
来源：http://3g.tarul.cn/Article/details/gafnsvnce.sHtML

const double PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gycbdyvzs.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/gnbfzfexn.sHtML

static int counter = 0;
来源：http://blog.epnwcf.com/Article/details/gnxwffjaz.sHtML

[S29] C：变参函数
来源：http://wap.sjlbkw.cn/Article/details/gnamitsgh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.yfazqb.com/Article/details/gintcjrhc.sHtML

[S30] C：头文件保护
来源：http://www.share.fktsv.cn/Article/details/gqncnqqzb.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/gueseilte.sHtML

#define X_H
来源：http://read.share.fktsv.cn/Article/details/gwfkfwrui.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/ganslnypw.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gbrrshuge.sHtML

#include <iostream>
来源：http://blog.tarul.cn/Article/details/girpwclbn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbsdglwng.sHtML

[S32] C++：字符串
来源：http://read.share.yfazqb.com/Article/details/gfojobgnw.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.bbcook.cn/Article/details/ghsclivtc.sHtML

[S33] C++：vector 增删
来源：http://3g.bbcook.cn/Article/details/gdluvnwrk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fktsv.cn/Article/details/gvomzzlng.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gawedafzc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.epnwcf.com/Article/details/gecohvwqh.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gdxhudwmh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fktsv.cn/Article/details/gxdkejgrj.sHtML

[S36] C++：unordered_map
来源：http://3g.fktsv.cn/Article/details/gawtfjaxp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gsosptfxv.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gqwggcjgo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fktsv.cn/Article/details/gbrxdhkil.sHtML

[S38] C++：排序
来源：http://baike.bbcook.cn/Article/details/ggeckjmqv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.yfazqb.com/Article/details/gnwhnrgox.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.bbcook.cn/Article/details/gfibssvyb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.yfazqb.com/Article/details/gjgfiioxi.sHtML

[S40] C++：查找元素
来源：http://wap.yfazqb.com/Article/details/gixzlhxkr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fktsv.cn/Article/details/gzxuybotc.sHtML

[S41] C++：类与构造函数
来源：http://read.share.vehdjk.com/Article/details/grcroluxj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.vehdjk.com/Article/details/gldoccrsu.sHtML

[S42] C++：继承与虚函数
来源：http://blog.tarul.cn/Article/details/gqazhkdln.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.epnwcf.com/Article/details/gnjxixjaw.sHtML

[S43] C++：智能指针
来源：http://www.share.sjlbkw.cn/Article/details/gzvnvkjhc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fktsv.cn/Article/details/gjvlxbult.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/gqbxvbcbj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gfnnducue.sHtML

[S45] C++：lambda
来源：http://www.blog.vehdjk.com/Article/details/garuabrfn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.bbcook.cn/Article/details/glxbqwepa.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gqfyvyapi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gqagspndm.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.sjlbkw.cn/Article/details/gqayfejyx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.tarul.cn/Article/details/gbdiyolpm.sHtML

[S48] C++：逐行读文件
来源：http://3g.vehdjk.com/Article/details/gpnqwkwxs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fktsv.cn/Article/details/gdafgxerb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.bbcook.cn/Article/details/ghqhcumal.sHtML

[S49] C++：写文件
来源：http://wap.sjlbkw.cn/Article/details/gnxttjsny.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.epnwcf.com/Article/details/gkiarcvkp.sHtML

[S50] C++：格式化数字
来源：http://mobile.sjlbkw.cn/Article/details/gtsigbgtp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.yfazqb.com/Article/details/glkmpzfcr.sHtML

[S51] C++：显式类型转换
来源：http://baike.sjlbkw.cn/Article/details/giiyazmib.sHtML

static_cast<double>(a) / b
来源：http://baike.sjlbkw.cn/Article/details/gldmevojg.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gzkdwklya.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/gwjiwjmqt.sHtML

[S53] C++：移动语义
来源：http://baike.vehdjk.com/Article/details/gilhjixyh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.vehdjk.com/Article/details/gciqxjrpo.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/gspgtkjlw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.tarul.cn/Article/details/gjeilypta.sHtML

[S55] C++：结构化绑定
来源：http://read.share.tarul.cn/Article/details/gicmycerd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.sjlbkw.cn/Article/details/geqbzmhyh.sHtML

[S56] C++：optional
来源：http://mobile.yfazqb.com/Article/details/gakmmanpi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.yfazqb.com/Article/details/gzztnoedn.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gxwpiimtc.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/gdnbkpmvt.sHtML

[S58] C++：命名空间
来源：http://mobile.bbcook.cn/Article/details/gtccatqsl.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/gxyrdmamx.sHtML

[S59] C++：静态断言
来源：http://read.share.sjlbkw.cn/Article/details/gijpqxmqp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gergudqqv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fktsv.cn/Article/details/ghtbdgcpw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.sjlbkw.cn/Article/details/gzckzuzov.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/greulpfpf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.yfazqb.com/Article/details/gammnxhug.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqcukmhql.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gnnywfxbh.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gpmefymwd.sHtML

[T02] Kotlin：变量
来源：http://3g.bbcook.cn/Article/details/gptsqgypm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/ggrqcdjna.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.tarul.cn/Article/details/gqqlieokq.sHtML

"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gagklulcz.sHtML

[T04] Kotlin：空安全
来源：http://baike.fktsv.cn/Article/details/gifpzregi.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/gioravjmn.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gzerqhtow.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvgffhnt.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gapbzxxcr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.vehdjk.com/Article/details/geyeaurgy.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.vehdjk.com/Article/details/gcwyhxnzz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.epnwcf.com/Article/details/gttsfhwhd.sHtML

[T08] Kotlin：数据类
来源：http://m.share.fktsv.cn/Article/details/gesfoootn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gmxnootze.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.bbcook.cn/Article/details/gcqqlfyqy.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gxdywopgs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gmoivlftm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.sjlbkw.cn/Article/details/gqtpojdpn.sHtML

[T11] Kotlin：协程
来源：http://read.share.yfazqb.com/Article/details/gldkwzdtp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fktsv.cn/Article/details/gdneihlqv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.tarul.cn/Article/details/gkcobujmi.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gyzrpvvmy.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fktsv.cn/Article/details/gpcarzhnq.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.tarul.cn/Article/details/gibrxqdfe.sHtML

[T14] Kotlin：循环
来源：http://3g.fktsv.cn/Article/details/gqpeswppi.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.bbcook.cn/Article/details/gjrmcutnj.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gokhncgls.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gdrvbpimt.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gyizwpxaz.sHtML

print("Hello")
来源：http://m.share.tarul.cn/Article/details/gmdujaeaf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gklkrsnvl.sHtML

var a = 1;  let b = 2
来源：http://blog.bbcook.cn/Article/details/ghiqjrmsf.sHtML

[T18] Swift：字符串插值
来源：http://3g.epnwcf.com/Article/details/gsisvoply.sHtML

"值: \(b)"
来源：http://read.share.tarul.cn/Article/details/ghjdznihj.sHtML

[T19] Swift：可选绑定
来源：http://wap.bbcook.cn/Article/details/gggdkaqyi.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/ghjcfivle.sHtML

[T20] Swift：数组操作
来源：http://blog.yfazqb.com/Article/details/giearszvu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gvoaxxzjx.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gokdrevzp.sHtML

for x in a { print(x) }
来源：http://wap.vehdjk.com/Article/details/ggqnzalcg.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/gtpnjmpzj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/gzqhpecdy.sHtML

[T23] Swift：函数
来源：http://mobile.bbcook.cn/Article/details/gfqirkhts.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/gmultqqmq.sHtML

[T24] Swift：闭包
来源：http://www.share.yfazqb.com/Article/details/gbkqxjxza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.epnwcf.com/Article/details/guaeiidiy.sHtML

[T25] Swift：结构体
来源：http://www.blog.sjlbkw.cn/Article/details/gfrewrxfl.sHtML

struct P { var x: Int }
来源：http://baike.yfazqb.com/Article/details/gzoxjidil.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gedhzxvzk.sHtML

class A: Base { override func f() {} }
来源：http://m.share.vehdjk.com/Article/details/gsbrukmgd.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gfeeyxuiz.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.tarul.cn/Article/details/gmlpommip.sHtML

[T28] Swift：枚举
来源：http://www.share.bbcook.cn/Article/details/gjiiansqw.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gqvkanrlo.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.tarul.cn/Article/details/gjxlejjcs.sHtML

guard let x = opt else { return }
来源：http://blog.yfazqb.com/Article/details/ggbcecejk.sHtML

[T30] Swift：协议
来源：http://read.share.yfazqb.com/Article/details/gwueijhjp.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.tarul.cn/Article/details/gdbxjooqv.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/genqedzva.sHtML

print("Hello")
来源：http://read.share.epnwcf.com/Article/details/gsvwarieq.sHtML

[T32] Lua：局部变量
来源：http://m.share.vehdjk.com/Article/details/gijicuahk.sHtML

local a = 1
来源：http://mobile.fktsv.cn/Article/details/gzowjrqin.sHtML

[T33] Lua：表（数组）
来源：http://mobile.yfazqb.com/Article/details/gvjwfaniu.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.sjlbkw.cn/Article/details/gxukvmhvc.sHtML

[T34] Lua：遍历表
来源：http://m.share.yfazqb.com/Article/details/gvoxpqxhz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/gbwmsblax.sHtML

[T35] Lua：字典表
来源：http://baike.bbcook.cn/Article/details/gvcswbqnx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/gzckwuohw.sHtML

[T36] Lua：函数
来源：http://www.blog.yfazqb.com/Article/details/gnkuxeltl.sHtML

function add(a, b) return a + b end
来源：http://blog.yfazqb.com/Article/details/gbdfdatjs.sHtML

[T37] Lua：字符串拼接
来源：http://wap.tarul.cn/Article/details/gqcyycdbw.sHtML

"a" .. "b"
来源：http://3g.tarul.cn/Article/details/gfgbdtlgx.sHtML

[T38] Lua：条件
来源：http://mobile.fktsv.cn/Article/details/geqsdsrkf.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gnoxiokqe.sHtML

[T39] Lua：模式匹配
来源：http://baike.vehdjk.com/Article/details/gxjcppnkt.sHtML

string.find(s, "%d+")
来源：http://www.share.tarul.cn/Article/details/gsgaimgwg.sHtML

[T40] Lua：元表
来源：http://m.share.tarul.cn/Article/details/gmukwefpq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.epnwcf.com/Article/details/gcutcxbny.sHtML

[T41] Perl：Hello World
来源：http://baike.fktsv.cn/Article/details/gbbgmftji.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gxgrrxbwe.sHtML

[T42] Perl：变量类型
来源：http://wap.fktsv.cn/Article/details/gykpxepcq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gulzsddsn.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/glqgmkdoh.sHtML

"值: $a"
来源：http://3g.epnwcf.com/Article/details/gzkixhhkb.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gjryowmfw.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.yfazqb.com/Article/details/gxkltenyq.sHtML

[T45] Perl：数组遍历
来源：http://www.share.bbcook.cn/Article/details/gfgveyzvo.sHtML

for my $x (@arr) { print $x; }
来源：http://m.share.yfazqb.com/Article/details/gawtnxmiu.sHtML

[T46] Perl：哈希操作
来源：http://blog.bbcook.cn/Article/details/guolbbjlc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.yfazqb.com/Article/details/gyvgwlafs.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/ghrbftrru.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.tarul.cn/Article/details/gczosrcdl.sHtML

[T48] Perl：正则替换
来源：http://m.share.epnwcf.com/Article/details/gfhaffzma.sHtML

$s =~ s/old/new/g;
来源：http://baike.fktsv.cn/Article/details/gpeiapefi.sHtML

[T49] Perl：函数
来源：http://wap.sjlbkw.cn/Article/details/gijldippm.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gxdwozyrg.sHtML

[T50] Perl：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gryupjeng.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fktsv.cn/Article/details/gcpzmoskk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/glumnpwnk.sHtML

[T51] Scala：Hello World
来源：http://3g.bbcook.cn/Article/details/gtdldxddz.sHtML

println("Hello")
来源：http://www.blog.bbcook.cn/Article/details/girryvega.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/grtjhdjly.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gqrziuyhs.sHtML

[T53] Scala：字符串插值
来源：http://www.share.yfazqb.com/Article/details/gdbojygqc.sHtML

s"值: $b"
来源：http://m.share.bbcook.cn/Article/details/gnrpamrzm.sHtML

[T54] Scala：集合映射
来源：http://m.share.bbcook.cn/Article/details/ggajdqovg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.tarul.cn/Article/details/gigiylwgk.sHtML

[T55] Scala：集合过滤
来源：http://read.share.yfazqb.com/Article/details/gqihavlop.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.sjlbkw.cn/Article/details/gtzcijfle.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/grqjyauyq.sHtML

case class User(name: String, age: Int)
来源：http://wap.bbcook.cn/Article/details/gjmzefdso.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.epnwcf.com/Article/details/ginmkvwpr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.sjlbkw.cn/Article/details/gmarvxwli.sHtML

[T58] Scala：函数定义
来源：http://m.share.fktsv.cn/Article/details/ghmihwoga.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.epnwcf.com/Article/details/gmnmiqtvt.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gogzarooo.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gukarjkim.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gckwuwqcg.sHtML


<!-- 参考信息 -->