代发 wailian999

ssh user@host 'uptime'
来源：http://wap.vehdjk.com/Article/details/goxkpkutf.sHtML

[R58] 下载文件
来源：http://wap.sjlbkw.cn/Article/details/gwpksotbe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gkwpjoffm.sHtML

[R59] 发 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gwwkjgtbe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fktsv.cn/Article/details/gbspuxmjr.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/gdvgmevez.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.vehdjk.com/Article/details/gvnsbmpdi.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/guxwrxrot.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gsmsxugoa.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gjjzfkvzs.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.bbcook.cn/Article/details/gbuwawpaq.sHtML

[R63] 内存与进程
来源：http://m.share.tarul.cn/Article/details/ghxrwatmp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gdqkmnnoa.sHtML

[R64] 结束进程
来源：http://mobile.sjlbkw.cn/Article/details/grnnxgjlo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gbunnoapf.sHtML

[R65] 查看端口占用
来源：http://www.m.share.yfazqb.com/Article/details/gmvemrqop.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.sjlbkw.cn/Article/details/gvuorbeoc.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/geyhjrphy.sHtML

crontab -e;  crontab -l
来源：http://read.share.epnwcf.com/Article/details/gapxspxcx.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gxpqmdawl.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gqoygedlv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.sjlbkw.cn/Article/details/gqesyauou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fktsv.cn/Article/details/gqhaojbex.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gcvzcmfxy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.yfazqb.com/Article/details/gsnnuivfh.sHtML

[R70] 时间戳与互转
来源：http://baike.fktsv.cn/Article/details/gswumrlms.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fktsv.cn/Article/details/gsqeckemp.sHtML

[R71] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gybngvvvj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gqqqzzayh.sHtML

[R72] 等待端口就绪
来源：http://wap.yfazqb.com/Article/details/godikylna.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gllvosqru.sHtML

[R73] 分割大日志
来源：http://wap.vehdjk.com/Article/details/gkhofcprc.sHtML

split -l 1000 big.log part_
来源：http://blog.sjlbkw.cn/Article/details/gqkxdxtkt.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gizbnjisr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/golcmpkkg.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/gbylqtqfg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.bbcook.cn/Article/details/gllroxebg.sHtML

[R76] 使用临时文件
来源：http://read.share.tarul.cn/Article/details/gpdngzdhw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.vehdjk.com/Article/details/gcyccplsk.sHtML

[R77] 读取用户输入
来源：http://3g.tarul.cn/Article/details/gfwzlixhp.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gixqnsziq.sHtML

[R78] 交互式菜单
来源：http://www.share.epnwcf.com/Article/details/gwlufwwmq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.bbcook.cn/Article/details/gbouzszjs.sHtML

[R79] 解析命令行选项
来源：http://wap.epnwcf.com/Article/details/gecwvrexo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.yfazqb.com/Article/details/gxmogpbay.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.vehdjk.com/Article/details/gqkqwjemo.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gykiemrte.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gerzzpujh.sHtML

S. C / C++ 专题
来源：http://3g.bbcook.cn/Article/details/gyaiwgklc.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzderxnxw.sHtML

[S01] C：Hello World
来源：http://wap.fktsv.cn/Article/details/gtidtxyhk.sHtML

#include <stdio.h>
来源：http://www.m.share.vehdjk.com/Article/details/gmkuijssf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gajjacbjz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gdxrdemok.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.vehdjk.com/Article/details/gyeiuvkzu.sHtML

[S03] C：读入整数
来源：http://blog.sjlbkw.cn/Article/details/gpdhgqhok.sHtML

int x; scanf("%d", &x);
来源：http://baike.sjlbkw.cn/Article/details/goianoapi.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gbijblcwc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.bbcook.cn/Article/details/gtxugpyty.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/ghohsffzd.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gyhomivhj.sHtML

[S06] C：字符串比较
来源：http://m.share.bbcook.cn/Article/details/grngmxaar.sHtML

strcmp(a, b) == 0
来源：http://blog.fktsv.cn/Article/details/ghftyoclv.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gufjnylxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gducijtep.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/grcrssrlx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.vehdjk.com/Article/details/gscnnbzjh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.sjlbkw.cn/Article/details/gncibdpet.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.vehdjk.com/Article/details/gctoocwuc.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gkzpqgzvm.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiouepmz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/gumaikdxk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.sjlbkw.cn/Article/details/gppivtdui.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.tarul.cn/Article/details/gxkihmsob.sHtML

fclose(f);
来源：http://m.share.fktsv.cn/Article/details/gufuwfucf.sHtML

[S12] C：写文件
来源：http://m.share.fktsv.cn/Article/details/gxazwpqyv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/ggmnddaeb.sHtML

[S13] C：宏定义
来源：http://read.share.yfazqb.com/Article/details/ggfqouwfl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gatolnqik.sHtML

[S14] C：枚举
来源：http://wap.vehdjk.com/Article/details/giqqgadaf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fktsv.cn/Article/details/giuwahysx.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gomntuoxg.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/ggiyfmnqj.sHtML

[S16] C：位操作置位
来源：http://www.m.share.bbcook.cn/Article/details/gybqdgiie.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gjfuzntnr.sHtML

[S17] C：安全拼接字符串
来源：http://baike.vehdjk.com/Article/details/gtlriskaz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fktsv.cn/Article/details/gsinlcypk.sHtML

[S18] C：命令行参数
来源：http://mobile.bbcook.cn/Article/details/guxqqryrv.sHtML

int main(int argc, char **argv)
来源：http://www.blog.yfazqb.com/Article/details/gfzqejejw.sHtML

[S19] C：快速排序
来源：http://read.share.yfazqb.com/Article/details/gykvodhbb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.bbcook.cn/Article/details/gzomauooe.sHtML

[S20] C：二分查找
来源：http://m.share.tarul.cn/Article/details/gryclsprk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/gqlkhubdz.sHtML

[S21] C：字符类别判断
来源：http://mobile.vehdjk.com/Article/details/glsqneodp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.vehdjk.com/Article/details/gpxqawlac.sHtML

[S22] C：字符串转数字
来源：http://3g.epnwcf.com/Article/details/gwzyrzfwk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.tarul.cn/Article/details/gqztvdrwc.sHtML

[S23] C：随机数
来源：http://www.share.sjlbkw.cn/Article/details/gxayqyawp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.epnwcf.com/Article/details/guyozsaxj.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gnpikfszp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.sjlbkw.cn/Article/details/gtmmkbgoh.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzxeiukk.sHtML

memcpy(dst, src, n);
来源：http://wap.sjlbkw.cn/Article/details/gnifhvtit.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/gvvacknxg.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.tarul.cn/Article/details/gbxgkvqac.sHtML

[S27] C：定义常量
来源：http://mobile.fktsv.cn/Article/details/gxmbsoyye.sHtML

const double PI = 3.14159;
来源：http://baike.fktsv.cn/Article/details/gnybzbtxo.sHtML

[S28] C：静态变量
来源：http://blog.bbcook.cn/Article/details/gwqkhwhrb.sHtML

static int counter = 0;
来源：http://m.share.tarul.cn/Article/details/gyajciuxz.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/guonxvmim.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gyzfjaern.sHtML

[S30] C：头文件保护
来源：http://blog.epnwcf.com/Article/details/grhfaqzts.sHtML

#ifndef X_H
来源：http://wap.vehdjk.com/Article/details/gqoionrtp.sHtML

#define X_H
来源：http://mobile.bbcook.cn/Article/details/gfsopwgbx.sHtML

#endif
来源：http://3g.epnwcf.com/Article/details/gklbrcebk.sHtML

[S31] C++：Hello World
来源：http://3g.epnwcf.com/Article/details/gcgpunnwm.sHtML

#include <iostream>
来源：http://read.share.tarul.cn/Article/details/gjwgaqkup.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdpxhhlwk.sHtML

[S32] C++：字符串
来源：http://blog.fktsv.cn/Article/details/gdzmdnxev.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.vehdjk.com/Article/details/gdhsetysc.sHtML

[S33] C++：vector 增删
来源：http://wap.fktsv.cn/Article/details/gjwpbdvdc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.bbcook.cn/Article/details/gihmynjyy.sHtML

[S34] C++：遍历 vector
来源：http://baike.yfazqb.com/Article/details/gcqxtrbkq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.bbcook.cn/Article/details/gmvzmjygv.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/grvhatoyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fktsv.cn/Article/details/gakzwccpt.sHtML

[S36] C++：unordered_map
来源：http://www.share.fktsv.cn/Article/details/guhrnkyrc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.tarul.cn/Article/details/gblpggvpy.sHtML

[S37] C++：set
来源：http://www.m.share.yfazqb.com/Article/details/grotcyubs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.sjlbkw.cn/Article/details/gqvftwgax.sHtML

[S38] C++：排序
来源：http://www.m.share.tarul.cn/Article/details/gtincnpbb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fktsv.cn/Article/details/gowjtzesj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.sjlbkw.cn/Article/details/gguxisjkw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.tarul.cn/Article/details/gmzsgvtvt.sHtML

[S40] C++：查找元素
来源：http://baike.fktsv.cn/Article/details/gzdawacwa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.tarul.cn/Article/details/gqssxeexx.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.epnwcf.com/Article/details/gynnncdio.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.epnwcf.com/Article/details/gjqetdhbe.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.tarul.cn/Article/details/gdgopopdq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fktsv.cn/Article/details/gwgzreuvj.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gzhrqiizq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.vehdjk.com/Article/details/gedllcqfa.sHtML

[S44] C++：引用传参
来源：http://read.share.bbcook.cn/Article/details/gfafmrifh.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fktsv.cn/Article/details/gcbbkjkjr.sHtML

[S45] C++：lambda
来源：http://read.share.tarul.cn/Article/details/gwsczjasd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.sjlbkw.cn/Article/details/glnkofaqc.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gsrcwghtj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.yfazqb.com/Article/details/gvsnkwsls.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.epnwcf.com/Article/details/gyhhkbccg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/gacgqmeto.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gqfivndmg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.yfazqb.com/Article/details/gpajbwdti.sHtML

while (std::getline(in, line)) { }
来源：http://baike.bbcook.cn/Article/details/gvndlfuzz.sHtML

[S49] C++：写文件
来源：http://read.share.epnwcf.com/Article/details/gxihzjvyv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fktsv.cn/Article/details/ggrqjtpvy.sHtML

[S50] C++：格式化数字
来源：http://blog.tarul.cn/Article/details/gqakvvxeb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.epnwcf.com/Article/details/glumwnkda.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.bbcook.cn/Article/details/gobkwarjw.sHtML

static_cast<double>(a) / b
来源：http://mobile.bbcook.cn/Article/details/gdidawwgk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.tarul.cn/Article/details/gvweavyac.sHtML

int size() const noexcept { return n_; }
来源：http://blog.yfazqb.com/Article/details/gcqjgsddx.sHtML

[S53] C++：移动语义
来源：http://blog.epnwcf.com/Article/details/ggzeoungf.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/grnwwococ.sHtML

[S54] C++：异常处理
来源：http://mobile.bbcook.cn/Article/details/giwhcgzev.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.sjlbkw.cn/Article/details/gzwmteeiv.sHtML

[S55] C++：结构化绑定
来源：http://baike.sjlbkw.cn/Article/details/gttiomdey.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.tarul.cn/Article/details/gajvfouxl.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gtbzaenxt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gtzdvddal.sHtML

[S57] C++：编译期常量
来源：http://blog.sjlbkw.cn/Article/details/gzhetzssh.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/grcveccwn.sHtML

[S58] C++：命名空间
来源：http://wap.tarul.cn/Article/details/gcavwybwj.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.tarul.cn/Article/details/ggeodccjg.sHtML

[S59] C++：静态断言
来源：http://www.m.share.tarul.cn/Article/details/gfwrjgwyi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.vehdjk.com/Article/details/gaiwjbuxl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gibwlqexh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.yfazqb.com/Article/details/glmmxsqjs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqjlgvmeg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gxjsnzpht.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ggghjdkfv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/geqbghrro.sHtML

println("Hello")
来源：http://www.m.share.bbcook.cn/Article/details/gxiqffyhq.sHtML

[T02] Kotlin：变量
来源：http://baike.yfazqb.com/Article/details/gtkydgjof.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.yfazqb.com/Article/details/grgurcprq.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.sjlbkw.cn/Article/details/gyzzwusap.sHtML

"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gkhhekpel.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.epnwcf.com/Article/details/gnwippjrd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.yfazqb.com/Article/details/grgonngcm.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.yfazqb.com/Article/details/gdyenehdr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.tarul.cn/Article/details/gpocvcgao.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gqiwllhlf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.vehdjk.com/Article/details/gaxtngtyv.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.epnwcf.com/Article/details/gqtgnlueu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gntpezlml.sHtML

[T08] Kotlin：数据类
来源：http://3g.yfazqb.com/Article/details/glhvwvnlj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.epnwcf.com/Article/details/gxntcnadz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.yfazqb.com/Article/details/gjcfmdxlu.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fktsv.cn/Article/details/ggscxyraw.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.epnwcf.com/Article/details/gzhxxdmhc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.bbcook.cn/Article/details/goxpadtok.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.vehdjk.com/Article/details/gepmtajvd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.bbcook.cn/Article/details/ghbfvgcnt.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gspwxwttq.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gwhdzotgj.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.sjlbkw.cn/Article/details/gcwacitur.sHtML

val m = mapOf("a" to 1)
来源：http://baike.bbcook.cn/Article/details/gwfuehdnv.sHtML

[T14] Kotlin：循环
来源：http://m.share.tarul.cn/Article/details/gdusvyfxz.sHtML

for (i in 1..10) println(i)
来源：http://mobile.bbcook.cn/Article/details/glnhzjpol.sHtML

[T15] Kotlin：接口
来源：http://baike.fktsv.cn/Article/details/gucjxyuck.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.vehdjk.com/Article/details/gvuxtgrjs.sHtML

[T16] Swift：Hello World
来源：http://m.share.tarul.cn/Article/details/gyjbpwrqc.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gckpcijgi.sHtML

[T17] Swift：变量与常量
来源：http://mobile.tarul.cn/Article/details/gheugtssd.sHtML

var a = 1;  let b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gnrrybxpc.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gghlqgjht.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gsvxanwox.sHtML

[T19] Swift：可选绑定
来源：http://www.share.vehdjk.com/Article/details/gidxpmbrg.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gymzpiqmm.sHtML

[T20] Swift：数组操作
来源：http://mobile.yfazqb.com/Article/details/gqynoxwic.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.bbcook.cn/Article/details/gubjdtbbg.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fktsv.cn/Article/details/gxvwslwcw.sHtML

for x in a { print(x) }
来源：http://mobile.vehdjk.com/Article/details/ghunyhwpz.sHtML

[T22] Swift：字典
来源：http://m.share.tarul.cn/Article/details/glaftqadw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.epnwcf.com/Article/details/gumwyhtcs.sHtML

[T23] Swift：函数
来源：http://wap.sjlbkw.cn/Article/details/gckcjpgsa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fktsv.cn/Article/details/gzevwnmii.sHtML

[T24] Swift：闭包
来源：http://m.share.bbcook.cn/Article/details/gpmzopquq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.vehdjk.com/Article/details/gpzfhnumu.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/gsfbegneo.sHtML

struct P { var x: Int }
来源：http://wap.yfazqb.com/Article/details/goeombetp.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/grvnoirht.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fktsv.cn/Article/details/guyhjvfwr.sHtML

[T27] Swift：错误处理
来源：http://read.share.epnwcf.com/Article/details/ghwauwhsz.sHtML

do { try f() } catch { print(error) }
来源：http://3g.sjlbkw.cn/Article/details/gdhcpchad.sHtML

[T28] Swift：枚举
来源：http://mobile.tarul.cn/Article/details/gpanbptfc.sHtML

enum Color { case red, green }
来源：http://www.blog.vehdjk.com/Article/details/gucivupbx.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.bbcook.cn/Article/details/gtpkzxuqb.sHtML

guard let x = opt else { return }
来源：http://m.share.yfazqb.com/Article/details/giqpnqube.sHtML

[T30] Swift：协议
来源：http://baike.yfazqb.com/Article/details/gaqsqmygi.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.sjlbkw.cn/Article/details/gfvyqmzwx.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gmlwatuiv.sHtML

print("Hello")
来源：http://www.share.fktsv.cn/Article/details/gmhdkegrm.sHtML

[T32] Lua：局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gdbkikkjl.sHtML

local a = 1
来源：http://www.m.share.epnwcf.com/Article/details/gwqehcohh.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.yfazqb.com/Article/details/gmfnbbfws.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.epnwcf.com/Article/details/gnzyfaxas.sHtML

[T34] Lua：遍历表
来源：http://www.share.fktsv.cn/Article/details/ggrjusgmh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.vehdjk.com/Article/details/gdrjbtdow.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gduneqofh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.vehdjk.com/Article/details/gypeefrbf.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gshjhnqcy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwiykvsi.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.bbcook.cn/Article/details/gmcdacqsw.sHtML

"a" .. "b"
来源：http://blog.fktsv.cn/Article/details/gvuejwrdw.sHtML

[T38] Lua：条件
来源：http://3g.yfazqb.com/Article/details/gdwsthsfp.sHtML

if x > 0 then print("正") end
来源：http://m.share.yfazqb.com/Article/details/gfmqkqxoj.sHtML

[T39] Lua：模式匹配
来源：http://read.share.yfazqb.com/Article/details/gaujbuheh.sHtML

string.find(s, "%d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gdvijoixw.sHtML

[T40] Lua：元表
来源：http://blog.fktsv.cn/Article/details/gleeshkqg.sHtML

setmetatable({}, { __index = base })
来源：http://baike.yfazqb.com/Article/details/gzorbokod.sHtML

[T41] Perl：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gfadhqrju.sHtML

print "Hello\n";
来源：http://wap.vehdjk.com/Article/details/gauqqzuri.sHtML

[T42] Perl：变量类型
来源：http://mobile.epnwcf.com/Article/details/gzpgsnhmc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.yfazqb.com/Article/details/gvhlzycot.sHtML

[T43] Perl：字符串插值
来源：http://blog.fktsv.cn/Article/details/gbgnthdpx.sHtML

"值: $a"
来源：http://www.blog.tarul.cn/Article/details/gifhcnhlc.sHtML

[T44] Perl：条件
来源：http://wap.yfazqb.com/Article/details/glrcjxkmm.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.sjlbkw.cn/Article/details/guzggkjiv.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fktsv.cn/Article/details/gdrkvhxse.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.fktsv.cn/Article/details/gsbhaqafd.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/gwqaobcvg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.tarul.cn/Article/details/gcaoyposv.sHtML

[T47] Perl：正则捕获
来源：http://3g.bbcook.cn/Article/details/ghornqrwo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fktsv.cn/Article/details/gfvigzoui.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gbucfehgu.sHtML

$s =~ s/old/new/g;
来源：http://m.share.vehdjk.com/Article/details/gdjsijdzm.sHtML

[T49] Perl：函数
来源：http://blog.bbcook.cn/Article/details/gjvkuniwh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gvtsnnnqo.sHtML

[T50] Perl：逐行读文件
来源：http://3g.epnwcf.com/Article/details/golknfuwn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/gdqtyauqr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.bbcook.cn/Article/details/gkpunzmvi.sHtML

[T51] Scala：Hello World
来源：http://wap.epnwcf.com/Article/details/gjcvilfmx.sHtML

println("Hello")
来源：http://mobile.bbcook.cn/Article/details/gyskqnyog.sHtML

[T52] Scala：变量
来源：http://3g.vehdjk.com/Article/details/gqtlbftwq.sHtML

val a = 1;  var b = 2
来源：http://read.share.epnwcf.com/Article/details/gewfcsfey.sHtML

[T53] Scala：字符串插值
来源：http://wap.bbcook.cn/Article/details/gkoiwtvll.sHtML

s"值: $b"
来源：http://3g.sjlbkw.cn/Article/details/guohdsewf.sHtML

[T54] Scala：集合映射
来源：http://blog.vehdjk.com/Article/details/gomfaukrg.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/govqyronc.sHtML

[T55] Scala：集合过滤
来源：http://wap.fktsv.cn/Article/details/gpgmlxuod.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.epnwcf.com/Article/details/geaxmmlly.sHtML

[T56] Scala：样例类
来源：http://mobile.bbcook.cn/Article/details/giddalngg.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuphdjbb.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gkbvrpiji.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/gkvggcblt.sHtML

[T58] Scala：函数定义
来源：http://blog.bbcook.cn/Article/details/gwkhqlksi.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.yfazqb.com/Article/details/gadqctndg.sHtML

[T59] Scala：循环
来源：http://baike.tarul.cn/Article/details/glkvaoxoj.sHtML

for (i <- 1 to 10) println(i)
来源：http://wap.epnwcf.com/Article/details/gajfbvfjn.sHtML

[T60] Scala：折叠
来源：http://mobile.sjlbkw.cn/Article/details/gqyhzzzqx.sHtML


<!-- 参考信息 -->