代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.epnwcf.com/Article/details/gtktsgfgw.sHtML

[R56] 远程拷贝
来源：http://www.blog.fktsv.cn/Article/details/guaoynrkn.sHtML

scp file user@host:/path/
来源：http://baike.tarul.cn/Article/details/gplluzneg.sHtML

[R57] 远程执行命令
来源：http://m.share.sjlbkw.cn/Article/details/geuamzwri.sHtML

ssh user@host 'uptime'
来源：http://m.share.vehdjk.com/Article/details/gotbvqqdw.sHtML

[R58] 下载文件
来源：http://m.share.vehdjk.com/Article/details/goukjjewo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.epnwcf.com/Article/details/gzkugedjo.sHtML

[R59] 发 POST JSON
来源：http://3g.tarul.cn/Article/details/ghgehpdpp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.tarul.cn/Article/details/gmwctfftp.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gvwfpwmvj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.sjlbkw.cn/Article/details/gcsslfitr.sHtML

[R61] 磁盘占用
来源：http://m.share.vehdjk.com/Article/details/gqygvxjkg.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gcowwjqnw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fktsv.cn/Article/details/gqmykzidl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fktsv.cn/Article/details/gklybjkxm.sHtML

[R63] 内存与进程
来源：http://baike.fktsv.cn/Article/details/gluczwhkq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.tarul.cn/Article/details/gtwwdoydv.sHtML

[R64] 结束进程
来源：http://www.blog.tarul.cn/Article/details/gxyxkkapx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhsfvbiq.sHtML

[R65] 查看端口占用
来源：http://blog.fktsv.cn/Article/details/gkfjgpsjy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.tarul.cn/Article/details/ghhcbprpb.sHtML

[R66] 定时任务
来源：http://www.m.share.sjlbkw.cn/Article/details/goahojfaj.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gjohrdsls.sHtML

[R67] 生成随机十六进制串
来源：http://3g.epnwcf.com/Article/details/gptafyhug.sHtML

openssl rand -hex 16
来源：http://m.share.tarul.cn/Article/details/gnllzowjc.sHtML

[R68] 计算文件校验值
来源：http://read.share.bbcook.cn/Article/details/gcmahltpo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.yfazqb.com/Article/details/gatkrjyze.sHtML

[R69] 生成随机密码
来源：http://3g.sjlbkw.cn/Article/details/gkiteploa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.sjlbkw.cn/Article/details/gadlgisej.sHtML

[R70] 时间戳与互转
来源：http://www.share.vehdjk.com/Article/details/gnbtsrqpq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.bbcook.cn/Article/details/gfkirlzxj.sHtML

[R71] 日期格式化
来源：http://read.share.epnwcf.com/Article/details/ggjplnzwz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gwpucqfif.sHtML

[R72] 等待端口就绪
来源：http://blog.sjlbkw.cn/Article/details/gganfjwep.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.vehdjk.com/Article/details/gxezftdrj.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/gmubbhqog.sHtML

split -l 1000 big.log part_
来源：http://mobile.sjlbkw.cn/Article/details/gflfdkncx.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gaqmzptsf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.yfazqb.com/Article/details/gywimjwdm.sHtML

[R75] 导出环境变量
来源：http://wap.sjlbkw.cn/Article/details/gvxihrjqo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.epnwcf.com/Article/details/gttvibklg.sHtML

[R76] 使用临时文件
来源：http://3g.tarul.cn/Article/details/gbfisfxcu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/gjlzcwgrh.sHtML

[R77] 读取用户输入
来源：http://www.share.bbcook.cn/Article/details/giobapqrx.sHtML

read -rp "请输入: " ans
来源：http://blog.vehdjk.com/Article/details/gmsgjfdjk.sHtML

[R78] 交互式菜单
来源：http://wap.fktsv.cn/Article/details/gjrtnmoiy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.epnwcf.com/Article/details/gjqremanx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fktsv.cn/Article/details/gqgferhou.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fktsv.cn/Article/details/gkrzcurjh.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.yfazqb.com/Article/details/goyadlrmz.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/glwcitoxj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggzuxxdsn.sHtML

S. C / C++ 专题
来源：http://m.share.tarul.cn/Article/details/gaqicmktl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnsnqgifd.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gjgtovhat.sHtML

#include <stdio.h>
来源：http://m.share.vehdjk.com/Article/details/gagplhqss.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fktsv.cn/Article/details/gnwvcuymb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.epnwcf.com/Article/details/gytnyttsa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.vehdjk.com/Article/details/gsdzxczbo.sHtML

[S03] C：读入整数
来源：http://www.m.share.yfazqb.com/Article/details/gyymdagtc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.epnwcf.com/Article/details/gzepuipet.sHtML

[S04] C：字符串复制
来源：http://3g.fktsv.cn/Article/details/gpeqorigp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.yfazqb.com/Article/details/ggylgzvab.sHtML

[S05] C：字符串长度
来源：http://blog.sjlbkw.cn/Article/details/gscjukgub.sHtML

strlen(s)
来源：http://m.share.epnwcf.com/Article/details/gzqrnpayl.sHtML

[S06] C：字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gqxcbebpd.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/gqaysnrdp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fktsv.cn/Article/details/gtvmgyvtr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gtzxsebck.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fktsv.cn/Article/details/gtmhbmqek.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.vehdjk.com/Article/details/gugvltjpn.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/gfosuwtwj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.tarul.cn/Article/details/ghnfjhfzs.sHtML

[S10] C：指针与解引用
来源：http://read.share.epnwcf.com/Article/details/goxthhkkk.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gklyzvhhy.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gnnkosnah.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.sjlbkw.cn/Article/details/gvvmvyjcv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.sjlbkw.cn/Article/details/gnyzclsef.sHtML

fclose(f);
来源：http://read.share.yfazqb.com/Article/details/gplfgvuhl.sHtML

[S12] C：写文件
来源：http://www.m.share.fktsv.cn/Article/details/genxkkdwg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.vehdjk.com/Article/details/gdojxemcb.sHtML

[S13] C：宏定义
来源：http://www.m.share.bbcook.cn/Article/details/goufqkjkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.bbcook.cn/Article/details/gymikkfir.sHtML

[S14] C：枚举
来源：http://www.share.tarul.cn/Article/details/gwmqhvovf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.vehdjk.com/Article/details/gufqevfnk.sHtML

[S15] C：类型转换
来源：http://baike.sjlbkw.cn/Article/details/gvktvuvmn.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/gwwqnnzfv.sHtML

[S16] C：位操作置位
来源：http://3g.epnwcf.com/Article/details/gzekfgmvn.sHtML

x |= (1 << 3);
来源：http://blog.epnwcf.com/Article/details/gbawgcyub.sHtML

[S17] C：安全拼接字符串
来源：http://baike.yfazqb.com/Article/details/giiqtfbzf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fktsv.cn/Article/details/gdvqfjthe.sHtML

[S18] C：命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gvvfiahag.sHtML

int main(int argc, char **argv)
来源：http://m.share.epnwcf.com/Article/details/gykwivfvk.sHtML

[S19] C：快速排序
来源：http://baike.vehdjk.com/Article/details/gvdgmzmmr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.epnwcf.com/Article/details/glvdeohac.sHtML

[S20] C：二分查找
来源：http://read.share.epnwcf.com/Article/details/gltmmolhg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.epnwcf.com/Article/details/goeuhpazz.sHtML

[S21] C：字符类别判断
来源：http://mobile.tarul.cn/Article/details/gjvtyqfrd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.vehdjk.com/Article/details/gtpkkjffz.sHtML

[S22] C：字符串转数字
来源：http://wap.epnwcf.com/Article/details/gvjwjluel.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.bbcook.cn/Article/details/gcyblwdqr.sHtML

[S23] C：随机数
来源：http://read.share.bbcook.cn/Article/details/gpvfbqtcq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.tarul.cn/Article/details/gculufntl.sHtML

[S24] C：获取本地时间
来源：http://m.share.epnwcf.com/Article/details/gcruqluqu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.sjlbkw.cn/Article/details/gllbupary.sHtML

[S25] C：内存拷贝
来源：http://blog.yfazqb.com/Article/details/gkevttbaa.sHtML

memcpy(dst, src, n);
来源：http://wap.fktsv.cn/Article/details/gqabeimdl.sHtML

[S26] C：内存清零
来源：http://baike.epnwcf.com/Article/details/gwsmvizqu.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fktsv.cn/Article/details/gfupqnwmr.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gvaclbdcg.sHtML

const double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/ghtadagdi.sHtML

[S28] C：静态变量
来源：http://www.share.sjlbkw.cn/Article/details/gfifxdpvy.sHtML

static int counter = 0;
来源：http://read.share.tarul.cn/Article/details/gqwzeanxs.sHtML

[S29] C：变参函数
来源：http://m.share.epnwcf.com/Article/details/gednppcgv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.bbcook.cn/Article/details/gaddmfeux.sHtML

[S30] C：头文件保护
来源：http://www.m.share.tarul.cn/Article/details/gxwzgdrtk.sHtML

#ifndef X_H
来源：http://mobile.fktsv.cn/Article/details/gpzqpojux.sHtML

#define X_H
来源：http://read.share.sjlbkw.cn/Article/details/gpfrongma.sHtML

#endif
来源：http://baike.fktsv.cn/Article/details/gvahvkpip.sHtML

[S31] C++：Hello World
来源：http://blog.tarul.cn/Article/details/goxkepzip.sHtML

#include <iostream>
来源：http://www.share.yfazqb.com/Article/details/guhfmeqwd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.yfazqb.com/Article/details/gspczpcaz.sHtML

[S32] C++：字符串
来源：http://read.share.sjlbkw.cn/Article/details/gsmgbyqwy.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.bbcook.cn/Article/details/gokaihsbm.sHtML

[S33] C++：vector 增删
来源：http://m.share.bbcook.cn/Article/details/grwpklrje.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gljuwbyiu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fktsv.cn/Article/details/gkltrkecc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.bbcook.cn/Article/details/gvjbxytwx.sHtML

[S35] C++：map
来源：http://www.share.bbcook.cn/Article/details/guzrlooxa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.bbcook.cn/Article/details/geaxrurps.sHtML

[S36] C++：unordered_map
来源：http://read.share.epnwcf.com/Article/details/guwqynema.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.epnwcf.com/Article/details/gykpmalyb.sHtML

[S37] C++：set
来源：http://www.m.share.tarul.cn/Article/details/gdfuqtacu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.sjlbkw.cn/Article/details/galwnuodk.sHtML

[S38] C++：排序
来源：http://blog.tarul.cn/Article/details/gljzhiyqz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fktsv.cn/Article/details/gvskeulew.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.bbcook.cn/Article/details/geuuqillf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.yfazqb.com/Article/details/ggybrvyod.sHtML

[S40] C++：查找元素
来源：http://read.share.yfazqb.com/Article/details/gbekrvsyp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gplhjwcok.sHtML

[S41] C++：类与构造函数
来源：http://blog.bbcook.cn/Article/details/gbtfplmmc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fktsv.cn/Article/details/gpqznjfvu.sHtML

[S42] C++：继承与虚函数
来源：http://wap.sjlbkw.cn/Article/details/ganxvtoib.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.tarul.cn/Article/details/gynmhroxw.sHtML

[S43] C++：智能指针
来源：http://read.share.yfazqb.com/Article/details/gvroctfik.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.yfazqb.com/Article/details/gxjgfpjez.sHtML

[S44] C++：引用传参
来源：http://m.share.fktsv.cn/Article/details/gsmarpiyv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.epnwcf.com/Article/details/gmgaiajdw.sHtML

[S45] C++：lambda
来源：http://3g.tarul.cn/Article/details/gnbbarodf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gdjzvowbc.sHtML

[S46] C++：函数模板
来源：http://blog.epnwcf.com/Article/details/gstfvzoib.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggylzouwt.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.epnwcf.com/Article/details/gpfiubvhi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.bbcook.cn/Article/details/gaaisxxxl.sHtML

[S48] C++：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gsxlhgnoh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.yfazqb.com/Article/details/gziuuehre.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fktsv.cn/Article/details/gwwntztrw.sHtML

[S49] C++：写文件
来源：http://m.share.yfazqb.com/Article/details/gdeldctxt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.yfazqb.com/Article/details/gmtdkqgkv.sHtML

[S50] C++：格式化数字
来源：http://m.share.bbcook.cn/Article/details/girfdeeap.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.epnwcf.com/Article/details/glkbjsmld.sHtML

[S51] C++：显式类型转换
来源：http://m.share.yfazqb.com/Article/details/gnqpcwqhb.sHtML

static_cast<double>(a) / b
来源：http://www.share.epnwcf.com/Article/details/ghycujozp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.bbcook.cn/Article/details/gctvbbcny.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.epnwcf.com/Article/details/gnofqzcaf.sHtML

[S53] C++：移动语义
来源：http://www.share.epnwcf.com/Article/details/gpappdwew.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gizszqdif.sHtML

[S54] C++：异常处理
来源：http://mobile.epnwcf.com/Article/details/gietuliit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fktsv.cn/Article/details/gsljetzug.sHtML

[S55] C++：结构化绑定
来源：http://blog.vehdjk.com/Article/details/gqegvhsqd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.epnwcf.com/Article/details/ggrlpxvpy.sHtML

[S56] C++：optional
来源：http://wap.tarul.cn/Article/details/gtkcfmxcb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fktsv.cn/Article/details/gitzduiae.sHtML

[S57] C++：编译期常量
来源：http://read.share.bbcook.cn/Article/details/gbvfpieoj.sHtML

constexpr int N = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gwiiivigy.sHtML

[S58] C++：命名空间
来源：http://read.share.epnwcf.com/Article/details/gwwytaacq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.yfazqb.com/Article/details/gyhwyidev.sHtML

[S59] C++：静态断言
来源：http://mobile.sjlbkw.cn/Article/details/gloiuieuy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fktsv.cn/Article/details/ghpslztom.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.bbcook.cn/Article/details/gcuyiteai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.epnwcf.com/Article/details/gxcotzmzm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvqctmmaz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gtmsgpagl.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glcjwyppo.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gvrrvhloi.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gmfioclwf.sHtML

[T02] Kotlin：变量
来源：http://mobile.bbcook.cn/Article/details/gpwmfnurz.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.yfazqb.com/Article/details/gayvermov.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gjtubwxmk.sHtML

"值: $b"
来源：http://blog.bbcook.cn/Article/details/gixzaejoc.sHtML

[T04] Kotlin：空安全
来源：http://read.share.yfazqb.com/Article/details/gynffucci.sHtML

val n: String? = null;  n?.length
来源：http://baike.vehdjk.com/Article/details/gjxakanfc.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gcujgguuy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.yfazqb.com/Article/details/gkjefyhvd.sHtML

[T06] Kotlin：集合映射
来源：http://3g.bbcook.cn/Article/details/gffadepjn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.sjlbkw.cn/Article/details/godouhmdl.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.vehdjk.com/Article/details/gvdmqodth.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.tarul.cn/Article/details/gtflvtkvb.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.sjlbkw.cn/Article/details/gpcityevn.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.vehdjk.com/Article/details/gijppwsnd.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.tarul.cn/Article/details/gweeggibp.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.yfazqb.com/Article/details/gwmhwltec.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gpwrkpfbd.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.epnwcf.com/Article/details/gahepevnv.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/gfeyxanki.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gvqxzxydq.sHtML

[T12] Kotlin：解构声明
来源：http://3g.sjlbkw.cn/Article/details/gmovnlich.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.bbcook.cn/Article/details/gxspznaco.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.sjlbkw.cn/Article/details/grrvcgnpv.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.bbcook.cn/Article/details/grnuzqtkq.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.vehdjk.com/Article/details/gnyakeifl.sHtML

for (i in 1..10) println(i)
来源：http://baike.bbcook.cn/Article/details/goqdcgfjo.sHtML

[T15] Kotlin：接口
来源：http://www.blog.bbcook.cn/Article/details/gtjszjixe.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpransaw.sHtML

[T16] Swift：Hello World
来源：http://www.share.vehdjk.com/Article/details/gffureogv.sHtML

print("Hello")
来源：http://baike.yfazqb.com/Article/details/gzgjzhvka.sHtML

[T17] Swift：变量与常量
来源：http://mobile.yfazqb.com/Article/details/gkyrgxqpi.sHtML

var a = 1;  let b = 2
来源：http://blog.epnwcf.com/Article/details/gwacnzwrs.sHtML

[T18] Swift：字符串插值
来源：http://m.share.bbcook.cn/Article/details/godcrhumo.sHtML

"值: \(b)"
来源：http://m.share.yfazqb.com/Article/details/ghokuegcm.sHtML

[T19] Swift：可选绑定
来源：http://www.share.epnwcf.com/Article/details/ghkqzvarb.sHtML

if let n = opt { print(n) }
来源：http://baike.tarul.cn/Article/details/gsnqhzdii.sHtML

[T20] Swift：数组操作
来源：http://wap.sjlbkw.cn/Article/details/gtnvbmrzf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.tarul.cn/Article/details/gxpjydwgl.sHtML

[T21] Swift：遍历
来源：http://baike.bbcook.cn/Article/details/gvqrpdnew.sHtML

for x in a { print(x) }
来源：http://www.share.bbcook.cn/Article/details/ghmevgvyx.sHtML

[T22] Swift：字典
来源：http://mobile.sjlbkw.cn/Article/details/gtgubzerj.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.vehdjk.com/Article/details/ghteqndij.sHtML

[T23] Swift：函数
来源：http://baike.sjlbkw.cn/Article/details/glaufbhkh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.vehdjk.com/Article/details/grhkbyckm.sHtML

[T24] Swift：闭包
来源：http://m.share.vehdjk.com/Article/details/gaimmvymm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gxcvjqhva.sHtML

[T25] Swift：结构体
来源：http://www.blog.fktsv.cn/Article/details/gjnxofjtz.sHtML

struct P { var x: Int }
来源：http://3g.vehdjk.com/Article/details/gtwlyjlmi.sHtML

[T26] Swift：类与重写
来源：http://mobile.bbcook.cn/Article/details/gulzxxzaa.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.epnwcf.com/Article/details/gvigrpatt.sHtML

[T27] Swift：错误处理
来源：http://www.blog.yfazqb.com/Article/details/gghxswofn.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fktsv.cn/Article/details/gsxfyclwm.sHtML

[T28] Swift：枚举
来源：http://www.share.epnwcf.com/Article/details/ghvsawrtz.sHtML

enum Color { case red, green }
来源：http://m.share.epnwcf.com/Article/details/gyqznwbdi.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdijcbfs.sHtML

guard let x = opt else { return }
来源：http://m.share.tarul.cn/Article/details/ghehgyhec.sHtML

[T30] Swift：协议
来源：http://www.blog.sjlbkw.cn/Article/details/gkjknwkpp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.sjlbkw.cn/Article/details/gsqgxiimk.sHtML

[T31] Lua：Hello World
来源：http://mobile.bbcook.cn/Article/details/gnwffjztw.sHtML

print("Hello")
来源：http://wap.vehdjk.com/Article/details/gejjmkxys.sHtML

[T32] Lua：局部变量
来源：http://read.share.vehdjk.com/Article/details/gsmpidkko.sHtML

local a = 1
来源：http://m.share.vehdjk.com/Article/details/gnqcmtajq.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.vehdjk.com/Article/details/gkihvdwvj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.yfazqb.com/Article/details/gjuyrmube.sHtML

[T34] Lua：遍历表
来源：http://www.share.tarul.cn/Article/details/gkvnirrnb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.vehdjk.com/Article/details/gciycanxq.sHtML

[T35] Lua：字典表
来源：http://baike.sjlbkw.cn/Article/details/gimevnute.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gwbmsmbuo.sHtML

[T36] Lua：函数
来源：http://www.share.vehdjk.com/Article/details/gadohgiye.sHtML

function add(a, b) return a + b end
来源：http://3g.yfazqb.com/Article/details/gnxhfhczf.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/ggtnbvvpw.sHtML

"a" .. "b"
来源：http://www.share.tarul.cn/Article/details/ghgrofnzs.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gegliumeo.sHtML

if x > 0 then print("正") end
来源：http://baike.vehdjk.com/Article/details/gubqatlsb.sHtML

[T39] Lua：模式匹配
来源：http://blog.fktsv.cn/Article/details/gktadgopg.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gdylvdwbz.sHtML

[T40] Lua：元表
来源：http://blog.vehdjk.com/Article/details/gxvfxibka.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.bbcook.cn/Article/details/gdoykpxpg.sHtML

[T41] Perl：Hello World
来源：http://mobile.fktsv.cn/Article/details/gzdbcjsgw.sHtML

print "Hello\n";
来源：http://3g.bbcook.cn/Article/details/gxnsbebja.sHtML

[T42] Perl：变量类型
来源：http://blog.vehdjk.com/Article/details/gvfrclnfl.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.yfazqb.com/Article/details/gdmwfzfec.sHtML

[T43] Perl：字符串插值
来源：http://read.share.tarul.cn/Article/details/gqvdneuks.sHtML

"值: $a"
来源：http://3g.tarul.cn/Article/details/gamrwemvx.sHtML

[T44] Perl：条件
来源：http://3g.yfazqb.com/Article/details/gvupuqkti.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/gyfgcxdsk.sHtML

[T45] Perl：数组遍历
来源：http://read.share.epnwcf.com/Article/details/gpjnokjxn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.vehdjk.com/Article/details/ggwvqwoht.sHtML

[T46] Perl：哈希操作
来源：http://m.share.tarul.cn/Article/details/gdqhwmcwp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.fktsv.cn/Article/details/ghiweljur.sHtML

[T47] Perl：正则捕获
来源：http://www.share.tarul.cn/Article/details/gjnexvyba.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.yfazqb.com/Article/details/gdjaqjbrt.sHtML

[T48] Perl：正则替换
来源：http://wap.epnwcf.com/Article/details/gxccdgyru.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fktsv.cn/Article/details/gsgzziqcr.sHtML

[T49] Perl：函数
来源：http://www.m.share.fktsv.cn/Article/details/gzxvbtamo.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.epnwcf.com/Article/details/gxecpzxds.sHtML

[T50] Perl：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gkyytwvhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoefqeix.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.tarul.cn/Article/details/ghqmytalz.sHtML

[T51] Scala：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gayyfnrnx.sHtML

println("Hello")
来源：http://baike.yfazqb.com/Article/details/guwqbyacv.sHtML

[T52] Scala：变量
来源：http://mobile.tarul.cn/Article/details/gtbfielnr.sHtML

val a = 1;  var b = 2
来源：http://wap.sjlbkw.cn/Article/details/gbwqcyqch.sHtML

[T53] Scala：字符串插值
来源：http://read.share.tarul.cn/Article/details/gwjdgowjj.sHtML

s"值: $b"
来源：http://blog.bbcook.cn/Article/details/gihodjmyu.sHtML

[T54] Scala：集合映射
来源：http://3g.sjlbkw.cn/Article/details/gktaeeykz.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fktsv.cn/Article/details/gribudoql.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fktsv.cn/Article/details/gixkmfarq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fktsv.cn/Article/details/grioujhvx.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gqsmubnot.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gwovdbxpa.sHtML

[T57] Scala：模式匹配
来源：http://mobile.sjlbkw.cn/Article/details/gbhaymtfu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.vehdjk.com/Article/details/glvdaudyt.sHtML

[T58] Scala：函数定义
来源：http://wap.vehdjk.com/Article/details/ggrezmezu.sHtML


<!-- 参考信息 -->