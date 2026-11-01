代发 wailian999

free -h;  ps aux | grep nginx
来源：http://read.share.vehdjk.com/Article/details/gfiuhwkyv.sHtML

[R64] 结束进程
来源：http://mobile.vehdjk.com/Article/details/gbejvtwqv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fktsv.cn/Article/details/gmdqlrefm.sHtML

[R65] 查看端口占用
来源：http://www.share.sjlbkw.cn/Article/details/guqdyrfxr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fktsv.cn/Article/details/gcesdyfmu.sHtML

[R66] 定时任务
来源：http://read.share.bbcook.cn/Article/details/gjpusqbbo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.yfazqb.com/Article/details/gfodocxzg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.epnwcf.com/Article/details/giidazatn.sHtML

openssl rand -hex 16
来源：http://www.share.sjlbkw.cn/Article/details/glhjmebiy.sHtML

[R68] 计算文件校验值
来源：http://read.share.yfazqb.com/Article/details/gcywgwchm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.epnwcf.com/Article/details/gwvhhhlrm.sHtML

[R69] 生成随机密码
来源：http://read.share.yfazqb.com/Article/details/gyqzuhmvu.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.vehdjk.com/Article/details/glmgvtqxg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.bbcook.cn/Article/details/gfbdodxnh.sHtML

date +%s;  date -d @1700000000
来源：http://3g.tarul.cn/Article/details/gvqqoxjxd.sHtML

[R71] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gwvujyxzg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.sjlbkw.cn/Article/details/gtxqceypu.sHtML

[R72] 等待端口就绪
来源：http://3g.fktsv.cn/Article/details/gkikedvin.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gccypcsbq.sHtML

[R73] 分割大日志
来源：http://mobile.fktsv.cn/Article/details/gmpdtgsqc.sHtML

split -l 1000 big.log part_
来源：http://3g.epnwcf.com/Article/details/gewqnfrjx.sHtML

[R74] 批量重命名
来源：http://wap.fktsv.cn/Article/details/gcglznqww.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.yfazqb.com/Article/details/gypsvahou.sHtML

[R75] 导出环境变量
来源：http://baike.yfazqb.com/Article/details/gljwjroak.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdgkpjom.sHtML

[R76] 使用临时文件
来源：http://blog.bbcook.cn/Article/details/ghxdzisbn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.tarul.cn/Article/details/grxqinqnp.sHtML

[R77] 读取用户输入
来源：http://www.share.sjlbkw.cn/Article/details/gvfvuyuls.sHtML

read -rp "请输入: " ans
来源：http://baike.sjlbkw.cn/Article/details/gqpixgiat.sHtML

[R78] 交互式菜单
来源：http://www.m.share.sjlbkw.cn/Article/details/gcugsulek.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.epnwcf.com/Article/details/gmcoikdpy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.sjlbkw.cn/Article/details/gjoxqygvt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.tarul.cn/Article/details/grsycoicu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.tarul.cn/Article/details/ggtonzunj.sHtML

time ./run.sh
来源：http://read.share.sjlbkw.cn/Article/details/gswsvvsvu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gndgneidd.sHtML

S. C / C++ 专题
来源：http://blog.yfazqb.com/Article/details/galabfufh.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdwriegwu.sHtML

[S01] C：Hello World
来源：http://wap.epnwcf.com/Article/details/gsnoafvjw.sHtML

#include <stdio.h>
来源：http://m.share.sjlbkw.cn/Article/details/glvjofksu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.epnwcf.com/Article/details/gzdqmwmmg.sHtML

[S02] C：变量与格式化输出
来源：http://blog.yfazqb.com/Article/details/gsbixrifu.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.yfazqb.com/Article/details/gfcwfhdmb.sHtML

[S03] C：读入整数
来源：http://www.blog.bbcook.cn/Article/details/gsjblhksn.sHtML

int x; scanf("%d", &x);
来源：http://3g.epnwcf.com/Article/details/gjmrjyfpn.sHtML

[S04] C：字符串复制
来源：http://blog.vehdjk.com/Article/details/gofzkgitm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fktsv.cn/Article/details/gyllzxwsy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gzotowwku.sHtML

strlen(s)
来源：http://blog.fktsv.cn/Article/details/gjatpvcqk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/gsqqxyibb.sHtML

strcmp(a, b) == 0
来源：http://baike.epnwcf.com/Article/details/goowptzrd.sHtML

[S07] C：数组遍历求和
来源：http://mobile.sjlbkw.cn/Article/details/gdrsiwsmp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.vehdjk.com/Article/details/gpegtblec.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.vehdjk.com/Article/details/gpzdhjtus.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.yfazqb.com/Article/details/gzjbjmbia.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.tarul.cn/Article/details/gbdsbvhex.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.tarul.cn/Article/details/gsfcxzoxm.sHtML

[S10] C：指针与解引用
来源：http://baike.fktsv.cn/Article/details/gwiuequks.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.tarul.cn/Article/details/giwjvvtvn.sHtML

[S11] C：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/glvzbmquk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.tarul.cn/Article/details/gykgofacc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.epnwcf.com/Article/details/gnsvypuwb.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/ghljrmpog.sHtML

[S12] C：写文件
来源：http://3g.fktsv.cn/Article/details/gshaysjdf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.bbcook.cn/Article/details/gtscrkmkk.sHtML

[S13] C：宏定义
来源：http://3g.fktsv.cn/Article/details/gzcydehnq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.tarul.cn/Article/details/gwmyrmant.sHtML

[S14] C：枚举
来源：http://wap.yfazqb.com/Article/details/gjvybmlco.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.epnwcf.com/Article/details/grpdwexyy.sHtML

[S15] C：类型转换
来源：http://blog.fktsv.cn/Article/details/glqsknxkh.sHtML

(double) a / b
来源：http://3g.vehdjk.com/Article/details/ggavrxngc.sHtML

[S16] C：位操作置位
来源：http://3g.yfazqb.com/Article/details/gicaarcwi.sHtML

x |= (1 << 3);
来源：http://mobile.bbcook.cn/Article/details/gvpsobdws.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gztilexjr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.vehdjk.com/Article/details/gvdqkyzlo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gqyrpfroq.sHtML

int main(int argc, char **argv)
来源：http://baike.yfazqb.com/Article/details/gehqhvvsr.sHtML

[S19] C：快速排序
来源：http://www.blog.tarul.cn/Article/details/gktnoexkx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.yfazqb.com/Article/details/gealrtrxd.sHtML

[S20] C：二分查找
来源：http://www.share.vehdjk.com/Article/details/gdsvafves.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fktsv.cn/Article/details/ghscbhroe.sHtML

[S21] C：字符类别判断
来源：http://wap.yfazqb.com/Article/details/girulyunj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fktsv.cn/Article/details/gmdtkhpas.sHtML

[S22] C：字符串转数字
来源：http://mobile.fktsv.cn/Article/details/grrxtkpwh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.vehdjk.com/Article/details/gqirtbszg.sHtML

[S23] C：随机数
来源：http://m.share.epnwcf.com/Article/details/gvnpdiign.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fktsv.cn/Article/details/gpnlxipmn.sHtML

[S24] C：获取本地时间
来源：http://m.share.fktsv.cn/Article/details/gbpphrfsa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.vehdjk.com/Article/details/ggtgymsxa.sHtML

[S25] C：内存拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gryrutoqy.sHtML

memcpy(dst, src, n);
来源：http://mobile.sjlbkw.cn/Article/details/gvgnvhujl.sHtML

[S26] C：内存清零
来源：http://baike.tarul.cn/Article/details/ggdmkacue.sHtML

memset(a, 0, sizeof a);
来源：http://blog.tarul.cn/Article/details/ggprtqjpb.sHtML

[S27] C：定义常量
来源：http://read.share.fktsv.cn/Article/details/gnbggcnce.sHtML

const double PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/ggpngmbln.sHtML

[S28] C：静态变量
来源：http://wap.tarul.cn/Article/details/gteefvyuc.sHtML

static int counter = 0;
来源：http://www.share.yfazqb.com/Article/details/gvxpwsbsn.sHtML

[S29] C：变参函数
来源：http://baike.sjlbkw.cn/Article/details/gkgdfcznc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gkaciesft.sHtML

[S30] C：头文件保护
来源：http://m.share.tarul.cn/Article/details/gaocqdign.sHtML

#ifndef X_H
来源：http://3g.yfazqb.com/Article/details/gvvatrydb.sHtML

#define X_H
来源：http://m.share.vehdjk.com/Article/details/ggekeqcqn.sHtML

#endif
来源：http://m.share.sjlbkw.cn/Article/details/gcstagzwi.sHtML

[S31] C++：Hello World
来源：http://baike.yfazqb.com/Article/details/gkzgmnjof.sHtML

#include <iostream>
来源：http://www.m.share.vehdjk.com/Article/details/guclzgows.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.yfazqb.com/Article/details/gjbpjcteg.sHtML

[S32] C++：字符串
来源：http://read.share.bbcook.cn/Article/details/goktnkdsl.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fktsv.cn/Article/details/gjangwvhb.sHtML

[S33] C++：vector 增删
来源：http://blog.sjlbkw.cn/Article/details/gpfkkwhqy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.bbcook.cn/Article/details/gbqarshbl.sHtML

[S34] C++：遍历 vector
来源：http://wap.bbcook.cn/Article/details/gpemjzeyl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.yfazqb.com/Article/details/gylovqvbb.sHtML

[S35] C++：map
来源：http://www.m.share.vehdjk.com/Article/details/gmdzfmuet.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fktsv.cn/Article/details/gtosikzlk.sHtML

[S36] C++：unordered_map
来源：http://3g.vehdjk.com/Article/details/gqakitcil.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.epnwcf.com/Article/details/gabaxekbg.sHtML

[S37] C++：set
来源：http://3g.yfazqb.com/Article/details/gftdtfmvf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.epnwcf.com/Article/details/guzmjmacn.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gupuscmjn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fktsv.cn/Article/details/gcnmycknv.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.tarul.cn/Article/details/gyfdfegua.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.vehdjk.com/Article/details/glluyjvem.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gtriqoxjp.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.sjlbkw.cn/Article/details/gxwxxannw.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.tarul.cn/Article/details/gnuodwbbi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.epnwcf.com/Article/details/gqhrxvmnv.sHtML

[S42] C++：继承与虚函数
来源：http://blog.sjlbkw.cn/Article/details/geniioftn.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fktsv.cn/Article/details/gtonjqumz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fktsv.cn/Article/details/gibioyfsf.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.yfazqb.com/Article/details/gbfuvbtvy.sHtML

[S44] C++：引用传参
来源：http://www.blog.vehdjk.com/Article/details/ggmjiizhr.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.sjlbkw.cn/Article/details/gpilzqxis.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/gpjmhkxtx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.yfazqb.com/Article/details/gvmnfjtnk.sHtML

[S46] C++：函数模板
来源：http://mobile.sjlbkw.cn/Article/details/gubfxslii.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmjohzidh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.epnwcf.com/Article/details/gpbtjyqjy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gutqznubm.sHtML

[S48] C++：逐行读文件
来源：http://wap.fktsv.cn/Article/details/gxricgelp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/ganevjbay.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fktsv.cn/Article/details/gemamoetk.sHtML

[S49] C++：写文件
来源：http://www.blog.vehdjk.com/Article/details/glnglsqiv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.sjlbkw.cn/Article/details/gavlylqys.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.bbcook.cn/Article/details/gpaqqmnmf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/gpseryygi.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.yfazqb.com/Article/details/gshupjxme.sHtML

static_cast<double>(a) / b
来源：http://blog.vehdjk.com/Article/details/gcmwjzkpp.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gvaiatwbk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.epnwcf.com/Article/details/gkoucyflt.sHtML

[S53] C++：移动语义
来源：http://blog.bbcook.cn/Article/details/gbdrmhnbi.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fktsv.cn/Article/details/gymytjczz.sHtML

[S54] C++：异常处理
来源：http://wap.sjlbkw.cn/Article/details/gmmzobdep.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.bbcook.cn/Article/details/gnglpwqvt.sHtML

[S55] C++：结构化绑定
来源：http://m.share.sjlbkw.cn/Article/details/glzylhmfc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.bbcook.cn/Article/details/gchmmbqdd.sHtML

[S56] C++：optional
来源：http://www.m.share.vehdjk.com/Article/details/gobvmhnjm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.bbcook.cn/Article/details/glvzxjkit.sHtML

[S57] C++：编译期常量
来源：http://3g.yfazqb.com/Article/details/gdvjpdrrl.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gwlgqgxkk.sHtML

[S58] C++：命名空间
来源：http://wap.bbcook.cn/Article/details/gbdjmvmpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.tarul.cn/Article/details/gznwgwqmq.sHtML

[S59] C++：静态断言
来源：http://3g.vehdjk.com/Article/details/gsusegmnd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.epnwcf.com/Article/details/gsoeesirk.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.yfazqb.com/Article/details/gphkbjctc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.sjlbkw.cn/Article/details/ggjvzwtye.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwwbdiayh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gkwzyiotj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpwpyngvm.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.sjlbkw.cn/Article/details/glfmzkoqk.sHtML

println("Hello")
来源：http://wap.bbcook.cn/Article/details/gzuxsaezv.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.vehdjk.com/Article/details/gisgofldm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.tarul.cn/Article/details/gdnbbgckp.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.tarul.cn/Article/details/gcriefroa.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gupiqimqz.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fktsv.cn/Article/details/gxkosfaeb.sHtML

val n: String? = null;  n?.length
来源：http://blog.sjlbkw.cn/Article/details/gmwqiaixv.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.bbcook.cn/Article/details/giliphlxf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.yfazqb.com/Article/details/gywbdoxql.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.yfazqb.com/Article/details/gbmbyhrlv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.yfazqb.com/Article/details/gkaoinvxe.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.sjlbkw.cn/Article/details/glxjonosk.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.yfazqb.com/Article/details/giuevgpkm.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gqxbyeulp.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.sjlbkw.cn/Article/details/gkxkvoamy.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.epnwcf.com/Article/details/gtwollybc.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.sjlbkw.cn/Article/details/gmlzvhzhc.sHtML

[T10] Kotlin：默认参数
来源：http://wap.vehdjk.com/Article/details/ghxfywshk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.yfazqb.com/Article/details/gqhuaosip.sHtML

[T11] Kotlin：协程
来源：http://read.share.tarul.cn/Article/details/gfhqzxski.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fktsv.cn/Article/details/gtcnphlqp.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.bbcook.cn/Article/details/guweadmto.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.tarul.cn/Article/details/gxqfnvdkj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.vehdjk.com/Article/details/gdebmroyz.sHtML

val m = mapOf("a" to 1)
来源：http://blog.bbcook.cn/Article/details/gkceohzvd.sHtML

[T14] Kotlin：循环
来源：http://wap.vehdjk.com/Article/details/grzdvntya.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fktsv.cn/Article/details/gtliptwab.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fktsv.cn/Article/details/gbalatypd.sHtML

interface Shape { fun area(): Double }
来源：http://3g.vehdjk.com/Article/details/gmgvcgpjj.sHtML

[T16] Swift：Hello World
来源：http://m.share.fktsv.cn/Article/details/gxgrdcmuk.sHtML

print("Hello")
来源：http://baike.vehdjk.com/Article/details/gniqvdovw.sHtML

[T17] Swift：变量与常量
来源：http://blog.yfazqb.com/Article/details/geictyusc.sHtML

var a = 1;  let b = 2
来源：http://3g.fktsv.cn/Article/details/grsdnqwce.sHtML

[T18] Swift：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gvwrzbvyk.sHtML

"值: \(b)"
来源：http://3g.sjlbkw.cn/Article/details/glkvopwiw.sHtML

[T19] Swift：可选绑定
来源：http://mobile.sjlbkw.cn/Article/details/gltyfscew.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fktsv.cn/Article/details/gxflssxuq.sHtML

[T20] Swift：数组操作
来源：http://baike.epnwcf.com/Article/details/gbnsvvmxw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.bbcook.cn/Article/details/gpjqeivvo.sHtML

[T21] Swift：遍历
来源：http://read.share.sjlbkw.cn/Article/details/gifaermpd.sHtML

for x in a { print(x) }
来源：http://www.m.share.vehdjk.com/Article/details/geqjnnjdr.sHtML

[T22] Swift：字典
来源：http://www.share.epnwcf.com/Article/details/gcewwxiwg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.bbcook.cn/Article/details/gwrpotend.sHtML

[T23] Swift：函数
来源：http://mobile.vehdjk.com/Article/details/gethxqinp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.epnwcf.com/Article/details/gykdffycy.sHtML

[T24] Swift：闭包
来源：http://m.share.fktsv.cn/Article/details/gsrotllxb.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.vehdjk.com/Article/details/ggkkoimvr.sHtML

[T25] Swift：结构体
来源：http://baike.fktsv.cn/Article/details/gpfgcajvb.sHtML

struct P { var x: Int }
来源：http://www.blog.vehdjk.com/Article/details/gjjpqqfav.sHtML

[T26] Swift：类与重写
来源：http://3g.sjlbkw.cn/Article/details/gowxwfssr.sHtML

class A: Base { override func f() {} }
来源：http://wap.bbcook.cn/Article/details/ghlxnqpqn.sHtML

[T27] Swift：错误处理
来源：http://wap.yfazqb.com/Article/details/gydiffbtx.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.bbcook.cn/Article/details/gqqduqvrx.sHtML

[T28] Swift：枚举
来源：http://www.blog.epnwcf.com/Article/details/gylxyynda.sHtML

enum Color { case red, green }
来源：http://m.share.vehdjk.com/Article/details/ggrjiskry.sHtML

[T29] Swift：guard 提前返回
来源：http://www.share.fktsv.cn/Article/details/gwnlvokzi.sHtML

guard let x = opt else { return }
来源：http://www.blog.fktsv.cn/Article/details/gybqsqgsy.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/ghjdghvkc.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.sjlbkw.cn/Article/details/gurjvrumc.sHtML

[T31] Lua：Hello World
来源：http://blog.epnwcf.com/Article/details/gvcuuxrjy.sHtML

print("Hello")
来源：http://m.share.bbcook.cn/Article/details/gevgevkcl.sHtML

[T32] Lua：局部变量
来源：http://3g.sjlbkw.cn/Article/details/gxmexwwtk.sHtML

local a = 1
来源：http://m.share.bbcook.cn/Article/details/gpbfdobli.sHtML

[T33] Lua：表（数组）
来源：http://mobile.bbcook.cn/Article/details/gyjnphrrs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fktsv.cn/Article/details/gtalpnrmf.sHtML

[T34] Lua：遍历表
来源：http://www.blog.epnwcf.com/Article/details/godultoxn.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.vehdjk.com/Article/details/geumktkub.sHtML

[T35] Lua：字典表
来源：http://blog.bbcook.cn/Article/details/goixghzgg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fktsv.cn/Article/details/gwpbhjatw.sHtML

[T36] Lua：函数
来源：http://blog.bbcook.cn/Article/details/gpnbsbufp.sHtML

function add(a, b) return a + b end
来源：http://baike.vehdjk.com/Article/details/gqbhctdox.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gpjvxhezd.sHtML

"a" .. "b"
来源：http://3g.bbcook.cn/Article/details/gwltbrzof.sHtML

[T38] Lua：条件
来源：http://wap.epnwcf.com/Article/details/givnmssuq.sHtML

if x > 0 then print("正") end
来源：http://blog.epnwcf.com/Article/details/glopqsvcs.sHtML

[T39] Lua：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gwfzotkkt.sHtML

string.find(s, "%d+")
来源：http://read.share.epnwcf.com/Article/details/gqwaonwcz.sHtML

[T40] Lua：元表
来源：http://wap.bbcook.cn/Article/details/gtngiailr.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.tarul.cn/Article/details/gnojwaskq.sHtML

[T41] Perl：Hello World
来源：http://www.share.vehdjk.com/Article/details/ggsnkonis.sHtML

print "Hello\n";
来源：http://www.blog.epnwcf.com/Article/details/gjmbigvbm.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.tarul.cn/Article/details/gbqambxny.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.epnwcf.com/Article/details/ggyeyixjr.sHtML

[T43] Perl：字符串插值
来源：http://blog.tarul.cn/Article/details/gaxibalse.sHtML

"值: $a"
来源：http://m.share.epnwcf.com/Article/details/gskxurjtq.sHtML

[T44] Perl：条件
来源：http://www.share.epnwcf.com/Article/details/gebwdizbq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.epnwcf.com/Article/details/guudvgtbg.sHtML

[T45] Perl：数组遍历
来源：http://wap.vehdjk.com/Article/details/gakqqistx.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.tarul.cn/Article/details/ggqanuysc.sHtML

[T46] Perl：哈希操作
来源：http://mobile.epnwcf.com/Article/details/gbdebynhw.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.bbcook.cn/Article/details/gqqgbclcy.sHtML

[T47] Perl：正则捕获
来源：http://blog.bbcook.cn/Article/details/ghshkpwof.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbljctty.sHtML

[T48] Perl：正则替换
来源：http://www.share.fktsv.cn/Article/details/gwtufasvp.sHtML

$s =~ s/old/new/g;
来源：http://m.share.yfazqb.com/Article/details/gzoqcuiyx.sHtML

[T49] Perl：函数
来源：http://www.blog.vehdjk.com/Article/details/gktspqieu.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gbhbcmcmx.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.tarul.cn/Article/details/gihwmpttx.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.sjlbkw.cn/Article/details/gmkvjmfju.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.bbcook.cn/Article/details/ggqpuicqs.sHtML

[T51] Scala：Hello World
来源：http://blog.vehdjk.com/Article/details/gsbgxkbzk.sHtML

println("Hello")
来源：http://www.blog.fktsv.cn/Article/details/gsvzbqbbz.sHtML

[T52] Scala：变量
来源：http://wap.epnwcf.com/Article/details/gjxybepws.sHtML

val a = 1;  var b = 2
来源：http://mobile.bbcook.cn/Article/details/gngtpqlsv.sHtML

[T53] Scala：字符串插值
来源：http://www.share.tarul.cn/Article/details/gewczrild.sHtML

s"值: $b"
来源：http://www.share.yfazqb.com/Article/details/gtfxdudyf.sHtML

[T54] Scala：集合映射
来源：http://read.share.yfazqb.com/Article/details/gvmgucvmp.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.epnwcf.com/Article/details/glanijogg.sHtML

[T55] Scala：集合过滤
来源：http://mobile.sjlbkw.cn/Article/details/gammwqlih.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.epnwcf.com/Article/details/gcblckbzt.sHtML

[T56] Scala：样例类
来源：http://3g.bbcook.cn/Article/details/gtfnweqnj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.tarul.cn/Article/details/gsphpdsvu.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fktsv.cn/Article/details/gfazkiwzi.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.bbcook.cn/Article/details/gedsqcjba.sHtML

[T58] Scala：函数定义
来源：http://m.share.vehdjk.com/Article/details/grhsrsaqp.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gkhopdsks.sHtML

[T59] Scala：循环
来源：http://3g.bbcook.cn/Article/details/gmsafmedd.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.tarul.cn/Article/details/ggiwrjvtz.sHtML

[T60] Scala：折叠
来源：http://www.share.sjlbkw.cn/Article/details/giminlrrf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.sjlbkw.cn/Article/details/gnjdnndfm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gawzufolq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.epnwcf.com/Article/details/grtownehi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gagchassy.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.fktsv.cn/Article/details/gdhjwksgu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://baike.epnwcf.com/Article/details/gfealybse.sHtML

[U02] Py：导出 / 安装依赖
来源：http://read.share.yfazqb.com/Article/details/glifckjyn.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.tarul.cn/Article/details/gqtrbfthy.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.vehdjk.com/Article/details/givsylmzs.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.sjlbkw.cn/Article/details/gilaykhwj.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gmdcvwopm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.fktsv.cn/Article/details/gciayelfn.sHtML


<!-- 参考信息 -->