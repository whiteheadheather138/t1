代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gasoxetwk.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gfntlydfo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.tarul.cn/Article/details/galzbnvve.sHtML

[R61] 磁盘占用
来源：http://blog.bbcook.cn/Article/details/gcelrcixu.sHtML

df -h;  du -sh *
来源：http://wap.vehdjk.com/Article/details/gfqldmmpx.sHtML

[R62] 找最占空间的文件
来源：http://mobile.epnwcf.com/Article/details/gcrlkpfwj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.epnwcf.com/Article/details/gbbzmsinv.sHtML

[R63] 内存与进程
来源：http://www.share.sjlbkw.cn/Article/details/gmcmodcpl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.vehdjk.com/Article/details/gsfiukgma.sHtML

[R64] 结束进程
来源：http://blog.sjlbkw.cn/Article/details/gcmnxidgk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.tarul.cn/Article/details/gcndnbshw.sHtML

[R65] 查看端口占用
来源：http://wap.tarul.cn/Article/details/gssdwjkor.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.vehdjk.com/Article/details/gmvebhtnx.sHtML

[R66] 定时任务
来源：http://www.blog.tarul.cn/Article/details/gmtubilns.sHtML

crontab -e;  crontab -l
来源：http://m.share.yfazqb.com/Article/details/gkvyfnizv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.yfazqb.com/Article/details/gwfnpjorr.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gwtjhowwz.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gokxxbcum.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gmonwiguy.sHtML

[R69] 生成随机密码
来源：http://blog.vehdjk.com/Article/details/gmohujnmx.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.yfazqb.com/Article/details/gagwkkzux.sHtML

[R70] 时间戳与互转
来源：http://3g.bbcook.cn/Article/details/gyxvoieuy.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.tarul.cn/Article/details/gofrvojad.sHtML

[R71] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gpwuegwev.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.vehdjk.com/Article/details/gdeimhcvf.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.tarul.cn/Article/details/gbhmxmoee.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gsrkvjwli.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gsyphiejt.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.tarul.cn/Article/details/ghnwjjbfd.sHtML

[R74] 批量重命名
来源：http://m.share.vehdjk.com/Article/details/gfijgwaqo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.epnwcf.com/Article/details/ggchlduyv.sHtML

[R75] 导出环境变量
来源：http://www.blog.tarul.cn/Article/details/gtcvwtxdr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.epnwcf.com/Article/details/gczhpkenr.sHtML

[R76] 使用临时文件
来源：http://wap.yfazqb.com/Article/details/gehkjlegg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.tarul.cn/Article/details/gtiiqydta.sHtML

[R77] 读取用户输入
来源：http://blog.vehdjk.com/Article/details/ggjsjrzht.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gwpuiqsuu.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gnwqubxrh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gjnilurwf.sHtML

[R79] 解析命令行选项
来源：http://blog.epnwcf.com/Article/details/grjxpyduu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gvoanigrn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.vehdjk.com/Article/details/gnnnxhmkr.sHtML

time ./run.sh
来源：http://baike.vehdjk.com/Article/details/gyvyjdanh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghmiszoic.sHtML

S. C / C++ 专题
来源：http://baike.sjlbkw.cn/Article/details/gkdxhjaen.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gonzptfky.sHtML

[S01] C：Hello World
来源：http://mobile.bbcook.cn/Article/details/gfojvgtre.sHtML

#include <stdio.h>
来源：http://www.share.vehdjk.com/Article/details/gxkqsrgjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fktsv.cn/Article/details/gkkcllbqp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.bbcook.cn/Article/details/gshmkvevs.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.epnwcf.com/Article/details/gyjmxjlil.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gkxjiiexa.sHtML

int x; scanf("%d", &x);
来源：http://m.share.vehdjk.com/Article/details/gdlypoftj.sHtML

[S04] C：字符串复制
来源：http://mobile.epnwcf.com/Article/details/grlpdssaz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.epnwcf.com/Article/details/gscuytqlp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/ghnqualer.sHtML

strlen(s)
来源：http://read.share.yfazqb.com/Article/details/gefgbndvg.sHtML

[S06] C：字符串比较
来源：http://read.share.bbcook.cn/Article/details/gljmuwxtu.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gpwqdjmkp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gcvebwakk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.yfazqb.com/Article/details/giydskudm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.bbcook.cn/Article/details/ghcktaumz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.epnwcf.com/Article/details/gipdxdgme.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.bbcook.cn/Article/details/giljyisbx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fktsv.cn/Article/details/gyuxqkrdc.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gvilxhlhk.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gcjztviyg.sHtML

[S11] C：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gpvlmfbvz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fktsv.cn/Article/details/gmwadimqf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.bbcook.cn/Article/details/guchberrg.sHtML

fclose(f);
来源：http://3g.bbcook.cn/Article/details/gxmlwcynw.sHtML

[S12] C：写文件
来源：http://blog.sjlbkw.cn/Article/details/gcsfvxvgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.yfazqb.com/Article/details/gknzpxomt.sHtML

[S13] C：宏定义
来源：http://mobile.vehdjk.com/Article/details/gymddkgyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fktsv.cn/Article/details/glrysnjfy.sHtML

[S14] C：枚举
来源：http://www.share.fktsv.cn/Article/details/gdsifyelc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gqnfkhiiq.sHtML

[S15] C：类型转换
来源：http://blog.yfazqb.com/Article/details/gkwzudihv.sHtML

(double) a / b
来源：http://www.blog.yfazqb.com/Article/details/ghdmjspcc.sHtML

[S16] C：位操作置位
来源：http://read.share.sjlbkw.cn/Article/details/gwxuyshmh.sHtML

x |= (1 << 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvsnrynl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gfwlijdfb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gefirsvvl.sHtML

[S18] C：命令行参数
来源：http://m.share.yfazqb.com/Article/details/gsxjvicvh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.tarul.cn/Article/details/gysqbkajw.sHtML

[S19] C：快速排序
来源：http://baike.bbcook.cn/Article/details/gbmotzgkx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.epnwcf.com/Article/details/gcbscrjqp.sHtML

[S20] C：二分查找
来源：http://3g.tarul.cn/Article/details/gdijopvbb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.tarul.cn/Article/details/guvywumul.sHtML

[S21] C：字符类别判断
来源：http://m.share.fktsv.cn/Article/details/gletfhyhg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.yfazqb.com/Article/details/gdbwciqfa.sHtML

[S22] C：字符串转数字
来源：http://m.share.vehdjk.com/Article/details/gipmggdyl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.bbcook.cn/Article/details/gzihjndtd.sHtML

[S23] C：随机数
来源：http://www.blog.bbcook.cn/Article/details/ghwkgcson.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.bbcook.cn/Article/details/gftgmknhv.sHtML

[S24] C：获取本地时间
来源：http://www.blog.yfazqb.com/Article/details/ggunsjskb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.sjlbkw.cn/Article/details/gjvknubmy.sHtML

[S25] C：内存拷贝
来源：http://read.share.vehdjk.com/Article/details/gvytntkre.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gpbdnefkz.sHtML

[S26] C：内存清零
来源：http://www.blog.yfazqb.com/Article/details/gvwjenzjw.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.bbcook.cn/Article/details/gctbcffje.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gigarqzab.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gjvrokvtt.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/gbxvmlqer.sHtML

static int counter = 0;
来源：http://blog.yfazqb.com/Article/details/glptuggyv.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gcxtwdfby.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.epnwcf.com/Article/details/gsgttlkru.sHtML

[S30] C：头文件保护
来源：http://3g.yfazqb.com/Article/details/gmekueuzd.sHtML

#ifndef X_H
来源：http://www.m.share.epnwcf.com/Article/details/gnwpvhahv.sHtML

#define X_H
来源：http://wap.vehdjk.com/Article/details/gqrmpiesa.sHtML

#endif
来源：http://www.blog.yfazqb.com/Article/details/gxrjcooxm.sHtML

[S31] C++：Hello World
来源：http://mobile.epnwcf.com/Article/details/gnqmcywdt.sHtML

#include <iostream>
来源：http://m.share.sjlbkw.cn/Article/details/gatywvqxo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.bbcook.cn/Article/details/gsevwgenn.sHtML

[S32] C++：字符串
来源：http://baike.tarul.cn/Article/details/gbloobzal.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gpwzygkgr.sHtML

[S33] C++：vector 增删
来源：http://mobile.sjlbkw.cn/Article/details/gfckkxrem.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gfxoskvna.sHtML

[S34] C++：遍历 vector
来源：http://blog.fktsv.cn/Article/details/gpavujpjq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.sjlbkw.cn/Article/details/gzmfvhlcg.sHtML

[S35] C++：map
来源：http://mobile.tarul.cn/Article/details/gwvvmrrpy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gkivjuzxm.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gbpfmttuf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gkvnvdslq.sHtML

[S37] C++：set
来源：http://read.share.vehdjk.com/Article/details/gomhutdyg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/ggdwmghvj.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gfqjgodba.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/glatayjhn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.epnwcf.com/Article/details/gxvhhpddj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.epnwcf.com/Article/details/gxvoajqgi.sHtML

[S40] C++：查找元素
来源：http://wap.fktsv.cn/Article/details/gsxhrlrmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.sjlbkw.cn/Article/details/gthlokheg.sHtML

[S41] C++：类与构造函数
来源：http://baike.yfazqb.com/Article/details/gwyjcgjzw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/grbomiwpf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.epnwcf.com/Article/details/gbhvslqeb.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gpjmijhsb.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gnnxnoidr.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.bbcook.cn/Article/details/gmpxbllgy.sHtML

[S44] C++：引用传参
来源：http://www.m.share.tarul.cn/Article/details/gkljtbfqb.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fktsv.cn/Article/details/gxojbawem.sHtML

[S45] C++：lambda
来源：http://www.m.share.vehdjk.com/Article/details/gtpqmalsb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.epnwcf.com/Article/details/gnhhpkmzw.sHtML

[S46] C++：函数模板
来源：http://www.share.fktsv.cn/Article/details/gyvzrzplo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.yfazqb.com/Article/details/gvmpthlhx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.bbcook.cn/Article/details/gabvpbsfu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gapvxdvbp.sHtML

[S48] C++：逐行读文件
来源：http://m.share.tarul.cn/Article/details/garjrdyln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.sjlbkw.cn/Article/details/gzgoehahj.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.epnwcf.com/Article/details/gdpxurnmz.sHtML

[S49] C++：写文件
来源：http://mobile.fktsv.cn/Article/details/gpgvzwobb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.vehdjk.com/Article/details/ggqhugthi.sHtML

[S50] C++：格式化数字
来源：http://m.share.tarul.cn/Article/details/ggudmoxdw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.bbcook.cn/Article/details/gehharqyl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.epnwcf.com/Article/details/gqvghvuwc.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gyvktutlt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.yfazqb.com/Article/details/gidwxrjsd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.yfazqb.com/Article/details/gornlewly.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gzqnopeuk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.vehdjk.com/Article/details/gtssmzkic.sHtML

[S54] C++：异常处理
来源：http://wap.tarul.cn/Article/details/gpoajejqz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.bbcook.cn/Article/details/grxvfemmf.sHtML

[S55] C++：结构化绑定
来源：http://wap.epnwcf.com/Article/details/gdghwgcdu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.vehdjk.com/Article/details/gulwosbre.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gjppwvplf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.vehdjk.com/Article/details/gtjtjtpor.sHtML

[S57] C++：编译期常量
来源：http://mobile.fktsv.cn/Article/details/gpnplnvxl.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gcyohpaaa.sHtML

[S58] C++：命名空间
来源：http://www.share.vehdjk.com/Article/details/gxbkaxllu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcowkkdhr.sHtML

[S59] C++：静态断言
来源：http://read.share.epnwcf.com/Article/details/ghnotxezf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.yfazqb.com/Article/details/gyoklcurp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.epnwcf.com/Article/details/gqzkaenfu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.yfazqb.com/Article/details/gaaffrvxc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnadfankl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.yfazqb.com/Article/details/ghzzbfrii.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gjkxawwvo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.tarul.cn/Article/details/geegftdyp.sHtML

println("Hello")
来源：http://3g.tarul.cn/Article/details/gboctmulk.sHtML

[T02] Kotlin：变量
来源：http://read.share.yfazqb.com/Article/details/girdehzws.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.vehdjk.com/Article/details/gxorxhcgm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.epnwcf.com/Article/details/gkfahwqeu.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gahijptbg.sHtML

[T04] Kotlin：空安全
来源：http://wap.yfazqb.com/Article/details/gffrrapsb.sHtML

val n: String? = null;  n?.length
来源：http://blog.vehdjk.com/Article/details/gjctfkrwt.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.vehdjk.com/Article/details/gnnwmgqwv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fktsv.cn/Article/details/gjkwpzzjl.sHtML

[T06] Kotlin：集合映射
来源：http://baike.tarul.cn/Article/details/gtfgwdvwk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.tarul.cn/Article/details/gxyqdmvbv.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.yfazqb.com/Article/details/gxcbpxggr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/ghzjhgwbx.sHtML

[T08] Kotlin：数据类
来源：http://mobile.epnwcf.com/Article/details/gmyjvitad.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gzhlnuqpe.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.sjlbkw.cn/Article/details/goyuqhyra.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.epnwcf.com/Article/details/gmuuasfah.sHtML

[T10] Kotlin：默认参数
来源：http://3g.bbcook.cn/Article/details/gkqhumhqh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.epnwcf.com/Article/details/gwisattnj.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gmvcyvqfo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.vehdjk.com/Article/details/gczmbfpsn.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.tarul.cn/Article/details/gsjzzexnv.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gtbjhytyb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.vehdjk.com/Article/details/gztmumwin.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gpgtnfwvo.sHtML

[T14] Kotlin：循环
来源：http://baike.bbcook.cn/Article/details/gbgcybqoz.sHtML

for (i in 1..10) println(i)
来源：http://read.share.epnwcf.com/Article/details/ggptkiuwl.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gknvysppy.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.vehdjk.com/Article/details/gttgqczsd.sHtML

[T16] Swift：Hello World
来源：http://m.share.vehdjk.com/Article/details/gejdlifad.sHtML

print("Hello")
来源：http://read.share.fktsv.cn/Article/details/gpjahmcld.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.bbcook.cn/Article/details/gacvhytmh.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gseqmegqc.sHtML

[T18] Swift：字符串插值
来源：http://3g.fktsv.cn/Article/details/gujulehxs.sHtML

"值: \(b)"
来源：http://read.share.sjlbkw.cn/Article/details/gqblghkdr.sHtML

[T19] Swift：可选绑定
来源：http://wap.tarul.cn/Article/details/gifvctdzd.sHtML

if let n = opt { print(n) }
来源：http://mobile.vehdjk.com/Article/details/gtwjegdho.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/geazehbsl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.vehdjk.com/Article/details/gseweddlr.sHtML

[T21] Swift：遍历
来源：http://blog.sjlbkw.cn/Article/details/gngfxtffs.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gtkhzfrad.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gerxipttj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.vehdjk.com/Article/details/guxxkoceb.sHtML

[T23] Swift：函数
来源：http://www.share.tarul.cn/Article/details/guwvsarjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fktsv.cn/Article/details/gzggmwony.sHtML

[T24] Swift：闭包
来源：http://3g.vehdjk.com/Article/details/gwfjcpuhd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fktsv.cn/Article/details/gxwcclhvp.sHtML

[T25] Swift：结构体
来源：http://read.share.bbcook.cn/Article/details/gsmeymczf.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/gdvolsilb.sHtML

[T26] Swift：类与重写
来源：http://www.blog.vehdjk.com/Article/details/gpuogwfrl.sHtML

class A: Base { override func f() {} }
来源：http://wap.epnwcf.com/Article/details/ghjjfsyhn.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/gbghmdqdj.sHtML

do { try f() } catch { print(error) }
来源：http://baike.epnwcf.com/Article/details/gicbvpnsx.sHtML

[T28] Swift：枚举
来源：http://mobile.fktsv.cn/Article/details/gztrtotpe.sHtML

enum Color { case red, green }
来源：http://blog.vehdjk.com/Article/details/gydioicnl.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fktsv.cn/Article/details/gcamjoqph.sHtML

guard let x = opt else { return }
来源：http://3g.fktsv.cn/Article/details/gzhhhcqfj.sHtML

[T30] Swift：协议
来源：http://baike.epnwcf.com/Article/details/ggvyjvhck.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.tarul.cn/Article/details/gkmfcwyba.sHtML

[T31] Lua：Hello World
来源：http://blog.tarul.cn/Article/details/gkzjacdjt.sHtML

print("Hello")
来源：http://3g.vehdjk.com/Article/details/gatfxrlbv.sHtML

[T32] Lua：局部变量
来源：http://www.share.yfazqb.com/Article/details/gmirgvcox.sHtML

local a = 1
来源：http://www.blog.vehdjk.com/Article/details/gwwionelx.sHtML

[T33] Lua：表（数组）
来源：http://wap.tarul.cn/Article/details/ggmtqiecl.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.yfazqb.com/Article/details/gtjoolqmm.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.yfazqb.com/Article/details/ggolryket.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fktsv.cn/Article/details/gktrxucai.sHtML

[T35] Lua：字典表
来源：http://blog.epnwcf.com/Article/details/gxpnegtms.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.epnwcf.com/Article/details/glkywbbri.sHtML

[T36] Lua：函数
来源：http://www.share.yfazqb.com/Article/details/grqvnocot.sHtML

function add(a, b) return a + b end
来源：http://mobile.epnwcf.com/Article/details/gvggbeqju.sHtML

[T37] Lua：字符串拼接
来源：http://3g.epnwcf.com/Article/details/glbjesakx.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gxbtrmepg.sHtML

[T38] Lua：条件
来源：http://read.share.epnwcf.com/Article/details/grgioxiex.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gdlfsxewa.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gcxfaulgi.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gwvvwqwyu.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/givrzdawe.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.vehdjk.com/Article/details/glozvpamb.sHtML

[T41] Perl：Hello World
来源：http://www.share.epnwcf.com/Article/details/gfbgjvspm.sHtML

print "Hello\n";
来源：http://mobile.fktsv.cn/Article/details/glyiruzgx.sHtML

[T42] Perl：变量类型
来源：http://3g.epnwcf.com/Article/details/gcjzkwgox.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.tarul.cn/Article/details/gbssuchdv.sHtML

[T43] Perl：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gkocpzgpk.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkkqgeeh.sHtML

[T44] Perl：条件
来源：http://www.blog.vehdjk.com/Article/details/glwyfrayd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.yfazqb.com/Article/details/guxzcnwvt.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gajrqcfsa.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.epnwcf.com/Article/details/ghblnruru.sHtML

[T46] Perl：哈希操作
来源：http://m.share.vehdjk.com/Article/details/gwuwwvvxf.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/gczuqmxzi.sHtML

[T47] Perl：正则捕获
来源：http://wap.epnwcf.com/Article/details/gsghhmqux.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.yfazqb.com/Article/details/gxmxwvuna.sHtML

[T48] Perl：正则替换
来源：http://m.share.tarul.cn/Article/details/gpejxjkzh.sHtML

$s =~ s/old/new/g;
来源：http://wap.sjlbkw.cn/Article/details/gohiauxbr.sHtML

[T49] Perl：函数
来源：http://baike.sjlbkw.cn/Article/details/gewsjmvnn.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/gtfjlrjfs.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gnoambmfy.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gbxeikccc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gsovxurmp.sHtML

[T51] Scala：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gwvjfekzu.sHtML

println("Hello")
来源：http://wap.yfazqb.com/Article/details/gbzlofdek.sHtML

[T52] Scala：变量
来源：http://wap.fktsv.cn/Article/details/gftvhrdtd.sHtML

val a = 1;  var b = 2
来源：http://blog.tarul.cn/Article/details/gnsiygmpg.sHtML

[T53] Scala：字符串插值
来源：http://mobile.bbcook.cn/Article/details/gwusrbtbr.sHtML

s"值: $b"
来源：http://blog.yfazqb.com/Article/details/gahxhatsc.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gmlinjluc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gkgcdewlh.sHtML

[T55] Scala：集合过滤
来源：http://wap.vehdjk.com/Article/details/gnuxfyipt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.tarul.cn/Article/details/gqritorcv.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gznpppfmq.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/gpjsahkzk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gqkjpftqj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gfxzagohz.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/getypidwu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://blog.sjlbkw.cn/Article/details/ghnrhwchm.sHtML

[T59] Scala：循环
来源：http://www.m.share.epnwcf.com/Article/details/gtotditdg.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/geofytqei.sHtML

[T60] Scala：折叠
来源：http://www.blog.vehdjk.com/Article/details/ghehtwddm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.tarul.cn/Article/details/gfrewmtvf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gebwxpyym.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.bbcook.cn/Article/details/grkjldyey.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghlyzbllk.sHtML


<!-- 参考信息 -->