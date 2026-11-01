代发 wailian999

df -h;  du -sh *
来源：http://read.share.bbcook.cn/Article/details/gphczkimy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.vehdjk.com/Article/details/gcebrxkwx.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.bbcook.cn/Article/details/gdjdhjhcv.sHtML

[R63] 内存与进程
来源：http://www.share.tarul.cn/Article/details/gojentnms.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gwlgplnfh.sHtML

[R64] 结束进程
来源：http://read.share.bbcook.cn/Article/details/gzutqzipi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gfmpeihsj.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gkaxjdkob.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.bbcook.cn/Article/details/gpciqalbx.sHtML

[R66] 定时任务
来源：http://mobile.bbcook.cn/Article/details/gzugqwtcl.sHtML

crontab -e;  crontab -l
来源：http://baike.sjlbkw.cn/Article/details/ghcombgen.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.bbcook.cn/Article/details/gzndtlzji.sHtML

openssl rand -hex 16
来源：http://3g.sjlbkw.cn/Article/details/gfhmyhlyz.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gnplabwtz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.vehdjk.com/Article/details/gwrxcjcov.sHtML

[R69] 生成随机密码
来源：http://read.share.bbcook.cn/Article/details/gjddtdirj.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/grkhvncgt.sHtML

[R70] 时间戳与互转
来源：http://www.blog.sjlbkw.cn/Article/details/gxgxpofpt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gmlqeiwck.sHtML

[R71] 日期格式化
来源：http://mobile.tarul.cn/Article/details/glewtjtke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.epnwcf.com/Article/details/gghwazcic.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.yfazqb.com/Article/details/gxgdngkvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/grvusgexm.sHtML

[R73] 分割大日志
来源：http://www.share.yfazqb.com/Article/details/gihqopeyo.sHtML

split -l 1000 big.log part_
来源：http://m.share.tarul.cn/Article/details/gxullnjro.sHtML

[R74] 批量重命名
来源：http://www.blog.vehdjk.com/Article/details/guotajwcc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.bbcook.cn/Article/details/glfutozoe.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/gpnhaedwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.epnwcf.com/Article/details/gftbkckqa.sHtML

[R76] 使用临时文件
来源：http://3g.epnwcf.com/Article/details/geyrhoena.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gloptemqs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.tarul.cn/Article/details/gypbxicrx.sHtML

read -rp "请输入: " ans
来源：http://baike.bbcook.cn/Article/details/gjcfkwjuh.sHtML

[R78] 交互式菜单
来源：http://www.blog.tarul.cn/Article/details/gqkxpruwq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fktsv.cn/Article/details/gjbfhvkiq.sHtML

[R79] 解析命令行选项
来源：http://blog.vehdjk.com/Article/details/gvgvcxvrq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.bbcook.cn/Article/details/gappafqnv.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.sjlbkw.cn/Article/details/gjltpyglr.sHtML

time ./run.sh
来源：http://baike.yfazqb.com/Article/details/ggnekmggh.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gaseliyua.sHtML

S. C / C++ 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gzaeouobp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/grsnnssge.sHtML

[S01] C：Hello World
来源：http://3g.vehdjk.com/Article/details/gdoqvdjdc.sHtML

#include <stdio.h>
来源：http://www.share.fktsv.cn/Article/details/gdknfaxmi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gcezmgzmq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.bbcook.cn/Article/details/grwfthihz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gjqhyjyts.sHtML

[S03] C：读入整数
来源：http://mobile.epnwcf.com/Article/details/gugclzemi.sHtML

int x; scanf("%d", &x);
来源：http://baike.vehdjk.com/Article/details/guiidbhwi.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gszuvmphu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.bbcook.cn/Article/details/ghfcydhsc.sHtML

[S05] C：字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gilttxbrs.sHtML

strlen(s)
来源：http://baike.yfazqb.com/Article/details/gojklaoqs.sHtML

[S06] C：字符串比较
来源：http://3g.bbcook.cn/Article/details/glxqxunhy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.sjlbkw.cn/Article/details/ggspszspa.sHtML

[S07] C：数组遍历求和
来源：http://baike.bbcook.cn/Article/details/gzvwvthwn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.bbcook.cn/Article/details/gzxyeamte.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.bbcook.cn/Article/details/gptjrwfpj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.bbcook.cn/Article/details/gmhbsddmk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gzpfbumej.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.bbcook.cn/Article/details/gfxrvuhfq.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/grsqyanlm.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fktsv.cn/Article/details/globptbqd.sHtML

[S11] C：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gjuhgmpsq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.vehdjk.com/Article/details/gfpqwiumq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.yfazqb.com/Article/details/gxyzensum.sHtML

fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gbmluilgw.sHtML

[S12] C：写文件
来源：http://m.share.bbcook.cn/Article/details/gjljuypsi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.vehdjk.com/Article/details/ghnxzyehp.sHtML

[S13] C：宏定义
来源：http://blog.epnwcf.com/Article/details/gbcpzilkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.vehdjk.com/Article/details/gnmxeykfv.sHtML

[S14] C：枚举
来源：http://baike.sjlbkw.cn/Article/details/grnnpgwmh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.bbcook.cn/Article/details/gprnkbqcc.sHtML

[S15] C：类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gruprvwbe.sHtML

(double) a / b
来源：http://m.share.vehdjk.com/Article/details/gfdnwwlwt.sHtML

[S16] C：位操作置位
来源：http://www.share.sjlbkw.cn/Article/details/gkubqdcph.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/glxsgmahv.sHtML

[S17] C：安全拼接字符串
来源：http://3g.vehdjk.com/Article/details/gqmemetes.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fktsv.cn/Article/details/gqnxtabwg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gpunpgzht.sHtML

int main(int argc, char **argv)
来源：http://m.share.fktsv.cn/Article/details/gzegposuz.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gpiyxuoeu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gwriszbnv.sHtML

[S20] C：二分查找
来源：http://read.share.fktsv.cn/Article/details/gjrgojghp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxblsbgeg.sHtML

[S21] C：字符类别判断
来源：http://read.share.sjlbkw.cn/Article/details/gkgzzfooh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.vehdjk.com/Article/details/goytwbzuq.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gjiriojui.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.bbcook.cn/Article/details/gxpevceti.sHtML

[S23] C：随机数
来源：http://wap.yfazqb.com/Article/details/gywmtoftp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.tarul.cn/Article/details/gwulblfav.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.yfazqb.com/Article/details/gfdaedzxf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fktsv.cn/Article/details/gqumljpwi.sHtML

[S25] C：内存拷贝
来源：http://blog.tarul.cn/Article/details/gxxbigbsj.sHtML

memcpy(dst, src, n);
来源：http://m.share.sjlbkw.cn/Article/details/gdejhgyie.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gougaynps.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fktsv.cn/Article/details/ghvrubzmk.sHtML

[S27] C：定义常量
来源：http://www.share.sjlbkw.cn/Article/details/gklitosqk.sHtML

const double PI = 3.14159;
来源：http://3g.fktsv.cn/Article/details/gufoskrbc.sHtML

[S28] C：静态变量
来源：http://mobile.tarul.cn/Article/details/gvbeopnrk.sHtML

static int counter = 0;
来源：http://baike.yfazqb.com/Article/details/ggvjfjglf.sHtML

[S29] C：变参函数
来源：http://www.m.share.bbcook.cn/Article/details/gwzmvwtgc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/ggivslacu.sHtML

[S30] C：头文件保护
来源：http://wap.vehdjk.com/Article/details/gbtpjgeru.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gsztkihft.sHtML

#define X_H
来源：http://mobile.yfazqb.com/Article/details/ginboepby.sHtML

#endif
来源：http://3g.sjlbkw.cn/Article/details/gdnrhagiv.sHtML

[S31] C++：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gbzhcwcsh.sHtML

#include <iostream>
来源：http://wap.fktsv.cn/Article/details/ghndxwxis.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.epnwcf.com/Article/details/genwqakxq.sHtML

[S32] C++：字符串
来源：http://www.blog.yfazqb.com/Article/details/gvzowjrhh.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fktsv.cn/Article/details/gndbpitov.sHtML

[S33] C++：vector 增删
来源：http://read.share.vehdjk.com/Article/details/getpshmkj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.epnwcf.com/Article/details/gfmzasisi.sHtML

[S34] C++：遍历 vector
来源：http://blog.yfazqb.com/Article/details/ggcqjkqiv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gwtmtugsn.sHtML

[S35] C++：map
来源：http://blog.sjlbkw.cn/Article/details/gekzypesq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gpjiujabj.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fktsv.cn/Article/details/gqzjivlsp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gwyrwgbzw.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gghirtppe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.epnwcf.com/Article/details/gzgngejsv.sHtML

[S38] C++：排序
来源：http://baike.sjlbkw.cn/Article/details/gzozsywkz.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.yfazqb.com/Article/details/gbpdglylw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.vehdjk.com/Article/details/glrqufend.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.yfazqb.com/Article/details/gaoeabcrr.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/gvkrwiysn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.vehdjk.com/Article/details/gvjhzvbuo.sHtML

[S41] C++：类与构造函数
来源：http://www.share.epnwcf.com/Article/details/gjiuvuiwt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.bbcook.cn/Article/details/gqjbwvglm.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fktsv.cn/Article/details/gyxapkhhf.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.yfazqb.com/Article/details/gulotcszc.sHtML

[S43] C++：智能指针
来源：http://m.share.vehdjk.com/Article/details/gyiqpzejy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.tarul.cn/Article/details/gelvhmptf.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/gdtmhnbqj.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/ginbwfvze.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gysafppli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/guhpqpfuv.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gniyuabom.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.bbcook.cn/Article/details/gcdztrgnc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fktsv.cn/Article/details/gayzjjrkp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfvlvbcr.sHtML

[S48] C++：逐行读文件
来源：http://blog.epnwcf.com/Article/details/gjprjbmqi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fktsv.cn/Article/details/gxxurzzhz.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.epnwcf.com/Article/details/gcbafevdb.sHtML

[S49] C++：写文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtaaircn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fktsv.cn/Article/details/gnbbgbiay.sHtML

[S50] C++：格式化数字
来源：http://www.share.sjlbkw.cn/Article/details/gzpwkxyyp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.yfazqb.com/Article/details/giwbcfgdo.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.tarul.cn/Article/details/gtribvjxq.sHtML

static_cast<double>(a) / b
来源：http://m.share.epnwcf.com/Article/details/ggrqupkmp.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fktsv.cn/Article/details/gjofhescl.sHtML

int size() const noexcept { return n_; }
来源：http://baike.yfazqb.com/Article/details/gyggvryki.sHtML

[S53] C++：移动语义
来源：http://read.share.epnwcf.com/Article/details/getbvoumj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gzuytewbo.sHtML

[S54] C++：异常处理
来源：http://baike.vehdjk.com/Article/details/gyubbpxjh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.epnwcf.com/Article/details/gooezztge.sHtML

[S55] C++：结构化绑定
来源：http://www.share.sjlbkw.cn/Article/details/gmumbxwjp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.vehdjk.com/Article/details/guzrvphgd.sHtML

[S56] C++：optional
来源：http://www.blog.vehdjk.com/Article/details/gaumdeway.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fktsv.cn/Article/details/gubclgwsf.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/ggojsngpx.sHtML

constexpr int N = 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gvyfdmbnl.sHtML

[S58] C++：命名空间
来源：http://www.share.bbcook.cn/Article/details/gmpsuittl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.bbcook.cn/Article/details/gwvuvidio.sHtML

[S59] C++：静态断言
来源：http://mobile.bbcook.cn/Article/details/glkfucdyz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.yfazqb.com/Article/details/gcykuhgzi.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.bbcook.cn/Article/details/germegomr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fktsv.cn/Article/details/gnejijquc.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkaleicvj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gmpqzlwmj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glydpmtka.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.vehdjk.com/Article/details/geqwzcgne.sHtML

println("Hello")
来源：http://m.share.yfazqb.com/Article/details/gxpslvwxj.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gqxyheopv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.sjlbkw.cn/Article/details/gdptbdhdy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.vehdjk.com/Article/details/gdkwlugdv.sHtML

"值: $b"
来源：http://m.share.sjlbkw.cn/Article/details/grsctovjm.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/gpzkbkrhm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gqvgleidw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gbudhorxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.yfazqb.com/Article/details/gojqmlugd.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.bbcook.cn/Article/details/gpegdhpdq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/grxultcnh.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gpfbpzvmt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.epnwcf.com/Article/details/gverhazru.sHtML

[T08] Kotlin：数据类
来源：http://3g.epnwcf.com/Article/details/gbyoebpxc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.yfazqb.com/Article/details/gdqkholjj.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.vehdjk.com/Article/details/gmloladve.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.vehdjk.com/Article/details/gpadoyqzn.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gfhiydwsu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/guapqadxc.sHtML

[T11] Kotlin：协程
来源：http://wap.fktsv.cn/Article/details/gtwyzuodt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gywkklkvu.sHtML

[T12] Kotlin：解构声明
来源：http://baike.yfazqb.com/Article/details/gkojdanne.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.yfazqb.com/Article/details/gyscvykal.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.bbcook.cn/Article/details/gfvtabfhh.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.sjlbkw.cn/Article/details/gwhbotraw.sHtML

[T14] Kotlin：循环
来源：http://blog.tarul.cn/Article/details/gapgdwlcm.sHtML

for (i in 1..10) println(i)
来源：http://3g.epnwcf.com/Article/details/gwgwvwpkz.sHtML

[T15] Kotlin：接口
来源：http://blog.bbcook.cn/Article/details/gvosklbxs.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/gxnoiqisq.sHtML

[T16] Swift：Hello World
来源：http://read.share.bbcook.cn/Article/details/gwoqevfwu.sHtML

print("Hello")
来源：http://mobile.tarul.cn/Article/details/gmzlgqarj.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gamjgcgkr.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gldrcvcyc.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gdvkydfum.sHtML

"值: \(b)"
来源：http://blog.sjlbkw.cn/Article/details/gharevbok.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gnmbewxzt.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gckydipex.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gacsalgzo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.vehdjk.com/Article/details/glmmkcjzb.sHtML

[T21] Swift：遍历
来源：http://read.share.epnwcf.com/Article/details/gitpcxjbj.sHtML

for x in a { print(x) }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggghkmbek.sHtML

[T22] Swift：字典
来源：http://read.share.tarul.cn/Article/details/gzfgnlyci.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.sjlbkw.cn/Article/details/gzsygywvx.sHtML

[T23] Swift：函数
来源：http://www.m.share.fktsv.cn/Article/details/gmmorqccp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gmsrymqsx.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fktsv.cn/Article/details/gfzkkngqr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/ggpuubpic.sHtML

[T25] Swift：结构体
来源：http://mobile.epnwcf.com/Article/details/grjczjyjn.sHtML

struct P { var x: Int }
来源：http://www.share.sjlbkw.cn/Article/details/goxrhqrwa.sHtML

[T26] Swift：类与重写
来源：http://www.blog.sjlbkw.cn/Article/details/gejmvnwmp.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/grvslqzpd.sHtML

[T27] Swift：错误处理
来源：http://read.share.yfazqb.com/Article/details/guzutevdq.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gtonvqpig.sHtML

[T28] Swift：枚举
来源：http://www.share.tarul.cn/Article/details/gejiaysut.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/ggwpmkics.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.epnwcf.com/Article/details/gfujspzkd.sHtML

guard let x = opt else { return }
来源：http://read.share.sjlbkw.cn/Article/details/gtcraubgz.sHtML

[T30] Swift：协议
来源：http://www.blog.tarul.cn/Article/details/ggoxytmpi.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/grkclphtu.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gdwqjsaoy.sHtML

print("Hello")
来源：http://3g.tarul.cn/Article/details/gtxrwjrlo.sHtML

[T32] Lua：局部变量
来源：http://read.share.bbcook.cn/Article/details/gawuuegpp.sHtML

local a = 1
来源：http://3g.sjlbkw.cn/Article/details/giifaxyay.sHtML

[T33] Lua：表（数组）
来源：http://wap.fktsv.cn/Article/details/gyftgsvey.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.sjlbkw.cn/Article/details/gvykevgtp.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.sjlbkw.cn/Article/details/gunjzevpi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fktsv.cn/Article/details/giqorkdis.sHtML

[T35] Lua：字典表
来源：http://read.share.epnwcf.com/Article/details/gcbybique.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fktsv.cn/Article/details/gbynrxuyc.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gnvjzzhzy.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.yfazqb.com/Article/details/gyzsasxcv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.yfazqb.com/Article/details/gpvibsste.sHtML

"a" .. "b"
来源：http://m.share.bbcook.cn/Article/details/gnsdvasat.sHtML

[T38] Lua：条件
来源：http://m.share.vehdjk.com/Article/details/gjptxtlmo.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gegwnwetb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gapluhmeb.sHtML

string.find(s, "%d+")
来源：http://www.blog.yfazqb.com/Article/details/gvgdmpybz.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gnfuqnhpy.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.sjlbkw.cn/Article/details/godhjstro.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gopjzsrha.sHtML

print "Hello\n";
来源：http://m.share.sjlbkw.cn/Article/details/guhayluni.sHtML

[T42] Perl：变量类型
来源：http://wap.vehdjk.com/Article/details/gliuseskk.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.epnwcf.com/Article/details/guhswcwbk.sHtML

[T43] Perl：字符串插值
来源：http://www.share.sjlbkw.cn/Article/details/gmcsdcrxe.sHtML

"值: $a"
来源：http://www.m.share.tarul.cn/Article/details/gvlsscdai.sHtML

[T44] Perl：条件
来源：http://www.m.share.vehdjk.com/Article/details/gpfoobjxi.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/greyyfmmd.sHtML

[T45] Perl：数组遍历
来源：http://blog.vehdjk.com/Article/details/gdyvopxws.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.sjlbkw.cn/Article/details/gezfvmopz.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gwiwnqddx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gxntzbdfk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/gcsysvohh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.vehdjk.com/Article/details/gieenhsyj.sHtML

[T48] Perl：正则替换
来源：http://baike.sjlbkw.cn/Article/details/gdmszrkvy.sHtML

$s =~ s/old/new/g;
来源：http://blog.epnwcf.com/Article/details/gjnwoafie.sHtML

[T49] Perl：函数
来源：http://blog.epnwcf.com/Article/details/gdjscgfnk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.tarul.cn/Article/details/gshxctqvq.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/ghhgzkfdn.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/glkdctdbq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.vehdjk.com/Article/details/giiqumqcs.sHtML

[T51] Scala：Hello World
来源：http://www.blog.bbcook.cn/Article/details/geewnaysy.sHtML

println("Hello")
来源：http://read.share.bbcook.cn/Article/details/guaolvuqt.sHtML

[T52] Scala：变量
来源：http://www.share.epnwcf.com/Article/details/gpbjpmlmb.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.epnwcf.com/Article/details/gdnsjnmst.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gwxvcwoeo.sHtML

s"值: $b"
来源：http://3g.vehdjk.com/Article/details/gqagoatvk.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/ghrrincfh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.fktsv.cn/Article/details/gnwyzfmcz.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gxmigysih.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.sjlbkw.cn/Article/details/geclmbtbd.sHtML

[T56] Scala：样例类
来源：http://wap.epnwcf.com/Article/details/ggqtschxq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.yfazqb.com/Article/details/grkctsfmq.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gwgliuygl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.yfazqb.com/Article/details/gvunncmxy.sHtML

[T58] Scala：函数定义
来源：http://baike.fktsv.cn/Article/details/gchywzatf.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gwuqbyxkd.sHtML

[T59] Scala：循环
来源：http://3g.tarul.cn/Article/details/gzfbfhchr.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.epnwcf.com/Article/details/gugexdjul.sHtML

[T60] Scala：折叠
来源：http://www.share.bbcook.cn/Article/details/gorjmpoyn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.yfazqb.com/Article/details/gskdcqeuo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvemcdyct.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/giopozphu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grwjrnjjm.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.bbcook.cn/Article/details/gtrdqvqwj.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.tarul.cn/Article/details/grqwloppz.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/ghmfabybd.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.bbcook.cn/Article/details/gzkpiugnt.sHtML


<!-- 参考信息 -->