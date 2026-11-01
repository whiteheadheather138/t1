代发 wailian999

df -h;  du -sh *
来源：http://read.share.fktsv.cn/Article/details/gghtzlpkb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.bbcook.cn/Article/details/gkgwikdqc.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.vehdjk.com/Article/details/gbsdjzgwh.sHtML

[R63] 内存与进程
来源：http://mobile.yfazqb.com/Article/details/gstmxorkl.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.bbcook.cn/Article/details/gbtpftoln.sHtML

[R64] 结束进程
来源：http://www.m.share.yfazqb.com/Article/details/gxihxgxor.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.epnwcf.com/Article/details/gttbifupx.sHtML

[R65] 查看端口占用
来源：http://read.share.tarul.cn/Article/details/gmfjvxlvb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gstxxuukm.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/ggwxdavze.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.vehdjk.com/Article/details/gjnrvltcf.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.vehdjk.com/Article/details/grwjvipcm.sHtML

openssl rand -hex 16
来源：http://wap.tarul.cn/Article/details/gcbghtsru.sHtML

[R68] 计算文件校验值
来源：http://blog.fktsv.cn/Article/details/gkfkbbjhj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.vehdjk.com/Article/details/gbgawwiev.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gecbcexrs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.vehdjk.com/Article/details/gugbhpikb.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.tarul.cn/Article/details/gvvcfurcw.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gdzwoatqf.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gldxwjtrs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.tarul.cn/Article/details/goqgaignd.sHtML

[R72] 等待端口就绪
来源：http://m.share.epnwcf.com/Article/details/gqhflmgxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/gwjrqacgm.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gijzrosbx.sHtML

split -l 1000 big.log part_
来源：http://baike.fktsv.cn/Article/details/gttwtsbug.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gsotwsmnm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/gyeiburjv.sHtML

[R75] 导出环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gwujtfxsb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.epnwcf.com/Article/details/glatrbwvr.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gyppofhpa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gljsurrsw.sHtML

[R77] 读取用户输入
来源：http://wap.vehdjk.com/Article/details/gdundzxhe.sHtML

read -rp "请输入: " ans
来源：http://mobile.sjlbkw.cn/Article/details/ghidyzlak.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gxtkooghm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fktsv.cn/Article/details/gzrxqnpnn.sHtML

[R79] 解析命令行选项
来源：http://baike.fktsv.cn/Article/details/gvkdxpoxk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gpoebzjip.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gdshcrmqw.sHtML

time ./run.sh
来源：http://read.share.epnwcf.com/Article/details/ggrfenako.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtncsqgmo.sHtML

S. C / C++ 专题
来源：http://3g.sjlbkw.cn/Article/details/gcczzkklo.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glbofjvgm.sHtML

[S01] C：Hello World
来源：http://read.share.fktsv.cn/Article/details/gyyheobjk.sHtML

#include <stdio.h>
来源：http://baike.yfazqb.com/Article/details/gjizhuhma.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fktsv.cn/Article/details/gosupmaiy.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.epnwcf.com/Article/details/gyxzqrvlg.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.tarul.cn/Article/details/gsjxnpgse.sHtML

[S03] C：读入整数
来源：http://wap.bbcook.cn/Article/details/gymipeolq.sHtML

int x; scanf("%d", &x);
来源：http://blog.tarul.cn/Article/details/gklpexstm.sHtML

[S04] C：字符串复制
来源：http://www.share.sjlbkw.cn/Article/details/gedyiuwqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gjblipmqd.sHtML

[S05] C：字符串长度
来源：http://www.share.bbcook.cn/Article/details/gfikfrxkx.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gvavffzgl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gebgucxou.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gjfylhccu.sHtML

[S07] C：数组遍历求和
来源：http://wap.tarul.cn/Article/details/gznakxxex.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.epnwcf.com/Article/details/ghtrvugsi.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.epnwcf.com/Article/details/gpeykhgfh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.vehdjk.com/Article/details/gzenuugrw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gkualvucw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.sjlbkw.cn/Article/details/gkqobcogf.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gzryzbflc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.sjlbkw.cn/Article/details/gpgpvwzph.sHtML

[S11] C：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/gbsznjggm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.bbcook.cn/Article/details/gdurjzidr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.epnwcf.com/Article/details/glyxdoknu.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gcdrefpij.sHtML

[S12] C：写文件
来源：http://read.share.vehdjk.com/Article/details/gybuhphsu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gnhbnapkt.sHtML

[S13] C：宏定义
来源：http://m.share.vehdjk.com/Article/details/gpgyomdvm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.tarul.cn/Article/details/gudfculac.sHtML

[S14] C：枚举
来源：http://mobile.tarul.cn/Article/details/golcaqkea.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.sjlbkw.cn/Article/details/gwdrieloq.sHtML

[S15] C：类型转换
来源：http://blog.bbcook.cn/Article/details/gubnwldjd.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/gxwdqadkj.sHtML

[S16] C：位操作置位
来源：http://wap.vehdjk.com/Article/details/ggogqtips.sHtML

x |= (1 << 3);
来源：http://wap.fktsv.cn/Article/details/gldrqunlh.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gahfdzdlw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.epnwcf.com/Article/details/gbjrsrivf.sHtML

[S18] C：命令行参数
来源：http://baike.bbcook.cn/Article/details/gtnvqgwvf.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gbhclqsjz.sHtML

[S19] C：快速排序
来源：http://www.share.fktsv.cn/Article/details/gqjkjfoah.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.bbcook.cn/Article/details/gqvdxuaib.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/glhfdirvo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gmshqyytn.sHtML

[S21] C：字符类别判断
来源：http://blog.vehdjk.com/Article/details/gbqqtasbp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.tarul.cn/Article/details/gfjdgjwzw.sHtML

[S22] C：字符串转数字
来源：http://wap.vehdjk.com/Article/details/gchvywkjc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/gugbyeajw.sHtML

[S23] C：随机数
来源：http://blog.tarul.cn/Article/details/gacextnoo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gasuhhysq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gkqolfhck.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.tarul.cn/Article/details/ghqwnpfoq.sHtML

[S25] C：内存拷贝
来源：http://3g.yfazqb.com/Article/details/gfpxfjamg.sHtML

memcpy(dst, src, n);
来源：http://read.share.yfazqb.com/Article/details/gaqjtdtqg.sHtML

[S26] C：内存清零
来源：http://baike.sjlbkw.cn/Article/details/gjtsbkegf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.tarul.cn/Article/details/gldqbgycu.sHtML

[S27] C：定义常量
来源：http://wap.epnwcf.com/Article/details/gbbucxoqi.sHtML

const double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gfznhpcgv.sHtML

[S28] C：静态变量
来源：http://www.blog.epnwcf.com/Article/details/ggfmtuwau.sHtML

static int counter = 0;
来源：http://www.share.vehdjk.com/Article/details/gpbnhokrx.sHtML

[S29] C：变参函数
来源：http://blog.epnwcf.com/Article/details/gntdaalab.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fktsv.cn/Article/details/gbafztwzb.sHtML

[S30] C：头文件保护
来源：http://baike.vehdjk.com/Article/details/gxsbaysyc.sHtML

#ifndef X_H
来源：http://www.share.epnwcf.com/Article/details/gnisrpkls.sHtML

#define X_H
来源：http://www.blog.tarul.cn/Article/details/ggksptglt.sHtML

#endif
来源：http://read.share.epnwcf.com/Article/details/ggqbwjrmw.sHtML

[S31] C++：Hello World
来源：http://m.share.tarul.cn/Article/details/gjqxpheip.sHtML

#include <iostream>
来源：http://blog.sjlbkw.cn/Article/details/gzaujdbnc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.epnwcf.com/Article/details/gxauqksyw.sHtML

[S32] C++：字符串
来源：http://www.share.fktsv.cn/Article/details/gjwuxtfny.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.vehdjk.com/Article/details/gzujaxmgr.sHtML

[S33] C++：vector 增删
来源：http://m.share.fktsv.cn/Article/details/gruilzvaa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.vehdjk.com/Article/details/genkzzsfi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.bbcook.cn/Article/details/givagxwyq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.bbcook.cn/Article/details/gkyxjnlrv.sHtML

[S35] C++：map
来源：http://3g.epnwcf.com/Article/details/gjdjaldbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gcjddueac.sHtML

[S36] C++：unordered_map
来源：http://blog.fktsv.cn/Article/details/guoonxcww.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gianvhyig.sHtML

[S37] C++：set
来源：http://wap.tarul.cn/Article/details/grspgzkph.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.epnwcf.com/Article/details/ghkappoxk.sHtML

[S38] C++：排序
来源：http://read.share.sjlbkw.cn/Article/details/gmkpsdbrq.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/gvnuineru.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.vehdjk.com/Article/details/gcylnalod.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.bbcook.cn/Article/details/gnbagkfit.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gmsehpptu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/gurnktnvg.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gqlsymkfu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.tarul.cn/Article/details/gyqdumpjf.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gzlzubohw.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/geudeyjzr.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gwvxriqef.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.vehdjk.com/Article/details/gcfglgwaa.sHtML

[S44] C++：引用传参
来源：http://wap.bbcook.cn/Article/details/gybkjzyqw.sHtML

void inc(int &x) { ++x; }
来源：http://blog.vehdjk.com/Article/details/glrpcrhxy.sHtML

[S45] C++：lambda
来源：http://mobile.sjlbkw.cn/Article/details/gustakkye.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fktsv.cn/Article/details/gsqdrhvdg.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gzsiyvwbz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fktsv.cn/Article/details/gqboctvcv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/ggpiqcqzb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.vehdjk.com/Article/details/ggdwuoeum.sHtML

[S48] C++：逐行读文件
来源：http://wap.tarul.cn/Article/details/gkdvjnvme.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gkusqtvwc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.yfazqb.com/Article/details/gitlkfrhx.sHtML

[S49] C++：写文件
来源：http://mobile.vehdjk.com/Article/details/gifadtgul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.yfazqb.com/Article/details/gvgqapjur.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxfiujkb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.sjlbkw.cn/Article/details/gzqjksakp.sHtML

[S51] C++：显式类型转换
来源：http://3g.fktsv.cn/Article/details/gjmlmaxez.sHtML

static_cast<double>(a) / b
来源：http://read.share.vehdjk.com/Article/details/gddzcpccf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.yfazqb.com/Article/details/ggrhxskzo.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fktsv.cn/Article/details/gwftyzrhm.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/gzpnsxdwk.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.sjlbkw.cn/Article/details/gcglfjtuc.sHtML

[S54] C++：异常处理
来源：http://3g.bbcook.cn/Article/details/glbbzqevz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.sjlbkw.cn/Article/details/gtykkvywa.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fktsv.cn/Article/details/gryczjfyg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gykkprobm.sHtML

[S56] C++：optional
来源：http://www.blog.epnwcf.com/Article/details/gkigvctwd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/gjovtfgjq.sHtML

[S57] C++：编译期常量
来源：http://wap.vehdjk.com/Article/details/gapaomfey.sHtML

constexpr int N = 10;
来源：http://www.share.vehdjk.com/Article/details/gezxtgpsd.sHtML

[S58] C++：命名空间
来源：http://3g.epnwcf.com/Article/details/gvoastaih.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.tarul.cn/Article/details/goiwucsaj.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gicewxakn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.sjlbkw.cn/Article/details/gmsxcsshz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fktsv.cn/Article/details/gneqyvtvv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.sjlbkw.cn/Article/details/gfroqfwiu.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gukwcdkpg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/ghjkzbmnf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gmkbavzby.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gerzqknrb.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gewjtcnvj.sHtML

[T02] Kotlin：变量
来源：http://wap.yfazqb.com/Article/details/gfrubvoez.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gwfdghmkc.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.sjlbkw.cn/Article/details/glskwjxkf.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gmtmykzcy.sHtML

[T04] Kotlin：空安全
来源：http://wap.vehdjk.com/Article/details/gsfhlacvr.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/gjkyfgxdb.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.tarul.cn/Article/details/gltdyshlo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fktsv.cn/Article/details/gleqblulc.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.vehdjk.com/Article/details/ghrdrfuwy.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/gtvekpmku.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gkjajdykl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.vehdjk.com/Article/details/gpvpkzkqt.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.tarul.cn/Article/details/gnsofkcdt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.bbcook.cn/Article/details/glkpsdfmx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.yfazqb.com/Article/details/guydrcevl.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.yfazqb.com/Article/details/gsqhjggnj.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.vehdjk.com/Article/details/ghmdzkmvx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fktsv.cn/Article/details/gdkuiowjz.sHtML

[T11] Kotlin：协程
来源：http://mobile.tarul.cn/Article/details/gioqoayye.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/ghrtquypr.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.bbcook.cn/Article/details/gxuquhzpx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gyegxyomr.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.sjlbkw.cn/Article/details/gcosvjwxg.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fktsv.cn/Article/details/gfazbicez.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gblbcnvca.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.yfazqb.com/Article/details/gygmadhps.sHtML

[T15] Kotlin：接口
来源：http://read.share.bbcook.cn/Article/details/gnjbofvwa.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/grevxkztx.sHtML

[T16] Swift：Hello World
来源：http://www.blog.vehdjk.com/Article/details/gnyqapawt.sHtML

print("Hello")
来源：http://m.share.sjlbkw.cn/Article/details/gcoqqcevi.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gzytwcavk.sHtML

var a = 1;  let b = 2
来源：http://blog.fktsv.cn/Article/details/gieuqdfnw.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gefvuyivb.sHtML

"值: \(b)"
来源：http://www.m.share.yfazqb.com/Article/details/geaxknovq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.sjlbkw.cn/Article/details/gwbahwpmj.sHtML

if let n = opt { print(n) }
来源：http://wap.bbcook.cn/Article/details/gnrkqqguz.sHtML

[T20] Swift：数组操作
来源：http://wap.tarul.cn/Article/details/gpifxdyjo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gxqkzeogh.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gufkghlcl.sHtML

for x in a { print(x) }
来源：http://m.share.vehdjk.com/Article/details/gczecghvb.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gdwzuhdup.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.sjlbkw.cn/Article/details/gfdwecnsr.sHtML

[T23] Swift：函数
来源：http://3g.bbcook.cn/Article/details/genmxdkoo.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.vehdjk.com/Article/details/gozrqacdh.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gwkmctslq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.bbcook.cn/Article/details/ggijeoukn.sHtML

[T25] Swift：结构体
来源：http://m.share.epnwcf.com/Article/details/gtpxfabop.sHtML

struct P { var x: Int }
来源：http://wap.bbcook.cn/Article/details/gnzfvztch.sHtML

[T26] Swift：类与重写
来源：http://read.share.bbcook.cn/Article/details/ghaxvcdjm.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.vehdjk.com/Article/details/gxuvixkej.sHtML

[T27] Swift：错误处理
来源：http://wap.sjlbkw.cn/Article/details/gxqpxeoot.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.yfazqb.com/Article/details/gkjrxmihp.sHtML

[T28] Swift：枚举
来源：http://blog.yfazqb.com/Article/details/gzoksbdvd.sHtML

enum Color { case red, green }
来源：http://blog.sjlbkw.cn/Article/details/giuasjiit.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gguzxlxug.sHtML

guard let x = opt else { return }
来源：http://mobile.tarul.cn/Article/details/grwecgvbg.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/ggecrrmlg.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.tarul.cn/Article/details/gytfzangp.sHtML

[T31] Lua：Hello World
来源：http://blog.bbcook.cn/Article/details/gogrolzex.sHtML

print("Hello")
来源：http://3g.epnwcf.com/Article/details/gemlqpxoq.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.tarul.cn/Article/details/gviylzhac.sHtML

local a = 1
来源：http://www.share.tarul.cn/Article/details/gayiocloa.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.tarul.cn/Article/details/gvyudyvpr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.sjlbkw.cn/Article/details/gzvcghehp.sHtML

[T34] Lua：遍历表
来源：http://m.share.sjlbkw.cn/Article/details/gqcrtquvp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/gvsqhuomx.sHtML

[T35] Lua：字典表
来源：http://www.blog.fktsv.cn/Article/details/gkdbyzqbb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fktsv.cn/Article/details/gzccbexbo.sHtML

[T36] Lua：函数
来源：http://m.share.sjlbkw.cn/Article/details/gczlfjcgo.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/glqppowzr.sHtML

[T37] Lua：字符串拼接
来源：http://baike.tarul.cn/Article/details/gjzfbofcx.sHtML

"a" .. "b"
来源：http://www.blog.yfazqb.com/Article/details/glhgdrcnn.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gxmizpypc.sHtML

if x > 0 then print("正") end
来源：http://read.share.fktsv.cn/Article/details/gohnmhigh.sHtML

[T39] Lua：模式匹配
来源：http://baike.fktsv.cn/Article/details/ghseswwze.sHtML

string.find(s, "%d+")
来源：http://mobile.fktsv.cn/Article/details/gtxdelxjm.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/gczbpzyqq.sHtML

setmetatable({}, { __index = base })
来源：http://blog.epnwcf.com/Article/details/gkotzuybt.sHtML

[T41] Perl：Hello World
来源：http://read.share.sjlbkw.cn/Article/details/goujhcwgw.sHtML

print "Hello\n";
来源：http://m.share.bbcook.cn/Article/details/gvrhegjmd.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.vehdjk.com/Article/details/gqvgphmkq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.epnwcf.com/Article/details/ghdnuftea.sHtML

[T43] Perl：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/gizetljfg.sHtML

"值: $a"
来源：http://m.share.sjlbkw.cn/Article/details/gllnuzczq.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/ghhhhfvuy.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.vehdjk.com/Article/details/gsdmzysut.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gqbvwwfia.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gxwjkdvbn.sHtML

[T46] Perl：哈希操作
来源：http://read.share.bbcook.cn/Article/details/gkousteqr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.vehdjk.com/Article/details/gzksesani.sHtML

[T47] Perl：正则捕获
来源：http://wap.bbcook.cn/Article/details/gigkutchh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkqwpgwe.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/grccljwun.sHtML

$s =~ s/old/new/g;
来源：http://read.share.tarul.cn/Article/details/gyupukghz.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/grpunzuxb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.sjlbkw.cn/Article/details/gnupklyof.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gokbqprwa.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/ggnheezgx.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gchrdpeym.sHtML

[T51] Scala：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gflvjcdfo.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/gyeqjmjic.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gnjjoqecw.sHtML

val a = 1;  var b = 2
来源：http://read.share.tarul.cn/Article/details/gbcslvpdp.sHtML

[T53] Scala：字符串插值
来源：http://3g.vehdjk.com/Article/details/ghhnoaupy.sHtML

s"值: $b"
来源：http://blog.sjlbkw.cn/Article/details/gxkjwudpd.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gjnlhullv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.yfazqb.com/Article/details/gmsqlfjsu.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gkhnruemf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.vehdjk.com/Article/details/gzmsybwjp.sHtML

[T56] Scala：样例类
来源：http://www.blog.tarul.cn/Article/details/grsaefuug.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gplrmgpmv.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gqmtxzrrd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.bbcook.cn/Article/details/gtxfjbegt.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.tarul.cn/Article/details/geoeuiyxr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.sjlbkw.cn/Article/details/geoukglju.sHtML

[T59] Scala：循环
来源：http://mobile.bbcook.cn/Article/details/gcyodyhil.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/guonzewus.sHtML

[T60] Scala：折叠
来源：http://www.share.tarul.cn/Article/details/gleuyutev.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fktsv.cn/Article/details/ggecvulni.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvfkposzt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.tarul.cn/Article/details/geczrlfzx.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwsvxapmk.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/gjxcmdqdu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.sjlbkw.cn/Article/details/gawjymilr.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.bbcook.cn/Article/details/gmrjkrito.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.bbcook.cn/Article/details/ggpmavocd.sHtML


<!-- 参考信息 -->