代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.bbcook.cn/Article/details/gzumghccr.sHtML

[R66] 定时任务
来源：http://www.m.share.vehdjk.com/Article/details/gjuvugziz.sHtML

crontab -e;  crontab -l
来源：http://blog.fktsv.cn/Article/details/gjntndwse.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.epnwcf.com/Article/details/gbutjbxkt.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gbwlksqao.sHtML

[R68] 计算文件校验值
来源：http://m.share.vehdjk.com/Article/details/ghsmolznl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fktsv.cn/Article/details/gcegumgmc.sHtML

[R69] 生成随机密码
来源：http://blog.bbcook.cn/Article/details/gnvmcglou.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.yfazqb.com/Article/details/gxtzwhywb.sHtML

[R70] 时间戳与互转
来源：http://m.share.sjlbkw.cn/Article/details/glmrquhjf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.yfazqb.com/Article/details/gjmpobprf.sHtML

[R71] 日期格式化
来源：http://baike.vehdjk.com/Article/details/gbryvxsdr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.epnwcf.com/Article/details/gvygljxwt.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gnxodfcre.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.yfazqb.com/Article/details/ggaooyghf.sHtML

[R73] 分割大日志
来源：http://m.share.yfazqb.com/Article/details/gpxirvjap.sHtML

split -l 1000 big.log part_
来源：http://www.blog.bbcook.cn/Article/details/gfbqjinqn.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gftrntxkv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.yfazqb.com/Article/details/gljvznrpz.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/glyufeemi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fktsv.cn/Article/details/gjgdotasl.sHtML

[R76] 使用临时文件
来源：http://wap.fktsv.cn/Article/details/glxyeupkf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.sjlbkw.cn/Article/details/gibuvusli.sHtML

[R77] 读取用户输入
来源：http://www.m.share.bbcook.cn/Article/details/gbomzypsd.sHtML

read -rp "请输入: " ans
来源：http://3g.tarul.cn/Article/details/gztkzedxq.sHtML

[R78] 交互式菜单
来源：http://baike.yfazqb.com/Article/details/gjcrlnfnh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.tarul.cn/Article/details/gkddqiypv.sHtML

[R79] 解析命令行选项
来源：http://www.share.yfazqb.com/Article/details/gmqtwjawk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.yfazqb.com/Article/details/gmnyskhms.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fktsv.cn/Article/details/gtfjbepwz.sHtML

time ./run.sh
来源：http://mobile.bbcook.cn/Article/details/gqmoupyhl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdiytonri.sHtML

S. C / C++ 专题
来源：http://mobile.yfazqb.com/Article/details/gkhszrdgp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gutvxwouj.sHtML

[S01] C：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gigvdnovp.sHtML

#include <stdio.h>
来源：http://mobile.bbcook.cn/Article/details/gymglojuy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.bbcook.cn/Article/details/gpoubsick.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gigxwgenq.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.vehdjk.com/Article/details/grvpldwkw.sHtML

[S03] C：读入整数
来源：http://mobile.yfazqb.com/Article/details/gxnbignyb.sHtML

int x; scanf("%d", &x);
来源：http://blog.vehdjk.com/Article/details/ghampujhp.sHtML

[S04] C：字符串复制
来源：http://blog.bbcook.cn/Article/details/gvrimtsio.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.bbcook.cn/Article/details/gobefszqh.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/glkojnvrv.sHtML

strlen(s)
来源：http://baike.epnwcf.com/Article/details/gcwhdyimt.sHtML

[S06] C：字符串比较
来源：http://www.share.epnwcf.com/Article/details/gpiyjrkae.sHtML

strcmp(a, b) == 0
来源：http://m.share.vehdjk.com/Article/details/gobmyxzfc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gglwebouf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/ggfgcvjqb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fktsv.cn/Article/details/glnlvdezc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.tarul.cn/Article/details/gyapslbla.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.sjlbkw.cn/Article/details/gdtuuelss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.sjlbkw.cn/Article/details/gahkwjuog.sHtML

[S10] C：指针与解引用
来源：http://baike.vehdjk.com/Article/details/gktwlvxhw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.tarul.cn/Article/details/gfianrgub.sHtML

[S11] C：逐行读文件
来源：http://baike.bbcook.cn/Article/details/grobuosam.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.tarul.cn/Article/details/gpjuxhayk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gxibjbwfy.sHtML

fclose(f);
来源：http://wap.yfazqb.com/Article/details/gomssqjdf.sHtML

[S12] C：写文件
来源：http://www.m.share.tarul.cn/Article/details/gozxcfvlr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gicmqphxs.sHtML

[S13] C：宏定义
来源：http://www.m.share.yfazqb.com/Article/details/gbncwygci.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gexajjglw.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gsvjejigw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fktsv.cn/Article/details/gjuounems.sHtML

[S15] C：类型转换
来源：http://www.blog.bbcook.cn/Article/details/gbpccdgai.sHtML

(double) a / b
来源：http://www.m.share.epnwcf.com/Article/details/gfbkbrqcy.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/ghfkqcykw.sHtML

x |= (1 << 3);
来源：http://read.share.epnwcf.com/Article/details/gbxkitvxc.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fktsv.cn/Article/details/ggrauxsnp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.bbcook.cn/Article/details/ggvtrbeya.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/ghskguzbw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gnvwwfqhi.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gspvzkjxx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.vehdjk.com/Article/details/ghaavwphr.sHtML

[S20] C：二分查找
来源：http://www.m.share.yfazqb.com/Article/details/gseohlpru.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.epnwcf.com/Article/details/gywcjpqhl.sHtML

[S21] C：字符类别判断
来源：http://read.share.epnwcf.com/Article/details/gajgmmgke.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.vehdjk.com/Article/details/gxnxzifly.sHtML

[S22] C：字符串转数字
来源：http://baike.vehdjk.com/Article/details/gaqufagxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.epnwcf.com/Article/details/gjaueknme.sHtML

[S23] C：随机数
来源：http://www.m.share.epnwcf.com/Article/details/gxjlmpykp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fktsv.cn/Article/details/gyptlyeiy.sHtML

[S24] C：获取本地时间
来源：http://blog.vehdjk.com/Article/details/gdfmiqjcp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fktsv.cn/Article/details/gvtyhazsf.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gfxkfpywe.sHtML

memcpy(dst, src, n);
来源：http://read.share.epnwcf.com/Article/details/gomngqihe.sHtML

[S26] C：内存清零
来源：http://m.share.yfazqb.com/Article/details/gblolljro.sHtML

memset(a, 0, sizeof a);
来源：http://blog.vehdjk.com/Article/details/gjxxcowow.sHtML

[S27] C：定义常量
来源：http://mobile.epnwcf.com/Article/details/ghlegffoi.sHtML

const double PI = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gkwnvmone.sHtML

[S28] C：静态变量
来源：http://baike.fktsv.cn/Article/details/gwdqjyrgb.sHtML

static int counter = 0;
来源：http://www.m.share.vehdjk.com/Article/details/gmxkaijtt.sHtML

[S29] C：变参函数
来源：http://read.share.epnwcf.com/Article/details/gzbitlajp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.vehdjk.com/Article/details/gjjwpqnqy.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gcksogqhm.sHtML

#ifndef X_H
来源：http://mobile.bbcook.cn/Article/details/gernazjli.sHtML

#define X_H
来源：http://m.share.tarul.cn/Article/details/gtarmpodf.sHtML

#endif
来源：http://www.blog.epnwcf.com/Article/details/gdmajyill.sHtML

[S31] C++：Hello World
来源：http://wap.fktsv.cn/Article/details/ghyxcwvie.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gyslimvwu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.epnwcf.com/Article/details/guatfxesr.sHtML

[S32] C++：字符串
来源：http://www.blog.sjlbkw.cn/Article/details/grrivzopt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/grgxytani.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gaktbukdu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.yfazqb.com/Article/details/gutzhenco.sHtML

[S34] C++：遍历 vector
来源：http://mobile.vehdjk.com/Article/details/gasvxmtlc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/gmvqhzvks.sHtML

[S35] C++：map
来源：http://m.share.epnwcf.com/Article/details/geucllsnx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gteqhacvd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.bbcook.cn/Article/details/gjqgilbpn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/glojsfcmz.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gsntgmhcm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/gsxpenazk.sHtML

[S38] C++：排序
来源：http://m.share.fktsv.cn/Article/details/gyofliokq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.tarul.cn/Article/details/gabhoxrbz.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/guebtlhlw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gsybtcesj.sHtML

[S40] C++：查找元素
来源：http://mobile.fktsv.cn/Article/details/gmyyrokbe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.yfazqb.com/Article/details/gpjwrqnok.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.vehdjk.com/Article/details/gzuofzzgz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.epnwcf.com/Article/details/giowyztpv.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.epnwcf.com/Article/details/gbutrzgwq.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gimjmdexb.sHtML

[S43] C++：智能指针
来源：http://www.blog.fktsv.cn/Article/details/gjwbjqcjq.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gkwtycmwi.sHtML

[S44] C++：引用传参
来源：http://3g.fktsv.cn/Article/details/gamgbemjz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.epnwcf.com/Article/details/gpbkxzlsy.sHtML

[S45] C++：lambda
来源：http://baike.epnwcf.com/Article/details/gumajnaol.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.sjlbkw.cn/Article/details/gfumiucdk.sHtML

[S46] C++：函数模板
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsmgqhag.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.sjlbkw.cn/Article/details/ghtxqqigs.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.yfazqb.com/Article/details/gfsllrdsa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fktsv.cn/Article/details/gonrrfjwl.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/glmndohqm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.sjlbkw.cn/Article/details/grygcvixf.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gtrduejzd.sHtML

[S49] C++：写文件
来源：http://3g.tarul.cn/Article/details/gtfspsjbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.bbcook.cn/Article/details/gtbxiakqt.sHtML

[S50] C++：格式化数字
来源：http://3g.tarul.cn/Article/details/gpidfwejk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.tarul.cn/Article/details/gqvlhsipl.sHtML

[S51] C++：显式类型转换
来源：http://3g.sjlbkw.cn/Article/details/gheqabooy.sHtML

static_cast<double>(a) / b
来源：http://blog.sjlbkw.cn/Article/details/grgtudmah.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gferbodde.sHtML

int size() const noexcept { return n_; }
来源：http://3g.yfazqb.com/Article/details/gctriikbe.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gcrbwmivj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/gbmzufkui.sHtML

[S54] C++：异常处理
来源：http://www.m.share.vehdjk.com/Article/details/gsstuzlag.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.yfazqb.com/Article/details/gigyussni.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.vehdjk.com/Article/details/ggcziaajp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.yfazqb.com/Article/details/gnbgbtwfk.sHtML

[S56] C++：optional
来源：http://www.blog.bbcook.cn/Article/details/gsfxhhmjq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.yfazqb.com/Article/details/gyyhyiukx.sHtML

[S57] C++：编译期常量
来源：http://baike.bbcook.cn/Article/details/gvdazlnvr.sHtML

constexpr int N = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggihhnmuu.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gzaumngqq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gknuggbri.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/gsrijakan.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.epnwcf.com/Article/details/gapyhvdpz.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.sjlbkw.cn/Article/details/gqgsbwkty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fktsv.cn/Article/details/gkcihzafa.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grefhpdpe.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.yfazqb.com/Article/details/gpetqxzqt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmnakjqaw.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fktsv.cn/Article/details/gsbrswylb.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gzjmsrlpc.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gixjdwcvs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.tarul.cn/Article/details/gllloiuzb.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.tarul.cn/Article/details/grjyexxpe.sHtML

"值: $b"
来源：http://www.blog.sjlbkw.cn/Article/details/gtxeciosj.sHtML

[T04] Kotlin：空安全
来源：http://blog.tarul.cn/Article/details/gbnijandc.sHtML

val n: String? = null;  n?.length
来源：http://m.share.epnwcf.com/Article/details/gwzqazmhv.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.bbcook.cn/Article/details/ghzcecaft.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.tarul.cn/Article/details/gkqhnllha.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.bbcook.cn/Article/details/gauwejzra.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gznnagjaa.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gecgpypyf.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.bbcook.cn/Article/details/ghbqdrkpx.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/geajscomq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gtpyhsynk.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gvwlunmnc.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/glfimbwcf.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/geqvlmtmz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.tarul.cn/Article/details/gyoopprmd.sHtML

[T11] Kotlin：协程
来源：http://www.share.tarul.cn/Article/details/gowbejuez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gkohrdidz.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gzwvqppms.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fktsv.cn/Article/details/gfcteiaap.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.bbcook.cn/Article/details/gnyiekjoe.sHtML

val m = mapOf("a" to 1)
来源：http://3g.vehdjk.com/Article/details/gqslhieby.sHtML

[T14] Kotlin：循环
来源：http://blog.epnwcf.com/Article/details/gxposnffx.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/goqipgxve.sHtML

[T15] Kotlin：接口
来源：http://wap.tarul.cn/Article/details/gqbeihpye.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.yfazqb.com/Article/details/gncwgdtfx.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gktborulg.sHtML

print("Hello")
来源：http://www.m.share.vehdjk.com/Article/details/gvkzdmdsz.sHtML

[T17] Swift：变量与常量
来源：http://wap.fktsv.cn/Article/details/gebgvbcib.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gvjgrsuim.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gowayovoi.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/guiexbxlw.sHtML

[T19] Swift：可选绑定
来源：http://blog.fktsv.cn/Article/details/gjvtwjpib.sHtML

if let n = opt { print(n) }
来源：http://www.blog.vehdjk.com/Article/details/gzzltwepc.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/givezxbdh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gxbtmraqi.sHtML

[T21] Swift：遍历
来源：http://3g.fktsv.cn/Article/details/gtkiozewl.sHtML

for x in a { print(x) }
来源：http://mobile.sjlbkw.cn/Article/details/gvmgzntfm.sHtML

[T22] Swift：字典
来源：http://www.share.vehdjk.com/Article/details/gntnhpugv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.yfazqb.com/Article/details/gzxptgiwb.sHtML

[T23] Swift：函数
来源：http://baike.yfazqb.com/Article/details/gezegrnbs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gnkgkuzjw.sHtML

[T24] Swift：闭包
来源：http://www.m.share.vehdjk.com/Article/details/ggpikvkvk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gdrbkkuqw.sHtML

[T25] Swift：结构体
来源：http://www.blog.tarul.cn/Article/details/gqnyvlbyi.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gjvjlaawj.sHtML

[T26] Swift：类与重写
来源：http://baike.bbcook.cn/Article/details/gqoeenewl.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gfjgscagv.sHtML

[T27] Swift：错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gklypurfa.sHtML

do { try f() } catch { print(error) }
来源：http://blog.bbcook.cn/Article/details/gfbglrtpy.sHtML

[T28] Swift：枚举
来源：http://www.blog.tarul.cn/Article/details/greimqumd.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gblrfqwoa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.yfazqb.com/Article/details/gmctkzofo.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/gmgjwdrrm.sHtML

[T30] Swift：协议
来源：http://www.blog.vehdjk.com/Article/details/grivkkeem.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fktsv.cn/Article/details/ghodjmznn.sHtML

[T31] Lua：Hello World
来源：http://3g.epnwcf.com/Article/details/gdicngapk.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gatfivqvr.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gybxkmalt.sHtML

local a = 1
来源：http://www.share.yfazqb.com/Article/details/gwodgacou.sHtML

[T33] Lua：表（数组）
来源：http://m.share.tarul.cn/Article/details/gqohuuhua.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.epnwcf.com/Article/details/gloahqarw.sHtML

[T34] Lua：遍历表
来源：http://www.blog.bbcook.cn/Article/details/gdaaakcbn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.bbcook.cn/Article/details/golxbwtpp.sHtML

[T35] Lua：字典表
来源：http://wap.vehdjk.com/Article/details/guwqaxebm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.yfazqb.com/Article/details/ghkyxoncc.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/genghidgj.sHtML

function add(a, b) return a + b end
来源：http://www.share.fktsv.cn/Article/details/gottenrbs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.fktsv.cn/Article/details/gtlmpnexa.sHtML

"a" .. "b"
来源：http://read.share.fktsv.cn/Article/details/gkiwijbue.sHtML

[T38] Lua：条件
来源：http://3g.fktsv.cn/Article/details/gzwtzrqlm.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.yfazqb.com/Article/details/gajbbnmos.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gvwftdlbb.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/grgsheous.sHtML

[T40] Lua：元表
来源：http://www.share.vehdjk.com/Article/details/gmokjdlih.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.tarul.cn/Article/details/gqjvlyamh.sHtML

[T41] Perl：Hello World
来源：http://read.share.fktsv.cn/Article/details/gmwvidkyu.sHtML

print "Hello\n";
来源：http://mobile.tarul.cn/Article/details/gldybrppu.sHtML

[T42] Perl：变量类型
来源：http://blog.fktsv.cn/Article/details/gdaeumudz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gylnpalyr.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gxkywxiio.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gmumdfavr.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/gttklkuvm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.yfazqb.com/Article/details/grcecmdtp.sHtML

[T45] Perl：数组遍历
来源：http://mobile.yfazqb.com/Article/details/gukqacjkk.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.epnwcf.com/Article/details/gxhyyvzgj.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.sjlbkw.cn/Article/details/gilfcogpz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gwlynbvag.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmixzlfo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.vehdjk.com/Article/details/gtvgiuzcf.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/gmcjwcnim.sHtML

$s =~ s/old/new/g;
来源：http://www.share.vehdjk.com/Article/details/gqjbuclyi.sHtML

[T49] Perl：函数
来源：http://www.m.share.yfazqb.com/Article/details/gvyaarmwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gzkwbxggh.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gfhbnqhti.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gzosgsggp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.bbcook.cn/Article/details/gqenttwcd.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gfahaozho.sHtML

println("Hello")
来源：http://www.blog.sjlbkw.cn/Article/details/gkpzazakg.sHtML

[T52] Scala：变量
来源：http://baike.sjlbkw.cn/Article/details/ghnkjqlge.sHtML

val a = 1;  var b = 2
来源：http://wap.tarul.cn/Article/details/ggujhdgfc.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gnoxvoobt.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gnpiknpct.sHtML

[T54] Scala：集合映射
来源：http://www.blog.yfazqb.com/Article/details/glsxjgnlh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.bbcook.cn/Article/details/gpfusqdeq.sHtML

[T55] Scala：集合过滤
来源：http://www.share.yfazqb.com/Article/details/gitkabcey.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gnpczmuys.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gwaxvdize.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.vehdjk.com/Article/details/gyfpfrbsq.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gybtmlwjc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.fktsv.cn/Article/details/gqnjwiwcb.sHtML

[T58] Scala：函数定义
来源：http://www.share.tarul.cn/Article/details/gadoapmbk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.sjlbkw.cn/Article/details/gcsuktyhy.sHtML

[T59] Scala：循环
来源：http://wap.yfazqb.com/Article/details/gsbsooxqb.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.yfazqb.com/Article/details/giodhaagq.sHtML

[T60] Scala：折叠
来源：http://blog.epnwcf.com/Article/details/gbqaqqfyd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/golwwgwxb.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gidgtceat.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gjjpsdwtr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gedbwkust.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.vehdjk.com/Article/details/gayzflgrw.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://read.share.yfazqb.com/Article/details/gdthuajwq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.bbcook.cn/Article/details/ghfasuksj.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.bbcook.cn/Article/details/gcegsuhzy.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.yfazqb.com/Article/details/gxrvmopxv.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.fktsv.cn/Article/details/glladejtd.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/goejgnbfx.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.sjlbkw.cn/Article/details/gsnivupeg.sHtML

[U05] Py：列表去重且保序
来源：http://baike.epnwcf.com/Article/details/ghdvdljmv.sHtML

list(dict.fromkeys(arr))
来源：http://baike.bbcook.cn/Article/details/gyhhjwawp.sHtML

[U06] Py：合并两个字典
来源：http://3g.sjlbkw.cn/Article/details/gozgdepdo.sHtML

{**a, **b}
来源：http://blog.yfazqb.com/Article/details/ggvtfkfrn.sHtML


<!-- 参考信息 -->