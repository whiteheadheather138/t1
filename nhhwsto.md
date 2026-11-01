代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.tarul.cn/Article/details/grjsfwrgz.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gwhdjdxof.sHtML

scp file user@host:/path/
来源：http://baike.fktsv.cn/Article/details/gexhawcct.sHtML

[R57] 远程执行命令
来源：http://3g.bbcook.cn/Article/details/gyrvwunhw.sHtML

ssh user@host 'uptime'
来源：http://wap.bbcook.cn/Article/details/gjlyxawzl.sHtML

[R58] 下载文件
来源：http://read.share.yfazqb.com/Article/details/gkurbreyk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.yfazqb.com/Article/details/gczwgiisg.sHtML

[R59] 发 POST JSON
来源：http://3g.epnwcf.com/Article/details/gvbchsjjr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.epnwcf.com/Article/details/gwabteubs.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gitvaosvq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.sjlbkw.cn/Article/details/gjsllrnzd.sHtML

[R61] 磁盘占用
来源：http://wap.epnwcf.com/Article/details/gaksbvupp.sHtML

df -h;  du -sh *
来源：http://3g.yfazqb.com/Article/details/gzefhqmms.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fktsv.cn/Article/details/gcprtsapi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.tarul.cn/Article/details/gtwawwgvy.sHtML

[R63] 内存与进程
来源：http://read.share.sjlbkw.cn/Article/details/givxqufws.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.sjlbkw.cn/Article/details/gnuebfxzb.sHtML

[R64] 结束进程
来源：http://m.share.yfazqb.com/Article/details/gimhkcgqm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.vehdjk.com/Article/details/gqxkbcpil.sHtML

[R65] 查看端口占用
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqeeqydr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.yfazqb.com/Article/details/gnkghzvdz.sHtML

[R66] 定时任务
来源：http://www.blog.yfazqb.com/Article/details/gzbqxbfes.sHtML

crontab -e;  crontab -l
来源：http://www.blog.sjlbkw.cn/Article/details/gthfcalwm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.vehdjk.com/Article/details/gbqklnrvy.sHtML

openssl rand -hex 16
来源：http://www.share.tarul.cn/Article/details/gbfmwiesm.sHtML

[R68] 计算文件校验值
来源：http://read.share.epnwcf.com/Article/details/gsfqhhjda.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gmlpauqoz.sHtML

[R69] 生成随机密码
来源：http://3g.fktsv.cn/Article/details/gruiwccvm.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.bbcook.cn/Article/details/galkgqjtm.sHtML

[R70] 时间戳与互转
来源：http://wap.sjlbkw.cn/Article/details/gegrdwflp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.yfazqb.com/Article/details/goxiphoyr.sHtML

[R71] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gfzwgjjdf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.epnwcf.com/Article/details/gdwofjjiw.sHtML

[R72] 等待端口就绪
来源：http://3g.epnwcf.com/Article/details/gmxtaojqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gwxaqbjol.sHtML

[R73] 分割大日志
来源：http://www.share.tarul.cn/Article/details/gpymoxlsk.sHtML

split -l 1000 big.log part_
来源：http://wap.sjlbkw.cn/Article/details/gkkpmnpgi.sHtML

[R74] 批量重命名
来源：http://blog.tarul.cn/Article/details/gkfugofhw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.tarul.cn/Article/details/giutmhrep.sHtML

[R75] 导出环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gchumbqjc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.vehdjk.com/Article/details/gvasrouqg.sHtML

[R76] 使用临时文件
来源：http://3g.yfazqb.com/Article/details/glghynjhr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gylmqrpqv.sHtML

[R77] 读取用户输入
来源：http://www.blog.yfazqb.com/Article/details/gnasewksn.sHtML

read -rp "请输入: " ans
来源：http://blog.epnwcf.com/Article/details/gkvdmdycz.sHtML

[R78] 交互式菜单
来源：http://baike.epnwcf.com/Article/details/gixulkpfy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.sjlbkw.cn/Article/details/gchiclfjo.sHtML

[R79] 解析命令行选项
来源：http://read.share.epnwcf.com/Article/details/gvbdhhygk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.yfazqb.com/Article/details/grqmtueqz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.bbcook.cn/Article/details/gzroauyae.sHtML

time ./run.sh
来源：http://www.share.epnwcf.com/Article/details/guypbryve.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpgakjpbg.sHtML

S. C / C++ 专题
来源：http://baike.epnwcf.com/Article/details/gnmoikrre.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcgxrarqc.sHtML

[S01] C：Hello World
来源：http://www.share.bbcook.cn/Article/details/gkgfpwjyl.sHtML

#include <stdio.h>
来源：http://3g.sjlbkw.cn/Article/details/gvrjwpjwe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.tarul.cn/Article/details/gmtygjcqi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fktsv.cn/Article/details/gzzmzznim.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fktsv.cn/Article/details/gjvtunltw.sHtML

[S03] C：读入整数
来源：http://blog.bbcook.cn/Article/details/gchvdmjdk.sHtML

int x; scanf("%d", &x);
来源：http://read.share.yfazqb.com/Article/details/gvubweowx.sHtML

[S04] C：字符串复制
来源：http://mobile.tarul.cn/Article/details/ghupkpkou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.tarul.cn/Article/details/gyuvnlmlu.sHtML

[S05] C：字符串长度
来源：http://read.share.epnwcf.com/Article/details/ggpmdtvds.sHtML

strlen(s)
来源：http://m.share.bbcook.cn/Article/details/gqprhtbyl.sHtML

[S06] C：字符串比较
来源：http://3g.vehdjk.com/Article/details/gpqvuvqzx.sHtML

strcmp(a, b) == 0
来源：http://wap.bbcook.cn/Article/details/gmjqaeaap.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fktsv.cn/Article/details/geszqfwip.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.bbcook.cn/Article/details/gcpwqyhnv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fktsv.cn/Article/details/gbzwgdwur.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fktsv.cn/Article/details/gnatglukp.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.epnwcf.com/Article/details/gvbspofrb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/gjydsgqwg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.bbcook.cn/Article/details/gefgxggsk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.yfazqb.com/Article/details/gntoxgbqu.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gsnzgnesk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.bbcook.cn/Article/details/gghtrffjs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.bbcook.cn/Article/details/gbtsctcos.sHtML

fclose(f);
来源：http://m.share.epnwcf.com/Article/details/gzmpactkz.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gohrgzjgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.yfazqb.com/Article/details/gbhzfuggd.sHtML

[S13] C：宏定义
来源：http://wap.epnwcf.com/Article/details/grvsvvgdz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.bbcook.cn/Article/details/gvrkrzgas.sHtML

[S14] C：枚举
来源：http://baike.fktsv.cn/Article/details/gdnnsnmue.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.epnwcf.com/Article/details/glwhndhdd.sHtML

[S15] C：类型转换
来源：http://m.share.tarul.cn/Article/details/gqsnfarkd.sHtML

(double) a / b
来源：http://read.share.tarul.cn/Article/details/gwjsgwyhd.sHtML

[S16] C：位操作置位
来源：http://m.share.tarul.cn/Article/details/gvzczexhi.sHtML

x |= (1 << 3);
来源：http://blog.yfazqb.com/Article/details/gsbdpcrrl.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gzvwhgwlp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.yfazqb.com/Article/details/gqtrbnosx.sHtML

[S18] C：命令行参数
来源：http://wap.tarul.cn/Article/details/ggntiwffo.sHtML

int main(int argc, char **argv)
来源：http://read.share.vehdjk.com/Article/details/guxiwslsn.sHtML

[S19] C：快速排序
来源：http://read.share.bbcook.cn/Article/details/gxynvvzbw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fktsv.cn/Article/details/gqayklvzp.sHtML

[S20] C：二分查找
来源：http://mobile.bbcook.cn/Article/details/gcuyhznqi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.vehdjk.com/Article/details/gitsgnbdc.sHtML

[S21] C：字符类别判断
来源：http://www.share.fktsv.cn/Article/details/gelsthhbv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.yfazqb.com/Article/details/gikwopykl.sHtML

[S22] C：字符串转数字
来源：http://wap.fktsv.cn/Article/details/gepeocked.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.sjlbkw.cn/Article/details/ggizydiht.sHtML

[S23] C：随机数
来源：http://baike.fktsv.cn/Article/details/gjbzujqdo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.vehdjk.com/Article/details/gdxzfpntv.sHtML

[S24] C：获取本地时间
来源：http://read.share.epnwcf.com/Article/details/gpkazrzrj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.vehdjk.com/Article/details/gqtpihdoh.sHtML

[S25] C：内存拷贝
来源：http://read.share.sjlbkw.cn/Article/details/gqokczvjb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.bbcook.cn/Article/details/gvhhrryom.sHtML

[S26] C：内存清零
来源：http://blog.bbcook.cn/Article/details/gtojgmely.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.vehdjk.com/Article/details/gslkqbucj.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/golplyzie.sHtML

const double PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/gixgedxoe.sHtML

[S28] C：静态变量
来源：http://wap.vehdjk.com/Article/details/girahpacu.sHtML

static int counter = 0;
来源：http://read.share.bbcook.cn/Article/details/ggarunddk.sHtML

[S29] C：变参函数
来源：http://www.m.share.fktsv.cn/Article/details/gubdfsnhg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.bbcook.cn/Article/details/galgurzch.sHtML

[S30] C：头文件保护
来源：http://blog.sjlbkw.cn/Article/details/gzewzftxf.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/geyfssuys.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gbpszgtfr.sHtML

#endif
来源：http://www.share.fktsv.cn/Article/details/gikeddqik.sHtML

[S31] C++：Hello World
来源：http://www.share.fktsv.cn/Article/details/gczzjhwyi.sHtML

#include <iostream>
来源：http://mobile.sjlbkw.cn/Article/details/gbmhafwpc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fktsv.cn/Article/details/grpytfscj.sHtML

[S32] C++：字符串
来源：http://wap.sjlbkw.cn/Article/details/gdhggogsj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.yfazqb.com/Article/details/gsntjwwjw.sHtML

[S33] C++：vector 增删
来源：http://3g.fktsv.cn/Article/details/gvayjwquu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.bbcook.cn/Article/details/gvchnotst.sHtML

[S34] C++：遍历 vector
来源：http://www.share.tarul.cn/Article/details/gmricujgl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.epnwcf.com/Article/details/gpafkwjjf.sHtML

[S35] C++：map
来源：http://www.blog.sjlbkw.cn/Article/details/getzueose.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.vehdjk.com/Article/details/gxtccwpbo.sHtML

[S36] C++：unordered_map
来源：http://www.share.vehdjk.com/Article/details/gamqoqndu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.epnwcf.com/Article/details/grdqfovjn.sHtML

[S37] C++：set
来源：http://www.blog.sjlbkw.cn/Article/details/ghfgrqkky.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.yfazqb.com/Article/details/gkrjkqqhz.sHtML

[S38] C++：排序
来源：http://baike.yfazqb.com/Article/details/golsgclbh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.sjlbkw.cn/Article/details/gkhgcirva.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fktsv.cn/Article/details/gqeqddhrw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.vehdjk.com/Article/details/gfixoxmhb.sHtML

[S40] C++：查找元素
来源：http://www.blog.epnwcf.com/Article/details/gtubqkkvr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.tarul.cn/Article/details/gixxopava.sHtML

[S41] C++：类与构造函数
来源：http://baike.tarul.cn/Article/details/guiojwmjs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.epnwcf.com/Article/details/gelxhmrua.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.vehdjk.com/Article/details/gfonkoxpc.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.tarul.cn/Article/details/gvbkloyzr.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gerqrzfgx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.vehdjk.com/Article/details/gnycwxjqf.sHtML

[S44] C++：引用传参
来源：http://wap.vehdjk.com/Article/details/gnxktvmno.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fktsv.cn/Article/details/gafnkttom.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/gmagwikbl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fktsv.cn/Article/details/gkgjilqai.sHtML

[S46] C++：函数模板
来源：http://mobile.tarul.cn/Article/details/gulfbscty.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.yfazqb.com/Article/details/gkbgvcdxp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.yfazqb.com/Article/details/gvewtcnif.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.tarul.cn/Article/details/gityikfcw.sHtML

[S48] C++：逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gxctahoer.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.tarul.cn/Article/details/gxdyewcnu.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.yfazqb.com/Article/details/gitjbfijn.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gtknjddky.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.epnwcf.com/Article/details/ghwiglwzr.sHtML

[S50] C++：格式化数字
来源：http://www.share.yfazqb.com/Article/details/gvtxjepoo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.tarul.cn/Article/details/gcxhhdkte.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fktsv.cn/Article/details/guhcnfgpr.sHtML

static_cast<double>(a) / b
来源：http://3g.tarul.cn/Article/details/gwniijgct.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.vehdjk.com/Article/details/glsxmrvel.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.yfazqb.com/Article/details/gxahhotyh.sHtML

[S53] C++：移动语义
来源：http://www.blog.bbcook.cn/Article/details/grippsihq.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.sjlbkw.cn/Article/details/gwwvslwke.sHtML

[S54] C++：异常处理
来源：http://mobile.vehdjk.com/Article/details/goigvlijt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fktsv.cn/Article/details/gcfkxtdnw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.yfazqb.com/Article/details/gqwnmrcws.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fktsv.cn/Article/details/gjfzctgii.sHtML

[S56] C++：optional
来源：http://mobile.tarul.cn/Article/details/gvzxxsypu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.yfazqb.com/Article/details/gneukobcz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.bbcook.cn/Article/details/gjlnzsjuy.sHtML

constexpr int N = 10;
来源：http://wap.vehdjk.com/Article/details/gauqwpdwf.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/gerreuaqe.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.yfazqb.com/Article/details/glgqayrmj.sHtML

[S59] C++：静态断言
来源：http://m.share.bbcook.cn/Article/details/gkhcjbkha.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fktsv.cn/Article/details/gxcyxebil.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.vehdjk.com/Article/details/garthqyvl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.bbcook.cn/Article/details/grpdhcoiu.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghnlyqlth.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gvmzelkiu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gfzaoknhk.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.yfazqb.com/Article/details/gclklcfbg.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gqpadfozf.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.epnwcf.com/Article/details/gfatvptna.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.yfazqb.com/Article/details/gaemydczk.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.yfazqb.com/Article/details/gveboztpz.sHtML

"值: $b"
来源：http://blog.fktsv.cn/Article/details/gvhjcuxtj.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.bbcook.cn/Article/details/ghwlrffmt.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gmrruzdny.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/gvyoytzdm.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.tarul.cn/Article/details/gsaqslsqu.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fktsv.cn/Article/details/gxatwgmko.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.tarul.cn/Article/details/gbvlckogp.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.tarul.cn/Article/details/gzfldtrww.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.bbcook.cn/Article/details/gpjkxvnao.sHtML

[T08] Kotlin：数据类
来源：http://baike.tarul.cn/Article/details/govqgtmxe.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.tarul.cn/Article/details/gfpthkzhw.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.yfazqb.com/Article/details/gdxpoymcg.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fktsv.cn/Article/details/gwyqcsuqi.sHtML

[T10] Kotlin：默认参数
来源：http://blog.yfazqb.com/Article/details/gaxyfwuen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fktsv.cn/Article/details/glprysisu.sHtML

[T11] Kotlin：协程
来源：http://mobile.fktsv.cn/Article/details/gervwxzqf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.bbcook.cn/Article/details/gkurxhgge.sHtML

[T12] Kotlin：解构声明
来源：http://wap.bbcook.cn/Article/details/gpdmffatn.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.tarul.cn/Article/details/guufzwdst.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.bbcook.cn/Article/details/gahlyldpk.sHtML

val m = mapOf("a" to 1)
来源：http://3g.tarul.cn/Article/details/gamuvwmtz.sHtML

[T14] Kotlin：循环
来源：http://wap.tarul.cn/Article/details/gxljmvxeh.sHtML

for (i in 1..10) println(i)
来源：http://blog.tarul.cn/Article/details/gaccoiixn.sHtML

[T15] Kotlin：接口
来源：http://www.share.bbcook.cn/Article/details/gcjhxnutk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.bbcook.cn/Article/details/gbvtncenh.sHtML

[T16] Swift：Hello World
来源：http://blog.yfazqb.com/Article/details/gzdbeqchl.sHtML

print("Hello")
来源：http://www.blog.yfazqb.com/Article/details/ghdrgrcou.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.vehdjk.com/Article/details/gilzefvlk.sHtML

var a = 1;  let b = 2
来源：http://www.share.fktsv.cn/Article/details/gnvlhwmvg.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gqgwpxelu.sHtML

"值: \(b)"
来源：http://read.share.bbcook.cn/Article/details/gpcjmkrnr.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.vehdjk.com/Article/details/gvfbfkrdq.sHtML

if let n = opt { print(n) }
来源：http://read.share.sjlbkw.cn/Article/details/gmhrnhbja.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.vehdjk.com/Article/details/gjwinbciz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.sjlbkw.cn/Article/details/gfoqkcmai.sHtML

[T21] Swift：遍历
来源：http://wap.yfazqb.com/Article/details/grzabkalr.sHtML

for x in a { print(x) }
来源：http://mobile.tarul.cn/Article/details/ggwlwsdzs.sHtML

[T22] Swift：字典
来源：http://baike.fktsv.cn/Article/details/gewixqiqz.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fktsv.cn/Article/details/gnviwnvuv.sHtML

[T23] Swift：函数
来源：http://blog.bbcook.cn/Article/details/glnzdogcu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.yfazqb.com/Article/details/gtkeqchej.sHtML

[T24] Swift：闭包
来源：http://mobile.tarul.cn/Article/details/gllzfywqc.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/givrlueah.sHtML

[T25] Swift：结构体
来源：http://www.blog.yfazqb.com/Article/details/gijjeyoqj.sHtML

struct P { var x: Int }
来源：http://blog.sjlbkw.cn/Article/details/geovdnfnm.sHtML

[T26] Swift：类与重写
来源：http://3g.fktsv.cn/Article/details/gytwfaoos.sHtML

class A: Base { override func f() {} }
来源：http://m.share.epnwcf.com/Article/details/gexljkwbs.sHtML

[T27] Swift：错误处理
来源：http://wap.fktsv.cn/Article/details/gnmolsvcx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fktsv.cn/Article/details/gilmpxnwv.sHtML

[T28] Swift：枚举
来源：http://www.blog.fktsv.cn/Article/details/gyqvsbsuz.sHtML

enum Color { case red, green }
来源：http://www.share.tarul.cn/Article/details/gbpjjxjns.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.epnwcf.com/Article/details/gettelwxm.sHtML

guard let x = opt else { return }
来源：http://baike.fktsv.cn/Article/details/ggiajqtgq.sHtML

[T30] Swift：协议
来源：http://wap.bbcook.cn/Article/details/gqvoldbsz.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.sjlbkw.cn/Article/details/grwygytto.sHtML

[T31] Lua：Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gkgzxtmgl.sHtML

print("Hello")
来源：http://mobile.sjlbkw.cn/Article/details/glevnzbvh.sHtML

[T32] Lua：局部变量
来源：http://www.blog.sjlbkw.cn/Article/details/gtxiffdvs.sHtML

local a = 1
来源：http://3g.tarul.cn/Article/details/gtdpkqscn.sHtML

[T33] Lua：表（数组）
来源：http://baike.epnwcf.com/Article/details/gsskuxudn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/gdgbrhcig.sHtML

[T34] Lua：遍历表
来源：http://3g.epnwcf.com/Article/details/gihnbrjil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.epnwcf.com/Article/details/guumezvwm.sHtML

[T35] Lua：字典表
来源：http://baike.epnwcf.com/Article/details/gxgyqlrvo.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.yfazqb.com/Article/details/gmiaeqqvl.sHtML

[T36] Lua：函数
来源：http://www.m.share.yfazqb.com/Article/details/gvyobmhnq.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gtexmccmm.sHtML

[T37] Lua：字符串拼接
来源：http://blog.tarul.cn/Article/details/gmfxgtvpp.sHtML

"a" .. "b"
来源：http://www.m.share.epnwcf.com/Article/details/ghfxlregr.sHtML

[T38] Lua：条件
来源：http://m.share.sjlbkw.cn/Article/details/ggmldoayi.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.vehdjk.com/Article/details/gerxurilc.sHtML

[T39] Lua：模式匹配
来源：http://www.share.vehdjk.com/Article/details/gdzcfndhq.sHtML

string.find(s, "%d+")
来源：http://www.blog.tarul.cn/Article/details/gksryuhtj.sHtML

[T40] Lua：元表
来源：http://www.m.share.bbcook.cn/Article/details/gkpysefff.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gemuaraxo.sHtML

[T41] Perl：Hello World
来源：http://m.share.bbcook.cn/Article/details/gpksrmxht.sHtML

print "Hello\n";
来源：http://blog.yfazqb.com/Article/details/gezgpzogg.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/gwaxjrrnr.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.vehdjk.com/Article/details/geyxqtcbp.sHtML

[T43] Perl：字符串插值
来源：http://3g.fktsv.cn/Article/details/gpuvotfwm.sHtML

"值: $a"
来源：http://mobile.bbcook.cn/Article/details/gijrnvatl.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gnrzvamtz.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.tarul.cn/Article/details/gefdgvrpx.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gxxqvauya.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.tarul.cn/Article/details/gyhnudquq.sHtML

[T46] Perl：哈希操作
来源：http://blog.fktsv.cn/Article/details/gjkdhlbmj.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.bbcook.cn/Article/details/gntjlklpq.sHtML

[T47] Perl：正则捕获
来源：http://wap.fktsv.cn/Article/details/gixrhqwgw.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.sjlbkw.cn/Article/details/gkjzbtkhq.sHtML

[T48] Perl：正则替换
来源：http://3g.vehdjk.com/Article/details/gkfzcggnu.sHtML

$s =~ s/old/new/g;
来源：http://wap.fktsv.cn/Article/details/gleptcjll.sHtML

[T49] Perl：函数
来源：http://wap.tarul.cn/Article/details/ggnzfctlu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fktsv.cn/Article/details/gcgerenwr.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/ggidsfdut.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fktsv.cn/Article/details/gkjaalecl.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.tarul.cn/Article/details/glrraqcud.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gkhhvnopy.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/gyajiqgqq.sHtML

[T52] Scala：变量
来源：http://www.m.share.epnwcf.com/Article/details/gmnbgcqtk.sHtML

val a = 1;  var b = 2
来源：http://www.blog.sjlbkw.cn/Article/details/gljkkqykg.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.vehdjk.com/Article/details/glwqjnzbp.sHtML

s"值: $b"
来源：http://m.share.vehdjk.com/Article/details/geihxfrhd.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.tarul.cn/Article/details/gswjnkqah.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxptvvcc.sHtML

[T55] Scala：集合过滤
来源：http://www.share.bbcook.cn/Article/details/gbaepyenf.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gqvyvzako.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/ghtmniepn.sHtML

case class User(name: String, age: Int)
来源：http://m.share.tarul.cn/Article/details/gpkelganx.sHtML

[T57] Scala：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gsgczosoa.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gncahtapz.sHtML

[T58] Scala：函数定义
来源：http://read.share.epnwcf.com/Article/details/gzwqcwuzt.sHtML


<!-- 参考信息 -->