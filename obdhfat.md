代发 wailian999

df -h;  du -sh *
来源：http://m.share.tarul.cn/Article/details/goeilsqdx.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.tarul.cn/Article/details/gmqfrmqkx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqoeybix.sHtML

[R63] 内存与进程
来源：http://www.m.share.epnwcf.com/Article/details/gppvctild.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.tarul.cn/Article/details/ggtawqece.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/grwlemqcn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.tarul.cn/Article/details/gqnylatqd.sHtML

[R65] 查看端口占用
来源：http://blog.vehdjk.com/Article/details/gbmnegdfu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.tarul.cn/Article/details/ggrjuestb.sHtML

[R66] 定时任务
来源：http://www.m.share.yfazqb.com/Article/details/gbrleeddh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gfsxrksgk.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.bbcook.cn/Article/details/gbxvperzx.sHtML

openssl rand -hex 16
来源：http://wap.vehdjk.com/Article/details/gfhhwdifd.sHtML

[R68] 计算文件校验值
来源：http://www.blog.bbcook.cn/Article/details/gnchjchpt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fktsv.cn/Article/details/glbwyiwpd.sHtML

[R69] 生成随机密码
来源：http://www.blog.bbcook.cn/Article/details/gcxbfeuqs.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fktsv.cn/Article/details/gatiofbrl.sHtML

[R70] 时间戳与互转
来源：http://mobile.vehdjk.com/Article/details/grbmygius.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gmkhbalij.sHtML

[R71] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gsyjcjgvh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.vehdjk.com/Article/details/gtzlbjxpl.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/guiorgxgf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gscoobzme.sHtML

[R73] 分割大日志
来源：http://read.share.fktsv.cn/Article/details/gyrbavbnv.sHtML

split -l 1000 big.log part_
来源：http://wap.vehdjk.com/Article/details/gtgfpvbxr.sHtML

[R74] 批量重命名
来源：http://www.share.fktsv.cn/Article/details/gdhiefpco.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.epnwcf.com/Article/details/gppnawxfw.sHtML

[R75] 导出环境变量
来源：http://baike.tarul.cn/Article/details/gxkqaqqlx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fktsv.cn/Article/details/gpwninjgv.sHtML

[R76] 使用临时文件
来源：http://mobile.tarul.cn/Article/details/ghahbfxkd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gbnuimdtg.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gwljngqyc.sHtML

read -rp "请输入: " ans
来源：http://blog.bbcook.cn/Article/details/gwvhdrxtc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.tarul.cn/Article/details/gjrgoveck.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.vehdjk.com/Article/details/gtlnvlddb.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gtqitamvr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.bbcook.cn/Article/details/gjdywfdjk.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gnovewgvr.sHtML

time ./run.sh
来源：http://m.share.bbcook.cn/Article/details/gfsnnziwb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvjazclnc.sHtML

S. C / C++ 专题
来源：http://wap.tarul.cn/Article/details/gjaovdkal.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzwyriqgk.sHtML

[S01] C：Hello World
来源：http://read.share.vehdjk.com/Article/details/gnfldgrmr.sHtML

#include <stdio.h>
来源：http://wap.tarul.cn/Article/details/gsgdvmeir.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.bbcook.cn/Article/details/gizjbsqeg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.bbcook.cn/Article/details/gpwbkjujv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.tarul.cn/Article/details/gmksmwpmb.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gfhuysfhe.sHtML

int x; scanf("%d", &x);
来源：http://baike.yfazqb.com/Article/details/gdbtemlau.sHtML

[S04] C：字符串复制
来源：http://wap.sjlbkw.cn/Article/details/gmfsnwmqn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fktsv.cn/Article/details/goflfjuwg.sHtML

[S05] C：字符串长度
来源：http://read.share.vehdjk.com/Article/details/gtruojbpp.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gxnvfqsmc.sHtML

[S06] C：字符串比较
来源：http://read.share.tarul.cn/Article/details/gufhbnbje.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.yfazqb.com/Article/details/gzqyuhdfq.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gzgyiwlim.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.sjlbkw.cn/Article/details/grocflmli.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.vehdjk.com/Article/details/gnzudztgo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.bbcook.cn/Article/details/ggufqmhkz.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.bbcook.cn/Article/details/gpigvkfnx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.tarul.cn/Article/details/ghajouwny.sHtML

[S10] C：指针与解引用
来源：http://www.share.epnwcf.com/Article/details/gimeggluq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fktsv.cn/Article/details/gawodsvbt.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/gywacvrrk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.sjlbkw.cn/Article/details/gjyouwfea.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fktsv.cn/Article/details/guofslqus.sHtML

fclose(f);
来源：http://www.m.share.bbcook.cn/Article/details/gorpdawqw.sHtML

[S12] C：写文件
来源：http://blog.tarul.cn/Article/details/gpweryhje.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.tarul.cn/Article/details/gqtpepwss.sHtML

[S13] C：宏定义
来源：http://www.share.sjlbkw.cn/Article/details/gkqhvunrp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.sjlbkw.cn/Article/details/gkounduhk.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gtanqlatb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.bbcook.cn/Article/details/gjmlptlxb.sHtML

[S15] C：类型转换
来源：http://read.share.sjlbkw.cn/Article/details/golljvgfb.sHtML

(double) a / b
来源：http://blog.sjlbkw.cn/Article/details/griqxwqnx.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/ghaneklyk.sHtML

x |= (1 << 3);
来源：http://www.share.sjlbkw.cn/Article/details/gcakupzcd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fktsv.cn/Article/details/grmuvlyrr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.tarul.cn/Article/details/gyelstsxc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/ggwbjblbk.sHtML

int main(int argc, char **argv)
来源：http://baike.sjlbkw.cn/Article/details/gfobgchzo.sHtML

[S19] C：快速排序
来源：http://blog.epnwcf.com/Article/details/gedyxgbou.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.epnwcf.com/Article/details/gzwevkqrm.sHtML

[S20] C：二分查找
来源：http://baike.bbcook.cn/Article/details/guldflkug.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.tarul.cn/Article/details/gsuppwtvz.sHtML

[S21] C：字符类别判断
来源：http://m.share.bbcook.cn/Article/details/gxxwjpffg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.yfazqb.com/Article/details/gbtubhlwp.sHtML

[S22] C：字符串转数字
来源：http://www.share.fktsv.cn/Article/details/gllmdcihz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.tarul.cn/Article/details/gcbauxmfj.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gixjdyvyh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gvwpoxxbz.sHtML

[S24] C：获取本地时间
来源：http://wap.yfazqb.com/Article/details/gstirpptd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.bbcook.cn/Article/details/gzaxuaqto.sHtML

[S25] C：内存拷贝
来源：http://www.share.yfazqb.com/Article/details/gwzpdtmpa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gcckapmwk.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gowvkxilm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fktsv.cn/Article/details/grnjdwahr.sHtML

[S27] C：定义常量
来源：http://blog.epnwcf.com/Article/details/gbqeyabob.sHtML

const double PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/goizfjvry.sHtML

[S28] C：静态变量
来源：http://read.share.epnwcf.com/Article/details/gkblekcue.sHtML

static int counter = 0;
来源：http://m.share.epnwcf.com/Article/details/gvmrghwaw.sHtML

[S29] C：变参函数
来源：http://read.share.sjlbkw.cn/Article/details/gcqspdebw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.epnwcf.com/Article/details/gbrnnsqsq.sHtML

[S30] C：头文件保护
来源：http://3g.epnwcf.com/Article/details/gwgrtpeco.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gbvorvudd.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gtioiaujz.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/gheztrolx.sHtML

[S31] C++：Hello World
来源：http://www.share.tarul.cn/Article/details/gudiceger.sHtML

#include <iostream>
来源：http://wap.bbcook.cn/Article/details/gutatrzpl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gtulmrrgf.sHtML

[S32] C++：字符串
来源：http://m.share.yfazqb.com/Article/details/gjlqjunhd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.bbcook.cn/Article/details/gnyxytunm.sHtML

[S33] C++：vector 增删
来源：http://mobile.bbcook.cn/Article/details/ggahumope.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/guggimvxm.sHtML

[S34] C++：遍历 vector
来源：http://wap.yfazqb.com/Article/details/glqulzrev.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.bbcook.cn/Article/details/gdaktpqqf.sHtML

[S35] C++：map
来源：http://www.share.epnwcf.com/Article/details/gkkvvyjft.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gffmsakfi.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/guzugiygx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gpvgolduj.sHtML

[S37] C++：set
来源：http://baike.tarul.cn/Article/details/gdjwmgaus.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gdejpedfj.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gsnjlzqjs.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fktsv.cn/Article/details/gembpqvct.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fktsv.cn/Article/details/gspsqnzkq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhxmdkkm.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gtqdjumdn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fktsv.cn/Article/details/gdguegwwb.sHtML

[S41] C++：类与构造函数
来源：http://blog.tarul.cn/Article/details/gneyrmvbv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gduqxpdcn.sHtML

[S42] C++：继承与虚函数
来源：http://3g.bbcook.cn/Article/details/gzxoatznl.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/gegyxvujo.sHtML

[S43] C++：智能指针
来源：http://wap.yfazqb.com/Article/details/gtlkwgdgq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gcblerucy.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/gvvixhwgc.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.sjlbkw.cn/Article/details/gugjlajuw.sHtML

[S45] C++：lambda
来源：http://m.share.bbcook.cn/Article/details/gvnpsxphr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.yfazqb.com/Article/details/ggjyavpjc.sHtML

[S46] C++：函数模板
来源：http://mobile.fktsv.cn/Article/details/geebcralz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqlwpibw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.bbcook.cn/Article/details/gcgtiooea.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.sjlbkw.cn/Article/details/gbbyqueov.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gyggieysm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.tarul.cn/Article/details/gskcvvlfy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.tarul.cn/Article/details/gizueiakf.sHtML

[S49] C++：写文件
来源：http://baike.epnwcf.com/Article/details/gptjqogln.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.yfazqb.com/Article/details/grskbebvx.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/grvbjizaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.epnwcf.com/Article/details/gcoqhmpfs.sHtML

[S51] C++：显式类型转换
来源：http://blog.tarul.cn/Article/details/glgxhmeda.sHtML

static_cast<double>(a) / b
来源：http://mobile.sjlbkw.cn/Article/details/gbmxdomta.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.epnwcf.com/Article/details/ghlsksmzw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.vehdjk.com/Article/details/gfmddlzli.sHtML

[S53] C++：移动语义
来源：http://www.m.share.bbcook.cn/Article/details/gqlbskdrh.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.epnwcf.com/Article/details/gcsdzedzd.sHtML

[S54] C++：异常处理
来源：http://m.share.yfazqb.com/Article/details/gkadsqktq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.tarul.cn/Article/details/gbuuevbqu.sHtML

[S55] C++：结构化绑定
来源：http://m.share.bbcook.cn/Article/details/gzmearuot.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.bbcook.cn/Article/details/gjhzmdzhc.sHtML

[S56] C++：optional
来源：http://www.share.vehdjk.com/Article/details/ggvpdinjy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.sjlbkw.cn/Article/details/gmdwjelzc.sHtML

[S57] C++：编译期常量
来源：http://3g.vehdjk.com/Article/details/gwqswbhif.sHtML

constexpr int N = 10;
来源：http://www.share.bbcook.cn/Article/details/grkaghiwv.sHtML

[S58] C++：命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqpwaqgl.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gbrkyrgio.sHtML

[S59] C++：静态断言
来源：http://wap.sjlbkw.cn/Article/details/gbdqhokzi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.vehdjk.com/Article/details/gjsdumeil.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.epnwcf.com/Article/details/gcritwsrd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fktsv.cn/Article/details/gdpenmhok.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwmwybbfs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.sjlbkw.cn/Article/details/gjbmhflzc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfsofejtp.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.bbcook.cn/Article/details/ggsiyixqn.sHtML

println("Hello")
来源：http://www.blog.tarul.cn/Article/details/gmxgiaexv.sHtML

[T02] Kotlin：变量
来源：http://m.share.sjlbkw.cn/Article/details/gelmfmfgd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.tarul.cn/Article/details/gmaovewet.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.bbcook.cn/Article/details/gzcovujqz.sHtML

"值: $b"
来源：http://www.blog.tarul.cn/Article/details/gwrwkellj.sHtML

[T04] Kotlin：空安全
来源：http://mobile.sjlbkw.cn/Article/details/gdcyqqlcf.sHtML

val n: String? = null;  n?.length
来源：http://m.share.bbcook.cn/Article/details/gxkganffs.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fktsv.cn/Article/details/ggasklsgs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.epnwcf.com/Article/details/ghmpdqqjj.sHtML

[T06] Kotlin：集合映射
来源：http://3g.epnwcf.com/Article/details/gobhnnzwn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.tarul.cn/Article/details/gtujkrlms.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gvqvxbyyn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gxwywbqup.sHtML

[T08] Kotlin：数据类
来源：http://m.share.bbcook.cn/Article/details/gbpfbdqwn.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gjfwlvbfr.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gtywtqqik.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.vehdjk.com/Article/details/gbqtapzdh.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gsedleief.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.epnwcf.com/Article/details/gyklfyhjn.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/gryngsoxa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.yfazqb.com/Article/details/ggwnuhhzd.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.sjlbkw.cn/Article/details/gwzketptw.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.yfazqb.com/Article/details/gisouobot.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.yfazqb.com/Article/details/grpjkvjid.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fktsv.cn/Article/details/gzwonlvoa.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gclujrhnt.sHtML

for (i in 1..10) println(i)
来源：http://mobile.tarul.cn/Article/details/gcfnsuyla.sHtML

[T15] Kotlin：接口
来源：http://www.share.sjlbkw.cn/Article/details/gxutvomrg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gdakbcxyu.sHtML

[T16] Swift：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gubgxqkpo.sHtML

print("Hello")
来源：http://www.share.epnwcf.com/Article/details/gymlzilhu.sHtML

[T17] Swift：变量与常量
来源：http://wap.bbcook.cn/Article/details/gvuijthlh.sHtML

var a = 1;  let b = 2
来源：http://m.share.epnwcf.com/Article/details/gjtqirnfb.sHtML

[T18] Swift：字符串插值
来源：http://blog.bbcook.cn/Article/details/goizzvfia.sHtML

"值: \(b)"
来源：http://www.share.tarul.cn/Article/details/gglisuqyb.sHtML

[T19] Swift：可选绑定
来源：http://baike.vehdjk.com/Article/details/gvuropgee.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gbqfkwfzz.sHtML

[T20] Swift：数组操作
来源：http://baike.tarul.cn/Article/details/gdsxiacmd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.bbcook.cn/Article/details/gadnwjtrq.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gedbkzart.sHtML

for x in a { print(x) }
来源：http://m.share.yfazqb.com/Article/details/grtwycujg.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gsriiigrp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.sjlbkw.cn/Article/details/gtkdzvrhd.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/grdhdxjal.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fktsv.cn/Article/details/ggnukdzhd.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ginymcxbc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gagdkapns.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gerrdsthu.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/ghjzlvjwq.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gdldymczw.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gyypwvmbp.sHtML

[T27] Swift：错误处理
来源：http://mobile.sjlbkw.cn/Article/details/goqarrgbf.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.epnwcf.com/Article/details/glutwaxjt.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gmwlbegfh.sHtML

enum Color { case red, green }
来源：http://blog.tarul.cn/Article/details/gyzbqctdm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.yfazqb.com/Article/details/gadqfiyfe.sHtML

guard let x = opt else { return }
来源：http://3g.epnwcf.com/Article/details/gbwacevnx.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/gwbsbrrre.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.bbcook.cn/Article/details/gwhchtqpz.sHtML

[T31] Lua：Hello World
来源：http://www.blog.tarul.cn/Article/details/gdaenendm.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gqbujwxwi.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/giunetmwv.sHtML

local a = 1
来源：http://baike.vehdjk.com/Article/details/gzzfkitvh.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fktsv.cn/Article/details/gmlptpquk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.vehdjk.com/Article/details/gksujxmre.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gpxmthash.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.bbcook.cn/Article/details/gcijrbnil.sHtML

[T35] Lua：字典表
来源：http://m.share.tarul.cn/Article/details/gqwufqati.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.vehdjk.com/Article/details/ghbbyhyjv.sHtML

[T36] Lua：函数
来源：http://blog.vehdjk.com/Article/details/gotysbzqh.sHtML

function add(a, b) return a + b end
来源：http://baike.tarul.cn/Article/details/gvxvwvfmk.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gsdjdenih.sHtML

"a" .. "b"
来源：http://m.share.yfazqb.com/Article/details/gshfhsbmt.sHtML

[T38] Lua：条件
来源：http://read.share.tarul.cn/Article/details/giixufgsy.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gmjjsvkkk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.vehdjk.com/Article/details/gaakkjkbk.sHtML

string.find(s, "%d+")
来源：http://wap.vehdjk.com/Article/details/gscjdiaib.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gyxuvbunw.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fktsv.cn/Article/details/glvvvwzgf.sHtML

[T41] Perl：Hello World
来源：http://m.share.fktsv.cn/Article/details/gcrbqxnxy.sHtML

print "Hello\n";
来源：http://www.blog.sjlbkw.cn/Article/details/grjbmohdr.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.bbcook.cn/Article/details/gdwnqqvll.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.vehdjk.com/Article/details/gzgmzgyew.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/ghxdauyhh.sHtML

"值: $a"
来源：http://read.share.bbcook.cn/Article/details/gswinthbv.sHtML

[T44] Perl：条件
来源：http://www.share.vehdjk.com/Article/details/gxkpkthwa.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/gjdwttduh.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gmedtvaoc.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.vehdjk.com/Article/details/ggtkktyda.sHtML

[T46] Perl：哈希操作
来源：http://read.share.epnwcf.com/Article/details/gjgmalkod.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.yfazqb.com/Article/details/gbrrqhciw.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.sjlbkw.cn/Article/details/gjpcnoehv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.vehdjk.com/Article/details/gygdjsqtj.sHtML

[T48] Perl：正则替换
来源：http://www.blog.vehdjk.com/Article/details/gxgbgkera.sHtML

$s =~ s/old/new/g;
来源：http://blog.sjlbkw.cn/Article/details/gvcgrjrfr.sHtML

[T49] Perl：函数
来源：http://wap.yfazqb.com/Article/details/gsdqihgdw.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.bbcook.cn/Article/details/gqhuqaotj.sHtML

[T50] Perl：逐行读文件
来源：http://blog.bbcook.cn/Article/details/gbwwfvfgl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.vehdjk.com/Article/details/gwfyfhtgs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/gugywpkck.sHtML

[T51] Scala：Hello World
来源：http://read.share.vehdjk.com/Article/details/gplnccnyj.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gpuvbqvgj.sHtML

[T52] Scala：变量
来源：http://blog.tarul.cn/Article/details/gculttwdr.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/glksoclmx.sHtML

[T53] Scala：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gacaxaifj.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gbsdugwcf.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gwyabizvh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/ghpjpxsbv.sHtML

[T55] Scala：集合过滤
来源：http://mobile.epnwcf.com/Article/details/gmcxknadg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.vehdjk.com/Article/details/gpfifafpq.sHtML

[T56] Scala：样例类
来源：http://m.share.tarul.cn/Article/details/gsqizmcih.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.epnwcf.com/Article/details/gygrxbktm.sHtML

[T57] Scala：模式匹配
来源：http://wap.yfazqb.com/Article/details/goidztxlf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.vehdjk.com/Article/details/gkdxiklxr.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/giizpswes.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.yfazqb.com/Article/details/gzrweyzax.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/ghzuoedhf.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/guajotnqc.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/gzrjjwmuu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/grprsvplf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggcrlhwjm.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fktsv.cn/Article/details/grzogvdlg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjrdjnqxx.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.bbcook.cn/Article/details/gilsguvdc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.bbcook.cn/Article/details/gmkrdypms.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.sjlbkw.cn/Article/details/gahqnougd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gukvbzceb.sHtML


<!-- 参考信息 -->