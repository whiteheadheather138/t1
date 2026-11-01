代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gkgkidbcm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gfskjhulx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.vehdjk.com/Article/details/gzwxtfmjn.sHtML

[R61] 磁盘占用
来源：http://www.share.yfazqb.com/Article/details/gyzcppfor.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gqdigbsuo.sHtML

[R62] 找最占空间的文件
来源：http://blog.sjlbkw.cn/Article/details/gajqzwxew.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.sjlbkw.cn/Article/details/gjirfyffa.sHtML

[R63] 内存与进程
来源：http://3g.sjlbkw.cn/Article/details/gcrzrprxa.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.bbcook.cn/Article/details/gupwblzcv.sHtML

[R64] 结束进程
来源：http://www.share.epnwcf.com/Article/details/gvmdxsssn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.epnwcf.com/Article/details/gjmewqdma.sHtML

[R65] 查看端口占用
来源：http://baike.yfazqb.com/Article/details/gogkumvsc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.bbcook.cn/Article/details/gnpclcoat.sHtML

[R66] 定时任务
来源：http://read.share.fktsv.cn/Article/details/gyzrtdtiy.sHtML

crontab -e;  crontab -l
来源：http://www.share.yfazqb.com/Article/details/gztrfmdja.sHtML

[R67] 生成随机十六进制串
来源：http://baike.tarul.cn/Article/details/gkrgwsiwo.sHtML

openssl rand -hex 16
来源：http://blog.bbcook.cn/Article/details/gshjxfgvi.sHtML

[R68] 计算文件校验值
来源：http://blog.tarul.cn/Article/details/gvpfphllx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.vehdjk.com/Article/details/gchpinamt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.tarul.cn/Article/details/gfvxetjnr.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/gngawzurq.sHtML

[R70] 时间戳与互转
来源：http://mobile.bbcook.cn/Article/details/glfgqjeoh.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.sjlbkw.cn/Article/details/gatscklka.sHtML

[R71] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gtzyawmia.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.yfazqb.com/Article/details/gmybjsldk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.epnwcf.com/Article/details/geibmebbp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.vehdjk.com/Article/details/gqrulifwh.sHtML

[R73] 分割大日志
来源：http://3g.tarul.cn/Article/details/goydtptse.sHtML

split -l 1000 big.log part_
来源：http://baike.vehdjk.com/Article/details/gpemrjedr.sHtML

[R74] 批量重命名
来源：http://3g.epnwcf.com/Article/details/gpiljdght.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.epnwcf.com/Article/details/gllpdzzsr.sHtML

[R75] 导出环境变量
来源：http://mobile.bbcook.cn/Article/details/ghjhlbkoi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.sjlbkw.cn/Article/details/gaozvheey.sHtML

[R76] 使用临时文件
来源：http://mobile.yfazqb.com/Article/details/glpfpkddf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.yfazqb.com/Article/details/gdjohlarw.sHtML

[R77] 读取用户输入
来源：http://read.share.fktsv.cn/Article/details/goxvtyyxj.sHtML

read -rp "请输入: " ans
来源：http://mobile.yfazqb.com/Article/details/galklorps.sHtML

[R78] 交互式菜单
来源：http://wap.epnwcf.com/Article/details/gwgyhhgva.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fktsv.cn/Article/details/gytlwobbw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.bbcook.cn/Article/details/guwhdwmjy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.tarul.cn/Article/details/gqvgdnxla.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.tarul.cn/Article/details/gnnwuldeu.sHtML

time ./run.sh
来源：http://3g.sjlbkw.cn/Article/details/gyenccxgc.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvnvmbvpq.sHtML

S. C / C++ 专题
来源：http://read.share.tarul.cn/Article/details/gqxwlqrrk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnfyslukz.sHtML

[S01] C：Hello World
来源：http://read.share.epnwcf.com/Article/details/gydjtigxq.sHtML

#include <stdio.h>
来源：http://www.m.share.bbcook.cn/Article/details/gewedjcby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.sjlbkw.cn/Article/details/gnljkufgw.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.sjlbkw.cn/Article/details/gslqjnfiv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.bbcook.cn/Article/details/geaxmgysx.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/grzxdrzqb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.bbcook.cn/Article/details/gfwvkseme.sHtML

[S04] C：字符串复制
来源：http://baike.fktsv.cn/Article/details/gvrkgfjos.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.vehdjk.com/Article/details/ggwfzivod.sHtML

[S05] C：字符串长度
来源：http://baike.epnwcf.com/Article/details/gqpezgzpv.sHtML

strlen(s)
来源：http://www.share.sjlbkw.cn/Article/details/gczekbgbi.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gbswsstvq.sHtML

strcmp(a, b) == 0
来源：http://m.share.sjlbkw.cn/Article/details/grrlzbfxm.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/gruagszxm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.bbcook.cn/Article/details/ghathxbqk.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.bbcook.cn/Article/details/gdoshcjgx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.tarul.cn/Article/details/gvjukdkxs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.bbcook.cn/Article/details/gqczufwdu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.tarul.cn/Article/details/gpouckytj.sHtML

[S10] C：指针与解引用
来源：http://read.share.tarul.cn/Article/details/gexrgwrbs.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fktsv.cn/Article/details/gmvsnxjao.sHtML

[S11] C：逐行读文件
来源：http://baike.sjlbkw.cn/Article/details/grvwgzidu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.yfazqb.com/Article/details/gkpylxnnz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.yfazqb.com/Article/details/gbfydsxqr.sHtML

fclose(f);
来源：http://blog.vehdjk.com/Article/details/gczuhebho.sHtML

[S12] C：写文件
来源：http://blog.bbcook.cn/Article/details/geurirovf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fktsv.cn/Article/details/gpliybwar.sHtML

[S13] C：宏定义
来源：http://www.share.yfazqb.com/Article/details/gctleronz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gyawojsks.sHtML

[S14] C：枚举
来源：http://www.blog.tarul.cn/Article/details/gzxjfmwpy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.tarul.cn/Article/details/gezsvbpfv.sHtML

[S15] C：类型转换
来源：http://wap.epnwcf.com/Article/details/gwbqawcmr.sHtML

(double) a / b
来源：http://mobile.fktsv.cn/Article/details/gcqmpaime.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gwmxrbngm.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gtjxruqsz.sHtML

[S17] C：安全拼接字符串
来源：http://baike.bbcook.cn/Article/details/gpjfznlrd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.yfazqb.com/Article/details/gonlrjksi.sHtML

[S18] C：命令行参数
来源：http://blog.vehdjk.com/Article/details/glyfokruc.sHtML

int main(int argc, char **argv)
来源：http://mobile.epnwcf.com/Article/details/guucfhhds.sHtML

[S19] C：快速排序
来源：http://blog.fktsv.cn/Article/details/glcrhsakf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gpajkslay.sHtML

[S20] C：二分查找
来源：http://www.share.fktsv.cn/Article/details/gosgnzrqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.vehdjk.com/Article/details/geyyojllf.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gscosgjcj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.tarul.cn/Article/details/gvjsndwwv.sHtML

[S22] C：字符串转数字
来源：http://3g.yfazqb.com/Article/details/gqitbzjep.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gjeefpxqi.sHtML

[S23] C：随机数
来源：http://3g.vehdjk.com/Article/details/gdvjlepiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gkgufbfgc.sHtML

[S24] C：获取本地时间
来源：http://read.share.vehdjk.com/Article/details/gqlvwgwwo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.sjlbkw.cn/Article/details/gyebyddzi.sHtML

[S25] C：内存拷贝
来源：http://mobile.vehdjk.com/Article/details/gomixxtuz.sHtML

memcpy(dst, src, n);
来源：http://www.blog.yfazqb.com/Article/details/gaykyaswl.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gxjxymidq.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.epnwcf.com/Article/details/gzuugrfya.sHtML

[S27] C：定义常量
来源：http://m.share.vehdjk.com/Article/details/gcfnlrfrz.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gcpmjueve.sHtML

[S28] C：静态变量
来源：http://www.blog.bbcook.cn/Article/details/gpeizhsrz.sHtML

static int counter = 0;
来源：http://wap.epnwcf.com/Article/details/grqrducuz.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/gwpxswvyt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.yfazqb.com/Article/details/gxutxuuvx.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/ghpovhfwv.sHtML

#ifndef X_H
来源：http://m.share.fktsv.cn/Article/details/gaqfcgxri.sHtML

#define X_H
来源：http://3g.tarul.cn/Article/details/glsejoorl.sHtML

#endif
来源：http://wap.yfazqb.com/Article/details/gdpmsoivb.sHtML

[S31] C++：Hello World
来源：http://baike.vehdjk.com/Article/details/giswkwlzc.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/gxxuysims.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fktsv.cn/Article/details/gqgavxlex.sHtML

[S32] C++：字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdscemcph.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.yfazqb.com/Article/details/gqvhrwmbe.sHtML

[S33] C++：vector 增删
来源：http://blog.epnwcf.com/Article/details/gxzkwvlbz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fktsv.cn/Article/details/grjosvsgm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.sjlbkw.cn/Article/details/gkbrqfizc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.sjlbkw.cn/Article/details/glposqnke.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gtdaljnyv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fktsv.cn/Article/details/ghztopfyk.sHtML

[S36] C++：unordered_map
来源：http://wap.epnwcf.com/Article/details/gmtobwgym.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gecwpcqji.sHtML

[S37] C++：set
来源：http://www.share.vehdjk.com/Article/details/gsgalydmx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.bbcook.cn/Article/details/geelfirlg.sHtML

[S38] C++：排序
来源：http://blog.yfazqb.com/Article/details/geojmukcx.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.epnwcf.com/Article/details/ghayvxpkt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.yfazqb.com/Article/details/gmznfmzke.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.bbcook.cn/Article/details/godzygaap.sHtML

[S40] C++：查找元素
来源：http://baike.sjlbkw.cn/Article/details/gxzgzsdmk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fktsv.cn/Article/details/gwyucbnix.sHtML

[S41] C++：类与构造函数
来源：http://m.share.bbcook.cn/Article/details/gwgvrzhmx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gscxyllro.sHtML

[S42] C++：继承与虚函数
来源：http://3g.epnwcf.com/Article/details/gvkbxiklc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fktsv.cn/Article/details/gfzithjtn.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gaerjlpuq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeuwwkqw.sHtML

[S44] C++：引用传参
来源：http://www.share.bbcook.cn/Article/details/ggqovyrku.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.epnwcf.com/Article/details/gazyfgbgu.sHtML

[S45] C++：lambda
来源：http://read.share.fktsv.cn/Article/details/guvecgyog.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.vehdjk.com/Article/details/gbkvzznhf.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/ggupinvbh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.bbcook.cn/Article/details/gleammaag.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.bbcook.cn/Article/details/gjhjvzqum.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.yfazqb.com/Article/details/ggevwsndh.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gkgmgockb.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.vehdjk.com/Article/details/gidoezvsz.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.yfazqb.com/Article/details/gylfohjea.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gzvxtahos.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.sjlbkw.cn/Article/details/gopocojip.sHtML

[S50] C++：格式化数字
来源：http://www.share.fktsv.cn/Article/details/ggqbfejzt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gbedmmiyy.sHtML

[S51] C++：显式类型转换
来源：http://blog.bbcook.cn/Article/details/gfkqvfigf.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gkyedryrh.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqzsmwuh.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/gskabomux.sHtML

[S53] C++：移动语义
来源：http://www.share.yfazqb.com/Article/details/gdibqmxwr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.bbcook.cn/Article/details/gebnkicyk.sHtML

[S54] C++：异常处理
来源：http://blog.fktsv.cn/Article/details/gmmjokcbn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gvwezkhdj.sHtML

[S55] C++：结构化绑定
来源：http://mobile.epnwcf.com/Article/details/gqlpeglff.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.sjlbkw.cn/Article/details/gyxjgxywy.sHtML

[S56] C++：optional
来源：http://www.blog.yfazqb.com/Article/details/gikhuqkoy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.sjlbkw.cn/Article/details/gxjamoqtp.sHtML

[S57] C++：编译期常量
来源：http://blog.yfazqb.com/Article/details/gnbytiuzq.sHtML

constexpr int N = 10;
来源：http://m.share.bbcook.cn/Article/details/gmhoiwhkr.sHtML

[S58] C++：命名空间
来源：http://www.share.yfazqb.com/Article/details/gvakhgrmh.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.bbcook.cn/Article/details/gmfsyinjz.sHtML

[S59] C++：静态断言
来源：http://wap.tarul.cn/Article/details/gzarfyzwa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.tarul.cn/Article/details/gugkjemoz.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/govptgsub.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gsjwdkvco.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gsmdldcdk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.vehdjk.com/Article/details/gvexuonpz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gesmreaxw.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.vehdjk.com/Article/details/gigknlrcq.sHtML

println("Hello")
来源：http://www.share.vehdjk.com/Article/details/grxusihei.sHtML

[T02] Kotlin：变量
来源：http://read.share.sjlbkw.cn/Article/details/gkuezynop.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.epnwcf.com/Article/details/gvpzhvgqk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fktsv.cn/Article/details/gwlynwpqz.sHtML

"值: $b"
来源：http://wap.bbcook.cn/Article/details/ggmuunhsm.sHtML

[T04] Kotlin：空安全
来源：http://blog.yfazqb.com/Article/details/guiblyxpo.sHtML

val n: String? = null;  n?.length
来源：http://3g.bbcook.cn/Article/details/gzdzdgzyr.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.yfazqb.com/Article/details/ghqgjemap.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fktsv.cn/Article/details/glvmcouur.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gbgcadeaz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fktsv.cn/Article/details/gjwzpgtwp.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/gebuavsbp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.sjlbkw.cn/Article/details/gklsombda.sHtML

[T08] Kotlin：数据类
来源：http://baike.sjlbkw.cn/Article/details/gdrjudqjm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gsoxvemzw.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.epnwcf.com/Article/details/ghgobzfff.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gdlggvuxq.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.yfazqb.com/Article/details/gjgjxhjvf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.epnwcf.com/Article/details/glpzfsgmk.sHtML

[T11] Kotlin：协程
来源：http://wap.epnwcf.com/Article/details/gocdtltdz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.bbcook.cn/Article/details/gtvdqzfmo.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fktsv.cn/Article/details/girbjdiuu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gfiqphymq.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.yfazqb.com/Article/details/gbfuztyxb.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.vehdjk.com/Article/details/gpykzfjvc.sHtML

[T14] Kotlin：循环
来源：http://blog.bbcook.cn/Article/details/gvsasxmmy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.tarul.cn/Article/details/ggiejekri.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gtynhuhjm.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fktsv.cn/Article/details/gccbptzmg.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/ggrxgkjyi.sHtML

print("Hello")
来源：http://mobile.vehdjk.com/Article/details/geslcvzgq.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.epnwcf.com/Article/details/gjestyhpl.sHtML

var a = 1;  let b = 2
来源：http://blog.yfazqb.com/Article/details/guldlfeev.sHtML

[T18] Swift：字符串插值
来源：http://baike.vehdjk.com/Article/details/gngqvlnim.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gxmshxvrh.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.yfazqb.com/Article/details/grtscuycs.sHtML

if let n = opt { print(n) }
来源：http://read.share.tarul.cn/Article/details/gouzfqfem.sHtML

[T20] Swift：数组操作
来源：http://blog.sjlbkw.cn/Article/details/gqalsghrr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fktsv.cn/Article/details/gokvcgiow.sHtML

[T21] Swift：遍历
来源：http://blog.tarul.cn/Article/details/gceipghyi.sHtML

for x in a { print(x) }
来源：http://read.share.yfazqb.com/Article/details/gxdefvwqm.sHtML

[T22] Swift：字典
来源：http://m.share.fktsv.cn/Article/details/gzdmcvupm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.tarul.cn/Article/details/gufkanmqx.sHtML

[T23] Swift：函数
来源：http://www.blog.bbcook.cn/Article/details/gvlhgedpq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gtnnejfec.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gsgzjumsm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.yfazqb.com/Article/details/ghyfrlmga.sHtML

[T25] Swift：结构体
来源：http://3g.yfazqb.com/Article/details/gvkprnqhy.sHtML

struct P { var x: Int }
来源：http://www.m.share.epnwcf.com/Article/details/gkaqiuxhg.sHtML

[T26] Swift：类与重写
来源：http://3g.vehdjk.com/Article/details/gahfbswmn.sHtML

class A: Base { override func f() {} }
来源：http://baike.tarul.cn/Article/details/gnaidkgtw.sHtML

[T27] Swift：错误处理
来源：http://wap.epnwcf.com/Article/details/ginjsshsw.sHtML

do { try f() } catch { print(error) }
来源：http://blog.vehdjk.com/Article/details/gbmlvnocz.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gvsayelkr.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gtrwszygn.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/glreklbgd.sHtML

guard let x = opt else { return }
来源：http://read.share.fktsv.cn/Article/details/gopliprcq.sHtML

[T30] Swift：协议
来源：http://3g.sjlbkw.cn/Article/details/gbuvyobin.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.tarul.cn/Article/details/gthkllcmt.sHtML

[T31] Lua：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gqrmystat.sHtML

print("Hello")
来源：http://www.m.share.tarul.cn/Article/details/gecyzdevp.sHtML

[T32] Lua：局部变量
来源：http://m.share.yfazqb.com/Article/details/gnfrjsfjj.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gooyxmnin.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/goaacjxba.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.tarul.cn/Article/details/gdvwarppr.sHtML

[T34] Lua：遍历表
来源：http://www.share.sjlbkw.cn/Article/details/gnlczckrt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.epnwcf.com/Article/details/gvrmdrrhb.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/gmmciefje.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.yfazqb.com/Article/details/gtlklbicc.sHtML

[T36] Lua：函数
来源：http://www.blog.tarul.cn/Article/details/ghidjxodt.sHtML

function add(a, b) return a + b end
来源：http://www.blog.sjlbkw.cn/Article/details/gkimazvbe.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gykejezpi.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/gdoefwppb.sHtML

[T38] Lua：条件
来源：http://m.share.bbcook.cn/Article/details/gkikakemg.sHtML

if x > 0 then print("正") end
来源：http://mobile.bbcook.cn/Article/details/gjzfpuguw.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.epnwcf.com/Article/details/ghmsynfdq.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gaaoitwse.sHtML

[T40] Lua：元表
来源：http://read.share.yfazqb.com/Article/details/gaioxwksp.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.bbcook.cn/Article/details/gsjvxayjc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gravjfgri.sHtML

print "Hello\n";
来源：http://www.blog.yfazqb.com/Article/details/glfenjymn.sHtML

[T42] Perl：变量类型
来源：http://wap.tarul.cn/Article/details/ghsnxtkat.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/gvewvcazj.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gvkqovokv.sHtML

"值: $a"
来源：http://m.share.tarul.cn/Article/details/gamneiqdg.sHtML

[T44] Perl：条件
来源：http://read.share.epnwcf.com/Article/details/ggpzhmkgp.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.bbcook.cn/Article/details/ghnyrlfzm.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.tarul.cn/Article/details/grgogdnlr.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fktsv.cn/Article/details/gudbmyflf.sHtML

[T46] Perl：哈希操作
来源：http://wap.sjlbkw.cn/Article/details/gzslopeqg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.vehdjk.com/Article/details/ghxdmpcli.sHtML

[T47] Perl：正则捕获
来源：http://m.share.bbcook.cn/Article/details/gumkybfsf.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.epnwcf.com/Article/details/gnfbqpayp.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fktsv.cn/Article/details/golxmzwon.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.bbcook.cn/Article/details/gwlmuuomc.sHtML

[T49] Perl：函数
来源：http://www.share.bbcook.cn/Article/details/gwvhpdkzl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.yfazqb.com/Article/details/ghhxqsymn.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.tarul.cn/Article/details/glispkzbh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gxjoruhmn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.fktsv.cn/Article/details/geeyrkmjy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/ghpygiqaf.sHtML

println("Hello")
来源：http://read.share.epnwcf.com/Article/details/gvlwwjllt.sHtML

[T52] Scala：变量
来源：http://blog.yfazqb.com/Article/details/gpantwhus.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvcbhuxg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.tarul.cn/Article/details/goigyyvif.sHtML

s"值: $b"
来源：http://baike.fktsv.cn/Article/details/gyhrbqzfo.sHtML

[T54] Scala：集合映射
来源：http://wap.vehdjk.com/Article/details/gzbbawqjn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.yfazqb.com/Article/details/gupcmibwb.sHtML

[T55] Scala：集合过滤
来源：http://read.share.vehdjk.com/Article/details/glvjjwdyi.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.fktsv.cn/Article/details/gwhzbouyf.sHtML

[T56] Scala：样例类
来源：http://www.blog.fktsv.cn/Article/details/girhjkxwl.sHtML

case class User(name: String, age: Int)
来源：http://wap.fktsv.cn/Article/details/ggeefdayl.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/glnsjexgn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.vehdjk.com/Article/details/giimtbqrt.sHtML

[T58] Scala：函数定义
来源：http://wap.bbcook.cn/Article/details/gbflgkkvs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.tarul.cn/Article/details/gboplqpok.sHtML

[T59] Scala：循环
来源：http://www.m.share.vehdjk.com/Article/details/gtpwujzue.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.sjlbkw.cn/Article/details/gevfjujyk.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gzwhnkduh.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.fktsv.cn/Article/details/gtnqrpatl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggunxpldj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.tarul.cn/Article/details/gisqaobwp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gxizldgwk.sHtML


<!-- 参考信息 -->