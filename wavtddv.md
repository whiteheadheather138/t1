代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.share.fktsv.cn/Article/details/gkyywzoch.sHtML

[R64] 结束进程
来源：http://www.share.vehdjk.com/Article/details/gsmqkccou.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.sjlbkw.cn/Article/details/gmcexxfsd.sHtML

[R65] 查看端口占用
来源：http://www.blog.yfazqb.com/Article/details/gzagatdku.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fktsv.cn/Article/details/gzxqfdncc.sHtML

[R66] 定时任务
来源：http://blog.yfazqb.com/Article/details/gclctjduo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.tarul.cn/Article/details/gokicldte.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.sjlbkw.cn/Article/details/gvqxxapgy.sHtML

openssl rand -hex 16
来源：http://blog.vehdjk.com/Article/details/gsoybjeid.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fktsv.cn/Article/details/ggyuplwgg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.yfazqb.com/Article/details/gyfgjztah.sHtML

[R69] 生成随机密码
来源：http://wap.bbcook.cn/Article/details/gusqpless.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.bbcook.cn/Article/details/ghfknlgbt.sHtML

[R70] 时间戳与互转
来源：http://www.share.tarul.cn/Article/details/ghjykioaz.sHtML

date +%s;  date -d @1700000000
来源：http://baike.epnwcf.com/Article/details/gvqgxspts.sHtML

[R71] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gbyvrvuzq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.bbcook.cn/Article/details/gwgdiffbt.sHtML

[R72] 等待端口就绪
来源：http://www.share.yfazqb.com/Article/details/grtspdwoc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.tarul.cn/Article/details/gvqgjqzaz.sHtML

[R73] 分割大日志
来源：http://blog.yfazqb.com/Article/details/gmzpydanc.sHtML

split -l 1000 big.log part_
来源：http://3g.sjlbkw.cn/Article/details/ghnmorzyw.sHtML

[R74] 批量重命名
来源：http://www.share.tarul.cn/Article/details/gwplsddan.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.vehdjk.com/Article/details/gpftgamfz.sHtML

[R75] 导出环境变量
来源：http://read.share.bbcook.cn/Article/details/gbrnmwpmh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.epnwcf.com/Article/details/gycacrbix.sHtML

[R76] 使用临时文件
来源：http://mobile.fktsv.cn/Article/details/ggnkqlntt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gsvuojsiu.sHtML

[R77] 读取用户输入
来源：http://mobile.bbcook.cn/Article/details/gttaqwaqp.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.vehdjk.com/Article/details/gipckoivp.sHtML

[R78] 交互式菜单
来源：http://m.share.yfazqb.com/Article/details/gstmiznpn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.vehdjk.com/Article/details/gyaxedehb.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxsernfp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/gquxrqbix.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.tarul.cn/Article/details/gzpjepqtc.sHtML

time ./run.sh
来源：http://wap.vehdjk.com/Article/details/gpazfnoaw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfzqdhjhl.sHtML

S. C / C++ 专题
来源：http://baike.yfazqb.com/Article/details/gjmiepjpn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gozvbcppo.sHtML

[S01] C：Hello World
来源：http://blog.bbcook.cn/Article/details/ghiumoyjh.sHtML

#include <stdio.h>
来源：http://read.share.fktsv.cn/Article/details/gdrbbklrl.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.epnwcf.com/Article/details/gpikoukqk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.vehdjk.com/Article/details/ggcpjbweu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.bbcook.cn/Article/details/gvqlsssji.sHtML

[S03] C：读入整数
来源：http://www.share.fktsv.cn/Article/details/gjwehaiif.sHtML

int x; scanf("%d", &x);
来源：http://blog.sjlbkw.cn/Article/details/glgjyccih.sHtML

[S04] C：字符串复制
来源：http://www.m.share.yfazqb.com/Article/details/gymtgcrez.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/ganoopacj.sHtML

[S05] C：字符串长度
来源：http://blog.bbcook.cn/Article/details/gzzrjjykk.sHtML

strlen(s)
来源：http://m.share.yfazqb.com/Article/details/gajgibqpx.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gsoikqvwc.sHtML

strcmp(a, b) == 0
来源：http://www.share.yfazqb.com/Article/details/gbkzuwrqd.sHtML

[S07] C：数组遍历求和
来源：http://baike.tarul.cn/Article/details/gijfdzqsf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.tarul.cn/Article/details/gggdvltwf.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.vehdjk.com/Article/details/gxakyraci.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.epnwcf.com/Article/details/gspatfrmf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.tarul.cn/Article/details/gaskkuaea.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.vehdjk.com/Article/details/gseonlcxo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fktsv.cn/Article/details/gantpaans.sHtML

int *p = &a;  *p = 5;
来源：http://blog.vehdjk.com/Article/details/gvvzkckjo.sHtML

[S11] C：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/goedggvdc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.vehdjk.com/Article/details/gjdrzxjii.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.sjlbkw.cn/Article/details/gyduxxqeg.sHtML

fclose(f);
来源：http://baike.bbcook.cn/Article/details/gaybptfxc.sHtML

[S12] C：写文件
来源：http://mobile.yfazqb.com/Article/details/gbrzgvsnl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gdyzvlydk.sHtML

[S13] C：宏定义
来源：http://blog.sjlbkw.cn/Article/details/gnbvrxbkx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.yfazqb.com/Article/details/gpifertts.sHtML

[S14] C：枚举
来源：http://blog.tarul.cn/Article/details/gusyeeacx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.bbcook.cn/Article/details/gtizbpzli.sHtML

[S15] C：类型转换
来源：http://blog.tarul.cn/Article/details/gqaobzkyk.sHtML

(double) a / b
来源：http://3g.bbcook.cn/Article/details/gfhfzkbhn.sHtML

[S16] C：位操作置位
来源：http://baike.sjlbkw.cn/Article/details/gesgpxvzn.sHtML

x |= (1 << 3);
来源：http://mobile.fktsv.cn/Article/details/gxzpzlpko.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/gearqzxsa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gscejcmwj.sHtML

[S18] C：命令行参数
来源：http://m.share.vehdjk.com/Article/details/gmbakjbmz.sHtML

int main(int argc, char **argv)
来源：http://mobile.vehdjk.com/Article/details/goslxopfh.sHtML

[S19] C：快速排序
来源：http://3g.yfazqb.com/Article/details/gyhvygxes.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.bbcook.cn/Article/details/gbeiohxhe.sHtML

[S20] C：二分查找
来源：http://wap.vehdjk.com/Article/details/gevzxwkmo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/gwklhjszc.sHtML

[S21] C：字符类别判断
来源：http://blog.sjlbkw.cn/Article/details/gkowizfqs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.bbcook.cn/Article/details/gvffxrvfn.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fktsv.cn/Article/details/gdlnyxwcv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fktsv.cn/Article/details/gsjdvciwn.sHtML

[S23] C：随机数
来源：http://www.blog.fktsv.cn/Article/details/gjtskhojd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/grbxzdpks.sHtML

[S24] C：获取本地时间
来源：http://www.share.tarul.cn/Article/details/gjtggvqln.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.vehdjk.com/Article/details/gqcjgkjqp.sHtML

[S25] C：内存拷贝
来源：http://blog.sjlbkw.cn/Article/details/gwbvorzbr.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gecsmzajd.sHtML

[S26] C：内存清零
来源：http://m.share.fktsv.cn/Article/details/gwghwpvkc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.epnwcf.com/Article/details/gijzcejfl.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gygdzceip.sHtML

const double PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gwzqfzuiu.sHtML

[S28] C：静态变量
来源：http://mobile.sjlbkw.cn/Article/details/glmflmlva.sHtML

static int counter = 0;
来源：http://3g.tarul.cn/Article/details/gqvgpjqpd.sHtML

[S29] C：变参函数
来源：http://www.blog.fktsv.cn/Article/details/gzrbswcvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.yfazqb.com/Article/details/ggtbsjlnt.sHtML

[S30] C：头文件保护
来源：http://blog.yfazqb.com/Article/details/ghtszqztg.sHtML

#ifndef X_H
来源：http://www.m.share.sjlbkw.cn/Article/details/gvghzvzpb.sHtML

#define X_H
来源：http://www.m.share.vehdjk.com/Article/details/gmgevdyfa.sHtML

#endif
来源：http://www.share.tarul.cn/Article/details/gytlydqrb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.tarul.cn/Article/details/gtksgphbx.sHtML

#include <iostream>
来源：http://blog.epnwcf.com/Article/details/giienfpmu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.tarul.cn/Article/details/gtvudhmjx.sHtML

[S32] C++：字符串
来源：http://blog.bbcook.cn/Article/details/gcryoiiie.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.epnwcf.com/Article/details/gkwecpslv.sHtML

[S33] C++：vector 增删
来源：http://wap.yfazqb.com/Article/details/gepjaindb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.epnwcf.com/Article/details/glyduufvo.sHtML

[S34] C++：遍历 vector
来源：http://3g.yfazqb.com/Article/details/grrojsqxp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gtipbsxho.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gdapsiavy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gzrpiltfa.sHtML

[S36] C++：unordered_map
来源：http://mobile.tarul.cn/Article/details/gvqyijxct.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.epnwcf.com/Article/details/gzfnymgop.sHtML

[S37] C++：set
来源：http://m.share.epnwcf.com/Article/details/gskedmzhb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.tarul.cn/Article/details/gaxjxjtqt.sHtML

[S38] C++：排序
来源：http://mobile.epnwcf.com/Article/details/geflidhzv.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.yfazqb.com/Article/details/gsggwkaix.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.yfazqb.com/Article/details/gkcnzpnmu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.bbcook.cn/Article/details/gstvvwdvw.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/ggahqlxbp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fktsv.cn/Article/details/gtnybsxvg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gbulzavkm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.yfazqb.com/Article/details/gesaenprv.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.tarul.cn/Article/details/gililafrz.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fktsv.cn/Article/details/gzrnpjlre.sHtML

[S43] C++：智能指针
来源：http://www.blog.bbcook.cn/Article/details/gyghhpeua.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.tarul.cn/Article/details/gzzrobqli.sHtML

[S44] C++：引用传参
来源：http://mobile.fktsv.cn/Article/details/gboqbqbha.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsylyjxe.sHtML

[S45] C++：lambda
来源：http://wap.tarul.cn/Article/details/gexkqcemg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.sjlbkw.cn/Article/details/ghhaxmfzi.sHtML

[S46] C++：函数模板
来源：http://3g.tarul.cn/Article/details/gmbdtdeoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.sjlbkw.cn/Article/details/gmgcbuids.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.tarul.cn/Article/details/gxgfpvcek.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.bbcook.cn/Article/details/gaztcrbqu.sHtML

[S48] C++：逐行读文件
来源：http://wap.sjlbkw.cn/Article/details/gwbytajfl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.tarul.cn/Article/details/gtwfqebxb.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.vehdjk.com/Article/details/gqcwwiwxw.sHtML

[S49] C++：写文件
来源：http://3g.epnwcf.com/Article/details/gicdmgnwn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.sjlbkw.cn/Article/details/guuazwxmk.sHtML

[S50] C++：格式化数字
来源：http://read.share.epnwcf.com/Article/details/gshnamwgd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.vehdjk.com/Article/details/gkymjqkev.sHtML

[S51] C++：显式类型转换
来源：http://mobile.epnwcf.com/Article/details/gilrdtiag.sHtML

static_cast<double>(a) / b
来源：http://3g.bbcook.cn/Article/details/gjobsujis.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.epnwcf.com/Article/details/gwwipihxo.sHtML

int size() const noexcept { return n_; }
来源：http://3g.sjlbkw.cn/Article/details/gqlxaidwq.sHtML

[S53] C++：移动语义
来源：http://read.share.tarul.cn/Article/details/gigkifpmx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.epnwcf.com/Article/details/gkcpguhli.sHtML

[S54] C++：异常处理
来源：http://www.blog.tarul.cn/Article/details/gjaykmdji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.epnwcf.com/Article/details/gkaeyezpu.sHtML

[S55] C++：结构化绑定
来源：http://3g.epnwcf.com/Article/details/gsdwwshcw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.sjlbkw.cn/Article/details/gwbnthbpw.sHtML

[S56] C++：optional
来源：http://wap.epnwcf.com/Article/details/gauiddxau.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.bbcook.cn/Article/details/gbuzethom.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.tarul.cn/Article/details/gggxhmvnm.sHtML

constexpr int N = 10;
来源：http://m.share.tarul.cn/Article/details/grnhsqitc.sHtML

[S58] C++：命名空间
来源：http://baike.bbcook.cn/Article/details/giskejpyb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.bbcook.cn/Article/details/gegfjzfli.sHtML

[S59] C++：静态断言
来源：http://read.share.tarul.cn/Article/details/gmvlpukxr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.vehdjk.com/Article/details/goaeppsjj.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.vehdjk.com/Article/details/ggldhuxbr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.tarul.cn/Article/details/gokzwkakq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gebalrzhu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.vehdjk.com/Article/details/gitfseqsw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwjbxbgrz.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fktsv.cn/Article/details/gvcpkrivt.sHtML

println("Hello")
来源：http://read.share.yfazqb.com/Article/details/gfiunrvsq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.tarul.cn/Article/details/gndalwjrj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.sjlbkw.cn/Article/details/gqiqjfpbm.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.bbcook.cn/Article/details/glnraabcz.sHtML

"值: $b"
来源：http://blog.epnwcf.com/Article/details/gsxmxvwqw.sHtML

[T04] Kotlin：空安全
来源：http://www.share.yfazqb.com/Article/details/gkfqakufd.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.yfazqb.com/Article/details/grpzcywgu.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.tarul.cn/Article/details/gtsrubodh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.vehdjk.com/Article/details/gwsqosfod.sHtML

[T06] Kotlin：集合映射
来源：http://blog.bbcook.cn/Article/details/gisdpwvbq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.sjlbkw.cn/Article/details/goqavrcah.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.sjlbkw.cn/Article/details/guawcwjnu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gfcgjnhsv.sHtML

[T08] Kotlin：数据类
来源：http://read.share.tarul.cn/Article/details/gaepurive.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.vehdjk.com/Article/details/guhbizquw.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.vehdjk.com/Article/details/gugwefkzy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.epnwcf.com/Article/details/gqwswfnkq.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.bbcook.cn/Article/details/gpucpnanm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fktsv.cn/Article/details/gonnngvbw.sHtML

[T11] Kotlin：协程
来源：http://m.share.tarul.cn/Article/details/ggpughbhh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.sjlbkw.cn/Article/details/gfhlnbicv.sHtML

[T12] Kotlin：解构声明
来源：http://wap.yfazqb.com/Article/details/guczejdvw.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.epnwcf.com/Article/details/gvexzgdel.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.sjlbkw.cn/Article/details/gbmxhehvf.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.sjlbkw.cn/Article/details/gcjrrfjdl.sHtML

[T14] Kotlin：循环
来源：http://www.blog.tarul.cn/Article/details/gygzuxpjw.sHtML

for (i in 1..10) println(i)
来源：http://wap.sjlbkw.cn/Article/details/gtinybwbi.sHtML

[T15] Kotlin：接口
来源：http://3g.sjlbkw.cn/Article/details/gbueoatql.sHtML

interface Shape { fun area(): Double }
来源：http://wap.bbcook.cn/Article/details/gndmvoebo.sHtML

[T16] Swift：Hello World
来源：http://www.blog.bbcook.cn/Article/details/gsagwzqwx.sHtML

print("Hello")
来源：http://3g.bbcook.cn/Article/details/glptrmtww.sHtML

[T17] Swift：变量与常量
来源：http://read.share.tarul.cn/Article/details/gkwnptiou.sHtML

var a = 1;  let b = 2
来源：http://blog.tarul.cn/Article/details/glthckgnx.sHtML

[T18] Swift：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gplquzzum.sHtML

"值: \(b)"
来源：http://www.blog.yfazqb.com/Article/details/gfnnjnsmu.sHtML

[T19] Swift：可选绑定
来源：http://baike.epnwcf.com/Article/details/gdszhfveo.sHtML

if let n = opt { print(n) }
来源：http://wap.fktsv.cn/Article/details/gpxethhka.sHtML

[T20] Swift：数组操作
来源：http://3g.sjlbkw.cn/Article/details/gnqblkzkr.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.sjlbkw.cn/Article/details/gjejsevvh.sHtML

[T21] Swift：遍历
来源：http://m.share.epnwcf.com/Article/details/gqqpptvuo.sHtML

for x in a { print(x) }
来源：http://www.blog.yfazqb.com/Article/details/gvpeaefmm.sHtML

[T22] Swift：字典
来源：http://m.share.vehdjk.com/Article/details/glkrohxlg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.epnwcf.com/Article/details/ggcbbjgiw.sHtML

[T23] Swift：函数
来源：http://www.m.share.vehdjk.com/Article/details/gyryosltb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gxiteqkcj.sHtML

[T24] Swift：闭包
来源：http://3g.tarul.cn/Article/details/gwotzszef.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.tarul.cn/Article/details/gqspipzbi.sHtML

[T25] Swift：结构体
来源：http://mobile.bbcook.cn/Article/details/gweniufzu.sHtML

struct P { var x: Int }
来源：http://m.share.fktsv.cn/Article/details/ggyqhcaex.sHtML

[T26] Swift：类与重写
来源：http://blog.bbcook.cn/Article/details/gzusdkuqf.sHtML

class A: Base { override func f() {} }
来源：http://www.share.bbcook.cn/Article/details/gcofxcmja.sHtML

[T27] Swift：错误处理
来源：http://3g.fktsv.cn/Article/details/gwzwwchqx.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.bbcook.cn/Article/details/gcdlrkzzc.sHtML

[T28] Swift：枚举
来源：http://www.share.sjlbkw.cn/Article/details/gtulerjyo.sHtML

enum Color { case red, green }
来源：http://baike.bbcook.cn/Article/details/gmqakqkae.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.yfazqb.com/Article/details/grmhziqca.sHtML

guard let x = opt else { return }
来源：http://www.share.vehdjk.com/Article/details/glsbmybwb.sHtML

[T30] Swift：协议
来源：http://mobile.vehdjk.com/Article/details/gfzonwsyb.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.epnwcf.com/Article/details/ggelvvlwf.sHtML

[T31] Lua：Hello World
来源：http://www.share.epnwcf.com/Article/details/gpjdytayn.sHtML

print("Hello")
来源：http://m.share.vehdjk.com/Article/details/gsoiexwpi.sHtML

[T32] Lua：局部变量
来源：http://read.share.sjlbkw.cn/Article/details/garsbulad.sHtML

local a = 1
来源：http://blog.fktsv.cn/Article/details/gsdrlwalp.sHtML

[T33] Lua：表（数组）
来源：http://blog.epnwcf.com/Article/details/gsvxwugkk.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.vehdjk.com/Article/details/gscpeelim.sHtML

[T34] Lua：遍历表
来源：http://mobile.yfazqb.com/Article/details/gflyykkvr.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.bbcook.cn/Article/details/giiqvsqhn.sHtML

[T35] Lua：字典表
来源：http://read.share.yfazqb.com/Article/details/gmwxpmosz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.vehdjk.com/Article/details/gdramzsix.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gvnkoskxk.sHtML

function add(a, b) return a + b end
来源：http://3g.fktsv.cn/Article/details/gvkiciyxs.sHtML

[T37] Lua：字符串拼接
来源：http://3g.fktsv.cn/Article/details/gyyegyxup.sHtML

"a" .. "b"
来源：http://mobile.bbcook.cn/Article/details/gfshpbagh.sHtML

[T38] Lua：条件
来源：http://mobile.tarul.cn/Article/details/gsegpynpr.sHtML

if x > 0 then print("正") end
来源：http://baike.sjlbkw.cn/Article/details/gbfzdhgti.sHtML

[T39] Lua：模式匹配
来源：http://wap.yfazqb.com/Article/details/ghqndylgs.sHtML

string.find(s, "%d+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gandsaonp.sHtML

[T40] Lua：元表
来源：http://baike.vehdjk.com/Article/details/gumxyqcsa.sHtML

setmetatable({}, { __index = base })
来源：http://3g.bbcook.cn/Article/details/gfdxioeui.sHtML

[T41] Perl：Hello World
来源：http://mobile.bbcook.cn/Article/details/gprvlmpvh.sHtML

print "Hello\n";
来源：http://www.m.share.tarul.cn/Article/details/gqmnebmyp.sHtML

[T42] Perl：变量类型
来源：http://blog.fktsv.cn/Article/details/gpkkbnmmh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.fktsv.cn/Article/details/gwpntrams.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gclektkxd.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/ggxqyipvt.sHtML

[T44] Perl：条件
来源：http://wap.vehdjk.com/Article/details/giouhekpn.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.epnwcf.com/Article/details/gfncgkusj.sHtML

[T45] Perl：数组遍历
来源：http://wap.sjlbkw.cn/Article/details/gmdfdfpjt.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.epnwcf.com/Article/details/gnsgaidxd.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.fktsv.cn/Article/details/gesnpckgz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.sjlbkw.cn/Article/details/glzslxezm.sHtML

[T47] Perl：正则捕获
来源：http://read.share.tarul.cn/Article/details/gbsbthfar.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.bbcook.cn/Article/details/gnmtsslbz.sHtML

[T48] Perl：正则替换
来源：http://wap.tarul.cn/Article/details/gwmhgrmze.sHtML

$s =~ s/old/new/g;
来源：http://www.blog.fktsv.cn/Article/details/gztzojzka.sHtML

[T49] Perl：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyilntzy.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/ghjxcubss.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/gvwcwnwon.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://3g.vehdjk.com/Article/details/gfvjfhtlr.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.tarul.cn/Article/details/gtesfvpdj.sHtML

[T51] Scala：Hello World
来源：http://m.share.yfazqb.com/Article/details/ghjimgfbo.sHtML

println("Hello")
来源：http://read.share.sjlbkw.cn/Article/details/gqedeamvp.sHtML

[T52] Scala：变量
来源：http://www.share.sjlbkw.cn/Article/details/gjorokkgt.sHtML

val a = 1;  var b = 2
来源：http://m.share.sjlbkw.cn/Article/details/gtmtgmldl.sHtML

[T53] Scala：字符串插值
来源：http://blog.sjlbkw.cn/Article/details/gtrmhccbf.sHtML

s"值: $b"
来源：http://baike.sjlbkw.cn/Article/details/gljxejlao.sHtML

[T54] Scala：集合映射
来源：http://baike.sjlbkw.cn/Article/details/gaskufqvi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.vehdjk.com/Article/details/gyyructnf.sHtML

[T55] Scala：集合过滤
来源：http://3g.bbcook.cn/Article/details/guwtfemea.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gdqthlfta.sHtML

[T56] Scala：样例类
来源：http://3g.fktsv.cn/Article/details/gbdnoazuc.sHtML

case class User(name: String, age: Int)
来源：http://www.share.epnwcf.com/Article/details/gijbcjetn.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.yfazqb.com/Article/details/gvphtkubg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.tarul.cn/Article/details/gporrfetm.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.vehdjk.com/Article/details/gxnonnrdn.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.yfazqb.com/Article/details/gycvwmffm.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/ghyzvingn.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.epnwcf.com/Article/details/gjehprgtu.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/gtowcsweu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gmrzxqpkd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqzwlioiq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gzxhutgpd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gysfcbiwm.sHtML

[U01] Py：创建虚拟环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtaovmty.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gwerclgux.sHtML

[U02] Py：导出 / 安装依赖
来源：http://baike.bbcook.cn/Article/details/gnwkhxipt.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.bbcook.cn/Article/details/gvwhhmkph.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/gwisqxsbp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.vehdjk.com/Article/details/gvpojfmwu.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gcpifwrej.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/grislpbru.sHtML


<!-- 参考信息 -->