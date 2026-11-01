代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.bbcook.cn/Article/details/gktmdgwtm.sHtML

[R56] 远程拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gylhjfenf.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/giyxzlqrs.sHtML

[R57] 远程执行命令
来源：http://3g.vehdjk.com/Article/details/grbwwzlyc.sHtML

ssh user@host 'uptime'
来源：http://read.share.sjlbkw.cn/Article/details/gonglduwf.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gakmgjnlm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.tarul.cn/Article/details/gqyvusgxy.sHtML

[R59] 发 POST JSON
来源：http://3g.fktsv.cn/Article/details/gjskdodlj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.bbcook.cn/Article/details/gbkxbrdfc.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gresoumdg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/goytrywdy.sHtML

[R61] 磁盘占用
来源：http://blog.epnwcf.com/Article/details/gnhooctxj.sHtML

df -h;  du -sh *
来源：http://blog.fktsv.cn/Article/details/gpvydqzch.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdykkuluu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.vehdjk.com/Article/details/gsjuiijkd.sHtML

[R63] 内存与进程
来源：http://3g.tarul.cn/Article/details/gjcigspfz.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.tarul.cn/Article/details/gjfaohigb.sHtML

[R64] 结束进程
来源：http://www.m.share.epnwcf.com/Article/details/gkmmeoael.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.bbcook.cn/Article/details/gdjutgeub.sHtML

[R65] 查看端口占用
来源：http://m.share.sjlbkw.cn/Article/details/ghmyrlfyz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.tarul.cn/Article/details/gewvbisct.sHtML

[R66] 定时任务
来源：http://baike.epnwcf.com/Article/details/gmsilosaq.sHtML

crontab -e;  crontab -l
来源：http://baike.bbcook.cn/Article/details/gumggdydn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.tarul.cn/Article/details/gujdcjndb.sHtML

openssl rand -hex 16
来源：http://3g.bbcook.cn/Article/details/gbwosjyxb.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gkquunmpo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fktsv.cn/Article/details/gstzkdvfa.sHtML

[R69] 生成随机密码
来源：http://mobile.sjlbkw.cn/Article/details/ghyodobue.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.epnwcf.com/Article/details/gxipbzfao.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdgcipov.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fktsv.cn/Article/details/gtgozqmyk.sHtML

[R71] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/giigepjbq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.bbcook.cn/Article/details/gkxudbgkk.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gdplnowtc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gkpucawcy.sHtML

[R73] 分割大日志
来源：http://www.share.bbcook.cn/Article/details/gpljdawyk.sHtML

split -l 1000 big.log part_
来源：http://read.share.bbcook.cn/Article/details/gozgdefpl.sHtML

[R74] 批量重命名
来源：http://3g.sjlbkw.cn/Article/details/goqljmrcu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fktsv.cn/Article/details/glijgibon.sHtML

[R75] 导出环境变量
来源：http://blog.fktsv.cn/Article/details/gsmhsqnmv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.tarul.cn/Article/details/gwchhdcyx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gbeiqyxge.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.sjlbkw.cn/Article/details/geeqrkywl.sHtML

[R77] 读取用户输入
来源：http://mobile.fktsv.cn/Article/details/gkffbxjfx.sHtML

read -rp "请输入: " ans
来源：http://3g.yfazqb.com/Article/details/gholokwar.sHtML

[R78] 交互式菜单
来源：http://www.blog.fktsv.cn/Article/details/gqezlvtrg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.bbcook.cn/Article/details/gytrblafw.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/giizcqtby.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.vehdjk.com/Article/details/giebgnptn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.sjlbkw.cn/Article/details/gyoaaqsmg.sHtML

time ./run.sh
来源：http://www.m.share.fktsv.cn/Article/details/gkgnilzgz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnzsemagw.sHtML

S. C / C++ 专题
来源：http://blog.vehdjk.com/Article/details/glnrzigsd.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjlhuzdvt.sHtML

[S01] C：Hello World
来源：http://www.share.tarul.cn/Article/details/glckkbidy.sHtML

#include <stdio.h>
来源：http://read.share.sjlbkw.cn/Article/details/ghqythhbj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.bbcook.cn/Article/details/gfxsffaqe.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.sjlbkw.cn/Article/details/gayhwwwrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.bbcook.cn/Article/details/gvhwokjir.sHtML

[S03] C：读入整数
来源：http://m.share.fktsv.cn/Article/details/gqgkrkjrx.sHtML

int x; scanf("%d", &x);
来源：http://wap.epnwcf.com/Article/details/gchlnaxot.sHtML

[S04] C：字符串复制
来源：http://www.share.fktsv.cn/Article/details/gnrtqnedj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.bbcook.cn/Article/details/ggvzzgvxl.sHtML

[S05] C：字符串长度
来源：http://mobile.yfazqb.com/Article/details/ggfcqwtcq.sHtML

strlen(s)
来源：http://m.share.fktsv.cn/Article/details/gmaltvhsj.sHtML

[S06] C：字符串比较
来源：http://blog.epnwcf.com/Article/details/gyrmfvaqg.sHtML

strcmp(a, b) == 0
来源：http://read.share.sjlbkw.cn/Article/details/gnskvdejo.sHtML

[S07] C：数组遍历求和
来源：http://wap.epnwcf.com/Article/details/gjcapcsdk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fktsv.cn/Article/details/gwdsgudtv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.bbcook.cn/Article/details/gzbpfcnor.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fktsv.cn/Article/details/grwmocmpm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.tarul.cn/Article/details/gwrjpvpes.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.sjlbkw.cn/Article/details/guspbuhox.sHtML

[S10] C：指针与解引用
来源：http://3g.fktsv.cn/Article/details/gqbznjpbc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.bbcook.cn/Article/details/gybgvkwat.sHtML

[S11] C：逐行读文件
来源：http://baike.epnwcf.com/Article/details/gcwyzbwoj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.yfazqb.com/Article/details/gmpdedxdb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.tarul.cn/Article/details/gxsxmomyu.sHtML

fclose(f);
来源：http://blog.epnwcf.com/Article/details/gbbiklrnz.sHtML

[S12] C：写文件
来源：http://www.share.yfazqb.com/Article/details/gfxxbuctl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.sjlbkw.cn/Article/details/gkterlurc.sHtML

[S13] C：宏定义
来源：http://wap.vehdjk.com/Article/details/gxyvzqbzg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.yfazqb.com/Article/details/gzawczgea.sHtML

[S14] C：枚举
来源：http://www.m.share.yfazqb.com/Article/details/gfeemqkxf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.yfazqb.com/Article/details/grzifzyzv.sHtML

[S15] C：类型转换
来源：http://www.blog.epnwcf.com/Article/details/gbhpdalsh.sHtML

(double) a / b
来源：http://read.share.fktsv.cn/Article/details/ghvdlwubr.sHtML

[S16] C：位操作置位
来源：http://www.m.share.epnwcf.com/Article/details/gqgjfiont.sHtML

x |= (1 << 3);
来源：http://www.share.yfazqb.com/Article/details/gqztzwkjk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gvbtkgnbt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.sjlbkw.cn/Article/details/gsxtycpjz.sHtML

[S18] C：命令行参数
来源：http://mobile.yfazqb.com/Article/details/gwmkvghhp.sHtML

int main(int argc, char **argv)
来源：http://www.share.bbcook.cn/Article/details/gctwxjfcb.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/gjhagcpde.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/gosqnicop.sHtML

[S20] C：二分查找
来源：http://3g.fktsv.cn/Article/details/garapgjdp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gizfewrmc.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gzluiurdf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.vehdjk.com/Article/details/gznmhmrmp.sHtML

[S22] C：字符串转数字
来源：http://3g.sjlbkw.cn/Article/details/gvpysyayi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.epnwcf.com/Article/details/guqtwpmlc.sHtML

[S23] C：随机数
来源：http://www.share.bbcook.cn/Article/details/gqcmukzub.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.epnwcf.com/Article/details/grsxsneyf.sHtML

[S24] C：获取本地时间
来源：http://baike.fktsv.cn/Article/details/gteftldgc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.epnwcf.com/Article/details/godxrdhou.sHtML

[S25] C：内存拷贝
来源：http://3g.vehdjk.com/Article/details/gbwbcnkwb.sHtML

memcpy(dst, src, n);
来源：http://baike.epnwcf.com/Article/details/gyvexbfzl.sHtML

[S26] C：内存清零
来源：http://baike.yfazqb.com/Article/details/gyfznvorb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.sjlbkw.cn/Article/details/geejlhcgm.sHtML

[S27] C：定义常量
来源：http://m.share.epnwcf.com/Article/details/gzugxbgfk.sHtML

const double PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/geyojztrl.sHtML

[S28] C：静态变量
来源：http://wap.sjlbkw.cn/Article/details/gxcsfrhwt.sHtML

static int counter = 0;
来源：http://blog.bbcook.cn/Article/details/ggmwvqiro.sHtML

[S29] C：变参函数
来源：http://mobile.bbcook.cn/Article/details/givdhapxc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/gdfjdvlse.sHtML

[S30] C：头文件保护
来源：http://3g.vehdjk.com/Article/details/gypkfvojv.sHtML

#ifndef X_H
来源：http://blog.bbcook.cn/Article/details/gxhtgdwuu.sHtML

#define X_H
来源：http://www.blog.sjlbkw.cn/Article/details/gjgurmeqj.sHtML

#endif
来源：http://wap.bbcook.cn/Article/details/grrbptagk.sHtML

[S31] C++：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrlapbh.sHtML

#include <iostream>
来源：http://blog.yfazqb.com/Article/details/gauzykfsq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.yfazqb.com/Article/details/gktvagisd.sHtML

[S32] C++：字符串
来源：http://mobile.sjlbkw.cn/Article/details/gletaefuc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gpqqulitb.sHtML

[S33] C++：vector 增删
来源：http://read.share.epnwcf.com/Article/details/ggcdklmtc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.yfazqb.com/Article/details/gaqrpgtid.sHtML

[S34] C++：遍历 vector
来源：http://blog.epnwcf.com/Article/details/gcjcvpnel.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fktsv.cn/Article/details/gulqtbykh.sHtML

[S35] C++：map
来源：http://baike.yfazqb.com/Article/details/glxrvwzeh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gldsbbcve.sHtML

[S36] C++：unordered_map
来源：http://3g.epnwcf.com/Article/details/gttbbidla.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gjdpptubq.sHtML

[S37] C++：set
来源：http://read.share.bbcook.cn/Article/details/gqdlxszop.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.yfazqb.com/Article/details/gnuocjpdl.sHtML

[S38] C++：排序
来源：http://m.share.vehdjk.com/Article/details/gxebxidbe.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.sjlbkw.cn/Article/details/ghlfjrilg.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.yfazqb.com/Article/details/gpjdysowt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.bbcook.cn/Article/details/ghogxynyx.sHtML

[S40] C++：查找元素
来源：http://www.blog.tarul.cn/Article/details/gwiibxhfa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.sjlbkw.cn/Article/details/gzyfbbyfi.sHtML

[S41] C++：类与构造函数
来源：http://www.share.bbcook.cn/Article/details/gouyvduak.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.tarul.cn/Article/details/gswblkxnc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.yfazqb.com/Article/details/gmbxsxhvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.tarul.cn/Article/details/gpxmldcpd.sHtML

[S43] C++：智能指针
来源：http://3g.bbcook.cn/Article/details/gmwenxdau.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.bbcook.cn/Article/details/gowtmmklo.sHtML

[S44] C++：引用传参
来源：http://baike.bbcook.cn/Article/details/gwcwkqrjc.sHtML

void inc(int &x) { ++x; }
来源：http://3g.vehdjk.com/Article/details/gqiskeijf.sHtML

[S45] C++：lambda
来源：http://www.m.share.yfazqb.com/Article/details/gnthehvyb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.epnwcf.com/Article/details/ggbfazydm.sHtML

[S46] C++：函数模板
来源：http://wap.sjlbkw.cn/Article/details/gstugkzix.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.vehdjk.com/Article/details/gkiaeleso.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.epnwcf.com/Article/details/gnkfescfx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.vehdjk.com/Article/details/gatkryckw.sHtML

[S48] C++：逐行读文件
来源：http://wap.vehdjk.com/Article/details/gvtffyqqv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.tarul.cn/Article/details/gtpiqowhj.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.bbcook.cn/Article/details/gfvsvxkgz.sHtML

[S49] C++：写文件
来源：http://mobile.epnwcf.com/Article/details/gvtxybjbb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gvxqwzcxx.sHtML

[S50] C++：格式化数字
来源：http://read.share.vehdjk.com/Article/details/gluzuwjhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gwwbjtzgv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.tarul.cn/Article/details/gafsrntli.sHtML

static_cast<double>(a) / b
来源：http://blog.fktsv.cn/Article/details/gqmbhoezb.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.vehdjk.com/Article/details/gdrzieaiv.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.bbcook.cn/Article/details/gyecoirqs.sHtML

[S53] C++：移动语义
来源：http://mobile.yfazqb.com/Article/details/gyyismhhx.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.sjlbkw.cn/Article/details/gaajtfzje.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gwdtormnn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fktsv.cn/Article/details/gfxelkstj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.vehdjk.com/Article/details/ghogujeft.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.sjlbkw.cn/Article/details/gbulquvph.sHtML

[S56] C++：optional
来源：http://wap.yfazqb.com/Article/details/gcehxxknk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.epnwcf.com/Article/details/glgeplmtl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fktsv.cn/Article/details/gaorsfkbj.sHtML

constexpr int N = 10;
来源：http://read.share.sjlbkw.cn/Article/details/glhhkrcac.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/gbzipkfqb.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.bbcook.cn/Article/details/gwvlzlzzk.sHtML

[S59] C++：静态断言
来源：http://www.blog.sjlbkw.cn/Article/details/glaqpwbbs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/gkxcklfkf.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.tarul.cn/Article/details/gevssfrob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fktsv.cn/Article/details/gribteyvz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guyflbtjq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.yfazqb.com/Article/details/ghairhjax.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/giqfmmssa.sHtML

[T01] Kotlin：Hello World
来源：http://baike.vehdjk.com/Article/details/glpxkbzkk.sHtML

println("Hello")
来源：http://www.m.share.yfazqb.com/Article/details/gxbuyepub.sHtML

[T02] Kotlin：变量
来源：http://www.share.vehdjk.com/Article/details/gleasgvrj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fktsv.cn/Article/details/gauoblzqn.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.vehdjk.com/Article/details/gtioqgkgd.sHtML

"值: $b"
来源：http://baike.vehdjk.com/Article/details/gsbhkgwts.sHtML

[T04] Kotlin：空安全
来源：http://mobile.tarul.cn/Article/details/gvdubigkt.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fktsv.cn/Article/details/gqsbxhhnk.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.bbcook.cn/Article/details/gvvpfjunz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.tarul.cn/Article/details/gjivxwdzy.sHtML

[T06] Kotlin：集合映射
来源：http://baike.vehdjk.com/Article/details/gzycvtguh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gwdmmozmc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gkxwkolxt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.yfazqb.com/Article/details/guygpgahx.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fktsv.cn/Article/details/gmfaixyzr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.yfazqb.com/Article/details/gqaiimonj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.tarul.cn/Article/details/gxqkzvyph.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.yfazqb.com/Article/details/gtgbqygel.sHtML

[T10] Kotlin：默认参数
来源：http://baike.sjlbkw.cn/Article/details/gmuaagryx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.yfazqb.com/Article/details/gqfjaqqox.sHtML

[T11] Kotlin：协程
来源：http://baike.vehdjk.com/Article/details/gtzcjvibu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.tarul.cn/Article/details/gbtlszucn.sHtML

[T12] Kotlin：解构声明
来源：http://blog.epnwcf.com/Article/details/gdowmxlws.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.bbcook.cn/Article/details/gycodttal.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.yfazqb.com/Article/details/gvlpcxxyf.sHtML

val m = mapOf("a" to 1)
来源：http://wap.sjlbkw.cn/Article/details/ghrmjmnnk.sHtML

[T14] Kotlin：循环
来源：http://wap.sjlbkw.cn/Article/details/gfufarbel.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gphazqaei.sHtML

[T15] Kotlin：接口
来源：http://blog.fktsv.cn/Article/details/gcqkwiwji.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.epnwcf.com/Article/details/glancoeom.sHtML

[T16] Swift：Hello World
来源：http://read.share.fktsv.cn/Article/details/gybsosfkv.sHtML

print("Hello")
来源：http://read.share.vehdjk.com/Article/details/gkcumebjz.sHtML

[T17] Swift：变量与常量
来源：http://baike.bbcook.cn/Article/details/gmhxsiaxf.sHtML

var a = 1;  let b = 2
来源：http://3g.bbcook.cn/Article/details/gvssuhawz.sHtML

[T18] Swift：字符串插值
来源：http://3g.bbcook.cn/Article/details/giykcjsng.sHtML

"值: \(b)"
来源：http://read.share.epnwcf.com/Article/details/golsklsxo.sHtML

[T19] Swift：可选绑定
来源：http://baike.tarul.cn/Article/details/gzvsribmb.sHtML

if let n = opt { print(n) }
来源：http://blog.yfazqb.com/Article/details/gjasjflnc.sHtML

[T20] Swift：数组操作
来源：http://mobile.epnwcf.com/Article/details/gotqrdvzk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.yfazqb.com/Article/details/gmvvpctry.sHtML

[T21] Swift：遍历
来源：http://m.share.yfazqb.com/Article/details/gukixkumr.sHtML

for x in a { print(x) }
来源：http://www.m.share.epnwcf.com/Article/details/gaswaglky.sHtML

[T22] Swift：字典
来源：http://www.m.share.fktsv.cn/Article/details/gitqanqiy.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.tarul.cn/Article/details/gjewssbwm.sHtML

[T23] Swift：函数
来源：http://blog.tarul.cn/Article/details/guejleqbv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.sjlbkw.cn/Article/details/gfnqohmof.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gyhypbokq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.epnwcf.com/Article/details/gbuglruwv.sHtML

[T25] Swift：结构体
来源：http://m.share.yfazqb.com/Article/details/ghwouzqsi.sHtML

struct P { var x: Int }
来源：http://wap.sjlbkw.cn/Article/details/gvzjmuqfy.sHtML

[T26] Swift：类与重写
来源：http://www.blog.bbcook.cn/Article/details/getjqalor.sHtML

class A: Base { override func f() {} }
来源：http://baike.vehdjk.com/Article/details/gfadzmxgw.sHtML

[T27] Swift：错误处理
来源：http://3g.yfazqb.com/Article/details/gowmndjkc.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.vehdjk.com/Article/details/gehmkmrwi.sHtML

[T28] Swift：枚举
来源：http://read.share.fktsv.cn/Article/details/gcvgdhcws.sHtML

enum Color { case red, green }
来源：http://blog.epnwcf.com/Article/details/gxsrixwup.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.sjlbkw.cn/Article/details/groifaaxe.sHtML

guard let x = opt else { return }
来源：http://www.blog.yfazqb.com/Article/details/gtdhfhzvg.sHtML

[T30] Swift：协议
来源：http://3g.tarul.cn/Article/details/gqaglmtfh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.epnwcf.com/Article/details/gunexurum.sHtML

[T31] Lua：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/glbnzsynr.sHtML

print("Hello")
来源：http://www.share.bbcook.cn/Article/details/gvyxwnwwl.sHtML

[T32] Lua：局部变量
来源：http://3g.epnwcf.com/Article/details/gacbfivll.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gtcuzjtes.sHtML

[T33] Lua：表（数组）
来源：http://3g.sjlbkw.cn/Article/details/gehvnamvf.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.tarul.cn/Article/details/grshakaqv.sHtML

[T34] Lua：遍历表
来源：http://baike.fktsv.cn/Article/details/gmfiwuzsx.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.epnwcf.com/Article/details/geggfqtgi.sHtML

[T35] Lua：字典表
来源：http://m.share.vehdjk.com/Article/details/gfoljgfpz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.tarul.cn/Article/details/gdxguhxjr.sHtML

[T36] Lua：函数
来源：http://blog.tarul.cn/Article/details/gzxgkwqwu.sHtML

function add(a, b) return a + b end
来源：http://read.share.fktsv.cn/Article/details/goekafgrx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.bbcook.cn/Article/details/gtdfsqzbh.sHtML

"a" .. "b"
来源：http://m.share.epnwcf.com/Article/details/glggrtwls.sHtML

[T38] Lua：条件
来源：http://www.m.share.fktsv.cn/Article/details/gxqyofiie.sHtML

if x > 0 then print("正") end
来源：http://m.share.epnwcf.com/Article/details/gpzfjleot.sHtML

[T39] Lua：模式匹配
来源：http://www.share.epnwcf.com/Article/details/gbakirxas.sHtML

string.find(s, "%d+")
来源：http://3g.vehdjk.com/Article/details/gmvthrgbx.sHtML

[T40] Lua：元表
来源：http://3g.yfazqb.com/Article/details/gxngexhyw.sHtML

setmetatable({}, { __index = base })
来源：http://blog.yfazqb.com/Article/details/gwkcmjyvy.sHtML

[T41] Perl：Hello World
来源：http://blog.bbcook.cn/Article/details/gvkfgqggs.sHtML

print "Hello\n";
来源：http://blog.vehdjk.com/Article/details/gxvtswhjv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.epnwcf.com/Article/details/gaakikhjo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.epnwcf.com/Article/details/gxnyccepx.sHtML

[T43] Perl：字符串插值
来源：http://www.share.tarul.cn/Article/details/gduwcijal.sHtML

"值: $a"
来源：http://mobile.epnwcf.com/Article/details/ghvbdutpv.sHtML

[T44] Perl：条件
来源：http://m.share.epnwcf.com/Article/details/glpqjpjal.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.yfazqb.com/Article/details/gsgkvyxth.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.yfazqb.com/Article/details/gbhmkqvav.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.sjlbkw.cn/Article/details/gsgnkirgk.sHtML

[T46] Perl：哈希操作
来源：http://blog.yfazqb.com/Article/details/gxvrcvqmu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.sjlbkw.cn/Article/details/gbxdqgqpn.sHtML

[T47] Perl：正则捕获
来源：http://mobile.yfazqb.com/Article/details/gweexfjun.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gwtzvjbmr.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.epnwcf.com/Article/details/gsqfpimra.sHtML

$s =~ s/old/new/g;
来源：http://3g.yfazqb.com/Article/details/gmqwvksuz.sHtML

[T49] Perl：函数
来源：http://3g.fktsv.cn/Article/details/gzmwfljfs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.yfazqb.com/Article/details/gikmhaoak.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gwedhaidf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.bbcook.cn/Article/details/gpictlazv.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://3g.epnwcf.com/Article/details/geayegsic.sHtML

[T51] Scala：Hello World
来源：http://read.share.bbcook.cn/Article/details/gsqjqylux.sHtML

println("Hello")
来源：http://m.share.tarul.cn/Article/details/gynzmavqp.sHtML

[T52] Scala：变量
来源：http://www.blog.sjlbkw.cn/Article/details/gldriupvv.sHtML

val a = 1;  var b = 2
来源：http://blog.sjlbkw.cn/Article/details/ggszekctq.sHtML

[T53] Scala：字符串插值
来源：http://baike.fktsv.cn/Article/details/gwmseekdg.sHtML

s"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/gomkatems.sHtML

[T54] Scala：集合映射
来源：http://blog.sjlbkw.cn/Article/details/giazfacvb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/glnrhpafj.sHtML

[T55] Scala：集合过滤
来源：http://mobile.bbcook.cn/Article/details/gcxtvejmb.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.yfazqb.com/Article/details/gsttjslpn.sHtML

[T56] Scala：样例类
来源：http://www.share.fktsv.cn/Article/details/gdtwxsqpo.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gihklayiy.sHtML

[T57] Scala：模式匹配
来源：http://www.share.yfazqb.com/Article/details/gbpandkdw.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/ghuwncmla.sHtML

[T58] Scala：函数定义
来源：http://3g.bbcook.cn/Article/details/gllvuasjs.sHtML


<!-- 参考信息 -->