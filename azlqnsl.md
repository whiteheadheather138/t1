代发 wailian999

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/grixvzbti.sHtML

[R58] 下载文件
来源：http://www.m.share.epnwcf.com/Article/details/guiwvukmd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.yfazqb.com/Article/details/glvdbonna.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/genrrcklu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.tarul.cn/Article/details/ghixxstbb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gfndnizir.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gsfjegnzz.sHtML

[R61] 磁盘占用
来源：http://read.share.yfazqb.com/Article/details/gnbjdpybu.sHtML

df -h;  du -sh *
来源：http://mobile.yfazqb.com/Article/details/gwngupfnt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.bbcook.cn/Article/details/gbberffno.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fktsv.cn/Article/details/gpuennmip.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gpxnkzcir.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.yfazqb.com/Article/details/gbmtzzuwq.sHtML

[R64] 结束进程
来源：http://3g.epnwcf.com/Article/details/gbptgwtso.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.bbcook.cn/Article/details/gcmfgqgks.sHtML

[R65] 查看端口占用
来源：http://read.share.yfazqb.com/Article/details/gwjratgvd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.yfazqb.com/Article/details/gyumsaykm.sHtML

[R66] 定时任务
来源：http://mobile.fktsv.cn/Article/details/gckyfyxze.sHtML

crontab -e;  crontab -l
来源：http://mobile.sjlbkw.cn/Article/details/gimatackt.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.bbcook.cn/Article/details/gwxnyltnc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fktsv.cn/Article/details/gfglqsprb.sHtML

[R68] 计算文件校验值
来源：http://baike.yfazqb.com/Article/details/gdpaxxeta.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.bbcook.cn/Article/details/gaashddga.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gkkaorsti.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fktsv.cn/Article/details/gcxqlygzx.sHtML

[R70] 时间戳与互转
来源：http://blog.tarul.cn/Article/details/gbunlxeuk.sHtML

date +%s;  date -d @1700000000
来源：http://wap.bbcook.cn/Article/details/guoqftiyc.sHtML

[R71] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gmvvrrdle.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.tarul.cn/Article/details/gccymmpvr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.vehdjk.com/Article/details/gqwxrynve.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/ggxzvzcxe.sHtML

[R73] 分割大日志
来源：http://3g.sjlbkw.cn/Article/details/gpjkchdzx.sHtML

split -l 1000 big.log part_
来源：http://wap.tarul.cn/Article/details/gweqjaste.sHtML

[R74] 批量重命名
来源：http://m.share.yfazqb.com/Article/details/gauglatnv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.bbcook.cn/Article/details/gurcgyfow.sHtML

[R75] 导出环境变量
来源：http://blog.vehdjk.com/Article/details/gwwkshgsd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.epnwcf.com/Article/details/gxupyoqmp.sHtML

[R76] 使用临时文件
来源：http://www.blog.vehdjk.com/Article/details/gldwjpkoi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/grjuioxre.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gxmtxayka.sHtML

read -rp "请输入: " ans
来源：http://3g.bbcook.cn/Article/details/gczrgxxme.sHtML

[R78] 交互式菜单
来源：http://www.share.vehdjk.com/Article/details/gkpvrntpx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.epnwcf.com/Article/details/gdjsbnvdm.sHtML

[R79] 解析命令行选项
来源：http://m.share.vehdjk.com/Article/details/gezjdqkui.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.sjlbkw.cn/Article/details/geuymujtt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fktsv.cn/Article/details/gsgcfnyho.sHtML

time ./run.sh
来源：http://wap.tarul.cn/Article/details/gssnutnnj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grlhdqfep.sHtML

S. C / C++ 专题
来源：http://www.blog.epnwcf.com/Article/details/gnpvxnzks.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gcjavruwo.sHtML

[S01] C：Hello World
来源：http://blog.fktsv.cn/Article/details/gizhuzyhe.sHtML

#include <stdio.h>
来源：http://www.blog.tarul.cn/Article/details/gtpqxbtmt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.sjlbkw.cn/Article/details/gslpkxpma.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/gagoctrvg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gxwwtxony.sHtML

[S03] C：读入整数
来源：http://www.m.share.epnwcf.com/Article/details/givejpqqi.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fktsv.cn/Article/details/gyksllfsf.sHtML

[S04] C：字符串复制
来源：http://m.share.fktsv.cn/Article/details/grqrjadam.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfmeicly.sHtML

[S05] C：字符串长度
来源：http://mobile.sjlbkw.cn/Article/details/gycqrmmrx.sHtML

strlen(s)
来源：http://read.share.epnwcf.com/Article/details/geeerhbor.sHtML

[S06] C：字符串比较
来源：http://read.share.yfazqb.com/Article/details/gevnlfvpy.sHtML

strcmp(a, b) == 0
来源：http://3g.bbcook.cn/Article/details/galuhpebl.sHtML

[S07] C：数组遍历求和
来源：http://mobile.yfazqb.com/Article/details/gjggymbzu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.vehdjk.com/Article/details/gpoofjjwy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fktsv.cn/Article/details/ghxogztwo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fktsv.cn/Article/details/giaoyppkl.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/glabgyurx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.epnwcf.com/Article/details/gqbvzjmkx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gkikhiewl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.yfazqb.com/Article/details/glsqhmqrq.sHtML

[S11] C：逐行读文件
来源：http://m.share.epnwcf.com/Article/details/gwfbcysjc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.tarul.cn/Article/details/gctypuwwg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.bbcook.cn/Article/details/gamtexcll.sHtML

fclose(f);
来源：http://www.blog.bbcook.cn/Article/details/gsfrwdxzz.sHtML

[S12] C：写文件
来源：http://www.m.share.vehdjk.com/Article/details/ghqchpjky.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxoczkir.sHtML

[S13] C：宏定义
来源：http://baike.fktsv.cn/Article/details/gxwtemdxt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gjslktxdz.sHtML

[S14] C：枚举
来源：http://baike.epnwcf.com/Article/details/gikdptqot.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.yfazqb.com/Article/details/gdnhiysyk.sHtML

[S15] C：类型转换
来源：http://mobile.epnwcf.com/Article/details/gsldwtszp.sHtML

(double) a / b
来源：http://www.blog.fktsv.cn/Article/details/gmqemidfr.sHtML

[S16] C：位操作置位
来源：http://m.share.yfazqb.com/Article/details/gmfbqujnf.sHtML

x |= (1 << 3);
来源：http://baike.vehdjk.com/Article/details/gvpyedfwm.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gahzlycre.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.vehdjk.com/Article/details/gssbulclp.sHtML

[S18] C：命令行参数
来源：http://3g.yfazqb.com/Article/details/gxikjlozw.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gkdhdiqqo.sHtML

[S19] C：快速排序
来源：http://www.blog.yfazqb.com/Article/details/gfdidqjop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/gbjaonvmb.sHtML

[S20] C：二分查找
来源：http://www.m.share.fktsv.cn/Article/details/gscncjvpf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fktsv.cn/Article/details/ghgpsixxr.sHtML

[S21] C：字符类别判断
来源：http://3g.tarul.cn/Article/details/gfzfzaxti.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.sjlbkw.cn/Article/details/glyudijch.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.tarul.cn/Article/details/gxmpncyxy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fktsv.cn/Article/details/gwjzisths.sHtML

[S23] C：随机数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghytfeyxs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.vehdjk.com/Article/details/gezewunwq.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/ggnkobleu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.yfazqb.com/Article/details/gbnpwjygy.sHtML

[S25] C：内存拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gnsxmqlnf.sHtML

memcpy(dst, src, n);
来源：http://baike.fktsv.cn/Article/details/ghijyazwl.sHtML

[S26] C：内存清零
来源：http://read.share.vehdjk.com/Article/details/goawsakla.sHtML

memset(a, 0, sizeof a);
来源：http://baike.epnwcf.com/Article/details/gvrejhytz.sHtML

[S27] C：定义常量
来源：http://www.blog.bbcook.cn/Article/details/glugojrqo.sHtML

const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gckkqzpdl.sHtML

[S28] C：静态变量
来源：http://www.blog.sjlbkw.cn/Article/details/glgedvuvc.sHtML

static int counter = 0;
来源：http://mobile.bbcook.cn/Article/details/gtwruekvu.sHtML

[S29] C：变参函数
来源：http://wap.yfazqb.com/Article/details/gzksrbqkl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.yfazqb.com/Article/details/gxncjvnda.sHtML

[S30] C：头文件保护
来源：http://3g.sjlbkw.cn/Article/details/gfcyepgcj.sHtML

#ifndef X_H
来源：http://www.m.share.bbcook.cn/Article/details/gccpxmmns.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/giwwepxla.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/gbtodjfav.sHtML

[S31] C++：Hello World
来源：http://wap.bbcook.cn/Article/details/gkzypfgyv.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/ggeipnizn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.vehdjk.com/Article/details/gzgrmxbqu.sHtML

[S32] C++：字符串
来源：http://blog.yfazqb.com/Article/details/gojwmikil.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.sjlbkw.cn/Article/details/gwkjhjmbj.sHtML

[S33] C++：vector 增删
来源：http://www.blog.epnwcf.com/Article/details/gtbvigwmu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.epnwcf.com/Article/details/gpvsxowfn.sHtML

[S34] C++：遍历 vector
来源：http://baike.sjlbkw.cn/Article/details/gxmprfkml.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fktsv.cn/Article/details/gxghvgqur.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/gjovgijef.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/glpxwojph.sHtML

[S36] C++：unordered_map
来源：http://mobile.bbcook.cn/Article/details/gcghvruhm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gnbxfbajq.sHtML

[S37] C++：set
来源：http://mobile.tarul.cn/Article/details/gbijbscoz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.epnwcf.com/Article/details/gbqifyitw.sHtML

[S38] C++：排序
来源：http://3g.fktsv.cn/Article/details/gumvlcplr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/gddjukbar.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.tarul.cn/Article/details/gbeuugaqr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fktsv.cn/Article/details/gsizwqjhl.sHtML

[S40] C++：查找元素
来源：http://www.share.fktsv.cn/Article/details/gttezicdk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.tarul.cn/Article/details/gqvcroddu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.vehdjk.com/Article/details/glzdygwwi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.bbcook.cn/Article/details/gskzgqnbe.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fktsv.cn/Article/details/gnlpkjnmp.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.epnwcf.com/Article/details/gahmedqrr.sHtML

[S43] C++：智能指针
来源：http://baike.epnwcf.com/Article/details/gwvpfjdcb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.tarul.cn/Article/details/grsohvbco.sHtML

[S44] C++：引用传参
来源：http://www.m.share.yfazqb.com/Article/details/gtydraidw.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/glsjyezgb.sHtML

[S45] C++：lambda
来源：http://www.share.sjlbkw.cn/Article/details/grchlllhw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.sjlbkw.cn/Article/details/gwjfhozsz.sHtML

[S46] C++：函数模板
来源：http://baike.fktsv.cn/Article/details/gojpjcdqf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fktsv.cn/Article/details/gexvmtkwy.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.yfazqb.com/Article/details/gahmlbqtd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.bbcook.cn/Article/details/gwvskoltq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gkauhkpbv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fktsv.cn/Article/details/grhncpnvr.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.epnwcf.com/Article/details/ggqxayexz.sHtML

[S49] C++：写文件
来源：http://mobile.sjlbkw.cn/Article/details/gqhvuwqye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.tarul.cn/Article/details/gkqktijdn.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gfeohdmis.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.bbcook.cn/Article/details/ghhpwnxqn.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gxzotwswr.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/geoxdfndw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.vehdjk.com/Article/details/gepgrgrqr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.tarul.cn/Article/details/gxjsoetwv.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gilcbhzdj.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.sjlbkw.cn/Article/details/gtdviifhc.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gtsvycyru.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.sjlbkw.cn/Article/details/gvbzmyqjo.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxltgwry.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.bbcook.cn/Article/details/geizexwyd.sHtML

[S56] C++：optional
来源：http://mobile.bbcook.cn/Article/details/gvvdsbxby.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gidsqjfmj.sHtML

[S57] C++：编译期常量
来源：http://m.share.bbcook.cn/Article/details/gytxijvmr.sHtML

constexpr int N = 10;
来源：http://read.share.vehdjk.com/Article/details/gnaauivvj.sHtML

[S58] C++：命名空间
来源：http://read.share.tarul.cn/Article/details/gqrvrnfcs.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.vehdjk.com/Article/details/gojhkopgj.sHtML

[S59] C++：静态断言
来源：http://www.blog.epnwcf.com/Article/details/gueqhmgyt.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.bbcook.cn/Article/details/gevodhtto.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.vehdjk.com/Article/details/geyuabiek.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gaewbiyjs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnwgptfzb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.yfazqb.com/Article/details/gdzyfsdkx.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyvkctalq.sHtML

[T01] Kotlin：Hello World
来源：http://3g.epnwcf.com/Article/details/gteavnmvs.sHtML

println("Hello")
来源：http://baike.fktsv.cn/Article/details/gzyavwlxh.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/glvthysgl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.vehdjk.com/Article/details/guakuyqkj.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.bbcook.cn/Article/details/ghqkiwfxc.sHtML

"值: $b"
来源：http://read.share.sjlbkw.cn/Article/details/gegbnlxwa.sHtML

[T04] Kotlin：空安全
来源：http://baike.vehdjk.com/Article/details/genxvqlri.sHtML

val n: String? = null;  n?.length
来源：http://www.share.sjlbkw.cn/Article/details/gstnzgjey.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.epnwcf.com/Article/details/gecqiayiz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.epnwcf.com/Article/details/ghlnmrcon.sHtML

[T06] Kotlin：集合映射
来源：http://blog.vehdjk.com/Article/details/gghknhkvg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.sjlbkw.cn/Article/details/gddyocaoo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.sjlbkw.cn/Article/details/gbryekiwi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.bbcook.cn/Article/details/gdxbgsoai.sHtML

[T08] Kotlin：数据类
来源：http://read.share.yfazqb.com/Article/details/gufukzlpu.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.bbcook.cn/Article/details/gqpznoupv.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.epnwcf.com/Article/details/gjqyyingb.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.sjlbkw.cn/Article/details/gyvjnhruv.sHtML

[T10] Kotlin：默认参数
来源：http://baike.epnwcf.com/Article/details/gzbguxhno.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.yfazqb.com/Article/details/goakxqzxe.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpaezmxy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fktsv.cn/Article/details/gwolofbvj.sHtML

[T12] Kotlin：解构声明
来源：http://blog.sjlbkw.cn/Article/details/gkivazbtm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.bbcook.cn/Article/details/gkeuitkrl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.bbcook.cn/Article/details/gtwdefoxb.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.bbcook.cn/Article/details/gklfgsvuw.sHtML

[T14] Kotlin：循环
来源：http://read.share.vehdjk.com/Article/details/gjskyzgzj.sHtML

for (i in 1..10) println(i)
来源：http://3g.tarul.cn/Article/details/gvcxqsycd.sHtML

[T15] Kotlin：接口
来源：http://www.share.fktsv.cn/Article/details/gfwlmirqn.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.sjlbkw.cn/Article/details/gwtizxnea.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gbhzwkdpk.sHtML

print("Hello")
来源：http://baike.sjlbkw.cn/Article/details/gbyrwfqud.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fktsv.cn/Article/details/gfivhcwmv.sHtML

var a = 1;  let b = 2
来源：http://read.share.tarul.cn/Article/details/gukchlave.sHtML

[T18] Swift：字符串插值
来源：http://baike.yfazqb.com/Article/details/gfengukvk.sHtML

"值: \(b)"
来源：http://www.share.bbcook.cn/Article/details/glyksmgqg.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gsedvavun.sHtML

if let n = opt { print(n) }
来源：http://www.blog.bbcook.cn/Article/details/gifkpwjpo.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/geuxmgyjm.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.sjlbkw.cn/Article/details/ggefeqqeh.sHtML

[T21] Swift：遍历
来源：http://3g.yfazqb.com/Article/details/gdytrozfc.sHtML

for x in a { print(x) }
来源：http://baike.bbcook.cn/Article/details/glccwxbpe.sHtML

[T22] Swift：字典
来源：http://wap.yfazqb.com/Article/details/gagcfgaen.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.yfazqb.com/Article/details/gizputaii.sHtML

[T23] Swift：函数
来源：http://wap.vehdjk.com/Article/details/gdoqhkcjl.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.vehdjk.com/Article/details/gytteuikp.sHtML

[T24] Swift：闭包
来源：http://baike.yfazqb.com/Article/details/gotvbhtqd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.sjlbkw.cn/Article/details/gbzxcmqzb.sHtML

[T25] Swift：结构体
来源：http://www.share.bbcook.cn/Article/details/gtqdahohd.sHtML

struct P { var x: Int }
来源：http://wap.vehdjk.com/Article/details/grkzxxscm.sHtML

[T26] Swift：类与重写
来源：http://mobile.tarul.cn/Article/details/gyazeenwd.sHtML

class A: Base { override func f() {} }
来源：http://baike.bbcook.cn/Article/details/geiddzhpv.sHtML

[T27] Swift：错误处理
来源：http://read.share.tarul.cn/Article/details/gozoybccv.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.bbcook.cn/Article/details/gdsxjghyy.sHtML

[T28] Swift：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gfbnpjxwq.sHtML

enum Color { case red, green }
来源：http://3g.tarul.cn/Article/details/gflxqxmpq.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.tarul.cn/Article/details/gzpvlvqff.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/grapayvgx.sHtML

[T30] Swift：协议
来源：http://www.m.share.sjlbkw.cn/Article/details/grbhfqqss.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.tarul.cn/Article/details/gesggjcru.sHtML

[T31] Lua：Hello World
来源：http://mobile.vehdjk.com/Article/details/gosruzozy.sHtML

print("Hello")
来源：http://read.share.tarul.cn/Article/details/gdaoykytw.sHtML

[T32] Lua：局部变量
来源：http://mobile.yfazqb.com/Article/details/gxyrnkjqj.sHtML

local a = 1
来源：http://3g.bbcook.cn/Article/details/gevbbdqon.sHtML

[T33] Lua：表（数组）
来源：http://wap.epnwcf.com/Article/details/ggeasjzsa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.epnwcf.com/Article/details/gjprdykkg.sHtML

[T34] Lua：遍历表
来源：http://m.share.bbcook.cn/Article/details/gygcyphqd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/genmeslrb.sHtML

[T35] Lua：字典表
来源：http://3g.tarul.cn/Article/details/gljqnhmyj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.sjlbkw.cn/Article/details/gpaqvpvpf.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gjgzocrys.sHtML

function add(a, b) return a + b end
来源：http://m.share.tarul.cn/Article/details/gquiraynd.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/ggmhapumw.sHtML

"a" .. "b"
来源：http://read.share.epnwcf.com/Article/details/gvvrpkgcn.sHtML

[T38] Lua：条件
来源：http://wap.vehdjk.com/Article/details/grljrvwng.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.yfazqb.com/Article/details/gtmztrvoy.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.fktsv.cn/Article/details/gwzpnlvtf.sHtML

string.find(s, "%d+")
来源：http://wap.fktsv.cn/Article/details/gbjiajhjs.sHtML

[T40] Lua：元表
来源：http://blog.tarul.cn/Article/details/glqttygwr.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gvwcatcci.sHtML

[T41] Perl：Hello World
来源：http://wap.yfazqb.com/Article/details/gouguqiax.sHtML

print "Hello\n";
来源：http://m.share.epnwcf.com/Article/details/gfavymzfr.sHtML

[T42] Perl：变量类型
来源：http://baike.fktsv.cn/Article/details/geicdoxni.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.sjlbkw.cn/Article/details/gudqvucky.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/gmrbzmywj.sHtML

"值: $a"
来源：http://3g.yfazqb.com/Article/details/gkvakhpkk.sHtML

[T44] Perl：条件
来源：http://wap.sjlbkw.cn/Article/details/gurzhgndg.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.tarul.cn/Article/details/gpfftrvrh.sHtML

[T45] Perl：数组遍历
来源：http://3g.fktsv.cn/Article/details/gqsumzthu.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.bbcook.cn/Article/details/gadhtemio.sHtML

[T46] Perl：哈希操作
来源：http://m.share.bbcook.cn/Article/details/goheynuzg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.bbcook.cn/Article/details/guphmivqj.sHtML

[T47] Perl：正则捕获
来源：http://read.share.epnwcf.com/Article/details/gysaigdso.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.vehdjk.com/Article/details/gbhxajlrp.sHtML

[T48] Perl：正则替换
来源：http://baike.yfazqb.com/Article/details/gioxkpwrm.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.epnwcf.com/Article/details/giuznieai.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gteriyjrl.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gytdxxcnd.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.bbcook.cn/Article/details/gggnbmkcf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.vehdjk.com/Article/details/gjjekjtau.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fktsv.cn/Article/details/gbgydhlmt.sHtML

[T51] Scala：Hello World
来源：http://wap.bbcook.cn/Article/details/gmoosrart.sHtML

println("Hello")
来源：http://m.share.vehdjk.com/Article/details/gqzolsmag.sHtML

[T52] Scala：变量
来源：http://m.share.tarul.cn/Article/details/gtoidnjpn.sHtML

val a = 1;  var b = 2
来源：http://baike.bbcook.cn/Article/details/gthudrend.sHtML

[T53] Scala：字符串插值
来源：http://blog.bbcook.cn/Article/details/gwbrttvdp.sHtML

s"值: $b"
来源：http://baike.tarul.cn/Article/details/gqplqczdf.sHtML

[T54] Scala：集合映射
来源：http://m.share.epnwcf.com/Article/details/gkkhfezoi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.yfazqb.com/Article/details/gbxwwhmjv.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fktsv.cn/Article/details/gnrwpqmli.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.epnwcf.com/Article/details/gvydgmcdj.sHtML

[T56] Scala：样例类
来源：http://3g.sjlbkw.cn/Article/details/goyyepczw.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gdklkmnop.sHtML

[T57] Scala：模式匹配
来源：http://blog.fktsv.cn/Article/details/gyezjstyr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gxfmecgal.sHtML

[T58] Scala：函数定义
来源：http://www.share.sjlbkw.cn/Article/details/gmghqutek.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.bbcook.cn/Article/details/gnvksbmzd.sHtML

[T59] Scala：循环
来源：http://read.share.bbcook.cn/Article/details/gdesqzfmy.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.sjlbkw.cn/Article/details/gnlqmxjhz.sHtML

[T60] Scala：折叠
来源：http://blog.tarul.cn/Article/details/glhztkzio.sHtML


<!-- 参考信息 -->