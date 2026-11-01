代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.yfazqb.com/Article/details/gpvjieygc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.tarul.cn/Article/details/gcwovxpyu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.bbcook.cn/Article/details/gtgidycqk.sHtML

[R61] 磁盘占用
来源：http://wap.vehdjk.com/Article/details/gglqqigrq.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/guqbfbapc.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.tarul.cn/Article/details/gxmdkkcym.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.bbcook.cn/Article/details/gpruiwxro.sHtML

[R63] 内存与进程
来源：http://read.share.yfazqb.com/Article/details/gmprzffhk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.epnwcf.com/Article/details/gjbbbawdb.sHtML

[R64] 结束进程
来源：http://m.share.vehdjk.com/Article/details/gienydlex.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.yfazqb.com/Article/details/gzbswvcja.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gkcrmyrof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.vehdjk.com/Article/details/gwvrisxqq.sHtML

[R66] 定时任务
来源：http://wap.bbcook.cn/Article/details/ghrytewnj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gdptadrrm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.bbcook.cn/Article/details/gvewewovb.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/grawmiiiu.sHtML

[R68] 计算文件校验值
来源：http://baike.tarul.cn/Article/details/gzghmmwry.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gnfydlvar.sHtML

[R69] 生成随机密码
来源：http://www.m.share.bbcook.cn/Article/details/giusdhtfs.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fktsv.cn/Article/details/gnwbfmzlx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gptgwxhmt.sHtML

date +%s;  date -d @1700000000
来源：http://3g.vehdjk.com/Article/details/gkozxextc.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gtswnuoqx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.yfazqb.com/Article/details/gadrnywrw.sHtML

[R72] 等待端口就绪
来源：http://m.share.sjlbkw.cn/Article/details/gzwkbxbbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/geldrpcpm.sHtML

[R73] 分割大日志
来源：http://read.share.bbcook.cn/Article/details/giluppuae.sHtML

split -l 1000 big.log part_
来源：http://blog.tarul.cn/Article/details/gekgdkkmw.sHtML

[R74] 批量重命名
来源：http://wap.yfazqb.com/Article/details/gdqcaenpm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fktsv.cn/Article/details/gemuykiev.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gjbcrzors.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwumvncd.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/govvzjhqx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.bbcook.cn/Article/details/gqhsxzmxh.sHtML

[R77] 读取用户输入
来源：http://wap.yfazqb.com/Article/details/gkvyrnuzx.sHtML

read -rp "请输入: " ans
来源：http://read.share.fktsv.cn/Article/details/gsywjtvye.sHtML

[R78] 交互式菜单
来源：http://www.share.bbcook.cn/Article/details/ggyfgcjeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.bbcook.cn/Article/details/giaycxvkd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.epnwcf.com/Article/details/gugulwetl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.epnwcf.com/Article/details/gjbcnldeq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/gcaqcjcwi.sHtML

time ./run.sh
来源：http://3g.epnwcf.com/Article/details/gwgqkiynk.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gawrfvlcd.sHtML

S. C / C++ 专题
来源：http://read.share.epnwcf.com/Article/details/gybmnfgyc.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwqidorq.sHtML

[S01] C：Hello World
来源：http://baike.bbcook.cn/Article/details/gfndsfabw.sHtML

#include <stdio.h>
来源：http://www.m.share.sjlbkw.cn/Article/details/gipmigtao.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gcgunilyu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/grsxmaowr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.bbcook.cn/Article/details/gbvvplsyy.sHtML

[S03] C：读入整数
来源：http://read.share.sjlbkw.cn/Article/details/gpmblqxrg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.bbcook.cn/Article/details/gfuduheoz.sHtML

[S04] C：字符串复制
来源：http://3g.tarul.cn/Article/details/gezhmwwpo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.sjlbkw.cn/Article/details/gvodomnln.sHtML

[S05] C：字符串长度
来源：http://www.share.vehdjk.com/Article/details/gcljoceta.sHtML

strlen(s)
来源：http://3g.epnwcf.com/Article/details/gfjnqgzya.sHtML

[S06] C：字符串比较
来源：http://blog.tarul.cn/Article/details/gpebyjlww.sHtML

strcmp(a, b) == 0
来源：http://read.share.vehdjk.com/Article/details/gtydjywmh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gtunvhyib.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.epnwcf.com/Article/details/gdwodrssy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gkezvmpeu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.tarul.cn/Article/details/gpcuhwmpi.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.sjlbkw.cn/Article/details/gqvbumrwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.sjlbkw.cn/Article/details/gqjuiircr.sHtML

[S10] C：指针与解引用
来源：http://www.share.bbcook.cn/Article/details/gyvraepmq.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gqabpaati.sHtML

[S11] C：逐行读文件
来源：http://3g.bbcook.cn/Article/details/gqeuvezcj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fktsv.cn/Article/details/gpkmlbruz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.sjlbkw.cn/Article/details/gzvekbmmh.sHtML

fclose(f);
来源：http://3g.sjlbkw.cn/Article/details/gagzqlura.sHtML

[S12] C：写文件
来源：http://baike.bbcook.cn/Article/details/gwkrvplyj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.yfazqb.com/Article/details/gfwsxmdbh.sHtML

[S13] C：宏定义
来源：http://read.share.epnwcf.com/Article/details/gmynhszrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.epnwcf.com/Article/details/guoczgggq.sHtML

[S14] C：枚举
来源：http://baike.tarul.cn/Article/details/gcwxdotvl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.bbcook.cn/Article/details/gehpqahhj.sHtML

[S15] C：类型转换
来源：http://read.share.yfazqb.com/Article/details/ghfplbhpp.sHtML

(double) a / b
来源：http://wap.bbcook.cn/Article/details/goglnbeyg.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/guyygpsyh.sHtML

x |= (1 << 3);
来源：http://blog.vehdjk.com/Article/details/gyunehsct.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.tarul.cn/Article/details/gozzqickr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.vehdjk.com/Article/details/gcgagwoey.sHtML

[S18] C：命令行参数
来源：http://wap.fktsv.cn/Article/details/guwrblhph.sHtML

int main(int argc, char **argv)
来源：http://www.blog.epnwcf.com/Article/details/gzllzfztq.sHtML

[S19] C：快速排序
来源：http://read.share.fktsv.cn/Article/details/gwgzatyjz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.sjlbkw.cn/Article/details/ginpscwud.sHtML

[S20] C：二分查找
来源：http://blog.bbcook.cn/Article/details/gubdvufmc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.sjlbkw.cn/Article/details/ghzdbskye.sHtML

[S21] C：字符类别判断
来源：http://blog.yfazqb.com/Article/details/gzknnzmxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.sjlbkw.cn/Article/details/ggazdnccc.sHtML

[S22] C：字符串转数字
来源：http://mobile.tarul.cn/Article/details/gfhohzvru.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.vehdjk.com/Article/details/ggazznyyy.sHtML

[S23] C：随机数
来源：http://blog.tarul.cn/Article/details/gznbxlced.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.vehdjk.com/Article/details/gqleddeqp.sHtML

[S24] C：获取本地时间
来源：http://www.share.vehdjk.com/Article/details/guogtiwma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gdjsozpvh.sHtML

[S25] C：内存拷贝
来源：http://read.share.bbcook.cn/Article/details/gcycccchj.sHtML

memcpy(dst, src, n);
来源：http://www.share.fktsv.cn/Article/details/gpitdyxff.sHtML

[S26] C：内存清零
来源：http://www.m.share.vehdjk.com/Article/details/gculttyne.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/gzllvdakz.sHtML

[S27] C：定义常量
来源：http://www.share.vehdjk.com/Article/details/gpmorpelr.sHtML

const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gbneecmis.sHtML

[S28] C：静态变量
来源：http://3g.fktsv.cn/Article/details/gllwazhms.sHtML

static int counter = 0;
来源：http://www.share.epnwcf.com/Article/details/grltfjgbd.sHtML

[S29] C：变参函数
来源：http://m.share.tarul.cn/Article/details/gohpwaxiz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.bbcook.cn/Article/details/gpmellyrv.sHtML

[S30] C：头文件保护
来源：http://read.share.vehdjk.com/Article/details/ggswuzote.sHtML

#ifndef X_H
来源：http://m.share.sjlbkw.cn/Article/details/gpgvdjwzs.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/ghddhhhwf.sHtML

#endif
来源：http://blog.vehdjk.com/Article/details/gwomqkipx.sHtML

[S31] C++：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/glsesbqjg.sHtML

#include <iostream>
来源：http://www.m.share.fktsv.cn/Article/details/gjgffqxxz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.epnwcf.com/Article/details/ghwpfmxzx.sHtML

[S32] C++：字符串
来源：http://3g.sjlbkw.cn/Article/details/gbceddooh.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.sjlbkw.cn/Article/details/gckmweath.sHtML

[S33] C++：vector 增删
来源：http://blog.tarul.cn/Article/details/ggunwdjfz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gmeluyktr.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gsgaytvbl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.sjlbkw.cn/Article/details/ghnlkbqlz.sHtML

[S35] C++：map
来源：http://www.blog.yfazqb.com/Article/details/gmxkqvqoa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gjdmwbrxh.sHtML

[S36] C++：unordered_map
来源：http://mobile.sjlbkw.cn/Article/details/gpzjupsty.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gtpehjexx.sHtML

[S37] C++：set
来源：http://3g.vehdjk.com/Article/details/gbrlmtgdv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.yfazqb.com/Article/details/glzijcsdp.sHtML

[S38] C++：排序
来源：http://m.share.bbcook.cn/Article/details/geaioxofb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.epnwcf.com/Article/details/gziitmuqs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.tarul.cn/Article/details/gzffaydry.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gifmtgqwp.sHtML

[S40] C++：查找元素
来源：http://m.share.vehdjk.com/Article/details/gaoteacun.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.yfazqb.com/Article/details/grhmexnhc.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/geowbofdo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.sjlbkw.cn/Article/details/gvvlynzxp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fktsv.cn/Article/details/gduzgapuc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.vehdjk.com/Article/details/gmtcrliwa.sHtML

[S43] C++：智能指针
来源：http://www.blog.vehdjk.com/Article/details/gaofwfenh.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.vehdjk.com/Article/details/gsbzorxai.sHtML

[S44] C++：引用传参
来源：http://m.share.tarul.cn/Article/details/gfdsvupaa.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.tarul.cn/Article/details/goomgfixb.sHtML

[S45] C++：lambda
来源：http://read.share.bbcook.cn/Article/details/gjsnlejwl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.bbcook.cn/Article/details/gpzdfjvfm.sHtML

[S46] C++：函数模板
来源：http://m.share.fktsv.cn/Article/details/gvlzpbene.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.tarul.cn/Article/details/gtbxgixkl.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.epnwcf.com/Article/details/gbfkefzrb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsumxynna.sHtML

[S48] C++：逐行读文件
来源：http://read.share.sjlbkw.cn/Article/details/gxrxbqbdt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fktsv.cn/Article/details/gobgtzeoj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/ghtcpoicz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fktsv.cn/Article/details/guuwybsqt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.epnwcf.com/Article/details/gshbgligd.sHtML

[S50] C++：格式化数字
来源：http://wap.tarul.cn/Article/details/gwsinqnns.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.vehdjk.com/Article/details/gcyzxopzj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.tarul.cn/Article/details/gnzzramoz.sHtML

static_cast<double>(a) / b
来源：http://www.share.vehdjk.com/Article/details/gywwkksrh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fktsv.cn/Article/details/gsforurmp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.epnwcf.com/Article/details/gfhchvjah.sHtML

[S53] C++：移动语义
来源：http://www.blog.vehdjk.com/Article/details/gjxseggbu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.yfazqb.com/Article/details/ghiudyvph.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gytppqwty.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.bbcook.cn/Article/details/gzfqfantr.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.bbcook.cn/Article/details/gymggdfeh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.tarul.cn/Article/details/gaovaarlk.sHtML

[S56] C++：optional
来源：http://www.m.share.yfazqb.com/Article/details/ghpneldjz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.sjlbkw.cn/Article/details/gciuhshfh.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.yfazqb.com/Article/details/gxhtiqtlf.sHtML

constexpr int N = 10;
来源：http://wap.tarul.cn/Article/details/gxfecfquy.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fktsv.cn/Article/details/gbblnlpmt.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.vehdjk.com/Article/details/gjvjiaxwa.sHtML

[S59] C++：静态断言
来源：http://mobile.fktsv.cn/Article/details/ganbgfxgy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.sjlbkw.cn/Article/details/gbevkgahi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.epnwcf.com/Article/details/gknqesdie.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fktsv.cn/Article/details/gznmpgvgj.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkzmsledf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/gglwuvxgu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnzrcgenz.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gqwunsyjd.sHtML

println("Hello")
来源：http://blog.fktsv.cn/Article/details/gymoatfnz.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/goykmhewa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.vehdjk.com/Article/details/gwkxagjmd.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.epnwcf.com/Article/details/geexdxgvv.sHtML

"值: $b"
来源：http://mobile.bbcook.cn/Article/details/gwckmqpbe.sHtML

[T04] Kotlin：空安全
来源：http://m.share.vehdjk.com/Article/details/gadfarodr.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gmgjvuskm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fktsv.cn/Article/details/gpsyqytpj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.tarul.cn/Article/details/gkuarttdo.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fktsv.cn/Article/details/gpwuumyul.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.bbcook.cn/Article/details/gurjsrfrx.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.tarul.cn/Article/details/gobmjwars.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fktsv.cn/Article/details/gywiznhkl.sHtML

[T08] Kotlin：数据类
来源：http://m.share.sjlbkw.cn/Article/details/gmvfvtiwb.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.sjlbkw.cn/Article/details/gwobiuitx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/glufzjyta.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fktsv.cn/Article/details/gyeabnelz.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fktsv.cn/Article/details/gagkeuifo.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.bbcook.cn/Article/details/gdhrotnam.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gltlqbitb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.sjlbkw.cn/Article/details/gsqpguqiz.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.tarul.cn/Article/details/gdvleprel.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gfmkumcsx.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.tarul.cn/Article/details/gpjbfuclb.sHtML

val m = mapOf("a" to 1)
来源：http://wap.epnwcf.com/Article/details/gxumykctu.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/gujxeelch.sHtML

for (i in 1..10) println(i)
来源：http://blog.fktsv.cn/Article/details/gtqeyvkmx.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/ghekpvvgg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/grmpcbxyv.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuzbzloc.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/goibnjhjd.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/gubhohmrm.sHtML

var a = 1;  let b = 2
来源：http://www.share.sjlbkw.cn/Article/details/gwgevsymb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gqakrkfgw.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/gyapedbhj.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fktsv.cn/Article/details/guhobvhnw.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gzcrempci.sHtML

[T20] Swift：数组操作
来源：http://baike.bbcook.cn/Article/details/greqqlsih.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.sjlbkw.cn/Article/details/gjxzomdsw.sHtML

[T21] Swift：遍历
来源：http://3g.tarul.cn/Article/details/glkfkmktp.sHtML

for x in a { print(x) }
来源：http://www.m.share.bbcook.cn/Article/details/grmpkdvyf.sHtML

[T22] Swift：字典
来源：http://baike.tarul.cn/Article/details/gkjalpnhv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.bbcook.cn/Article/details/gmjiuaohm.sHtML

[T23] Swift：函数
来源：http://blog.vehdjk.com/Article/details/gshqtwfzh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gztpceyve.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gyslceckp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/ggvdbqnhb.sHtML

[T25] Swift：结构体
来源：http://www.share.tarul.cn/Article/details/gzkqxdgnq.sHtML

struct P { var x: Int }
来源：http://blog.tarul.cn/Article/details/gwysjrfrv.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.tarul.cn/Article/details/gojzpojdk.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gixsvfvkt.sHtML

[T27] Swift：错误处理
来源：http://3g.sjlbkw.cn/Article/details/gwrhovhro.sHtML

do { try f() } catch { print(error) }
来源：http://3g.epnwcf.com/Article/details/gsfuotwlf.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gwxwzglmm.sHtML

enum Color { case red, green }
来源：http://www.blog.fktsv.cn/Article/details/giadyapum.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.tarul.cn/Article/details/gabmarujx.sHtML

guard let x = opt else { return }
来源：http://blog.bbcook.cn/Article/details/gyuajpiig.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gxpmmqmzy.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gfjpweihi.sHtML

[T31] Lua：Hello World
来源：http://www.share.tarul.cn/Article/details/gvytjjsid.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/gqkacyjps.sHtML

[T32] Lua：局部变量
来源：http://m.share.bbcook.cn/Article/details/gvafvvebh.sHtML

local a = 1
来源：http://www.blog.yfazqb.com/Article/details/gbozzzxnd.sHtML

[T33] Lua：表（数组）
来源：http://3g.epnwcf.com/Article/details/gevctjiye.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.tarul.cn/Article/details/gdrqllknw.sHtML

[T34] Lua：遍历表
来源：http://m.share.epnwcf.com/Article/details/gbtufnthn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.sjlbkw.cn/Article/details/gikcwlomb.sHtML

[T35] Lua：字典表
来源：http://www.share.bbcook.cn/Article/details/ghevvpbwv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.vehdjk.com/Article/details/gxdnrcsqx.sHtML

[T36] Lua：函数
来源：http://www.m.share.bbcook.cn/Article/details/gjlrrgruu.sHtML

function add(a, b) return a + b end
来源：http://blog.sjlbkw.cn/Article/details/grgnewmju.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gjvqzpvog.sHtML

"a" .. "b"
来源：http://mobile.vehdjk.com/Article/details/gkosccgyj.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/gcqfbwcah.sHtML

if x > 0 then print("正") end
来源：http://read.share.yfazqb.com/Article/details/gxlrcdzsg.sHtML

[T39] Lua：模式匹配
来源：http://wap.fktsv.cn/Article/details/gaywtyvdu.sHtML

string.find(s, "%d+")
来源：http://blog.yfazqb.com/Article/details/gqndoclbg.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/grkcqchoq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gkshkphss.sHtML

[T41] Perl：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gtuglvojg.sHtML

print "Hello\n";
来源：http://3g.bbcook.cn/Article/details/gjhxxpvam.sHtML

[T42] Perl：变量类型
来源：http://wap.epnwcf.com/Article/details/gawdljscb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.sjlbkw.cn/Article/details/gfngnwvlw.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gnzjohahs.sHtML

"值: $a"
来源：http://mobile.fktsv.cn/Article/details/gjyjmwtqj.sHtML

[T44] Perl：条件
来源：http://wap.tarul.cn/Article/details/ganjebjws.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.vehdjk.com/Article/details/gmqotzcfm.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gubxlenhx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.bbcook.cn/Article/details/ghuarcalk.sHtML

[T46] Perl：哈希操作
来源：http://mobile.tarul.cn/Article/details/gxhnfxzek.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fktsv.cn/Article/details/grsdjtamx.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fktsv.cn/Article/details/gqhzwnwup.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.epnwcf.com/Article/details/ginmbvlhu.sHtML

[T48] Perl：正则替换
来源：http://read.share.sjlbkw.cn/Article/details/gbugoschv.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/guwhrjvfr.sHtML

[T49] Perl：函数
来源：http://read.share.sjlbkw.cn/Article/details/gtferndhg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gjaosbwtx.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gidiznyfg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fktsv.cn/Article/details/gvaugeizl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.vehdjk.com/Article/details/gctclmgru.sHtML

[T51] Scala：Hello World
来源：http://read.share.yfazqb.com/Article/details/gcsqyoqqa.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/ghzasncqx.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/ghnmhysvl.sHtML

val a = 1;  var b = 2
来源：http://mobile.epnwcf.com/Article/details/glezcqlxa.sHtML

[T53] Scala：字符串插值
来源：http://baike.bbcook.cn/Article/details/ghxlszqeb.sHtML

s"值: $b"
来源：http://read.share.tarul.cn/Article/details/gdgbhijnf.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fktsv.cn/Article/details/ghxvyhhqt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjvlvqmhr.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gejinphhv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.vehdjk.com/Article/details/gfvgwmwub.sHtML

[T56] Scala：样例类
来源：http://3g.epnwcf.com/Article/details/gxabggovx.sHtML

case class User(name: String, age: Int)
来源：http://mobile.yfazqb.com/Article/details/gepfdaydg.sHtML

[T57] Scala：模式匹配
来源：http://m.share.tarul.cn/Article/details/gbunjqssd.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/giqhtjocb.sHtML

[T58] Scala：函数定义
来源：http://read.share.yfazqb.com/Article/details/gketspsnj.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.bbcook.cn/Article/details/gkacojigt.sHtML

[T59] Scala：循环
来源：http://www.share.tarul.cn/Article/details/gububhpnr.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.tarul.cn/Article/details/gasqafzse.sHtML

[T60] Scala：折叠
来源：http://read.share.vehdjk.com/Article/details/gqomicnfz.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.sjlbkw.cn/Article/details/geemuyomh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpeuymfru.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/geezrwpjq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkdbzrwrg.sHtML


<!-- 参考信息 -->