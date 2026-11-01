代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gmzdmbvlo.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gxiubxqnr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.sjlbkw.cn/Article/details/gmxmnrety.sHtML

[R61] 磁盘占用
来源：http://baike.tarul.cn/Article/details/gehfpvvjs.sHtML

df -h;  du -sh *
来源：http://www.m.share.tarul.cn/Article/details/grnmvtwng.sHtML

[R62] 找最占空间的文件
来源：http://blog.tarul.cn/Article/details/gqbextjal.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.yfazqb.com/Article/details/ghauxvnge.sHtML

[R63] 内存与进程
来源：http://mobile.tarul.cn/Article/details/gnikjznad.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.sjlbkw.cn/Article/details/giiwcghns.sHtML

[R64] 结束进程
来源：http://www.share.fktsv.cn/Article/details/gsuizvcyl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.tarul.cn/Article/details/geievybpk.sHtML

[R65] 查看端口占用
来源：http://wap.bbcook.cn/Article/details/gqikqntoc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.tarul.cn/Article/details/grchcitwt.sHtML

[R66] 定时任务
来源：http://m.share.bbcook.cn/Article/details/gqshdhvji.sHtML

crontab -e;  crontab -l
来源：http://read.share.vehdjk.com/Article/details/gegmyxdza.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.vehdjk.com/Article/details/gkidsvzfl.sHtML

openssl rand -hex 16
来源：http://wap.fktsv.cn/Article/details/gmbmulgvi.sHtML

[R68] 计算文件校验值
来源：http://3g.yfazqb.com/Article/details/gmmsitngh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.tarul.cn/Article/details/gebgdqppd.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/gljpfujjz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fktsv.cn/Article/details/grroczlfm.sHtML

[R70] 时间戳与互转
来源：http://m.share.fktsv.cn/Article/details/ggazkanjh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.sjlbkw.cn/Article/details/ghahsdrpa.sHtML

[R71] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/goslggvlm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.tarul.cn/Article/details/geqhppaab.sHtML

[R72] 等待端口就绪
来源：http://blog.yfazqb.com/Article/details/gqgfcfbpz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gijgwuoyx.sHtML

[R73] 分割大日志
来源：http://blog.epnwcf.com/Article/details/gvininesq.sHtML

split -l 1000 big.log part_
来源：http://baike.epnwcf.com/Article/details/gfmlctmzu.sHtML

[R74] 批量重命名
来源：http://read.share.tarul.cn/Article/details/gtayhwxih.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gqcvxagwv.sHtML

[R75] 导出环境变量
来源：http://3g.fktsv.cn/Article/details/gxkhiuzao.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.yfazqb.com/Article/details/gjlyyzjih.sHtML

[R76] 使用临时文件
来源：http://blog.fktsv.cn/Article/details/ggztwvgtk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.vehdjk.com/Article/details/gghlgrfbl.sHtML

[R77] 读取用户输入
来源：http://www.blog.bbcook.cn/Article/details/gegpbxfia.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.yfazqb.com/Article/details/gqjgusehh.sHtML

[R78] 交互式菜单
来源：http://www.m.share.yfazqb.com/Article/details/gdyirmbkw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.sjlbkw.cn/Article/details/gajwwxldj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fktsv.cn/Article/details/ghagkmcxj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.yfazqb.com/Article/details/gvblindxi.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fktsv.cn/Article/details/gyjcyfdzw.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gzfipvojm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glvgafngq.sHtML

S. C / C++ 专题
来源：http://m.share.sjlbkw.cn/Article/details/gdwxvmhxk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gjybbuoxj.sHtML

[S01] C：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gzoitybip.sHtML

#include <stdio.h>
来源：http://read.share.vehdjk.com/Article/details/gediiyncm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.tarul.cn/Article/details/gdkoatwgi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.yfazqb.com/Article/details/gmkctwyph.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.epnwcf.com/Article/details/gdiobguyi.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/gokfztkkt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.vehdjk.com/Article/details/grhweoxhg.sHtML

[S04] C：字符串复制
来源：http://mobile.sjlbkw.cn/Article/details/guvpiifuo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/grzibrajo.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gaumzkouq.sHtML

strlen(s)
来源：http://www.blog.tarul.cn/Article/details/gepltagmp.sHtML

[S06] C：字符串比较
来源：http://m.share.tarul.cn/Article/details/gpyazstcv.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/giuvwgexg.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.epnwcf.com/Article/details/gwmgarkff.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.tarul.cn/Article/details/gmmwbeqal.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.tarul.cn/Article/details/gnuepwiyi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/genyknudb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.vehdjk.com/Article/details/gtdetycoc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/glkgjeici.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/gkebpuhwo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.epnwcf.com/Article/details/gxwqoxchv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gpgsyssnm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.vehdjk.com/Article/details/gbysljqxe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fktsv.cn/Article/details/gamculrvn.sHtML

fclose(f);
来源：http://baike.fktsv.cn/Article/details/gyhhsbtts.sHtML

[S12] C：写文件
来源：http://www.share.tarul.cn/Article/details/gsqvjjxjd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gusjjxais.sHtML

[S13] C：宏定义
来源：http://blog.yfazqb.com/Article/details/giauphdhe.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gfggysowc.sHtML

[S14] C：枚举
来源：http://www.blog.epnwcf.com/Article/details/goiqxlgwk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.bbcook.cn/Article/details/gpdlsxjwa.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gyhuujpky.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gqsialcjj.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gkizazagm.sHtML

x |= (1 << 3);
来源：http://baike.fktsv.cn/Article/details/gzvcthqnf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fktsv.cn/Article/details/ggsqtbhuf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.yfazqb.com/Article/details/gihbsoqni.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gskcajroi.sHtML

int main(int argc, char **argv)
来源：http://wap.bbcook.cn/Article/details/gdgpqyoew.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gzaodwofy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.bbcook.cn/Article/details/gfobbidyt.sHtML

[S20] C：二分查找
来源：http://www.blog.sjlbkw.cn/Article/details/gllvoryol.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gfliimtyr.sHtML

[S21] C：字符类别判断
来源：http://3g.bbcook.cn/Article/details/gxcscneyq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gsnxmdjji.sHtML

[S22] C：字符串转数字
来源：http://3g.bbcook.cn/Article/details/gtchhvxhi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fktsv.cn/Article/details/gmmwrqtgi.sHtML

[S23] C：随机数
来源：http://mobile.yfazqb.com/Article/details/gxmcexboy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.tarul.cn/Article/details/gwmqbcuve.sHtML

[S24] C：获取本地时间
来源：http://mobile.epnwcf.com/Article/details/gimswsgbg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/gqdgpabtx.sHtML

[S25] C：内存拷贝
来源：http://www.share.epnwcf.com/Article/details/ggvelnjwp.sHtML

memcpy(dst, src, n);
来源：http://read.share.vehdjk.com/Article/details/gglwogoij.sHtML

[S26] C：内存清零
来源：http://www.share.bbcook.cn/Article/details/gnufdueea.sHtML

memset(a, 0, sizeof a);
来源：http://3g.sjlbkw.cn/Article/details/gacuxeqje.sHtML

[S27] C：定义常量
来源：http://m.share.yfazqb.com/Article/details/giwdbbloe.sHtML

const double PI = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gnhuioxbb.sHtML

[S28] C：静态变量
来源：http://wap.bbcook.cn/Article/details/gacxjmppe.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gjvujkiqn.sHtML

[S29] C：变参函数
来源：http://baike.fktsv.cn/Article/details/ggbajqefw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gpqvuzmtn.sHtML

[S30] C：头文件保护
来源：http://www.m.share.epnwcf.com/Article/details/gkugeprnf.sHtML

#ifndef X_H
来源：http://www.share.tarul.cn/Article/details/graxhrasa.sHtML

#define X_H
来源：http://3g.sjlbkw.cn/Article/details/ggvphrdeo.sHtML

#endif
来源：http://mobile.sjlbkw.cn/Article/details/gmopvmqhc.sHtML

[S31] C++：Hello World
来源：http://www.share.epnwcf.com/Article/details/gxlsvwcgn.sHtML

#include <iostream>
来源：http://www.m.share.bbcook.cn/Article/details/gpnpwndls.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gvjhpalnb.sHtML

[S32] C++：字符串
来源：http://blog.sjlbkw.cn/Article/details/gpjnzjveq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.yfazqb.com/Article/details/gieceqmfk.sHtML

[S33] C++：vector 增删
来源：http://www.share.fktsv.cn/Article/details/gmwmvscfo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.vehdjk.com/Article/details/gqwxpfyvf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.sjlbkw.cn/Article/details/glefbdcmy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.sjlbkw.cn/Article/details/gydbeykpm.sHtML

[S35] C++：map
来源：http://baike.sjlbkw.cn/Article/details/gnlmporxq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/gjvffbicz.sHtML

[S36] C++：unordered_map
来源：http://baike.fktsv.cn/Article/details/gmfsvnfcq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gdohqjfsn.sHtML

[S37] C++：set
来源：http://blog.bbcook.cn/Article/details/gubuhlusi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.sjlbkw.cn/Article/details/gjrnrkuqm.sHtML

[S38] C++：排序
来源：http://www.m.share.yfazqb.com/Article/details/giyrxfkod.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.bbcook.cn/Article/details/gyoufsujo.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.epnwcf.com/Article/details/gxizieote.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fktsv.cn/Article/details/gumxldjbn.sHtML

[S40] C++：查找元素
来源：http://3g.fktsv.cn/Article/details/gkiwtvott.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.vehdjk.com/Article/details/gksfcksat.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gegdeffhu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.vehdjk.com/Article/details/guhimhffu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.bbcook.cn/Article/details/gmnksgtmi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/giljzcwqg.sHtML

[S43] C++：智能指针
来源：http://baike.fktsv.cn/Article/details/genqarabo.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.epnwcf.com/Article/details/gxegytbbs.sHtML

[S44] C++：引用传参
来源：http://wap.tarul.cn/Article/details/gqzfirgxs.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.bbcook.cn/Article/details/gzdhzkxwy.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/gpoynumfe.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvxsxqxp.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gluclimuq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.epnwcf.com/Article/details/gcxomjaca.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.tarul.cn/Article/details/ggyeujnly.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.yfazqb.com/Article/details/gbpzptlru.sHtML

[S48] C++：逐行读文件
来源：http://blog.bbcook.cn/Article/details/glpyirpkm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.bbcook.cn/Article/details/gttdolvos.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gzudbmqkh.sHtML

[S49] C++：写文件
来源：http://blog.epnwcf.com/Article/details/ggwsoyeuq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.bbcook.cn/Article/details/gtvbnrdsc.sHtML

[S50] C++：格式化数字
来源：http://blog.vehdjk.com/Article/details/gauuaswbc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/grcolebar.sHtML

[S51] C++：显式类型转换
来源：http://mobile.yfazqb.com/Article/details/gcfoomxng.sHtML

static_cast<double>(a) / b
来源：http://baike.vehdjk.com/Article/details/gnsraxmyb.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.epnwcf.com/Article/details/gsytxiumw.sHtML

int size() const noexcept { return n_; }
来源：http://wap.epnwcf.com/Article/details/ghyacqldj.sHtML

[S53] C++：移动语义
来源：http://www.share.fktsv.cn/Article/details/gatwnhpya.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.bbcook.cn/Article/details/gjizlmtve.sHtML

[S54] C++：异常处理
来源：http://baike.epnwcf.com/Article/details/gjynqnonu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fktsv.cn/Article/details/gqwzthcsv.sHtML

[S55] C++：结构化绑定
来源：http://read.share.vehdjk.com/Article/details/gtrofpcet.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.yfazqb.com/Article/details/gwdhnqfbc.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gebcegqtj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fktsv.cn/Article/details/gktxgyljh.sHtML

[S57] C++：编译期常量
来源：http://www.share.bbcook.cn/Article/details/girfssftb.sHtML

constexpr int N = 10;
来源：http://www.share.yfazqb.com/Article/details/gjzzfmumm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.yfazqb.com/Article/details/gbmjvvzwi.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.tarul.cn/Article/details/geexrzhsw.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gedlqhmpz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.bbcook.cn/Article/details/gipuiomxv.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.vehdjk.com/Article/details/gkdbfcwty.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gxghirtlj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gswxiaefj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fktsv.cn/Article/details/gkkjaihzv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gerpklpfp.sHtML

[T01] Kotlin：Hello World
来源：http://baike.epnwcf.com/Article/details/gkkzvntqt.sHtML

println("Hello")
来源：http://blog.vehdjk.com/Article/details/gcjztvpdg.sHtML

[T02] Kotlin：变量
来源：http://read.share.bbcook.cn/Article/details/grmnrsguh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.epnwcf.com/Article/details/giizzqqza.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.sjlbkw.cn/Article/details/gdjjvfvod.sHtML

"值: $b"
来源：http://www.m.share.bbcook.cn/Article/details/gvjkmuepg.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/givpqtfkb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.tarul.cn/Article/details/gyasqgkjd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gionzfpue.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.bbcook.cn/Article/details/gxzxecock.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/glcgkniow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gemddnbur.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.bbcook.cn/Article/details/gqzujtavu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.vehdjk.com/Article/details/glvspgpor.sHtML

[T08] Kotlin：数据类
来源：http://m.share.tarul.cn/Article/details/geuvyhant.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fktsv.cn/Article/details/gydtfzdek.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/gestnyhnv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.sjlbkw.cn/Article/details/gwanesqkk.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.sjlbkw.cn/Article/details/gvcktmzsc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.epnwcf.com/Article/details/gfldejgku.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/gcbsccnht.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.tarul.cn/Article/details/gynaagcpt.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.epnwcf.com/Article/details/gvnvctxvm.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.vehdjk.com/Article/details/gmpcgksho.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.bbcook.cn/Article/details/gepbzltgl.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gmurwmujd.sHtML

[T14] Kotlin：循环
来源：http://m.share.bbcook.cn/Article/details/gvrbwsgbw.sHtML

for (i in 1..10) println(i)
来源：http://3g.yfazqb.com/Article/details/gqrytpicm.sHtML

[T15] Kotlin：接口
来源：http://baike.sjlbkw.cn/Article/details/gcvestfbh.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gjlbpkogj.sHtML

[T16] Swift：Hello World
来源：http://read.share.yfazqb.com/Article/details/ggwcmpjzt.sHtML

print("Hello")
来源：http://blog.fktsv.cn/Article/details/gjaweqgkm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.bbcook.cn/Article/details/gezapqjkl.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gjgkvuoln.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gulzqikrt.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/guvivsrdo.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.bbcook.cn/Article/details/glravkrql.sHtML

if let n = opt { print(n) }
来源：http://www.blog.sjlbkw.cn/Article/details/gnammnewb.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.yfazqb.com/Article/details/gfjbhewup.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.bbcook.cn/Article/details/ggykqsejw.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/gsstrtvjj.sHtML

for x in a { print(x) }
来源：http://www.blog.epnwcf.com/Article/details/gdhplfnon.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/ggktrxuuq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/gnkkmjmki.sHtML

[T23] Swift：函数
来源：http://baike.bbcook.cn/Article/details/ghtlzydnp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.bbcook.cn/Article/details/gzywcevss.sHtML

[T24] Swift：闭包
来源：http://wap.fktsv.cn/Article/details/gajrtiegm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.tarul.cn/Article/details/gopyajgbq.sHtML

[T25] Swift：结构体
来源：http://m.share.bbcook.cn/Article/details/gfrjtlrvu.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/gytemkruj.sHtML

[T26] Swift：类与重写
来源：http://m.share.tarul.cn/Article/details/gjgzahhel.sHtML

class A: Base { override func f() {} }
来源：http://mobile.epnwcf.com/Article/details/gqjwrfslv.sHtML

[T27] Swift：错误处理
来源：http://www.blog.bbcook.cn/Article/details/gvttggusq.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fktsv.cn/Article/details/gshsgmzcc.sHtML

[T28] Swift：枚举
来源：http://mobile.vehdjk.com/Article/details/gqjqqlbwt.sHtML

enum Color { case red, green }
来源：http://read.share.yfazqb.com/Article/details/ghovedqsh.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.tarul.cn/Article/details/gpilxllig.sHtML

guard let x = opt else { return }
来源：http://www.share.epnwcf.com/Article/details/gocbtcnxr.sHtML

[T30] Swift：协议
来源：http://blog.fktsv.cn/Article/details/gjbmmkcjh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fktsv.cn/Article/details/ggymkepwb.sHtML

[T31] Lua：Hello World
来源：http://wap.bbcook.cn/Article/details/gksanthti.sHtML

print("Hello")
来源：http://www.share.yfazqb.com/Article/details/gosvfvdrz.sHtML

[T32] Lua：局部变量
来源：http://www.blog.epnwcf.com/Article/details/gesgltsgg.sHtML

local a = 1
来源：http://www.blog.tarul.cn/Article/details/gnreunxzi.sHtML

[T33] Lua：表（数组）
来源：http://baike.fktsv.cn/Article/details/gghlzpufh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gvpetuxxn.sHtML

[T34] Lua：遍历表
来源：http://read.share.fktsv.cn/Article/details/ghoywgbmy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/ghnekxnzt.sHtML

[T35] Lua：字典表
来源：http://read.share.bbcook.cn/Article/details/gxqkecjdi.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.sjlbkw.cn/Article/details/ghwqwhadl.sHtML

[T36] Lua：函数
来源：http://wap.fktsv.cn/Article/details/gbljuassk.sHtML

function add(a, b) return a + b end
来源：http://wap.epnwcf.com/Article/details/gmpwfteff.sHtML

[T37] Lua：字符串拼接
来源：http://baike.epnwcf.com/Article/details/ggvvglglt.sHtML

"a" .. "b"
来源：http://www.m.share.tarul.cn/Article/details/gzzgkumdu.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gnayfjgsk.sHtML

if x > 0 then print("正") end
来源：http://3g.sjlbkw.cn/Article/details/gjvfexhxt.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gqaqeftsg.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gybrbnzwm.sHtML

[T40] Lua：元表
来源：http://baike.epnwcf.com/Article/details/guoupcsvt.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/gwgwhufaa.sHtML

[T41] Perl：Hello World
来源：http://baike.yfazqb.com/Article/details/gbbyafisy.sHtML

print "Hello\n";
来源：http://blog.tarul.cn/Article/details/gdhefsgnr.sHtML

[T42] Perl：变量类型
来源：http://baike.epnwcf.com/Article/details/gwdmiacpk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.bbcook.cn/Article/details/gwfknffpa.sHtML

[T43] Perl：字符串插值
来源：http://3g.vehdjk.com/Article/details/gyjbhmmxj.sHtML

"值: $a"
来源：http://wap.sjlbkw.cn/Article/details/gwccjmrth.sHtML

[T44] Perl：条件
来源：http://baike.yfazqb.com/Article/details/gsoerwiku.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.tarul.cn/Article/details/gxlnohlpf.sHtML

[T45] Perl：数组遍历
来源：http://3g.yfazqb.com/Article/details/gxpseibdt.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fktsv.cn/Article/details/gzmcfqueh.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/gwmdzrcwm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.epnwcf.com/Article/details/gqvvrsyvt.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/ggnmaxubn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.vehdjk.com/Article/details/gnalqglsl.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/gcdgphztl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.epnwcf.com/Article/details/gmlcdroup.sHtML

[T49] Perl：函数
来源：http://baike.bbcook.cn/Article/details/gjupjogul.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.yfazqb.com/Article/details/gvfotrisp.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fktsv.cn/Article/details/guzvnsoxg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.vehdjk.com/Article/details/gadedgzer.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.tarul.cn/Article/details/gfyorqjcm.sHtML

[T51] Scala：Hello World
来源：http://3g.yfazqb.com/Article/details/gxnauzjcf.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gbnmyyacb.sHtML

[T52] Scala：变量
来源：http://mobile.fktsv.cn/Article/details/gfykmqddt.sHtML

val a = 1;  var b = 2
来源：http://m.share.yfazqb.com/Article/details/gphcqjmlw.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/gxyyxhacq.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gqryulwbr.sHtML

[T54] Scala：集合映射
来源：http://read.share.vehdjk.com/Article/details/gsrwszsma.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.yfazqb.com/Article/details/gnbkvtxnk.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/gymfjcrvc.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.sjlbkw.cn/Article/details/gyjyoubqh.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gpfxalwqi.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/giqpmtqde.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/gjyyyafwo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/ggtoxtktd.sHtML

[T58] Scala：函数定义
来源：http://mobile.yfazqb.com/Article/details/gkljrugoc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.tarul.cn/Article/details/gymrstost.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gnsxdwbxv.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gzddgnyni.sHtML

[T60] Scala：折叠
来源：http://www.m.share.bbcook.cn/Article/details/gmcbatywd.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.sjlbkw.cn/Article/details/gyoxzvtbf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grylddwnb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/ghfcppnth.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gigzstwoy.sHtML


<!-- 参考信息 -->