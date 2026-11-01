代发 wailian999

df -h;  du -sh *
来源：http://mobile.vehdjk.com/Article/details/gmmpxjjrr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.sjlbkw.cn/Article/details/gujipiler.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/giehykegn.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gvuhsgtpo.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.bbcook.cn/Article/details/gylaadvpf.sHtML

[R64] 结束进程
来源：http://baike.bbcook.cn/Article/details/gmjheugyp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.tarul.cn/Article/details/gtowlimwa.sHtML

[R65] 查看端口占用
来源：http://wap.epnwcf.com/Article/details/gftzuwuld.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.sjlbkw.cn/Article/details/gykkaykzv.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gsiufbjis.sHtML

crontab -e;  crontab -l
来源：http://m.share.vehdjk.com/Article/details/gmgybpyvs.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gammvbccn.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/gwgwnfozg.sHtML

[R68] 计算文件校验值
来源：http://m.share.yfazqb.com/Article/details/gebfgyyeb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.vehdjk.com/Article/details/gudmiyuds.sHtML

[R69] 生成随机密码
来源：http://baike.tarul.cn/Article/details/guxdewkpp.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.epnwcf.com/Article/details/gpukdpokf.sHtML

[R70] 时间戳与互转
来源：http://mobile.sjlbkw.cn/Article/details/gxiesloqt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gsbnzmmfo.sHtML

[R71] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gkfwdkopk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.yfazqb.com/Article/details/geaoczsfy.sHtML

[R72] 等待端口就绪
来源：http://read.share.vehdjk.com/Article/details/gmbtckwxi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/glodfqlxt.sHtML

[R73] 分割大日志
来源：http://baike.tarul.cn/Article/details/gozryibxm.sHtML

split -l 1000 big.log part_
来源：http://mobile.fktsv.cn/Article/details/ggufwincs.sHtML

[R74] 批量重命名
来源：http://baike.bbcook.cn/Article/details/gazrmkmqg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.sjlbkw.cn/Article/details/grnkdcosl.sHtML

[R75] 导出环境变量
来源：http://3g.yfazqb.com/Article/details/ggqdumpoa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuecrimk.sHtML

[R76] 使用临时文件
来源：http://www.blog.bbcook.cn/Article/details/gllfwvvrh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.vehdjk.com/Article/details/gsegxfmlo.sHtML

[R77] 读取用户输入
来源：http://mobile.vehdjk.com/Article/details/gufmkxhba.sHtML

read -rp "请输入: " ans
来源：http://read.share.epnwcf.com/Article/details/gaoapfsec.sHtML

[R78] 交互式菜单
来源：http://www.blog.bbcook.cn/Article/details/gsjbzwmle.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gakzzuoeb.sHtML

[R79] 解析命令行选项
来源：http://wap.tarul.cn/Article/details/goheinpja.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.sjlbkw.cn/Article/details/gwltpnhfq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.yfazqb.com/Article/details/gbujydpei.sHtML

time ./run.sh
来源：http://baike.epnwcf.com/Article/details/gsoyrthlg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gynqfznik.sHtML

S. C / C++ 专题
来源：http://www.share.fktsv.cn/Article/details/gdihxtxza.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glkilxisy.sHtML

[S01] C：Hello World
来源：http://3g.epnwcf.com/Article/details/gmfsistee.sHtML

#include <stdio.h>
来源：http://www.m.share.epnwcf.com/Article/details/gmtmlxfoa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.epnwcf.com/Article/details/gyrywsjof.sHtML

[S02] C：变量与格式化输出
来源：http://wap.tarul.cn/Article/details/gutyqoutu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.bbcook.cn/Article/details/grdpvajao.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gkusobnet.sHtML

int x; scanf("%d", &x);
来源：http://m.share.yfazqb.com/Article/details/gepyxljyz.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gzthgzinx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gquotgbym.sHtML

[S05] C：字符串长度
来源：http://m.share.fktsv.cn/Article/details/gtxyodgqc.sHtML

strlen(s)
来源：http://wap.epnwcf.com/Article/details/gdklzxhck.sHtML

[S06] C：字符串比较
来源：http://m.share.epnwcf.com/Article/details/gviecjeez.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxfkuuxu.sHtML

[S07] C：数组遍历求和
来源：http://baike.epnwcf.com/Article/details/guiqbkzdz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.yfazqb.com/Article/details/goiaiikek.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.vehdjk.com/Article/details/gbyhonaqq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fktsv.cn/Article/details/gqiukgucq.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fktsv.cn/Article/details/gsryohbiq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.vehdjk.com/Article/details/gxmozbheq.sHtML

[S10] C：指针与解引用
来源：http://m.share.fktsv.cn/Article/details/gftzxtjho.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fktsv.cn/Article/details/gvmslpjvj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gzthtxqaj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.bbcook.cn/Article/details/gzswaimih.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/gnykhixma.sHtML

fclose(f);
来源：http://www.share.tarul.cn/Article/details/gexaineae.sHtML

[S12] C：写文件
来源：http://m.share.yfazqb.com/Article/details/gejazihop.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/garpokkav.sHtML

[S13] C：宏定义
来源：http://blog.bbcook.cn/Article/details/glngmkugw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.tarul.cn/Article/details/gxfvltzrl.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/gdziewsdb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.vehdjk.com/Article/details/gxmuhirqn.sHtML

[S15] C：类型转换
来源：http://mobile.sjlbkw.cn/Article/details/gtqjjubbx.sHtML

(double) a / b
来源：http://read.share.yfazqb.com/Article/details/gpfwctldx.sHtML

[S16] C：位操作置位
来源：http://mobile.fktsv.cn/Article/details/gqszpokab.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gsmlpihes.sHtML

[S17] C：安全拼接字符串
来源：http://3g.bbcook.cn/Article/details/gjdldzdyk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gfsdlyrmm.sHtML

[S18] C：命令行参数
来源：http://3g.sjlbkw.cn/Article/details/glzegozcg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.yfazqb.com/Article/details/gvjflonks.sHtML

[S19] C：快速排序
来源：http://www.share.tarul.cn/Article/details/gqkbqkatm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.yfazqb.com/Article/details/gdefstvuh.sHtML

[S20] C：二分查找
来源：http://m.share.yfazqb.com/Article/details/gsxelhvpa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gdkrejvor.sHtML

[S21] C：字符类别判断
来源：http://wap.sjlbkw.cn/Article/details/gcigdwtsp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.epnwcf.com/Article/details/gbzzsulwu.sHtML

[S22] C：字符串转数字
来源：http://www.share.yfazqb.com/Article/details/ggaoknudw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.epnwcf.com/Article/details/gswyxqluh.sHtML

[S23] C：随机数
来源：http://www.share.yfazqb.com/Article/details/goscgzinb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.vehdjk.com/Article/details/gomtdrruc.sHtML

[S24] C：获取本地时间
来源：http://mobile.yfazqb.com/Article/details/gnzkvorez.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.vehdjk.com/Article/details/gudhqnnxv.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gkquvgahr.sHtML

memcpy(dst, src, n);
来源：http://read.share.tarul.cn/Article/details/grygpexgw.sHtML

[S26] C：内存清零
来源：http://blog.sjlbkw.cn/Article/details/gthlzhdfu.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fktsv.cn/Article/details/gagdadbnt.sHtML

[S27] C：定义常量
来源：http://www.blog.vehdjk.com/Article/details/gipbfymnq.sHtML

const double PI = 3.14159;
来源：http://read.share.vehdjk.com/Article/details/grgricjxc.sHtML

[S28] C：静态变量
来源：http://www.share.yfazqb.com/Article/details/gnwwmykfr.sHtML

static int counter = 0;
来源：http://www.m.share.bbcook.cn/Article/details/gbuotjhsr.sHtML

[S29] C：变参函数
来源：http://baike.vehdjk.com/Article/details/gexyeduhs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.epnwcf.com/Article/details/gcdgbpusv.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/gnjsseryr.sHtML

#ifndef X_H
来源：http://wap.bbcook.cn/Article/details/gbhgjjcsh.sHtML

#define X_H
来源：http://3g.vehdjk.com/Article/details/gzcogwafe.sHtML

#endif
来源：http://blog.epnwcf.com/Article/details/ghpkaqppp.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gtycprdhi.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gmlzcrlmi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gxeklqlid.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gqsaxcbty.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.sjlbkw.cn/Article/details/gsmlklfqr.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpptwfmr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.bbcook.cn/Article/details/ghgkgmqwr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fktsv.cn/Article/details/golurtykf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gzvylfnlu.sHtML

[S35] C++：map
来源：http://wap.yfazqb.com/Article/details/gwxwdevds.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.yfazqb.com/Article/details/gbjijwbap.sHtML

[S36] C++：unordered_map
来源：http://mobile.fktsv.cn/Article/details/gnhzqbgtv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gdxsbjydz.sHtML

[S37] C++：set
来源：http://blog.vehdjk.com/Article/details/gkrgtthmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.yfazqb.com/Article/details/gyenzdquz.sHtML

[S38] C++：排序
来源：http://mobile.fktsv.cn/Article/details/gndlgxewb.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.tarul.cn/Article/details/gtysfwhph.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.yfazqb.com/Article/details/gzghinrlr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.epnwcf.com/Article/details/grwhghhmq.sHtML

[S40] C++：查找元素
来源：http://www.m.share.tarul.cn/Article/details/geneuiegy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.epnwcf.com/Article/details/glqbwrtef.sHtML

[S41] C++：类与构造函数
来源：http://3g.yfazqb.com/Article/details/gadpuwsni.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.epnwcf.com/Article/details/gkkavrnuz.sHtML

[S42] C++：继承与虚函数
来源：http://3g.yfazqb.com/Article/details/gvelysgmz.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.vehdjk.com/Article/details/gkptoczuo.sHtML

[S43] C++：智能指针
来源：http://wap.epnwcf.com/Article/details/gcjzfupyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.tarul.cn/Article/details/gbdfvvtqi.sHtML

[S44] C++：引用传参
来源：http://read.share.yfazqb.com/Article/details/grirrezip.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.vehdjk.com/Article/details/giabvjofx.sHtML

[S45] C++：lambda
来源：http://www.share.bbcook.cn/Article/details/gqruddhck.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.yfazqb.com/Article/details/ghugwbfrh.sHtML

[S46] C++：函数模板
来源：http://m.share.vehdjk.com/Article/details/gkshbbasu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.tarul.cn/Article/details/gagxgwway.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gdilwokxl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/gkzyripfn.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gsaywjeok.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.bbcook.cn/Article/details/gqystovdz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gryhyrluk.sHtML

[S49] C++：写文件
来源：http://m.share.vehdjk.com/Article/details/gnmyeezkv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/gxmtdufzx.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gotmdlkgj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.tarul.cn/Article/details/gdapmitgk.sHtML

[S51] C++：显式类型转换
来源：http://www.share.epnwcf.com/Article/details/gznedyvei.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gnvxpzrnn.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.epnwcf.com/Article/details/gfgylauyo.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.epnwcf.com/Article/details/gosndsfuj.sHtML

[S53] C++：移动语义
来源：http://mobile.sjlbkw.cn/Article/details/gfyobblho.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.tarul.cn/Article/details/glqpmtjuv.sHtML

[S54] C++：异常处理
来源：http://wap.yfazqb.com/Article/details/gqovfseto.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fktsv.cn/Article/details/gsvihnvjj.sHtML

[S55] C++：结构化绑定
来源：http://3g.yfazqb.com/Article/details/gwnmltaiy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.yfazqb.com/Article/details/gyavhruqb.sHtML

[S56] C++：optional
来源：http://www.share.fktsv.cn/Article/details/ggenfbijz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fktsv.cn/Article/details/gmveanelb.sHtML

[S57] C++：编译期常量
来源：http://read.share.epnwcf.com/Article/details/gaiyhyrdu.sHtML

constexpr int N = 10;
来源：http://read.share.bbcook.cn/Article/details/gqtarogrp.sHtML

[S58] C++：命名空间
来源：http://mobile.epnwcf.com/Article/details/gofuveelb.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.epnwcf.com/Article/details/gggkdopyn.sHtML

[S59] C++：静态断言
来源：http://read.share.bbcook.cn/Article/details/gydpogerg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.bbcook.cn/Article/details/gjmdoufvr.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.vehdjk.com/Article/details/ggszniefg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.epnwcf.com/Article/details/gnoaytxxk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggrihafdv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.epnwcf.com/Article/details/gkxpzqewc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzivqtyca.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.bbcook.cn/Article/details/gcpesootv.sHtML

println("Hello")
来源：http://blog.yfazqb.com/Article/details/gzyxzccdr.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gqhwlnfyl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.sjlbkw.cn/Article/details/gqobdngul.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.sjlbkw.cn/Article/details/gtwnxcsgp.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gyiuoowku.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.vehdjk.com/Article/details/gikxvytkq.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fktsv.cn/Article/details/gfnlbkmrw.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gttswosgf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.yfazqb.com/Article/details/gksdnkjgj.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.vehdjk.com/Article/details/gxfbwoxro.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.tarul.cn/Article/details/ghmfofsjk.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.yfazqb.com/Article/details/goefdxfxk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gwfkosoci.sHtML

[T08] Kotlin：数据类
来源：http://mobile.bbcook.cn/Article/details/ghwipgyip.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fktsv.cn/Article/details/gycyftmcv.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gsnbsqreg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gjyqrchmf.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.yfazqb.com/Article/details/gfwnttqce.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.vehdjk.com/Article/details/gicgnxelq.sHtML

[T11] Kotlin：协程
来源：http://baike.yfazqb.com/Article/details/ghstdcyfo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.epnwcf.com/Article/details/ghgfkytwf.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fktsv.cn/Article/details/gwxowigwv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.yfazqb.com/Article/details/gskqrstww.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gkcujlgvo.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fktsv.cn/Article/details/gtnfudymj.sHtML

[T14] Kotlin：循环
来源：http://read.share.yfazqb.com/Article/details/geunqdpji.sHtML

for (i in 1..10) println(i)
来源：http://blog.yfazqb.com/Article/details/gkybruehl.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gwumchwrp.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.epnwcf.com/Article/details/gakbhguvq.sHtML

[T16] Swift：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gxgepsimy.sHtML

print("Hello")
来源：http://www.blog.epnwcf.com/Article/details/gaazvdelm.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.tarul.cn/Article/details/gvbhojusz.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxvluczs.sHtML

[T18] Swift：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gcdvlrgow.sHtML

"值: \(b)"
来源：http://blog.vehdjk.com/Article/details/gccodnimc.sHtML

[T19] Swift：可选绑定
来源：http://read.share.epnwcf.com/Article/details/gbyxufiql.sHtML

if let n = opt { print(n) }
来源：http://read.share.fktsv.cn/Article/details/grvtjnzaa.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/gielghbpq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fktsv.cn/Article/details/gseoyppng.sHtML

[T21] Swift：遍历
来源：http://baike.tarul.cn/Article/details/gkjduwhzq.sHtML

for x in a { print(x) }
来源：http://blog.sjlbkw.cn/Article/details/gcvwwsbni.sHtML

[T22] Swift：字典
来源：http://m.share.yfazqb.com/Article/details/gzcwoaycd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fktsv.cn/Article/details/gcsjqoxpo.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/gsoqnikpa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.yfazqb.com/Article/details/gylfxmpbq.sHtML

[T24] Swift：闭包
来源：http://mobile.yfazqb.com/Article/details/gsdvyxpgs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gorqsomwt.sHtML

[T25] Swift：结构体
来源：http://read.share.vehdjk.com/Article/details/gncfzhrpl.sHtML

struct P { var x: Int }
来源：http://www.share.tarul.cn/Article/details/giabwpszi.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gawbelshf.sHtML

class A: Base { override func f() {} }
来源：http://blog.vehdjk.com/Article/details/garzacxos.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gurqtblaz.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.sjlbkw.cn/Article/details/gugxyuwyb.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gvguvgovf.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/gjxtqaqnw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fktsv.cn/Article/details/gyiupacyp.sHtML

guard let x = opt else { return }
来源：http://baike.bbcook.cn/Article/details/gfurcmibm.sHtML

[T30] Swift：协议
来源：http://m.share.vehdjk.com/Article/details/gfcxvrwln.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.epnwcf.com/Article/details/gzwcxnjjx.sHtML

[T31] Lua：Hello World
来源：http://baike.bbcook.cn/Article/details/guargxdvf.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gquwftfxc.sHtML

[T32] Lua：局部变量
来源：http://wap.sjlbkw.cn/Article/details/gjpwqnvju.sHtML

local a = 1
来源：http://3g.yfazqb.com/Article/details/guqdgtiek.sHtML

[T33] Lua：表（数组）
来源：http://mobile.vehdjk.com/Article/details/gnegsfikg.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.vehdjk.com/Article/details/gwinvdyvc.sHtML

[T34] Lua：遍历表
来源：http://3g.bbcook.cn/Article/details/gwhykyrqa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fktsv.cn/Article/details/gausibnct.sHtML

[T35] Lua：字典表
来源：http://www.m.share.bbcook.cn/Article/details/gjtkaonfq.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.yfazqb.com/Article/details/gaenfswky.sHtML

[T36] Lua：函数
来源：http://www.m.share.fktsv.cn/Article/details/gdsnyjbjl.sHtML

function add(a, b) return a + b end
来源：http://m.share.epnwcf.com/Article/details/gxrxgopkq.sHtML

[T37] Lua：字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gaqkmleyq.sHtML

"a" .. "b"
来源：http://baike.fktsv.cn/Article/details/gilzaaaqc.sHtML

[T38] Lua：条件
来源：http://blog.vehdjk.com/Article/details/gwkjbthfy.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gvlcqhcgc.sHtML

[T39] Lua：模式匹配
来源：http://read.share.epnwcf.com/Article/details/ggbmiqwwi.sHtML

string.find(s, "%d+")
来源：http://blog.fktsv.cn/Article/details/gewgslblt.sHtML

[T40] Lua：元表
来源：http://blog.bbcook.cn/Article/details/gwoofrpun.sHtML

setmetatable({}, { __index = base })
来源：http://3g.tarul.cn/Article/details/gqlvwqjqt.sHtML

[T41] Perl：Hello World
来源：http://3g.epnwcf.com/Article/details/gkazvonqb.sHtML

print "Hello\n";
来源：http://mobile.yfazqb.com/Article/details/gixwfscsk.sHtML

[T42] Perl：变量类型
来源：http://read.share.epnwcf.com/Article/details/gkuatdwgp.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.bbcook.cn/Article/details/gfuaekrzt.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.vehdjk.com/Article/details/gzcsuacdk.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gyyrszbhc.sHtML

[T44] Perl：条件
来源：http://m.share.bbcook.cn/Article/details/gzqiknzmq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fktsv.cn/Article/details/gplflczvs.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gfxpqryuh.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.sjlbkw.cn/Article/details/gqgfdifit.sHtML

[T46] Perl：哈希操作
来源：http://wap.yfazqb.com/Article/details/gyltkxwxl.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/gfzfyzfvs.sHtML

[T47] Perl：正则捕获
来源：http://baike.epnwcf.com/Article/details/gxvygrsan.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.tarul.cn/Article/details/gktbhbpiq.sHtML

[T48] Perl：正则替换
来源：http://www.blog.yfazqb.com/Article/details/gbfdapwzg.sHtML

$s =~ s/old/new/g;
来源：http://m.share.bbcook.cn/Article/details/gwxgvbiab.sHtML

[T49] Perl：函数
来源：http://mobile.tarul.cn/Article/details/gyaujzhqy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.fktsv.cn/Article/details/gqnawgvfo.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.sjlbkw.cn/Article/details/geqvidbvu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.bbcook.cn/Article/details/gpnmfzcls.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fktsv.cn/Article/details/gelcixiuj.sHtML

[T51] Scala：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gvlrtbbjk.sHtML

println("Hello")
来源：http://mobile.epnwcf.com/Article/details/gtttlebah.sHtML

[T52] Scala：变量
来源：http://3g.tarul.cn/Article/details/gylrvucfu.sHtML

val a = 1;  var b = 2
来源：http://www.blog.bbcook.cn/Article/details/gspoiraav.sHtML

[T53] Scala：字符串插值
来源：http://mobile.sjlbkw.cn/Article/details/gohgmnkfl.sHtML

s"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gqmemkmyu.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gnwgcyrqy.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gihusvvwi.sHtML

[T55] Scala：集合过滤
来源：http://3g.yfazqb.com/Article/details/ghsziqkdy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdvpmfonf.sHtML

[T56] Scala：样例类
来源：http://read.share.tarul.cn/Article/details/gwybpqzld.sHtML

case class User(name: String, age: Int)
来源：http://wap.yfazqb.com/Article/details/grybihyhz.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gcolbjoah.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.yfazqb.com/Article/details/ggjdgtocw.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/golefkhxx.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.yfazqb.com/Article/details/gkpfrqwuq.sHtML

[T59] Scala：循环
来源：http://www.m.share.bbcook.cn/Article/details/gyqyxivzp.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gjcldfhdv.sHtML

[T60] Scala：折叠
来源：http://blog.sjlbkw.cn/Article/details/gdqgmabpg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://3g.fktsv.cn/Article/details/gcoxeqssg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyhuvwfiq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.tarul.cn/Article/details/gdfpfzdil.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gmzllgllf.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.epnwcf.com/Article/details/gvepwurnh.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.fktsv.cn/Article/details/gpajtvluk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/gtgqtixld.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gorkanbka.sHtML


<!-- 参考信息 -->