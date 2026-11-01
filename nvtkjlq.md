代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.yfazqb.com/Article/details/gxiqomjbr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/ggliagqva.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.epnwcf.com/Article/details/gtrnfuden.sHtML

[R61] 磁盘占用
来源：http://3g.fktsv.cn/Article/details/gejeqzaww.sHtML

df -h;  du -sh *
来源：http://3g.bbcook.cn/Article/details/gkovuzweb.sHtML

[R62] 找最占空间的文件
来源：http://blog.vehdjk.com/Article/details/gpilaiwqv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlqdtyed.sHtML

[R63] 内存与进程
来源：http://m.share.yfazqb.com/Article/details/gfjfowhma.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.yfazqb.com/Article/details/gjldznvrr.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gejbowbuj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.tarul.cn/Article/details/gryhqnfzu.sHtML

[R65] 查看端口占用
来源：http://read.share.epnwcf.com/Article/details/gfxanyxoi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.yfazqb.com/Article/details/gpvkcdzuz.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gwjmexlpq.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gtbtokmym.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.tarul.cn/Article/details/gwcgkzoxh.sHtML

openssl rand -hex 16
来源：http://mobile.sjlbkw.cn/Article/details/gqhfzgyhe.sHtML

[R68] 计算文件校验值
来源：http://www.share.fktsv.cn/Article/details/gynigebmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.bbcook.cn/Article/details/ggpcuyvbl.sHtML

[R69] 生成随机密码
来源：http://www.share.sjlbkw.cn/Article/details/gdjjuecdl.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fktsv.cn/Article/details/gcazyrgyg.sHtML

[R70] 时间戳与互转
来源：http://m.share.vehdjk.com/Article/details/gcehtjwlj.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.sjlbkw.cn/Article/details/gfehxpuhb.sHtML

[R71] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gihgftfca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.epnwcf.com/Article/details/gqpedmsqi.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gnohtfavy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gglarokyj.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/gdooogmgw.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/glmlaebrz.sHtML

[R74] 批量重命名
来源：http://read.share.fktsv.cn/Article/details/gntznkixz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fktsv.cn/Article/details/gtltmcxet.sHtML

[R75] 导出环境变量
来源：http://blog.yfazqb.com/Article/details/gxxvafkdt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gsxgeivku.sHtML

[R76] 使用临时文件
来源：http://www.blog.tarul.cn/Article/details/gwpmsfnnq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/ghebsghga.sHtML

[R77] 读取用户输入
来源：http://wap.sjlbkw.cn/Article/details/gcbwywxak.sHtML

read -rp "请输入: " ans
来源：http://baike.fktsv.cn/Article/details/geuvebmlf.sHtML

[R78] 交互式菜单
来源：http://3g.bbcook.cn/Article/details/gyscteccz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.epnwcf.com/Article/details/gyrlcrhfv.sHtML

[R79] 解析命令行选项
来源：http://m.share.bbcook.cn/Article/details/gncbvqswc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gywwrojbr.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.tarul.cn/Article/details/gddxidqeg.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gzeftmypt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqclszzbc.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gxaqbvneu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfzvuirom.sHtML

[S01] C：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/geqvkurrr.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gpdxelhkr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.sjlbkw.cn/Article/details/gaarynmlb.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gswtdwsxc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fktsv.cn/Article/details/gtgflquga.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gbgqjcmxs.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fktsv.cn/Article/details/giemcltsy.sHtML

[S04] C：字符串复制
来源：http://3g.bbcook.cn/Article/details/gkusvxapv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.epnwcf.com/Article/details/ggbfxbcwh.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gtjcqvkht.sHtML

strlen(s)
来源：http://mobile.vehdjk.com/Article/details/gtvpfqwef.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gftlunbgy.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gimrfsddc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.tarul.cn/Article/details/gfxybqgjp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fktsv.cn/Article/details/ggdmmagui.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.epnwcf.com/Article/details/ggiosiujh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fktsv.cn/Article/details/ghjcofmxw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gngdvlsei.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gyqspzugb.sHtML

[S10] C：指针与解引用
来源：http://blog.bbcook.cn/Article/details/gfqtrxflq.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.tarul.cn/Article/details/gzkrwlzvf.sHtML

[S11] C：逐行读文件
来源：http://blog.yfazqb.com/Article/details/ghtujsvok.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.vehdjk.com/Article/details/ggwpoztwm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gziyqnfjg.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/grxepxgkf.sHtML

[S12] C：写文件
来源：http://m.share.epnwcf.com/Article/details/gjiknjxdw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.tarul.cn/Article/details/ghkvzvzia.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/grmoovcut.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.yfazqb.com/Article/details/gwznvbhjl.sHtML

[S14] C：枚举
来源：http://www.share.yfazqb.com/Article/details/gojkzchsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.yfazqb.com/Article/details/gbfoaazrt.sHtML

[S15] C：类型转换
来源：http://www.share.fktsv.cn/Article/details/givlciedw.sHtML

(double) a / b
来源：http://m.share.epnwcf.com/Article/details/gqiayzykk.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/goyljbpfp.sHtML

x |= (1 << 3);
来源：http://baike.yfazqb.com/Article/details/gwsvpboon.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gemlbgsjg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gprsgqdle.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gnvvevoik.sHtML

int main(int argc, char **argv)
来源：http://www.share.sjlbkw.cn/Article/details/gttafonph.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/gwvljwcoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gyfdflcpk.sHtML

[S20] C：二分查找
来源：http://mobile.yfazqb.com/Article/details/gcpbxdeat.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gsamakprw.sHtML

[S21] C：字符类别判断
来源：http://mobile.fktsv.cn/Article/details/ghkdnpeir.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.sjlbkw.cn/Article/details/gkihyetgr.sHtML

[S22] C：字符串转数字
来源：http://baike.bbcook.cn/Article/details/gjwsvxqmk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.epnwcf.com/Article/details/guhyveyri.sHtML

[S23] C：随机数
来源：http://baike.sjlbkw.cn/Article/details/gtehitjej.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gkjudsplh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.epnwcf.com/Article/details/gdwotmyvy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.sjlbkw.cn/Article/details/gvggtakxo.sHtML

[S25] C：内存拷贝
来源：http://www.blog.yfazqb.com/Article/details/grybtjfex.sHtML

memcpy(dst, src, n);
来源：http://www.blog.epnwcf.com/Article/details/ghnfdyban.sHtML

[S26] C：内存清零
来源：http://3g.tarul.cn/Article/details/gewmfmzkq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.epnwcf.com/Article/details/gxuesqjfu.sHtML

[S27] C：定义常量
来源：http://baike.vehdjk.com/Article/details/gtkybuphf.sHtML

const double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gizzxkszq.sHtML

[S28] C：静态变量
来源：http://baike.bbcook.cn/Article/details/gbrxtaxld.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gnzwweyjo.sHtML

[S29] C：变参函数
来源：http://mobile.tarul.cn/Article/details/ggcwxkqaa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.epnwcf.com/Article/details/gwukdamcx.sHtML

[S30] C：头文件保护
来源：http://mobile.sjlbkw.cn/Article/details/gaqshjcse.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gatailpmm.sHtML

#define X_H
来源：http://blog.fktsv.cn/Article/details/gkixcfjrc.sHtML

#endif
来源：http://mobile.yfazqb.com/Article/details/glnknkzgl.sHtML

[S31] C++：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gkfhzqgmr.sHtML

#include <iostream>
来源：http://read.share.vehdjk.com/Article/details/gzdwrsoxc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/gjibukqko.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gglnomyqk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/glyzlmklt.sHtML

[S33] C++：vector 增删
来源：http://3g.yfazqb.com/Article/details/ghaztdcws.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gfdvimwch.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.sjlbkw.cn/Article/details/gtljhtfsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gqobvwphi.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gmikufjhr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.vehdjk.com/Article/details/goiurmwgl.sHtML

[S36] C++：unordered_map
来源：http://read.share.tarul.cn/Article/details/gptqskydj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.yfazqb.com/Article/details/gbovkmeag.sHtML

[S37] C++：set
来源：http://3g.fktsv.cn/Article/details/gvkjgowqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.bbcook.cn/Article/details/grqpoqhax.sHtML

[S38] C++：排序
来源：http://blog.bbcook.cn/Article/details/gvstbobpj.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.bbcook.cn/Article/details/gpqbfyops.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.sjlbkw.cn/Article/details/gijllbdza.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.tarul.cn/Article/details/guoebffyd.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/goodwmzwe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.vehdjk.com/Article/details/gejltjytq.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbdymdqse.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fktsv.cn/Article/details/gsohhaaxa.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gnmtvggme.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/giasgzuhx.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gaazxubke.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.yfazqb.com/Article/details/gkqjzentr.sHtML

[S44] C++：引用传参
来源：http://read.share.epnwcf.com/Article/details/gijasjzgi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.bbcook.cn/Article/details/gqmgmzwwu.sHtML

[S45] C++：lambda
来源：http://baike.bbcook.cn/Article/details/gwfgjghoq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fktsv.cn/Article/details/gmzjbrmxz.sHtML

[S46] C++：函数模板
来源：http://blog.yfazqb.com/Article/details/gkpnoptqi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.vehdjk.com/Article/details/gdaxnvdwj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.sjlbkw.cn/Article/details/gdqvyzkpf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtlunoirt.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/grbchaadk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fktsv.cn/Article/details/gskfoladu.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.tarul.cn/Article/details/gpzqnextt.sHtML

[S49] C++：写文件
来源：http://baike.fktsv.cn/Article/details/gzwxtabbf.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.tarul.cn/Article/details/glttghvfx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.vehdjk.com/Article/details/gnojyzmbk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.tarul.cn/Article/details/gjtmdcsxu.sHtML

[S51] C++：显式类型转换
来源：http://wap.tarul.cn/Article/details/gieiakmhj.sHtML

static_cast<double>(a) / b
来源：http://mobile.tarul.cn/Article/details/gtfwpatif.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.vehdjk.com/Article/details/gaujyiusu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gobaqfeyt.sHtML

[S53] C++：移动语义
来源：http://baike.tarul.cn/Article/details/gfofuydft.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.bbcook.cn/Article/details/gfixbeegw.sHtML

[S54] C++：异常处理
来源：http://blog.epnwcf.com/Article/details/ghrxjorov.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.bbcook.cn/Article/details/gzbhyewsn.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gffnbmkqe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fktsv.cn/Article/details/ghmpeudwy.sHtML

[S56] C++：optional
来源：http://baike.fktsv.cn/Article/details/gcbtxmbdt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.bbcook.cn/Article/details/gnwkslqct.sHtML

[S57] C++：编译期常量
来源：http://blog.fktsv.cn/Article/details/gwhpuercc.sHtML

constexpr int N = 10;
来源：http://3g.tarul.cn/Article/details/gvysebsru.sHtML

[S58] C++：命名空间
来源：http://wap.fktsv.cn/Article/details/gjdyauhgk.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.yfazqb.com/Article/details/gjirhflzz.sHtML

[S59] C++：静态断言
来源：http://mobile.vehdjk.com/Article/details/gmpozsdeg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.yfazqb.com/Article/details/ghqnzkqlj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/gbdifexdv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.vehdjk.com/Article/details/gpxsoclza.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gstmbdvit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gdzsnnnze.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdvalfpbf.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.bbcook.cn/Article/details/gpemcwane.sHtML

println("Hello")
来源：http://baike.vehdjk.com/Article/details/gukrveknm.sHtML

[T02] Kotlin：变量
来源：http://mobile.fktsv.cn/Article/details/gjanchvsw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/glskzkdhi.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.yfazqb.com/Article/details/gomoqwljb.sHtML

"值: $b"
来源：http://wap.epnwcf.com/Article/details/gjjkwnyyt.sHtML

[T04] Kotlin：空安全
来源：http://www.share.epnwcf.com/Article/details/grprnlwku.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/gmcsjzxan.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.yfazqb.com/Article/details/gvhqjuacf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.vehdjk.com/Article/details/gddqviksx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gkerzycux.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.sjlbkw.cn/Article/details/guoruvipd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.vehdjk.com/Article/details/grjdcdyxe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fktsv.cn/Article/details/gzyoxetpa.sHtML

[T08] Kotlin：数据类
来源：http://mobile.yfazqb.com/Article/details/gvrpdtjqm.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fktsv.cn/Article/details/gncjykdow.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fktsv.cn/Article/details/geunlrwnz.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.tarul.cn/Article/details/glgvdfmwm.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/gpbqazaud.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gqvpsbmer.sHtML

[T11] Kotlin：协程
来源：http://baike.fktsv.cn/Article/details/gkbvspsvw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fktsv.cn/Article/details/gyniralhk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.epnwcf.com/Article/details/ggajkxhqw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gpytipgjn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fktsv.cn/Article/details/gorsmljgz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.yfazqb.com/Article/details/gmpmticht.sHtML

[T14] Kotlin：循环
来源：http://www.blog.bbcook.cn/Article/details/gxepvmsph.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.bbcook.cn/Article/details/ggohzzbro.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.yfazqb.com/Article/details/gkhvqvohy.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.yfazqb.com/Article/details/gkljqdbgs.sHtML

[T16] Swift：Hello World
来源：http://blog.epnwcf.com/Article/details/gbuoxbauv.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/ghobipsrl.sHtML

[T17] Swift：变量与常量
来源：http://3g.sjlbkw.cn/Article/details/gamwhfazj.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gnrsleame.sHtML

[T18] Swift：字符串插值
来源：http://m.share.tarul.cn/Article/details/gekhbshth.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/ghpvynuyh.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/glzxkrdxd.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/ggotxbtob.sHtML

[T20] Swift：数组操作
来源：http://m.share.epnwcf.com/Article/details/gymnvxifw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.epnwcf.com/Article/details/gqusppvww.sHtML

[T21] Swift：遍历
来源：http://www.m.share.tarul.cn/Article/details/gsflzmysc.sHtML

for x in a { print(x) }
来源：http://wap.epnwcf.com/Article/details/gznvtbhoh.sHtML

[T22] Swift：字典
来源：http://m.share.sjlbkw.cn/Article/details/gtafjerlv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gdflzylis.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gyifgsymi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.tarul.cn/Article/details/gwnyqmzax.sHtML

[T24] Swift：闭包
来源：http://www.blog.epnwcf.com/Article/details/gutefbtvr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.tarul.cn/Article/details/gugaoeckz.sHtML

[T25] Swift：结构体
来源：http://wap.fktsv.cn/Article/details/gkfyqsdos.sHtML

struct P { var x: Int }
来源：http://www.m.share.fktsv.cn/Article/details/guqzdgwkd.sHtML

[T26] Swift：类与重写
来源：http://3g.tarul.cn/Article/details/gnsjqcjyl.sHtML

class A: Base { override func f() {} }
来源：http://read.share.vehdjk.com/Article/details/glwmvvdmi.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gzcefzfzn.sHtML

do { try f() } catch { print(error) }
来源：http://3g.yfazqb.com/Article/details/gtoowlevv.sHtML

[T28] Swift：枚举
来源：http://wap.fktsv.cn/Article/details/gogcaoqnd.sHtML

enum Color { case red, green }
来源：http://3g.yfazqb.com/Article/details/gmqxbpgua.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.epnwcf.com/Article/details/ghftujevv.sHtML

guard let x = opt else { return }
来源：http://read.share.bbcook.cn/Article/details/gjpcirlzi.sHtML

[T30] Swift：协议
来源：http://www.m.share.bbcook.cn/Article/details/gqmeoftmv.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.vehdjk.com/Article/details/ggymmepdj.sHtML

[T31] Lua：Hello World
来源：http://www.share.yfazqb.com/Article/details/glhfidrke.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/ghqunspru.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/gfwhywfxz.sHtML

local a = 1
来源：http://mobile.epnwcf.com/Article/details/ghpqaboul.sHtML

[T33] Lua：表（数组）
来源：http://wap.yfazqb.com/Article/details/gotsqinfc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.vehdjk.com/Article/details/gttvwkxwr.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gyqlclwkt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.tarul.cn/Article/details/gutqfadko.sHtML

[T35] Lua：字典表
来源：http://www.share.yfazqb.com/Article/details/ggnttgjyc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.share.fktsv.cn/Article/details/gtrszdxth.sHtML

[T36] Lua：函数
来源：http://www.share.bbcook.cn/Article/details/gmpbpyihh.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.vehdjk.com/Article/details/gnhdyjioz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.yfazqb.com/Article/details/gcidlmmze.sHtML

"a" .. "b"
来源：http://3g.vehdjk.com/Article/details/gykjycojp.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gygrrnzik.sHtML

if x > 0 then print("正") end
来源：http://www.share.fktsv.cn/Article/details/gcfztfyto.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/ggescfoaq.sHtML

string.find(s, "%d+")
来源：http://read.share.tarul.cn/Article/details/ghbmgblvl.sHtML

[T40] Lua：元表
来源：http://mobile.vehdjk.com/Article/details/gsitsqrfw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.epnwcf.com/Article/details/galymqywf.sHtML

[T41] Perl：Hello World
来源：http://www.share.yfazqb.com/Article/details/gtogoycxw.sHtML

print "Hello\n";
来源：http://3g.vehdjk.com/Article/details/gpueieihd.sHtML

[T42] Perl：变量类型
来源：http://blog.yfazqb.com/Article/details/gwbuwetps.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fktsv.cn/Article/details/gzlerezsi.sHtML

[T43] Perl：字符串插值
来源：http://wap.fktsv.cn/Article/details/ggkpvecfn.sHtML

"值: $a"
来源：http://mobile.sjlbkw.cn/Article/details/gppfokhuh.sHtML

[T44] Perl：条件
来源：http://www.share.yfazqb.com/Article/details/gxonrkmeq.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.sjlbkw.cn/Article/details/gntkiwfqj.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/grtagkehd.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjavnozo.sHtML

[T46] Perl：哈希操作
来源：http://3g.bbcook.cn/Article/details/gmlrlqlss.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fktsv.cn/Article/details/gzqbcexuy.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gdrxxdhej.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.bbcook.cn/Article/details/greaeqasl.sHtML

[T48] Perl：正则替换
来源：http://wap.bbcook.cn/Article/details/gpadobnqp.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.epnwcf.com/Article/details/gjtzsdyxc.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gkfqsfuxu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdtgbcha.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/glqolrasb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.sjlbkw.cn/Article/details/gyjkszgij.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.sjlbkw.cn/Article/details/gfeyeuncn.sHtML

[T51] Scala：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gdbhkyrcp.sHtML

println("Hello")
来源：http://www.m.share.sjlbkw.cn/Article/details/glmreaigp.sHtML

[T52] Scala：变量
来源：http://wap.tarul.cn/Article/details/ghjchciud.sHtML

val a = 1;  var b = 2
来源：http://www.share.yfazqb.com/Article/details/gpsovwzhz.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/gbceujjdt.sHtML

s"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gsxgprxzc.sHtML

[T54] Scala：集合映射
来源：http://baike.vehdjk.com/Article/details/gzmyzgyho.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gdxmsnrna.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.bbcook.cn/Article/details/gnlsumvdj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gtzegaciy.sHtML

[T56] Scala：样例类
来源：http://www.m.share.fktsv.cn/Article/details/gguldlgho.sHtML

case class User(name: String, age: Int)
来源：http://mobile.vehdjk.com/Article/details/gfjyxdssk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.vehdjk.com/Article/details/gpbsvcaha.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://baike.yfazqb.com/Article/details/gfalfupuu.sHtML

[T58] Scala：函数定义
来源：http://3g.vehdjk.com/Article/details/garwigxtx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gcxehzopp.sHtML

[T59] Scala：循环
来源：http://www.share.sjlbkw.cn/Article/details/gkieoxtnc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gwhuwbbmm.sHtML

[T60] Scala：折叠
来源：http://mobile.bbcook.cn/Article/details/gohtkdmji.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.tarul.cn/Article/details/gxjncmmno.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gahlxjfbr.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.epnwcf.com/Article/details/gqtnzyhlf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvyimnrob.sHtML


<!-- 参考信息 -->