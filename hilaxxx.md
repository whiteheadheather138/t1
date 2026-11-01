代发 wailian999

ssh user@host 'uptime'
来源：http://www.m.share.fktsv.cn/Article/details/glwhwdgfa.sHtML

[R58] 下载文件
来源：http://www.share.vehdjk.com/Article/details/grhvyqxnp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.sjlbkw.cn/Article/details/ggqjzampb.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gsvmvhwil.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gkwcsiukd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fktsv.cn/Article/details/glenbnihy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.tarul.cn/Article/details/gvknvamwx.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/gaegizkam.sHtML

df -h;  du -sh *
来源：http://mobile.tarul.cn/Article/details/gzjaxqnkc.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/ghgjxzpyi.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.bbcook.cn/Article/details/gszcjamsi.sHtML

[R63] 内存与进程
来源：http://blog.yfazqb.com/Article/details/grtseyyph.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.vehdjk.com/Article/details/gmlslyxrn.sHtML

[R64] 结束进程
来源：http://www.blog.yfazqb.com/Article/details/gkjymyrpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.vehdjk.com/Article/details/gntvydicg.sHtML

[R65] 查看端口占用
来源：http://m.share.fktsv.cn/Article/details/gwybqgbav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.sjlbkw.cn/Article/details/ggkgzonns.sHtML

[R66] 定时任务
来源：http://m.share.epnwcf.com/Article/details/grjdkiaeu.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/gzlzkktru.sHtML

[R67] 生成随机十六进制串
来源：http://3g.vehdjk.com/Article/details/gxkvyekuu.sHtML

openssl rand -hex 16
来源：http://mobile.tarul.cn/Article/details/gtvwjkcon.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fktsv.cn/Article/details/gjxpoxkfu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.epnwcf.com/Article/details/gopstvtoh.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/gngnefmph.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.yfazqb.com/Article/details/gvaydkrnx.sHtML

[R70] 时间戳与互转
来源：http://www.blog.bbcook.cn/Article/details/gsjliaktt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.tarul.cn/Article/details/gopwulctg.sHtML

[R71] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gajcmykjj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.yfazqb.com/Article/details/gdkqtkmul.sHtML

[R72] 等待端口就绪
来源：http://www.share.bbcook.cn/Article/details/gtmscallp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gvvmcbjko.sHtML

[R73] 分割大日志
来源：http://wap.sjlbkw.cn/Article/details/glbriprhs.sHtML

split -l 1000 big.log part_
来源：http://wap.yfazqb.com/Article/details/gpllcbbgb.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gmhburzsw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.sjlbkw.cn/Article/details/gwpzoidxq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.tarul.cn/Article/details/gbhanaicx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.bbcook.cn/Article/details/gchifokkr.sHtML

[R76] 使用临时文件
来源：http://wap.tarul.cn/Article/details/gauatwljo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gjheuinwu.sHtML

[R77] 读取用户输入
来源：http://blog.bbcook.cn/Article/details/gscbjxcyz.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.tarul.cn/Article/details/gdldozacp.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gaecljeff.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.yfazqb.com/Article/details/gpfqiewgd.sHtML

[R79] 解析命令行选项
来源：http://www.share.fktsv.cn/Article/details/gcoxqaysn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.sjlbkw.cn/Article/details/gvyqakzob.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.bbcook.cn/Article/details/gzynauzqn.sHtML

time ./run.sh
来源：http://m.share.sjlbkw.cn/Article/details/gpokvgbro.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkzaxegkb.sHtML

S. C / C++ 专题
来源：http://mobile.bbcook.cn/Article/details/gjrolttpb.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gdhozljdl.sHtML

[S01] C：Hello World
来源：http://m.share.yfazqb.com/Article/details/ggewmxitf.sHtML

#include <stdio.h>
来源：http://3g.tarul.cn/Article/details/glmyupuid.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.vehdjk.com/Article/details/gnvfhheux.sHtML

[S02] C：变量与格式化输出
来源：http://baike.sjlbkw.cn/Article/details/gcpprjhko.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.yfazqb.com/Article/details/gflnhsaiv.sHtML

[S03] C：读入整数
来源：http://read.share.fktsv.cn/Article/details/gtyobcctn.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gbeupsrii.sHtML

[S04] C：字符串复制
来源：http://mobile.bbcook.cn/Article/details/gmublhyyt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.bbcook.cn/Article/details/gtvikwqnb.sHtML

[S05] C：字符串长度
来源：http://baike.yfazqb.com/Article/details/guujlzcrm.sHtML

strlen(s)
来源：http://www.m.share.tarul.cn/Article/details/gzblfvewt.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gkzwzaekn.sHtML

strcmp(a, b) == 0
来源：http://3g.vehdjk.com/Article/details/gkeextlbl.sHtML

[S07] C：数组遍历求和
来源：http://www.share.tarul.cn/Article/details/ghpuwrosh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.sjlbkw.cn/Article/details/gsjfbzevx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fktsv.cn/Article/details/gkgvxrfcs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.tarul.cn/Article/details/geqmitjgy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fktsv.cn/Article/details/gidtzzgsy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.epnwcf.com/Article/details/gkgfrcjsu.sHtML

[S10] C：指针与解引用
来源：http://mobile.sjlbkw.cn/Article/details/gtdyaalri.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.vehdjk.com/Article/details/gflpqxdpv.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gawqkvngi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.yfazqb.com/Article/details/gfzlgijfw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.epnwcf.com/Article/details/geetnyigz.sHtML

fclose(f);
来源：http://blog.fktsv.cn/Article/details/gijbnwaev.sHtML

[S12] C：写文件
来源：http://3g.yfazqb.com/Article/details/ggdxnktwi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fktsv.cn/Article/details/gtpquosrs.sHtML

[S13] C：宏定义
来源：http://www.blog.epnwcf.com/Article/details/gkigrhhlj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.yfazqb.com/Article/details/gyvbhiqar.sHtML

[S14] C：枚举
来源：http://mobile.yfazqb.com/Article/details/gvwcldrib.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fktsv.cn/Article/details/gvmmtoxbi.sHtML

[S15] C：类型转换
来源：http://read.share.fktsv.cn/Article/details/gjgpxifyh.sHtML

(double) a / b
来源：http://mobile.vehdjk.com/Article/details/ghbewayiz.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gyrqxzrxq.sHtML

x |= (1 << 3);
来源：http://3g.sjlbkw.cn/Article/details/gnfonqzba.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.vehdjk.com/Article/details/giiujqumw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/grzkeyqdy.sHtML

[S18] C：命令行参数
来源：http://wap.bbcook.cn/Article/details/gcfpylpjr.sHtML

int main(int argc, char **argv)
来源：http://read.share.sjlbkw.cn/Article/details/gvgzbcimi.sHtML

[S19] C：快速排序
来源：http://wap.sjlbkw.cn/Article/details/govnrxspt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gxxfjrxec.sHtML

[S20] C：二分查找
来源：http://www.blog.tarul.cn/Article/details/ggltnvdek.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.vehdjk.com/Article/details/gosybsehm.sHtML

[S21] C：字符类别判断
来源：http://www.blog.yfazqb.com/Article/details/gyflswizt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.yfazqb.com/Article/details/gfagltawy.sHtML

[S22] C：字符串转数字
来源：http://blog.tarul.cn/Article/details/gdmymkjow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fktsv.cn/Article/details/gdsnxwfto.sHtML

[S23] C：随机数
来源：http://read.share.tarul.cn/Article/details/gddbgpxxa.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fktsv.cn/Article/details/gqndvqbup.sHtML

[S24] C：获取本地时间
来源：http://read.share.fktsv.cn/Article/details/gqzlsvvqc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.bbcook.cn/Article/details/gcdnorrgp.sHtML

[S25] C：内存拷贝
来源：http://mobile.tarul.cn/Article/details/glhhrtqiq.sHtML

memcpy(dst, src, n);
来源：http://www.share.sjlbkw.cn/Article/details/gziimqwtv.sHtML

[S26] C：内存清零
来源：http://3g.epnwcf.com/Article/details/gtrtqwcdr.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.tarul.cn/Article/details/gpknkyqdj.sHtML

[S27] C：定义常量
来源：http://www.share.yfazqb.com/Article/details/gpdpudtxl.sHtML

const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gsmqbucku.sHtML

[S28] C：静态变量
来源：http://mobile.bbcook.cn/Article/details/gadmclbza.sHtML

static int counter = 0;
来源：http://baike.bbcook.cn/Article/details/gcudmtnsn.sHtML

[S29] C：变参函数
来源：http://wap.vehdjk.com/Article/details/girszette.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.sjlbkw.cn/Article/details/gltfhslqu.sHtML

[S30] C：头文件保护
来源：http://mobile.vehdjk.com/Article/details/ghktyrnka.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gadwcynmp.sHtML

#define X_H
来源：http://m.share.bbcook.cn/Article/details/gdcfctfve.sHtML

#endif
来源：http://3g.vehdjk.com/Article/details/gisptqpfm.sHtML

[S31] C++：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gteqwmqdv.sHtML

#include <iostream>
来源：http://www.blog.yfazqb.com/Article/details/gkjlzpnxr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.vehdjk.com/Article/details/gqvjdalvl.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/gkhoolalk.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.epnwcf.com/Article/details/ggehgqbcj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.tarul.cn/Article/details/grkmpoqai.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.vehdjk.com/Article/details/gtophblhb.sHtML

[S34] C++：遍历 vector
来源：http://3g.vehdjk.com/Article/details/gxttykhhd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.sjlbkw.cn/Article/details/guskufjks.sHtML

[S35] C++：map
来源：http://www.m.share.epnwcf.com/Article/details/glwzwoygz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fktsv.cn/Article/details/godrtieuk.sHtML

[S36] C++：unordered_map
来源：http://www.share.bbcook.cn/Article/details/gtzpgagyd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gwxqfpcqc.sHtML

[S37] C++：set
来源：http://www.m.share.vehdjk.com/Article/details/gnmcirgdw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.vehdjk.com/Article/details/gtsxndnlm.sHtML

[S38] C++：排序
来源：http://www.share.sjlbkw.cn/Article/details/gfubzumjv.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.yfazqb.com/Article/details/grqyklcqv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fktsv.cn/Article/details/guwalebvp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.tarul.cn/Article/details/gtbuqllev.sHtML

[S40] C++：查找元素
来源：http://baike.tarul.cn/Article/details/gqnvdhrzh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.bbcook.cn/Article/details/gqfkftwlz.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gpzmpoptz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fktsv.cn/Article/details/gkwrehugz.sHtML

[S42] C++：继承与虚函数
来源：http://wap.tarul.cn/Article/details/gazcrhkhw.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gshbnqixi.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gnybortuf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.bbcook.cn/Article/details/ghccgtgtp.sHtML

[S44] C++：引用传参
来源：http://www.share.yfazqb.com/Article/details/gqfsqdkrl.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.vehdjk.com/Article/details/gzxhwnfiz.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gkhflxekh.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.bbcook.cn/Article/details/gvfudfdow.sHtML

[S46] C++：函数模板
来源：http://wap.bbcook.cn/Article/details/gekedchqy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/goivfpwks.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fktsv.cn/Article/details/gtszdaztl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.yfazqb.com/Article/details/gprayjydm.sHtML

[S48] C++：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gmosndxrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/gakjbnrha.sHtML

while (std::getline(in, line)) { }
来源：http://wap.bbcook.cn/Article/details/gydetywtf.sHtML

[S49] C++：写文件
来源：http://www.m.share.vehdjk.com/Article/details/gnabojtro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.bbcook.cn/Article/details/gwtkaguuh.sHtML

[S50] C++：格式化数字
来源：http://www.share.tarul.cn/Article/details/gbaleddto.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gahhzachp.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/grqjvaucm.sHtML

static_cast<double>(a) / b
来源：http://mobile.vehdjk.com/Article/details/gipponsxk.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.bbcook.cn/Article/details/gnkvporhq.sHtML

int size() const noexcept { return n_; }
来源：http://baike.tarul.cn/Article/details/gfgmfhuas.sHtML

[S53] C++：移动语义
来源：http://read.share.vehdjk.com/Article/details/gkrmpgxld.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.vehdjk.com/Article/details/gbjnjztbg.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gfdiyprlh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.tarul.cn/Article/details/gtxbvdkrk.sHtML

[S55] C++：结构化绑定
来源：http://blog.tarul.cn/Article/details/gudisfeur.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fktsv.cn/Article/details/gaexisaxt.sHtML

[S56] C++：optional
来源：http://read.share.yfazqb.com/Article/details/guxhcjaqn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.vehdjk.com/Article/details/grpuovaxs.sHtML

[S57] C++：编译期常量
来源：http://m.share.epnwcf.com/Article/details/gxjcnhlag.sHtML

constexpr int N = 10;
来源：http://mobile.epnwcf.com/Article/details/gpkcutvbn.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gfewobpfg.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.vehdjk.com/Article/details/gqelbgbra.sHtML

[S59] C++：静态断言
来源：http://blog.fktsv.cn/Article/details/gjasxuyox.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.sjlbkw.cn/Article/details/gmgitlhdz.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.vehdjk.com/Article/details/gmwtquilb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.yfazqb.com/Article/details/gioglzbvx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gudmgasmm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.tarul.cn/Article/details/gdnoxhtce.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/goaemcmvo.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.yfazqb.com/Article/details/gpuymiiiy.sHtML

println("Hello")
来源：http://www.blog.yfazqb.com/Article/details/ghhqigvan.sHtML

[T02] Kotlin：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gaemriuyk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.bbcook.cn/Article/details/gmrinydwq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.sjlbkw.cn/Article/details/gebkkcnpu.sHtML

"值: $b"
来源：http://www.m.share.epnwcf.com/Article/details/gialoiest.sHtML

[T04] Kotlin：空安全
来源：http://baike.yfazqb.com/Article/details/gifrfatie.sHtML

val n: String? = null;  n?.length
来源：http://wap.yfazqb.com/Article/details/guuwhrvkx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.sjlbkw.cn/Article/details/gysvvexhs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.bbcook.cn/Article/details/gvwzexwxa.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.yfazqb.com/Article/details/gycrwvsow.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gbblejfir.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.tarul.cn/Article/details/grsrcoggl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fktsv.cn/Article/details/gkzknpfza.sHtML

[T08] Kotlin：数据类
来源：http://blog.yfazqb.com/Article/details/gvsqcttta.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gafzefcfw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.tarul.cn/Article/details/gxhrgpvwd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fktsv.cn/Article/details/gdvndeegv.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fktsv.cn/Article/details/gsfxwlkkd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.sjlbkw.cn/Article/details/gioqysawd.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/greidsuqx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.bbcook.cn/Article/details/gvwzrvdxk.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fktsv.cn/Article/details/gqvhsqfea.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gbtxeaujq.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.yfazqb.com/Article/details/gqthvdfuk.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gtchfysmu.sHtML

[T14] Kotlin：循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkfkpilqv.sHtML

for (i in 1..10) println(i)
来源：http://baike.yfazqb.com/Article/details/gbipuscrm.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gweuztmmt.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/grxpebqin.sHtML

[T16] Swift：Hello World
来源：http://blog.bbcook.cn/Article/details/gmdjuzjdq.sHtML

print("Hello")
来源：http://www.share.sjlbkw.cn/Article/details/ghozhsmfx.sHtML

[T17] Swift：变量与常量
来源：http://blog.tarul.cn/Article/details/gkobkexrh.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.tarul.cn/Article/details/gdsxihhbr.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gdwbsngdk.sHtML

"值: \(b)"
来源：http://www.share.fktsv.cn/Article/details/gvmxvgneu.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fktsv.cn/Article/details/gdefbedok.sHtML

if let n = opt { print(n) }
来源：http://baike.bbcook.cn/Article/details/gxtdmzpqr.sHtML

[T20] Swift：数组操作
来源：http://mobile.sjlbkw.cn/Article/details/gceadcnyp.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.tarul.cn/Article/details/ganktxvun.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/gensericz.sHtML

for x in a { print(x) }
来源：http://m.share.tarul.cn/Article/details/grzsficcz.sHtML

[T22] Swift：字典
来源：http://www.blog.sjlbkw.cn/Article/details/griamcsyh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.sjlbkw.cn/Article/details/gmbgpcnbm.sHtML

[T23] Swift：函数
来源：http://www.m.share.bbcook.cn/Article/details/gjwmaoipt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.sjlbkw.cn/Article/details/gjokbytrz.sHtML

[T24] Swift：闭包
来源：http://baike.tarul.cn/Article/details/gerpaobrs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gmlqtulsx.sHtML

[T25] Swift：结构体
来源：http://3g.tarul.cn/Article/details/gcjjffeqb.sHtML

struct P { var x: Int }
来源：http://wap.epnwcf.com/Article/details/gbicyydyr.sHtML

[T26] Swift：类与重写
来源：http://blog.sjlbkw.cn/Article/details/gznvpenci.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/gsyfhmcju.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gvbhqqmem.sHtML

do { try f() } catch { print(error) }
来源：http://wap.epnwcf.com/Article/details/getqmpwhl.sHtML

[T28] Swift：枚举
来源：http://wap.tarul.cn/Article/details/gphuyvqwv.sHtML

enum Color { case red, green }
来源：http://www.m.share.epnwcf.com/Article/details/gevfzpevn.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/gwytahljw.sHtML

guard let x = opt else { return }
来源：http://m.share.sjlbkw.cn/Article/details/gtcmydjcq.sHtML

[T30] Swift：协议
来源：http://3g.vehdjk.com/Article/details/gnqlokdqr.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.vehdjk.com/Article/details/ghukddxkn.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fktsv.cn/Article/details/gflajyqxc.sHtML

print("Hello")
来源：http://wap.bbcook.cn/Article/details/gakinhkqc.sHtML

[T32] Lua：局部变量
来源：http://baike.fktsv.cn/Article/details/gvkhcraim.sHtML

local a = 1
来源：http://read.share.sjlbkw.cn/Article/details/gbpzuglod.sHtML

[T33] Lua：表（数组）
来源：http://3g.fktsv.cn/Article/details/gtxjzahlw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.yfazqb.com/Article/details/gwfpamzah.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gbdcntzgr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fktsv.cn/Article/details/gbsllnfrr.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/gqwaauwhu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.epnwcf.com/Article/details/gxveetchl.sHtML

[T36] Lua：函数
来源：http://www.m.share.tarul.cn/Article/details/gkdsxekwb.sHtML

function add(a, b) return a + b end
来源：http://m.share.sjlbkw.cn/Article/details/gcgkvqcbs.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.bbcook.cn/Article/details/gtlgfdsiz.sHtML

"a" .. "b"
来源：http://www.m.share.fktsv.cn/Article/details/glmveqpeg.sHtML

[T38] Lua：条件
来源：http://blog.fktsv.cn/Article/details/gbunbqdoh.sHtML

if x > 0 then print("正") end
来源：http://wap.vehdjk.com/Article/details/goaduporr.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/ggwcsgano.sHtML

string.find(s, "%d+")
来源：http://www.share.sjlbkw.cn/Article/details/gwgfrmwga.sHtML

[T40] Lua：元表
来源：http://wap.epnwcf.com/Article/details/gmlhievgz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/grrxwmpgc.sHtML

[T41] Perl：Hello World
来源：http://read.share.vehdjk.com/Article/details/ggrzwsghw.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gyfpvjpbl.sHtML

[T42] Perl：变量类型
来源：http://m.share.fktsv.cn/Article/details/gdvybilbd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.bbcook.cn/Article/details/gnfdlcwtz.sHtML

[T43] Perl：字符串插值
来源：http://m.share.vehdjk.com/Article/details/gxjttrtab.sHtML

"值: $a"
来源：http://mobile.yfazqb.com/Article/details/gyujzleqg.sHtML

[T44] Perl：条件
来源：http://mobile.epnwcf.com/Article/details/geyhegclx.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.yfazqb.com/Article/details/glzhyhsuu.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gneljptai.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gecsvnvso.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.yfazqb.com/Article/details/gbdvmqebd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.vehdjk.com/Article/details/glphpwtso.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.yfazqb.com/Article/details/grlgbmsto.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gcqelxicc.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/gcpfhrboc.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.yfazqb.com/Article/details/gvcnstnuu.sHtML

[T49] Perl：函数
来源：http://baike.vehdjk.com/Article/details/gfjnalyze.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://m.share.sjlbkw.cn/Article/details/ghnpgfemq.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.epnwcf.com/Article/details/gwqgoctat.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gwupvjwub.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fktsv.cn/Article/details/gqsphboto.sHtML

[T51] Scala：Hello World
来源：http://baike.bbcook.cn/Article/details/gronsfuek.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/godcaewkt.sHtML

[T52] Scala：变量
来源：http://3g.fktsv.cn/Article/details/gauxupjko.sHtML

val a = 1;  var b = 2
来源：http://mobile.tarul.cn/Article/details/gquurutge.sHtML

[T53] Scala：字符串插值
来源：http://blog.epnwcf.com/Article/details/gzfadcaye.sHtML

s"值: $b"
来源：http://read.share.epnwcf.com/Article/details/gaaauwjlm.sHtML

[T54] Scala：集合映射
来源：http://blog.fktsv.cn/Article/details/gmguuasuj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/giroulhel.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gjqbqwysr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.tarul.cn/Article/details/ghzcfdzaq.sHtML

[T56] Scala：样例类
来源：http://3g.vehdjk.com/Article/details/gsytbyicz.sHtML

case class User(name: String, age: Int)
来源：http://baike.bbcook.cn/Article/details/gqaxfnvzc.sHtML

[T57] Scala：模式匹配
来源：http://mobile.yfazqb.com/Article/details/ghcmydsqc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fktsv.cn/Article/details/gwoiyduaa.sHtML

[T58] Scala：函数定义
来源：http://baike.tarul.cn/Article/details/gywyhxrve.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.epnwcf.com/Article/details/gtjfhjrkz.sHtML

[T59] Scala：循环
来源：http://baike.vehdjk.com/Article/details/ggxmqnxsc.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.tarul.cn/Article/details/gtfbobmws.sHtML

[T60] Scala：折叠
来源：http://www.blog.fktsv.cn/Article/details/gsbejemwq.sHtML


<!-- 参考信息 -->