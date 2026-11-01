代发 wailian999

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/glwqbbnll.sHtML

[R64] 结束进程
来源：http://3g.sjlbkw.cn/Article/details/gqntedbbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gkunrjind.sHtML

[R65] 查看端口占用
来源：http://www.blog.sjlbkw.cn/Article/details/glehjyrxr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/ggxayzqbf.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/ghndlwpva.sHtML

crontab -e;  crontab -l
来源：http://baike.tarul.cn/Article/details/gqqckjwyj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.bbcook.cn/Article/details/gdfpgjavg.sHtML

openssl rand -hex 16
来源：http://www.share.vehdjk.com/Article/details/ghircttlq.sHtML

[R68] 计算文件校验值
来源：http://wap.yfazqb.com/Article/details/gajxiepsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.tarul.cn/Article/details/gahweobph.sHtML

[R69] 生成随机密码
来源：http://www.share.fktsv.cn/Article/details/gzqfnwnvm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.sjlbkw.cn/Article/details/gjfavjgij.sHtML

[R70] 时间戳与互转
来源：http://3g.epnwcf.com/Article/details/gskmvwqlo.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gekjvirpg.sHtML

[R71] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gwowczzjn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.bbcook.cn/Article/details/gjzmmrzap.sHtML

[R72] 等待端口就绪
来源：http://blog.tarul.cn/Article/details/gyhhruads.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gesvqxtdq.sHtML

[R73] 分割大日志
来源：http://3g.epnwcf.com/Article/details/ghienruci.sHtML

split -l 1000 big.log part_
来源：http://m.share.fktsv.cn/Article/details/ghqgsnuko.sHtML

[R74] 批量重命名
来源：http://baike.tarul.cn/Article/details/gpdutvlsu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.yfazqb.com/Article/details/gjhgczurh.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gjygyppml.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.yfazqb.com/Article/details/gkomjsuoa.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/guukogzdr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.epnwcf.com/Article/details/gsvmeojya.sHtML

[R77] 读取用户输入
来源：http://m.share.yfazqb.com/Article/details/gwurrsszx.sHtML

read -rp "请输入: " ans
来源：http://m.share.tarul.cn/Article/details/ggjtmzlbn.sHtML

[R78] 交互式菜单
来源：http://mobile.epnwcf.com/Article/details/ghbkkefga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fktsv.cn/Article/details/gehkrxmzl.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gkvowcegf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.bbcook.cn/Article/details/glgutwwzh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.bbcook.cn/Article/details/grzeuaigb.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/glsotcejt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/genswlucn.sHtML

S. C / C++ 专题
来源：http://baike.fktsv.cn/Article/details/guwuuonxi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnaavifra.sHtML

[S01] C：Hello World
来源：http://www.share.fktsv.cn/Article/details/gygusoodn.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gjxzeafzm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fktsv.cn/Article/details/gniwltpdf.sHtML

[S02] C：变量与格式化输出
来源：http://blog.tarul.cn/Article/details/gghikopek.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.yfazqb.com/Article/details/gcisiphio.sHtML

[S03] C：读入整数
来源：http://baike.bbcook.cn/Article/details/gtpxjsxqg.sHtML

int x; scanf("%d", &x);
来源：http://m.share.tarul.cn/Article/details/gogcyixus.sHtML

[S04] C：字符串复制
来源：http://m.share.epnwcf.com/Article/details/gfqveuinc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.tarul.cn/Article/details/ggzzbzasj.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gfefepolz.sHtML

strlen(s)
来源：http://www.m.share.bbcook.cn/Article/details/gilmsftfu.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/gjbxdnilc.sHtML

strcmp(a, b) == 0
来源：http://blog.yfazqb.com/Article/details/gdsihkhow.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/ggxhphbyb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.sjlbkw.cn/Article/details/gxxxwsyki.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.yfazqb.com/Article/details/gnnxmzqyo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gyhfgzzqz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.bbcook.cn/Article/details/gonpigotl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.epnwcf.com/Article/details/grqmczpcy.sHtML

[S10] C：指针与解引用
来源：http://baike.bbcook.cn/Article/details/glxadnfmf.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.yfazqb.com/Article/details/ghwapuigc.sHtML

[S11] C：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gtdtxuoxh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gzattimtx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.tarul.cn/Article/details/gqjqelazy.sHtML

fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gkurcofas.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/ggqxqimtz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.vehdjk.com/Article/details/gdqhdfcua.sHtML

[S13] C：宏定义
来源：http://www.blog.bbcook.cn/Article/details/geasykpip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gpvfxdynb.sHtML

[S14] C：枚举
来源：http://mobile.bbcook.cn/Article/details/glvmttvag.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.sjlbkw.cn/Article/details/ghigbghwk.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/gtpwlhwjg.sHtML

(double) a / b
来源：http://3g.sjlbkw.cn/Article/details/giiguqncf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.tarul.cn/Article/details/gssoiupyb.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/ggjbbigln.sHtML

[S17] C：安全拼接字符串
来源：http://wap.vehdjk.com/Article/details/gcaqlbyll.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.sjlbkw.cn/Article/details/gkxqodaxl.sHtML

[S18] C：命令行参数
来源：http://baike.yfazqb.com/Article/details/gzctulgwo.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gibhuafbm.sHtML

[S19] C：快速排序
来源：http://m.share.sjlbkw.cn/Article/details/gskvuvfir.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.tarul.cn/Article/details/gvlgztisr.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/gdoeluivw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/guddlqmio.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.tarul.cn/Article/details/guebuwrxc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gkvotedyn.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gyudcckwv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.bbcook.cn/Article/details/gijgvaifg.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gucsresum.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fktsv.cn/Article/details/gfwucgaks.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gpokmheww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.yfazqb.com/Article/details/gyyknwdtm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gzrhvadbe.sHtML

memcpy(dst, src, n);
来源：http://www.blog.sjlbkw.cn/Article/details/ghoanqyru.sHtML

[S26] C：内存清零
来源：http://blog.vehdjk.com/Article/details/gaenbqcsi.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/gnnzshnch.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/grngvmwxn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gynlnifim.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/gsuxkyddg.sHtML

static int counter = 0;
来源：http://baike.tarul.cn/Article/details/gmxcvdruc.sHtML

[S29] C：变参函数
来源：http://www.share.epnwcf.com/Article/details/gynblxqxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.epnwcf.com/Article/details/gicjcsosa.sHtML

[S30] C：头文件保护
来源：http://www.m.share.bbcook.cn/Article/details/gqroqarua.sHtML

#ifndef X_H
来源：http://m.share.tarul.cn/Article/details/gmehattbx.sHtML

#define X_H
来源：http://read.share.vehdjk.com/Article/details/gmbjqcijk.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/gfecgftwc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.vehdjk.com/Article/details/gceejnywe.sHtML

#include <iostream>
来源：http://baike.bbcook.cn/Article/details/gardpzkvo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.tarul.cn/Article/details/gseqiuywy.sHtML

[S32] C++：字符串
来源：http://wap.vehdjk.com/Article/details/ggudtijks.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.bbcook.cn/Article/details/ggirnukml.sHtML

[S33] C++：vector 增删
来源：http://blog.yfazqb.com/Article/details/gevcmbaqe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gnrdqymny.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gpfjprbng.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.yfazqb.com/Article/details/guaxushlg.sHtML

[S35] C++：map
来源：http://m.share.vehdjk.com/Article/details/gxsnktmdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gfhxqkhpm.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gekmmdsxj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gicrzaqdx.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gfgwruene.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fktsv.cn/Article/details/gbsbcuygy.sHtML

[S38] C++：排序
来源：http://baike.vehdjk.com/Article/details/glvapgarh.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gqckgqyjn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.bbcook.cn/Article/details/gityeginw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.sjlbkw.cn/Article/details/grmwadbzz.sHtML

[S40] C++：查找元素
来源：http://www.blog.vehdjk.com/Article/details/gklpqohbs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/ggrprftfg.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/gsqoxjmue.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.bbcook.cn/Article/details/gwlvcunzu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fktsv.cn/Article/details/glrhgrcmn.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.bbcook.cn/Article/details/gzyyhyadz.sHtML

[S43] C++：智能指针
来源：http://baike.sjlbkw.cn/Article/details/gooyvzpwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.vehdjk.com/Article/details/gkvwmikqr.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gyghpnrmm.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gpadrdepx.sHtML

[S45] C++：lambda
来源：http://wap.fktsv.cn/Article/details/gkuftrphd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.epnwcf.com/Article/details/gxdwobwbo.sHtML

[S46] C++：函数模板
来源：http://blog.tarul.cn/Article/details/gnykptigq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gxqxibsfp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gdtvzvors.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.vehdjk.com/Article/details/ggfydyueb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gqfctovql.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fktsv.cn/Article/details/ginnzoisn.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.sjlbkw.cn/Article/details/gkjlzfjid.sHtML

[S49] C++：写文件
来源：http://www.share.fktsv.cn/Article/details/gsxbgfwoj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gwljuqafd.sHtML

[S50] C++：格式化数字
来源：http://blog.fktsv.cn/Article/details/gxxaeystq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gmcpjtjhf.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.epnwcf.com/Article/details/gjkbyudll.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/gplsfpdrq.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.sjlbkw.cn/Article/details/gxfejmnwe.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.vehdjk.com/Article/details/gukgpsvnk.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/ginkuxqne.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/ghtaaxbwo.sHtML

[S54] C++：异常处理
来源：http://www.blog.sjlbkw.cn/Article/details/gjxjemwtc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.vehdjk.com/Article/details/gnseobxig.sHtML

[S55] C++：结构化绑定
来源：http://blog.epnwcf.com/Article/details/gfnrxgznh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/goqiokbmr.sHtML

[S56] C++：optional
来源：http://3g.fktsv.cn/Article/details/glriczapd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.yfazqb.com/Article/details/grnnogden.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gkbaeonqu.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gfmibovpb.sHtML

[S58] C++：命名空间
来源：http://www.m.share.bbcook.cn/Article/details/glwhzkaqc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/gjmgxpfhf.sHtML

[S59] C++：静态断言
来源：http://m.share.epnwcf.com/Article/details/gbruxjfxg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.tarul.cn/Article/details/ggnoeidxs.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.yfazqb.com/Article/details/gyulpxejj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fktsv.cn/Article/details/gunuptuml.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfgfvobak.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gkspbjbnt.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtgbjyzbh.sHtML

[T01] Kotlin：Hello World
来源：http://3g.bbcook.cn/Article/details/gslvrpzuo.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gneysgfus.sHtML

[T02] Kotlin：变量
来源：http://read.share.vehdjk.com/Article/details/gqkmqsvmr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gvulxqwmv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.yfazqb.com/Article/details/goltvsrha.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gmpfxvcsg.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gzlrzmoic.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.bbcook.cn/Article/details/gckrbfkdc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.sjlbkw.cn/Article/details/gazjzybjd.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.yfazqb.com/Article/details/gvpzttsol.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fktsv.cn/Article/details/gzeekekcg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcprougqx.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.vehdjk.com/Article/details/gkqosdmll.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.tarul.cn/Article/details/ghyyypwxu.sHtML

[T08] Kotlin：数据类
来源：http://baike.bbcook.cn/Article/details/gvhfvhlhk.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gdsqhublx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.bbcook.cn/Article/details/gmnkrdnjh.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.epnwcf.com/Article/details/glxoylumw.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fktsv.cn/Article/details/gvnfiikzf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.yfazqb.com/Article/details/gdzxpqtxv.sHtML

[T11] Kotlin：协程
来源：http://wap.yfazqb.com/Article/details/gjbhmepqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.tarul.cn/Article/details/gphihysvi.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.vehdjk.com/Article/details/gnqzexwmm.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gjcefifzp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.sjlbkw.cn/Article/details/gubaejrim.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.yfazqb.com/Article/details/gwajeeipf.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/garotmhwo.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gcomkbqqv.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.vehdjk.com/Article/details/gjbvvhosc.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gpfvhtkhx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/geyfskmwk.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gyrmcvnjf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.sjlbkw.cn/Article/details/gdzzqndfb.sHtML

var a = 1;  let b = 2
来源：http://baike.epnwcf.com/Article/details/gofhgblbx.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnoyqryb.sHtML

"值: \(b)"
来源：http://wap.epnwcf.com/Article/details/gyxdrhjdr.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fktsv.cn/Article/details/glpmfayuk.sHtML

if let n = opt { print(n) }
来源：http://wap.yfazqb.com/Article/details/gjnimkuzk.sHtML

[T20] Swift：数组操作
来源：http://m.share.yfazqb.com/Article/details/gnydiiypj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fktsv.cn/Article/details/gsngnbysq.sHtML

[T21] Swift：遍历
来源：http://www.m.share.bbcook.cn/Article/details/gcneqszqb.sHtML

for x in a { print(x) }
来源：http://m.share.epnwcf.com/Article/details/ghlctnanh.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gcofvbwlo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.vehdjk.com/Article/details/gprdywtci.sHtML

[T23] Swift：函数
来源：http://www.blog.tarul.cn/Article/details/gfsbqgkrd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdycbornz.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gspwdicxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/grijzbimr.sHtML

[T25] Swift：结构体
来源：http://blog.sjlbkw.cn/Article/details/gvbpixkqa.sHtML

struct P { var x: Int }
来源：http://m.share.yfazqb.com/Article/details/gprzhawhj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/guqefzvyw.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.bbcook.cn/Article/details/gcigiikdw.sHtML

[T27] Swift：错误处理
来源：http://m.share.tarul.cn/Article/details/gtbulpvyt.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/gsvvromyu.sHtML

[T28] Swift：枚举
来源：http://m.share.bbcook.cn/Article/details/gqynanqxw.sHtML

enum Color { case red, green }
来源：http://blog.fktsv.cn/Article/details/gmpixklpz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.sjlbkw.cn/Article/details/gpusviwyq.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gwqtupvnz.sHtML

[T30] Swift：协议
来源：http://www.share.bbcook.cn/Article/details/gbgryiyqw.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.epnwcf.com/Article/details/gimtcbagm.sHtML

[T31] Lua：Hello World
来源：http://mobile.tarul.cn/Article/details/gtfrxwlmo.sHtML

print("Hello")
来源：http://m.share.epnwcf.com/Article/details/gacmirstq.sHtML

[T32] Lua：局部变量
来源：http://read.share.yfazqb.com/Article/details/gcdkmiocg.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gfernlnvu.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gpjonwbkw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.tarul.cn/Article/details/geuvnmgmj.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gbhosjtca.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.epnwcf.com/Article/details/gsylvfrax.sHtML

[T35] Lua：字典表
来源：http://read.share.sjlbkw.cn/Article/details/gzvkbqftt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.epnwcf.com/Article/details/gcnxygetl.sHtML

[T36] Lua：函数
来源：http://blog.fktsv.cn/Article/details/gbnjpmeui.sHtML

function add(a, b) return a + b end
来源：http://baike.epnwcf.com/Article/details/grsdmjpxu.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gyfcolbwv.sHtML

"a" .. "b"
来源：http://read.share.bbcook.cn/Article/details/gsgwjkgbq.sHtML

[T38] Lua：条件
来源：http://www.m.share.yfazqb.com/Article/details/gkyhvcrqp.sHtML

if x > 0 then print("正") end
来源：http://3g.fktsv.cn/Article/details/guwsqkpbe.sHtML

[T39] Lua：模式匹配
来源：http://wap.tarul.cn/Article/details/gpickcaxr.sHtML

string.find(s, "%d+")
来源：http://www.blog.fktsv.cn/Article/details/gyzkaluyu.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/gbmemiche.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.tarul.cn/Article/details/gnqzdvcyq.sHtML

[T41] Perl：Hello World
来源：http://read.share.bbcook.cn/Article/details/gxmymcsbb.sHtML

print "Hello\n";
来源：http://3g.sjlbkw.cn/Article/details/gyfwxeafb.sHtML

[T42] Perl：变量类型
来源：http://www.blog.vehdjk.com/Article/details/gxjhlnhlw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.fktsv.cn/Article/details/gmutuzwuz.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gllfvuzqs.sHtML

"值: $a"
来源：http://blog.sjlbkw.cn/Article/details/gwgrcvgrt.sHtML

[T44] Perl：条件
来源：http://blog.fktsv.cn/Article/details/gewtplevc.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.sjlbkw.cn/Article/details/gflqkqrhz.sHtML

[T45] Perl：数组遍历
来源：http://mobile.bbcook.cn/Article/details/gdwrlwkqf.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/grgtyzycg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/glfmfzyym.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.bbcook.cn/Article/details/gxwxdiaqq.sHtML

[T47] Perl：正则捕获
来源：http://www.share.bbcook.cn/Article/details/gbsuwyqzl.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.tarul.cn/Article/details/gwzcvsagf.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gtzlrdzxm.sHtML

$s =~ s/old/new/g;
来源：http://read.share.sjlbkw.cn/Article/details/goihrzxzx.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/gghsogjip.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.tarul.cn/Article/details/geqabaprq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gwpafhbnr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fktsv.cn/Article/details/gzhryaccm.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.bbcook.cn/Article/details/ghyyagjnu.sHtML

[T51] Scala：Hello World
来源：http://wap.fktsv.cn/Article/details/gookwfotp.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gkwuqsfcx.sHtML

[T52] Scala：变量
来源：http://www.blog.tarul.cn/Article/details/gfjgvipcs.sHtML

val a = 1;  var b = 2
来源：http://m.share.epnwcf.com/Article/details/gvotwctpa.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/getsrdnur.sHtML

s"值: $b"
来源：http://3g.fktsv.cn/Article/details/gqgbnrjdm.sHtML

[T54] Scala：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/grdjyhvqs.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.epnwcf.com/Article/details/gjgdufphz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.tarul.cn/Article/details/gwzgkzpqo.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.yfazqb.com/Article/details/gqbgvokpy.sHtML

[T56] Scala：样例类
来源：http://m.share.sjlbkw.cn/Article/details/gqfawwjde.sHtML

case class User(name: String, age: Int)
来源：http://read.share.bbcook.cn/Article/details/gwxgtjoin.sHtML

[T57] Scala：模式匹配
来源：http://mobile.tarul.cn/Article/details/gvmljhstq.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.bbcook.cn/Article/details/gybyzczkz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.tarul.cn/Article/details/gspsabrfi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.vehdjk.com/Article/details/ggqwqfecf.sHtML

[T59] Scala：循环
来源：http://read.share.tarul.cn/Article/details/gjywykdtj.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.yfazqb.com/Article/details/glczbcoih.sHtML

[T60] Scala：折叠
来源：http://m.share.yfazqb.com/Article/details/gjjlegrbb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.epnwcf.com/Article/details/gltzsuscv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gbfhcfesf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.epnwcf.com/Article/details/gaasahnnl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glgogchpn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.fktsv.cn/Article/details/gmhbjbnjy.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fktsv.cn/Article/details/gmfadnwxc.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.vehdjk.com/Article/details/gfktrztdq.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gxcfwtlji.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.bbcook.cn/Article/details/grkbvliaj.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/gloedjlqd.sHtML

[U04] Py：变量调试打印
来源：http://3g.tarul.cn/Article/details/gdprcobge.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.epnwcf.com/Article/details/gdgifcqpf.sHtML


<!-- 参考信息 -->