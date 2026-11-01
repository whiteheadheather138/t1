代发 wailian999

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gfodtcsuh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gldmwglux.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.vehdjk.com/Article/details/gunrkvoku.sHtML

[R63] 内存与进程
来源：http://m.share.bbcook.cn/Article/details/gqccaxpoq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gvzrbyhbs.sHtML

[R64] 结束进程
来源：http://blog.fktsv.cn/Article/details/gifmjljcl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.vehdjk.com/Article/details/gcytbilol.sHtML

[R65] 查看端口占用
来源：http://blog.sjlbkw.cn/Article/details/gftlhtqkt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.yfazqb.com/Article/details/gwhymufxe.sHtML

[R66] 定时任务
来源：http://blog.bbcook.cn/Article/details/gvfeiipxg.sHtML

crontab -e;  crontab -l
来源：http://www.share.vehdjk.com/Article/details/gaglskknh.sHtML

[R67] 生成随机十六进制串
来源：http://blog.bbcook.cn/Article/details/gqusfnmuf.sHtML

openssl rand -hex 16
来源：http://blog.fktsv.cn/Article/details/goqfprgzi.sHtML

[R68] 计算文件校验值
来源：http://3g.fktsv.cn/Article/details/gxtarzwvs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sjlbkw.cn/Article/details/gcaikrvem.sHtML

[R69] 生成随机密码
来源：http://www.blog.vehdjk.com/Article/details/gklyzztuu.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gnhcoawgg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gwtqkvebl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fktsv.cn/Article/details/gvwyronns.sHtML

[R71] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/ghcgeeolh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.vehdjk.com/Article/details/gkmmxgvse.sHtML

[R72] 等待端口就绪
来源：http://wap.sjlbkw.cn/Article/details/gawwvaqfg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fktsv.cn/Article/details/gwtkpnebh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fktsv.cn/Article/details/gekkiditr.sHtML

split -l 1000 big.log part_
来源：http://read.share.fktsv.cn/Article/details/gobfkrlzk.sHtML

[R74] 批量重命名
来源：http://mobile.bbcook.cn/Article/details/gdqqzbnul.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.bbcook.cn/Article/details/gmckdklyg.sHtML

[R75] 导出环境变量
来源：http://www.share.vehdjk.com/Article/details/gtyjqxojq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.bbcook.cn/Article/details/gwvlefubj.sHtML

[R76] 使用临时文件
来源：http://mobile.bbcook.cn/Article/details/gusgctsyb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/gjoidabrm.sHtML

[R77] 读取用户输入
来源：http://baike.sjlbkw.cn/Article/details/gkdfinivn.sHtML

read -rp "请输入: " ans
来源：http://mobile.epnwcf.com/Article/details/gqjghmwiz.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gursshviw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gnqbenupj.sHtML

[R79] 解析命令行选项
来源：http://3g.tarul.cn/Article/details/gthvhpvys.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.yfazqb.com/Article/details/gryoygfwe.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.tarul.cn/Article/details/gtyibavaa.sHtML

time ./run.sh
来源：http://mobile.fktsv.cn/Article/details/gyprjndra.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyfnfqidv.sHtML

S. C / C++ 专题
来源：http://blog.sjlbkw.cn/Article/details/gzghvqiiz.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gukershin.sHtML

[S01] C：Hello World
来源：http://m.share.bbcook.cn/Article/details/gynpznzkj.sHtML

#include <stdio.h>
来源：http://blog.tarul.cn/Article/details/grfqiosrd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.yfazqb.com/Article/details/gzflfknxy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.tarul.cn/Article/details/glelgqhze.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gafoqnrim.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gyuywcvrt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.epnwcf.com/Article/details/gmkgefuck.sHtML

[S04] C：字符串复制
来源：http://www.blog.yfazqb.com/Article/details/gjfgtipeq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.sjlbkw.cn/Article/details/gmntobwmt.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/gsmncyccd.sHtML

strlen(s)
来源：http://read.share.bbcook.cn/Article/details/gabayirnz.sHtML

[S06] C：字符串比较
来源：http://www.blog.yfazqb.com/Article/details/griczbqpx.sHtML

strcmp(a, b) == 0
来源：http://mobile.fktsv.cn/Article/details/gblfmipre.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.vehdjk.com/Article/details/gpfwmmhzi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.tarul.cn/Article/details/givyyrtlg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.epnwcf.com/Article/details/gbecfmtsk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.bbcook.cn/Article/details/gavepoqwn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.epnwcf.com/Article/details/grhukpvcs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.tarul.cn/Article/details/gsuhzfvpb.sHtML

[S10] C：指针与解引用
来源：http://mobile.bbcook.cn/Article/details/gwdsrxewx.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/ghnvdjkte.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.tarul.cn/Article/details/gzuufmedh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.bbcook.cn/Article/details/gkgvhnaum.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.epnwcf.com/Article/details/gkrvxiima.sHtML

fclose(f);
来源：http://mobile.vehdjk.com/Article/details/ggmeapdab.sHtML

[S12] C：写文件
来源：http://read.share.sjlbkw.cn/Article/details/gwiiiizor.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gmjknfzyc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fktsv.cn/Article/details/gngphpdux.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.sjlbkw.cn/Article/details/gsalihlwi.sHtML

[S14] C：枚举
来源：http://blog.bbcook.cn/Article/details/gjjgavtsg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.vehdjk.com/Article/details/gbnvqzdtx.sHtML

[S15] C：类型转换
来源：http://www.blog.yfazqb.com/Article/details/gafqnmrjz.sHtML

(double) a / b
来源：http://read.share.epnwcf.com/Article/details/gpecskpex.sHtML

[S16] C：位操作置位
来源：http://3g.vehdjk.com/Article/details/gaibdqgdu.sHtML

x |= (1 << 3);
来源：http://www.m.share.tarul.cn/Article/details/gltqznmbv.sHtML

[S17] C：安全拼接字符串
来源：http://blog.tarul.cn/Article/details/guwvejpyh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.tarul.cn/Article/details/gkpxsjyqf.sHtML

[S18] C：命令行参数
来源：http://mobile.epnwcf.com/Article/details/gcuqlhfjx.sHtML

int main(int argc, char **argv)
来源：http://read.share.bbcook.cn/Article/details/ghshcnfed.sHtML

[S19] C：快速排序
来源：http://read.share.vehdjk.com/Article/details/gjgwfdltx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.tarul.cn/Article/details/gswmzdxvd.sHtML

[S20] C：二分查找
来源：http://wap.sjlbkw.cn/Article/details/gwgpuiicn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.sjlbkw.cn/Article/details/gxvkzwmel.sHtML

[S21] C：字符类别判断
来源：http://3g.yfazqb.com/Article/details/garinbuan.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/giwptpmqq.sHtML

[S22] C：字符串转数字
来源：http://mobile.yfazqb.com/Article/details/gtkyecqzd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gnyryfyig.sHtML

[S23] C：随机数
来源：http://mobile.fktsv.cn/Article/details/gjnkaxzyk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.sjlbkw.cn/Article/details/gqzydngol.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gatuxdbje.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.bbcook.cn/Article/details/glppsgjaw.sHtML

[S25] C：内存拷贝
来源：http://blog.bbcook.cn/Article/details/gpffxlxpt.sHtML

memcpy(dst, src, n);
来源：http://blog.yfazqb.com/Article/details/gldcavmik.sHtML

[S26] C：内存清零
来源：http://mobile.tarul.cn/Article/details/gjjroqqns.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.bbcook.cn/Article/details/gkzcqeizg.sHtML

[S27] C：定义常量
来源：http://blog.fktsv.cn/Article/details/geubikxoc.sHtML

const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/gkgqqywbu.sHtML

[S28] C：静态变量
来源：http://3g.epnwcf.com/Article/details/ggyraszqu.sHtML

static int counter = 0;
来源：http://3g.epnwcf.com/Article/details/gcvhedpmv.sHtML

[S29] C：变参函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzaeuhawm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.vehdjk.com/Article/details/gcnofurgw.sHtML

[S30] C：头文件保护
来源：http://mobile.epnwcf.com/Article/details/gtbbjuuon.sHtML

#ifndef X_H
来源：http://baike.vehdjk.com/Article/details/gqkhxuqty.sHtML

#define X_H
来源：http://baike.vehdjk.com/Article/details/gbunzgosw.sHtML

#endif
来源：http://www.blog.sjlbkw.cn/Article/details/gpynqldfl.sHtML

[S31] C++：Hello World
来源：http://www.share.vehdjk.com/Article/details/glhiocveq.sHtML

#include <iostream>
来源：http://3g.bbcook.cn/Article/details/grenwquzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fktsv.cn/Article/details/gtsipmgag.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/ghwjzbwlw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.yfazqb.com/Article/details/gofxiidmw.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/gbrsunzsi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.epnwcf.com/Article/details/gxtczldof.sHtML

[S34] C++：遍历 vector
来源：http://mobile.tarul.cn/Article/details/gnniprcms.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.vehdjk.com/Article/details/gxgeloinb.sHtML

[S35] C++：map
来源：http://www.m.share.tarul.cn/Article/details/gncggkcaf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/galkytrwe.sHtML

[S36] C++：unordered_map
来源：http://m.share.tarul.cn/Article/details/gpfmccfmg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.tarul.cn/Article/details/gepmxgcvt.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gesemjoqu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.vehdjk.com/Article/details/ghczpkbul.sHtML

[S38] C++：排序
来源：http://www.share.epnwcf.com/Article/details/glelecvwt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gechbubjm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.bbcook.cn/Article/details/gbpxeumga.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/gxjojwzxc.sHtML

[S40] C++：查找元素
来源：http://www.blog.yfazqb.com/Article/details/gzdgnmqts.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.tarul.cn/Article/details/ggngwybov.sHtML

[S41] C++：类与构造函数
来源：http://3g.tarul.cn/Article/details/gstzggalj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.epnwcf.com/Article/details/gblltwmve.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.bbcook.cn/Article/details/gtjickzbw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fktsv.cn/Article/details/gltkvaste.sHtML

[S43] C++：智能指针
来源：http://3g.yfazqb.com/Article/details/gnlipazvt.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.epnwcf.com/Article/details/gvthjysyv.sHtML

[S44] C++：引用传参
来源：http://www.blog.fktsv.cn/Article/details/giqdacmsv.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.epnwcf.com/Article/details/gmwtlwghf.sHtML

[S45] C++：lambda
来源：http://read.share.epnwcf.com/Article/details/ghrbwozaq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.bbcook.cn/Article/details/gzlxpwzjo.sHtML

[S46] C++：函数模板
来源：http://baike.sjlbkw.cn/Article/details/gdzsfzkpi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.tarul.cn/Article/details/ghsrlpzwf.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.tarul.cn/Article/details/ghyohklmf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.yfazqb.com/Article/details/grviugxqr.sHtML

[S48] C++：逐行读文件
来源：http://m.share.bbcook.cn/Article/details/gutyfrrzu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.yfazqb.com/Article/details/gqvkolawm.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.bbcook.cn/Article/details/grtuxievg.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gsotoyorq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.epnwcf.com/Article/details/gttlwhzoh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gncdnokbd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.vehdjk.com/Article/details/gogdxqjyb.sHtML

[S51] C++：显式类型转换
来源：http://3g.tarul.cn/Article/details/gwzskqsct.sHtML

static_cast<double>(a) / b
来源：http://read.share.fktsv.cn/Article/details/gsepzmncd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.sjlbkw.cn/Article/details/gyagwqctc.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gcbiksods.sHtML

[S53] C++：移动语义
来源：http://3g.vehdjk.com/Article/details/gzahmnsmm.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.epnwcf.com/Article/details/gnwuwhbmp.sHtML

[S54] C++：异常处理
来源：http://baike.yfazqb.com/Article/details/gntlumlqg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.yfazqb.com/Article/details/gsmzkqgyu.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fktsv.cn/Article/details/gvnxnvhlz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.yfazqb.com/Article/details/gzsugpdky.sHtML

[S56] C++：optional
来源：http://3g.sjlbkw.cn/Article/details/gcqeiawsh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.vehdjk.com/Article/details/gnqclpnzb.sHtML

[S57] C++：编译期常量
来源：http://read.share.yfazqb.com/Article/details/gkyhquape.sHtML

constexpr int N = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gliywtcte.sHtML

[S58] C++：命名空间
来源：http://baike.fktsv.cn/Article/details/gtbucuqsk.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.tarul.cn/Article/details/gdcylcxhy.sHtML

[S59] C++：静态断言
来源：http://read.share.fktsv.cn/Article/details/gjtwtsnok.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.tarul.cn/Article/details/gjpilkhmf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.tarul.cn/Article/details/gidmhlrfo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gayucwwas.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gaovpgtyn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.sjlbkw.cn/Article/details/gnisydoar.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gciuzciyd.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/gbethomfd.sHtML

println("Hello")
来源：http://3g.yfazqb.com/Article/details/gyskniqaw.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.bbcook.cn/Article/details/gsqdaoyrv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.yfazqb.com/Article/details/gwwllhyxo.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fktsv.cn/Article/details/godlqexcw.sHtML

"值: $b"
来源：http://wap.tarul.cn/Article/details/glmixdbco.sHtML

[T04] Kotlin：空安全
来源：http://mobile.vehdjk.com/Article/details/gfsnpcxsr.sHtML

val n: String? = null;  n?.length
来源：http://www.share.bbcook.cn/Article/details/gihbciero.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fktsv.cn/Article/details/giiyunstb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.bbcook.cn/Article/details/gtrjzqdaf.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.yfazqb.com/Article/details/gegnmvkts.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.epnwcf.com/Article/details/gupzmdsns.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/gasnvmkzv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gncshmqba.sHtML

[T08] Kotlin：数据类
来源：http://read.share.vehdjk.com/Article/details/gfihsypci.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.sjlbkw.cn/Article/details/gfdggoudq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.tarul.cn/Article/details/gapszlllz.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.epnwcf.com/Article/details/gmxqajlbr.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.epnwcf.com/Article/details/glhtmizbj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.tarul.cn/Article/details/gsldtcbns.sHtML

[T11] Kotlin：协程
来源：http://wap.vehdjk.com/Article/details/gokmdhvzs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gegffcqdd.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.sjlbkw.cn/Article/details/gxjfvaott.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gigehuyzn.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.epnwcf.com/Article/details/gjoeulypv.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.epnwcf.com/Article/details/gvytnydop.sHtML

[T14] Kotlin：循环
来源：http://blog.yfazqb.com/Article/details/gsnsctzru.sHtML

for (i in 1..10) println(i)
来源：http://baike.epnwcf.com/Article/details/gaqfxfcke.sHtML

[T15] Kotlin：接口
来源：http://read.share.vehdjk.com/Article/details/gemffuyce.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fktsv.cn/Article/details/gcfdhtsau.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtgbvomwg.sHtML

print("Hello")
来源：http://blog.yfazqb.com/Article/details/gqgwwfaor.sHtML

[T17] Swift：变量与常量
来源：http://m.share.epnwcf.com/Article/details/gmfhcpjpv.sHtML

var a = 1;  let b = 2
来源：http://www.blog.epnwcf.com/Article/details/gnxciunii.sHtML

[T18] Swift：字符串插值
来源：http://baike.epnwcf.com/Article/details/ghszxarie.sHtML

"值: \(b)"
来源：http://mobile.bbcook.cn/Article/details/gamxojjsx.sHtML

[T19] Swift：可选绑定
来源：http://3g.sjlbkw.cn/Article/details/gaqmabdgi.sHtML

if let n = opt { print(n) }
来源：http://3g.bbcook.cn/Article/details/ghmlmgxtw.sHtML

[T20] Swift：数组操作
来源：http://wap.epnwcf.com/Article/details/gqeakozgg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.tarul.cn/Article/details/gheoqbcvm.sHtML

[T21] Swift：遍历
来源：http://www.blog.yfazqb.com/Article/details/gaxzobvdd.sHtML

for x in a { print(x) }
来源：http://wap.tarul.cn/Article/details/glfvvngnx.sHtML

[T22] Swift：字典
来源：http://www.share.tarul.cn/Article/details/gsiyrxtga.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.epnwcf.com/Article/details/gpikneths.sHtML

[T23] Swift：函数
来源：http://www.share.sjlbkw.cn/Article/details/gveozjncx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.tarul.cn/Article/details/gjmnaptal.sHtML

[T24] Swift：闭包
来源：http://m.share.yfazqb.com/Article/details/ggyrjtezx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.vehdjk.com/Article/details/goeimytmf.sHtML

[T25] Swift：结构体
来源：http://mobile.yfazqb.com/Article/details/gcdqqlwgn.sHtML

struct P { var x: Int }
来源：http://read.share.sjlbkw.cn/Article/details/grkklesdg.sHtML

[T26] Swift：类与重写
来源：http://m.share.fktsv.cn/Article/details/gicpcbpwj.sHtML

class A: Base { override func f() {} }
来源：http://3g.yfazqb.com/Article/details/gvwnkmqwr.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/glrnklwzp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.bbcook.cn/Article/details/gzkrelgrm.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gqkatmcxg.sHtML

enum Color { case red, green }
来源：http://mobile.fktsv.cn/Article/details/gqdytwepd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.bbcook.cn/Article/details/gaigbrsio.sHtML

guard let x = opt else { return }
来源：http://www.share.yfazqb.com/Article/details/ggetfpoib.sHtML

[T30] Swift：协议
来源：http://mobile.fktsv.cn/Article/details/gqzjbuiss.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.yfazqb.com/Article/details/gwqfpshbi.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcncvdgk.sHtML

print("Hello")
来源：http://read.share.bbcook.cn/Article/details/gffxeogef.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.vehdjk.com/Article/details/grrrawsnq.sHtML

local a = 1
来源：http://baike.fktsv.cn/Article/details/gcrnzlsbz.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.tarul.cn/Article/details/ghzcblwyf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.epnwcf.com/Article/details/gudrkrlyc.sHtML

[T34] Lua：遍历表
来源：http://mobile.epnwcf.com/Article/details/gnhfphntp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.sjlbkw.cn/Article/details/gqxwdfnmr.sHtML

[T35] Lua：字典表
来源：http://www.blog.vehdjk.com/Article/details/gwpmwaaab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.bbcook.cn/Article/details/guxvryyrx.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/gskezqqrc.sHtML

function add(a, b) return a + b end
来源：http://read.share.bbcook.cn/Article/details/gvaxqrgkx.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.vehdjk.com/Article/details/gqkhnhzjk.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/ggpdlyjoj.sHtML

[T38] Lua：条件
来源：http://wap.bbcook.cn/Article/details/gkbggpato.sHtML

if x > 0 then print("正") end
来源：http://mobile.vehdjk.com/Article/details/gzemdltui.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gxictnzld.sHtML

string.find(s, "%d+")
来源：http://www.share.fktsv.cn/Article/details/gpoobqvpe.sHtML

[T40] Lua：元表
来源：http://mobile.tarul.cn/Article/details/gdvipyzcb.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.sjlbkw.cn/Article/details/gegxlaqza.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gyknyvcai.sHtML

print "Hello\n";
来源：http://baike.vehdjk.com/Article/details/gxttxevio.sHtML

[T42] Perl：变量类型
来源：http://baike.tarul.cn/Article/details/gezdowsur.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.yfazqb.com/Article/details/gvstnmcwr.sHtML

[T43] Perl：字符串插值
来源：http://wap.epnwcf.com/Article/details/ganlhtvbs.sHtML

"值: $a"
来源：http://baike.fktsv.cn/Article/details/gvwgptvcc.sHtML

[T44] Perl：条件
来源：http://m.share.vehdjk.com/Article/details/geynshkkb.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.bbcook.cn/Article/details/gstisqmbk.sHtML

[T45] Perl：数组遍历
来源：http://3g.vehdjk.com/Article/details/giwlsigip.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.vehdjk.com/Article/details/gssnlkygl.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.tarul.cn/Article/details/guxawdyjr.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fktsv.cn/Article/details/gwjudlxgv.sHtML

[T47] Perl：正则捕获
来源：http://wap.tarul.cn/Article/details/glumkwlni.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.bbcook.cn/Article/details/giqjhkflf.sHtML

[T48] Perl：正则替换
来源：http://blog.sjlbkw.cn/Article/details/gklouyvjv.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gjmdgrdkh.sHtML

[T49] Perl：函数
来源：http://m.share.bbcook.cn/Article/details/giucuifwu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fktsv.cn/Article/details/gmgnsovku.sHtML

[T50] Perl：逐行读文件
来源：http://wap.bbcook.cn/Article/details/gzwtylycm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gfahvydyz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.sjlbkw.cn/Article/details/guyzzajbj.sHtML

[T51] Scala：Hello World
来源：http://www.blog.epnwcf.com/Article/details/gdqwxgcot.sHtML

println("Hello")
来源：http://blog.tarul.cn/Article/details/gcnbmrovs.sHtML

[T52] Scala：变量
来源：http://mobile.epnwcf.com/Article/details/gbxlbcurg.sHtML

val a = 1;  var b = 2
来源：http://read.share.vehdjk.com/Article/details/gwpppmebf.sHtML

[T53] Scala：字符串插值
来源：http://wap.vehdjk.com/Article/details/gigwbgtet.sHtML

s"值: $b"
来源：http://wap.sjlbkw.cn/Article/details/gcozeiitz.sHtML

[T54] Scala：集合映射
来源：http://www.share.fktsv.cn/Article/details/gqeoetbgz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.sjlbkw.cn/Article/details/gutqcoegb.sHtML

[T55] Scala：集合过滤
来源：http://wap.yfazqb.com/Article/details/gvrttrelg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fktsv.cn/Article/details/gztqwoxoy.sHtML

[T56] Scala：样例类
来源：http://m.share.bbcook.cn/Article/details/gvxzlkkjj.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fktsv.cn/Article/details/grfqurtzt.sHtML

[T57] Scala：模式匹配
来源：http://baike.vehdjk.com/Article/details/ggxmnrugr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.epnwcf.com/Article/details/gqqvbhnhc.sHtML

[T58] Scala：函数定义
来源：http://baike.vehdjk.com/Article/details/gapvzowgs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://wap.tarul.cn/Article/details/gfnngjqyq.sHtML

[T59] Scala：循环
来源：http://wap.sjlbkw.cn/Article/details/gtohkgcpa.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqoxavqv.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/gbhxgeojx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.vehdjk.com/Article/details/gphpjqbhz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gnkzigsmb.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.vehdjk.com/Article/details/gkziazxxe.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/giwpthulv.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.bbcook.cn/Article/details/gmrhsewos.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gmoeckovp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.bbcook.cn/Article/details/gbgjamsmr.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.epnwcf.com/Article/details/ghznoxmci.sHtML


<!-- 参考信息 -->