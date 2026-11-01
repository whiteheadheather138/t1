代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/glvpgyqtu.sHtML

[R58] 下载文件
来源：http://www.m.share.tarul.cn/Article/details/gmgykqfuy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.tarul.cn/Article/details/glzckgpar.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gstmmmfkj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.sjlbkw.cn/Article/details/gnxmuwcxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gtqqdlvnu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.bbcook.cn/Article/details/gxumwnoob.sHtML

[R61] 磁盘占用
来源：http://www.m.share.tarul.cn/Article/details/gaciypwdr.sHtML

df -h;  du -sh *
来源：http://www.blog.yfazqb.com/Article/details/gpotzzttr.sHtML

[R62] 找最占空间的文件
来源：http://m.share.yfazqb.com/Article/details/gkfpnpkhy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.yfazqb.com/Article/details/grcrnbdib.sHtML

[R63] 内存与进程
来源：http://www.blog.vehdjk.com/Article/details/gogcznnai.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gedeegsmd.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gdggwbnzn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.bbcook.cn/Article/details/ghdtqbodw.sHtML

[R65] 查看端口占用
来源：http://baike.fktsv.cn/Article/details/ghszsaaqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.tarul.cn/Article/details/gbazkzybt.sHtML

[R66] 定时任务
来源：http://read.share.sjlbkw.cn/Article/details/gbmwzrhlr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fktsv.cn/Article/details/giyqhacwc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.yfazqb.com/Article/details/gqqqtlthh.sHtML

openssl rand -hex 16
来源：http://mobile.epnwcf.com/Article/details/gojwdbqyn.sHtML

[R68] 计算文件校验值
来源：http://3g.sjlbkw.cn/Article/details/gfgyrhdds.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gbiymrlow.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fktsv.cn/Article/details/gwliymooj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.bbcook.cn/Article/details/gffhfyulz.sHtML

[R70] 时间戳与互转
来源：http://www.blog.vehdjk.com/Article/details/gywzxbhic.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.yfazqb.com/Article/details/gsxbalest.sHtML

[R71] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gsvyssayk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.tarul.cn/Article/details/gxlnvvact.sHtML

[R72] 等待端口就绪
来源：http://mobile.tarul.cn/Article/details/gzarvhzut.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gpsisqpws.sHtML

[R73] 分割大日志
来源：http://wap.yfazqb.com/Article/details/gdcssrqgk.sHtML

split -l 1000 big.log part_
来源：http://m.share.epnwcf.com/Article/details/gszpfdnsr.sHtML

[R74] 批量重命名
来源：http://3g.bbcook.cn/Article/details/gjmzylnfu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.bbcook.cn/Article/details/gsngdqtkm.sHtML

[R75] 导出环境变量
来源：http://www.share.bbcook.cn/Article/details/gyvubcsuh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfugraxf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.bbcook.cn/Article/details/gjagdhjrc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.bbcook.cn/Article/details/gjkfmrjbb.sHtML

[R77] 读取用户输入
来源：http://3g.fktsv.cn/Article/details/gpsywoivr.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gcrqkceev.sHtML

[R78] 交互式菜单
来源：http://wap.vehdjk.com/Article/details/gucusdbcs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.vehdjk.com/Article/details/gymljnxcu.sHtML

[R79] 解析命令行选项
来源：http://blog.bbcook.cn/Article/details/gnaghbhsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fktsv.cn/Article/details/gsjasesyq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/ghteuwebg.sHtML

time ./run.sh
来源：http://3g.yfazqb.com/Article/details/glgznsjzu.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gupakwymb.sHtML

S. C / C++ 专题
来源：http://3g.yfazqb.com/Article/details/grtlaljew.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxhwsmgze.sHtML

[S01] C：Hello World
来源：http://3g.bbcook.cn/Article/details/gtmllyvcm.sHtML

#include <stdio.h>
来源：http://wap.epnwcf.com/Article/details/ggkwiswjw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.bbcook.cn/Article/details/gdosiimlj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fktsv.cn/Article/details/gtahyziiu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.sjlbkw.cn/Article/details/gdshyebso.sHtML

[S03] C：读入整数
来源：http://wap.epnwcf.com/Article/details/gmvmwuvmu.sHtML

int x; scanf("%d", &x);
来源：http://3g.vehdjk.com/Article/details/gvlgrweyr.sHtML

[S04] C：字符串复制
来源：http://mobile.yfazqb.com/Article/details/gfnjrklgs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fktsv.cn/Article/details/gporhmtcp.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gbupwpnxr.sHtML

strlen(s)
来源：http://www.share.vehdjk.com/Article/details/guxevwina.sHtML

[S06] C：字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gzurixfuw.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/gwwgvlswo.sHtML

[S07] C：数组遍历求和
来源：http://read.share.sjlbkw.cn/Article/details/gxwjbaqlm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/giskjvmmh.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.yfazqb.com/Article/details/gmijxndrv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.yfazqb.com/Article/details/gaxkaevhm.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.yfazqb.com/Article/details/gtiraipks.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.bbcook.cn/Article/details/gpfgkxqvs.sHtML

[S10] C：指针与解引用
来源：http://m.share.epnwcf.com/Article/details/glvwqyinm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.yfazqb.com/Article/details/gbfjxbrfl.sHtML

[S11] C：逐行读文件
来源：http://m.share.tarul.cn/Article/details/ggothndxs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fktsv.cn/Article/details/grwjrknbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gifhmpfdq.sHtML

fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gphlisyxz.sHtML

[S12] C：写文件
来源：http://wap.tarul.cn/Article/details/gvzenuqwu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.tarul.cn/Article/details/gzsnkinim.sHtML

[S13] C：宏定义
来源：http://wap.tarul.cn/Article/details/giuwxtwhh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.sjlbkw.cn/Article/details/gtbtonwpk.sHtML

[S14] C：枚举
来源：http://mobile.epnwcf.com/Article/details/ggnnytume.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.tarul.cn/Article/details/ggflargaa.sHtML

[S15] C：类型转换
来源：http://3g.fktsv.cn/Article/details/gvcnalhqq.sHtML

(double) a / b
来源：http://www.share.tarul.cn/Article/details/grttgdjws.sHtML

[S16] C：位操作置位
来源：http://www.share.fktsv.cn/Article/details/gmnwrhvwj.sHtML

x |= (1 << 3);
来源：http://3g.tarul.cn/Article/details/gwggtqczi.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/goqfzfaba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.epnwcf.com/Article/details/gopdjnlxc.sHtML

[S18] C：命令行参数
来源：http://blog.bbcook.cn/Article/details/ggshpugzi.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/gqlrvtexa.sHtML

[S19] C：快速排序
来源：http://mobile.tarul.cn/Article/details/gayootcbp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.vehdjk.com/Article/details/ggxvvtqfe.sHtML

[S20] C：二分查找
来源：http://wap.yfazqb.com/Article/details/gwebzvnir.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.vehdjk.com/Article/details/gcfvlaljb.sHtML

[S21] C：字符类别判断
来源：http://wap.bbcook.cn/Article/details/gptaoimzn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.bbcook.cn/Article/details/grcfgijni.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gmobjmmer.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.sjlbkw.cn/Article/details/ggopabvxq.sHtML

[S23] C：随机数
来源：http://www.blog.vehdjk.com/Article/details/gfwtpoarj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.yfazqb.com/Article/details/gjdegjewy.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.sjlbkw.cn/Article/details/gijmpnoho.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.tarul.cn/Article/details/gmohvhjcl.sHtML

[S25] C：内存拷贝
来源：http://www.blog.bbcook.cn/Article/details/gnsqklmxb.sHtML

memcpy(dst, src, n);
来源：http://mobile.fktsv.cn/Article/details/gmzzaygml.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/garexcpmw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.tarul.cn/Article/details/gnjhrbtlp.sHtML

[S27] C：定义常量
来源：http://read.share.tarul.cn/Article/details/gkkrzidou.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/goeirbhib.sHtML

[S28] C：静态变量
来源：http://blog.tarul.cn/Article/details/gmiwrbpsi.sHtML

static int counter = 0;
来源：http://www.blog.epnwcf.com/Article/details/gpivankpj.sHtML

[S29] C：变参函数
来源：http://mobile.yfazqb.com/Article/details/ggrdxwzug.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.vehdjk.com/Article/details/gfjlginkw.sHtML

[S30] C：头文件保护
来源：http://www.share.vehdjk.com/Article/details/gnkyiffol.sHtML

#ifndef X_H
来源：http://blog.yfazqb.com/Article/details/gocpsatac.sHtML

#define X_H
来源：http://www.m.share.epnwcf.com/Article/details/gajsnujyk.sHtML

#endif
来源：http://m.share.bbcook.cn/Article/details/ggvufjvho.sHtML

[S31] C++：Hello World
来源：http://www.share.sjlbkw.cn/Article/details/gfoxhjqol.sHtML

#include <iostream>
来源：http://m.share.fktsv.cn/Article/details/gwaqkfqzk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzomexqnd.sHtML

[S32] C++：字符串
来源：http://read.share.vehdjk.com/Article/details/gbsxedbdq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.epnwcf.com/Article/details/gwkuesrwi.sHtML

[S33] C++：vector 增删
来源：http://3g.sjlbkw.cn/Article/details/gfafjmrrc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.epnwcf.com/Article/details/gxbdollbj.sHtML

[S34] C++：遍历 vector
来源：http://3g.fktsv.cn/Article/details/gxexzbzxq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.tarul.cn/Article/details/gqicadsge.sHtML

[S35] C++：map
来源：http://www.share.tarul.cn/Article/details/gssnitnhp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gaeystfvh.sHtML

[S36] C++：unordered_map
来源：http://wap.sjlbkw.cn/Article/details/gcqexzhji.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gesdppzby.sHtML

[S37] C++：set
来源：http://mobile.epnwcf.com/Article/details/gppvpgnjp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fktsv.cn/Article/details/glcxsbtbl.sHtML

[S38] C++：排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gkskzgdzb.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.vehdjk.com/Article/details/gdkxbdkbt.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.yfazqb.com/Article/details/gxhazdlzd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.tarul.cn/Article/details/glsrfghkq.sHtML

[S40] C++：查找元素
来源：http://wap.sjlbkw.cn/Article/details/ggvbthxvr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fktsv.cn/Article/details/gmwhrowmb.sHtML

[S41] C++：类与构造函数
来源：http://read.share.sjlbkw.cn/Article/details/geruewgbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fktsv.cn/Article/details/gypjnxxwq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.epnwcf.com/Article/details/gtjszpmmi.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.vehdjk.com/Article/details/gkzgnqafm.sHtML

[S43] C++：智能指针
来源：http://www.share.yfazqb.com/Article/details/gjglkyipa.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fktsv.cn/Article/details/gattbvmgk.sHtML

[S44] C++：引用传参
来源：http://3g.yfazqb.com/Article/details/gvnzrykwn.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/ghccwxrml.sHtML

[S45] C++：lambda
来源：http://www.share.tarul.cn/Article/details/glgypqcct.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.vehdjk.com/Article/details/gclxzkapc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.epnwcf.com/Article/details/gnypilowp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.sjlbkw.cn/Article/details/gjlbvdwwi.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.vehdjk.com/Article/details/gonlgarje.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.sjlbkw.cn/Article/details/gssadjpcr.sHtML

[S48] C++：逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gamwtootj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.epnwcf.com/Article/details/gefemwahz.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fktsv.cn/Article/details/gyxkpenlj.sHtML

[S49] C++：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gjtiitpbk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.epnwcf.com/Article/details/griomgsnv.sHtML

[S50] C++：格式化数字
来源：http://m.share.yfazqb.com/Article/details/ghvpyecoc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gkbvkhtkr.sHtML

[S51] C++：显式类型转换
来源：http://blog.epnwcf.com/Article/details/ggfruemwa.sHtML

static_cast<double>(a) / b
来源：http://m.share.vehdjk.com/Article/details/gwcvcvegu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fktsv.cn/Article/details/gexmiiwzx.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.sjlbkw.cn/Article/details/groeogifj.sHtML

[S53] C++：移动语义
来源：http://wap.epnwcf.com/Article/details/gasabcjtv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.vehdjk.com/Article/details/gpbnpnwyf.sHtML

[S54] C++：异常处理
来源：http://mobile.yfazqb.com/Article/details/ghqnwpcwv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.vehdjk.com/Article/details/gfzmvrfwf.sHtML

[S55] C++：结构化绑定
来源：http://3g.bbcook.cn/Article/details/gnjgteres.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.tarul.cn/Article/details/gmxiexkgt.sHtML

[S56] C++：optional
来源：http://baike.tarul.cn/Article/details/gtuzamyux.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.bbcook.cn/Article/details/gdblgzgqw.sHtML

[S57] C++：编译期常量
来源：http://www.blog.vehdjk.com/Article/details/gbgbhafpi.sHtML

constexpr int N = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gaczynqbp.sHtML

[S58] C++：命名空间
来源：http://baike.tarul.cn/Article/details/gpgtmtyit.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.vehdjk.com/Article/details/gxkahnsvc.sHtML

[S59] C++：静态断言
来源：http://baike.yfazqb.com/Article/details/ghiakywxe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.bbcook.cn/Article/details/growvqdvq.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.bbcook.cn/Article/details/gyojfiauv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.bbcook.cn/Article/details/gjrcnznby.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpllraisb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.epnwcf.com/Article/details/gylaeauby.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwalrlvbf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.yfazqb.com/Article/details/gcaukyprw.sHtML

println("Hello")
来源：http://baike.bbcook.cn/Article/details/gchcazpqp.sHtML

[T02] Kotlin：变量
来源：http://baike.fktsv.cn/Article/details/gfwqpzeig.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fktsv.cn/Article/details/ghxkplnmi.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gftiijvuu.sHtML

"值: $b"
来源：http://read.share.bbcook.cn/Article/details/gvpadjaum.sHtML

[T04] Kotlin：空安全
来源：http://read.share.epnwcf.com/Article/details/gberbmkyq.sHtML

val n: String? = null;  n?.length
来源：http://read.share.yfazqb.com/Article/details/gkscrybpw.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.epnwcf.com/Article/details/gsdywwtyo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fktsv.cn/Article/details/gkkznhgzl.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gxljnvlan.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.yfazqb.com/Article/details/glqjgautw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.sjlbkw.cn/Article/details/gvryxnmwe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.vehdjk.com/Article/details/geviflxaf.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.bbcook.cn/Article/details/gtywqvgdy.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fktsv.cn/Article/details/gmubtqjlm.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.epnwcf.com/Article/details/gumzgoymi.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.yfazqb.com/Article/details/gtkfdgjun.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fktsv.cn/Article/details/gdjnaefrx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.epnwcf.com/Article/details/gpboriazv.sHtML

[T11] Kotlin：协程
来源：http://baike.bbcook.cn/Article/details/gyohpbfcb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.bbcook.cn/Article/details/gepreslzl.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fktsv.cn/Article/details/gabpibhjp.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.tarul.cn/Article/details/gkwjulimy.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.tarul.cn/Article/details/gnltdwgez.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.bbcook.cn/Article/details/gqrkzwbrg.sHtML

[T14] Kotlin：循环
来源：http://m.share.sjlbkw.cn/Article/details/gxduaufjo.sHtML

for (i in 1..10) println(i)
来源：http://read.share.tarul.cn/Article/details/gasvrydjl.sHtML

[T15] Kotlin：接口
来源：http://baike.yfazqb.com/Article/details/gpcqplqtk.sHtML

interface Shape { fun area(): Double }
来源：http://baike.yfazqb.com/Article/details/gcaqqksvq.sHtML

[T16] Swift：Hello World
来源：http://www.share.fktsv.cn/Article/details/gcsplxcpa.sHtML

print("Hello")
来源：http://mobile.yfazqb.com/Article/details/gqviklqab.sHtML

[T17] Swift：变量与常量
来源：http://baike.yfazqb.com/Article/details/gtzpvajlv.sHtML

var a = 1;  let b = 2
来源：http://3g.tarul.cn/Article/details/gopeyzmdo.sHtML

[T18] Swift：字符串插值
来源：http://3g.sjlbkw.cn/Article/details/gnetdpvxj.sHtML

"值: \(b)"
来源：http://www.m.share.epnwcf.com/Article/details/gfophvcqd.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.yfazqb.com/Article/details/gblmwsscn.sHtML

if let n = opt { print(n) }
来源：http://blog.sjlbkw.cn/Article/details/ghcbhqupn.sHtML

[T20] Swift：数组操作
来源：http://m.share.sjlbkw.cn/Article/details/gjnhzhwmk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.vehdjk.com/Article/details/gkqtzgted.sHtML

[T21] Swift：遍历
来源：http://mobile.bbcook.cn/Article/details/gjledjolh.sHtML

for x in a { print(x) }
来源：http://3g.bbcook.cn/Article/details/geqndcvus.sHtML

[T22] Swift：字典
来源：http://m.share.epnwcf.com/Article/details/grswrjiuv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.yfazqb.com/Article/details/gbgpuxqqh.sHtML

[T23] Swift：函数
来源：http://blog.fktsv.cn/Article/details/gbcefweeb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.bbcook.cn/Article/details/gzjdicvuy.sHtML

[T24] Swift：闭包
来源：http://3g.sjlbkw.cn/Article/details/gjryqledn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gqxjregkb.sHtML

[T25] Swift：结构体
来源：http://www.share.sjlbkw.cn/Article/details/geoawjtdf.sHtML

struct P { var x: Int }
来源：http://m.share.vehdjk.com/Article/details/ggtqmmnfb.sHtML

[T26] Swift：类与重写
来源：http://blog.vehdjk.com/Article/details/gquugrfqv.sHtML

class A: Base { override func f() {} }
来源：http://www.share.vehdjk.com/Article/details/gleeplefw.sHtML

[T27] Swift：错误处理
来源：http://www.share.epnwcf.com/Article/details/gfeneokmp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.bbcook.cn/Article/details/gmdadxoyl.sHtML

[T28] Swift：枚举
来源：http://blog.bbcook.cn/Article/details/gqciipegi.sHtML

enum Color { case red, green }
来源：http://wap.vehdjk.com/Article/details/goblgdzas.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.bbcook.cn/Article/details/gnbaspahx.sHtML

guard let x = opt else { return }
来源：http://www.share.sjlbkw.cn/Article/details/gxiuwhhvz.sHtML

[T30] Swift：协议
来源：http://baike.vehdjk.com/Article/details/gzaakhmnp.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fktsv.cn/Article/details/gnoyuvkjs.sHtML

[T31] Lua：Hello World
来源：http://3g.bbcook.cn/Article/details/gnvdpgzyy.sHtML

print("Hello")
来源：http://read.share.yfazqb.com/Article/details/ghadwihpi.sHtML

[T32] Lua：局部变量
来源：http://m.share.fktsv.cn/Article/details/giaovqijd.sHtML

local a = 1
来源：http://mobile.vehdjk.com/Article/details/gcfyfmtif.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.bbcook.cn/Article/details/gzdgupplk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.sjlbkw.cn/Article/details/gymikoyho.sHtML

[T34] Lua：遍历表
来源：http://mobile.tarul.cn/Article/details/gqbwllsfk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.vehdjk.com/Article/details/gjnctgyak.sHtML

[T35] Lua：字典表
来源：http://www.blog.bbcook.cn/Article/details/gubzrwpqw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.yfazqb.com/Article/details/gvzakribc.sHtML

[T36] Lua：函数
来源：http://mobile.fktsv.cn/Article/details/ggpfkbbxg.sHtML

function add(a, b) return a + b end
来源：http://mobile.yfazqb.com/Article/details/gglfcreez.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/ghddphwpm.sHtML

"a" .. "b"
来源：http://www.share.vehdjk.com/Article/details/grjahxtxp.sHtML

[T38] Lua：条件
来源：http://baike.tarul.cn/Article/details/gxebigznd.sHtML

if x > 0 then print("正") end
来源：http://read.share.vehdjk.com/Article/details/gjreiughe.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fktsv.cn/Article/details/gdyjrdbuv.sHtML

string.find(s, "%d+")
来源：http://3g.fktsv.cn/Article/details/gchwztgjp.sHtML

[T40] Lua：元表
来源：http://3g.tarul.cn/Article/details/geitgpgji.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.yfazqb.com/Article/details/gihkgejkm.sHtML

[T41] Perl：Hello World
来源：http://www.share.bbcook.cn/Article/details/gwhjbyyno.sHtML

print "Hello\n";
来源：http://3g.fktsv.cn/Article/details/gydtgnyoi.sHtML

[T42] Perl：变量类型
来源：http://www.blog.bbcook.cn/Article/details/gqgyzecdx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.share.fktsv.cn/Article/details/gnpicndoj.sHtML

[T43] Perl：字符串插值
来源：http://www.share.fktsv.cn/Article/details/gfcbheedp.sHtML

"值: $a"
来源：http://read.share.tarul.cn/Article/details/gyylcaqty.sHtML

[T44] Perl：条件
来源：http://www.blog.sjlbkw.cn/Article/details/gfgeyfjkg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.tarul.cn/Article/details/gaigdughv.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.fktsv.cn/Article/details/gpkubnrcq.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.sjlbkw.cn/Article/details/gebdkmmzm.sHtML

[T46] Perl：哈希操作
来源：http://www.m.share.fktsv.cn/Article/details/ggmbtgrxb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.yfazqb.com/Article/details/guhmykuvw.sHtML

[T47] Perl：正则捕获
来源：http://mobile.vehdjk.com/Article/details/gpubhvmlr.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.bbcook.cn/Article/details/gyhifblzg.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.tarul.cn/Article/details/ghuqrqvuz.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fktsv.cn/Article/details/gbmycwyae.sHtML

[T49] Perl：函数
来源：http://www.share.epnwcf.com/Article/details/gmgqihllg.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/gwrnagqek.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fktsv.cn/Article/details/ghaczqjco.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.vehdjk.com/Article/details/gdcoumrii.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/ggstpewrl.sHtML

[T51] Scala：Hello World
来源：http://baike.tarul.cn/Article/details/gvvgdtquq.sHtML

println("Hello")
来源：http://baike.tarul.cn/Article/details/gufjhubxh.sHtML

[T52] Scala：变量
来源：http://wap.vehdjk.com/Article/details/gjbxaqegz.sHtML

val a = 1;  var b = 2
来源：http://3g.epnwcf.com/Article/details/gtnxamard.sHtML

[T53] Scala：字符串插值
来源：http://mobile.vehdjk.com/Article/details/gpamrfawf.sHtML

s"值: $b"
来源：http://mobile.epnwcf.com/Article/details/gdmbbaegm.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gblrluhwn.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.vehdjk.com/Article/details/gzlvxkuog.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/gpsloqvou.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.sjlbkw.cn/Article/details/gewvsxbnx.sHtML

[T56] Scala：样例类
来源：http://read.share.epnwcf.com/Article/details/gupjkehza.sHtML

case class User(name: String, age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gmmfantxt.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.fktsv.cn/Article/details/gntwolbzj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.epnwcf.com/Article/details/genxowuat.sHtML

[T58] Scala：函数定义
来源：http://www.share.bbcook.cn/Article/details/gsraetpxd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.tarul.cn/Article/details/gkebyohvu.sHtML

[T59] Scala：循环
来源：http://www.share.fktsv.cn/Article/details/gkpjhprsh.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.epnwcf.com/Article/details/gmwgaacod.sHtML

[T60] Scala：折叠
来源：http://3g.vehdjk.com/Article/details/gbzajbuyu.sHtML


<!-- 参考信息 -->