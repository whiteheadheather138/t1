代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.vehdjk.com/Article/details/ghaoryisy.sHtML

[R66] 定时任务
来源：http://3g.tarul.cn/Article/details/gyhqxqcym.sHtML

crontab -e;  crontab -l
来源：http://blog.yfazqb.com/Article/details/gvcasnuqo.sHtML

[R67] 生成随机十六进制串
来源：http://3g.bbcook.cn/Article/details/gqlshbces.sHtML

openssl rand -hex 16
来源：http://www.blog.epnwcf.com/Article/details/gmyyxlbwz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.epnwcf.com/Article/details/guybnhpjq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.yfazqb.com/Article/details/gupcydfuz.sHtML

[R69] 生成随机密码
来源：http://blog.sjlbkw.cn/Article/details/gvjjcfpax.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.epnwcf.com/Article/details/gqplyndmf.sHtML

[R70] 时间戳与互转
来源：http://3g.sjlbkw.cn/Article/details/gkkewpjrc.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fktsv.cn/Article/details/gqjjwuuyt.sHtML

[R71] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gwwqazxqq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fktsv.cn/Article/details/gjpaixzif.sHtML

[R72] 等待端口就绪
来源：http://blog.epnwcf.com/Article/details/gxcmldppw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/ghfvfohpb.sHtML

[R73] 分割大日志
来源：http://read.share.tarul.cn/Article/details/gpmmntuay.sHtML

split -l 1000 big.log part_
来源：http://www.blog.vehdjk.com/Article/details/gpxtdhmpr.sHtML

[R74] 批量重命名
来源：http://wap.tarul.cn/Article/details/gwrhniash.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.sjlbkw.cn/Article/details/ghfqewtrp.sHtML

[R75] 导出环境变量
来源：http://wap.tarul.cn/Article/details/gapivqxtg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.tarul.cn/Article/details/gxfyuibud.sHtML

[R76] 使用临时文件
来源：http://m.share.epnwcf.com/Article/details/gmiuaqcts.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/ggfxdgpkk.sHtML

[R77] 读取用户输入
来源：http://3g.bbcook.cn/Article/details/gnsmokkxo.sHtML

read -rp "请输入: " ans
来源：http://mobile.bbcook.cn/Article/details/goooxkumj.sHtML

[R78] 交互式菜单
来源：http://mobile.tarul.cn/Article/details/gvaiuqrvl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.sjlbkw.cn/Article/details/guaudhyfp.sHtML

[R79] 解析命令行选项
来源：http://www.blog.tarul.cn/Article/details/grrtdoghc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.sjlbkw.cn/Article/details/gcrpwhiio.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fktsv.cn/Article/details/gqvsjlibq.sHtML

time ./run.sh
来源：http://www.share.tarul.cn/Article/details/gtovdknnw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gstvairit.sHtML

S. C / C++ 专题
来源：http://www.m.share.tarul.cn/Article/details/gpvvvuonp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gydpglhkl.sHtML

[S01] C：Hello World
来源：http://3g.yfazqb.com/Article/details/gfyryiqqr.sHtML

#include <stdio.h>
来源：http://baike.tarul.cn/Article/details/gainzlukp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.tarul.cn/Article/details/gywrgaomf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.epnwcf.com/Article/details/gjngircew.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.yfazqb.com/Article/details/gluotobyg.sHtML

[S03] C：读入整数
来源：http://mobile.bbcook.cn/Article/details/gaktubpiv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.vehdjk.com/Article/details/ghvlklgiy.sHtML

[S04] C：字符串复制
来源：http://3g.vehdjk.com/Article/details/gpywprlww.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.bbcook.cn/Article/details/gvjsbzofi.sHtML

[S05] C：字符串长度
来源：http://blog.vehdjk.com/Article/details/gasjvfmmd.sHtML

strlen(s)
来源：http://m.share.sjlbkw.cn/Article/details/ggrilkuch.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gpggrtmvw.sHtML

strcmp(a, b) == 0
来源：http://wap.vehdjk.com/Article/details/gpkbjgbpz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.vehdjk.com/Article/details/guxpqsswr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gdkxpihft.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.epnwcf.com/Article/details/gkafryxpo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.sjlbkw.cn/Article/details/giswktuxd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fktsv.cn/Article/details/gbtsfziol.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.epnwcf.com/Article/details/gjszuziif.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gbcgvvvtn.sHtML

int *p = &a;  *p = 5;
来源：http://wap.epnwcf.com/Article/details/gxizaobxe.sHtML

[S11] C：逐行读文件
来源：http://blog.vehdjk.com/Article/details/gqrzikkjy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fktsv.cn/Article/details/gkauyjknf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.sjlbkw.cn/Article/details/gnhjybezo.sHtML

fclose(f);
来源：http://mobile.epnwcf.com/Article/details/glzmlwzse.sHtML

[S12] C：写文件
来源：http://3g.bbcook.cn/Article/details/gjjzwnnzp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/glzjdnpim.sHtML

[S13] C：宏定义
来源：http://www.blog.fktsv.cn/Article/details/ghyafbtfh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.vehdjk.com/Article/details/giijounqa.sHtML

[S14] C：枚举
来源：http://blog.yfazqb.com/Article/details/glafhrofc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.vehdjk.com/Article/details/gagupwurn.sHtML

[S15] C：类型转换
来源：http://mobile.fktsv.cn/Article/details/ggnpuubss.sHtML

(double) a / b
来源：http://www.blog.epnwcf.com/Article/details/ghhxdgdzg.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gkuvqejtb.sHtML

x |= (1 << 3);
来源：http://mobile.vehdjk.com/Article/details/gcsgwcmjg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gphjkbjfw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.bbcook.cn/Article/details/ggfrrmvbf.sHtML

[S18] C：命令行参数
来源：http://www.share.sjlbkw.cn/Article/details/gcqazdres.sHtML

int main(int argc, char **argv)
来源：http://www.share.tarul.cn/Article/details/grlqyfysn.sHtML

[S19] C：快速排序
来源：http://baike.sjlbkw.cn/Article/details/gxicsqgja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.sjlbkw.cn/Article/details/ghrmneeih.sHtML

[S20] C：二分查找
来源：http://www.m.share.bbcook.cn/Article/details/gxbdlyxah.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.bbcook.cn/Article/details/gmzmhindf.sHtML

[S21] C：字符类别判断
来源：http://baike.bbcook.cn/Article/details/gxquzlfat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fktsv.cn/Article/details/gefennqtm.sHtML

[S22] C：字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/ggufcnmhg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.epnwcf.com/Article/details/gqbdwlsdm.sHtML

[S23] C：随机数
来源：http://baike.tarul.cn/Article/details/gbixnvhtj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fktsv.cn/Article/details/grlgzsahc.sHtML

[S24] C：获取本地时间
来源：http://read.share.sjlbkw.cn/Article/details/gzgrfakwc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.bbcook.cn/Article/details/gukbqwxad.sHtML

[S25] C：内存拷贝
来源：http://blog.vehdjk.com/Article/details/gawbrhdxx.sHtML

memcpy(dst, src, n);
来源：http://blog.epnwcf.com/Article/details/gpyaxgyiu.sHtML

[S26] C：内存清零
来源：http://mobile.yfazqb.com/Article/details/goggtmjdp.sHtML

memset(a, 0, sizeof a);
来源：http://wap.bbcook.cn/Article/details/grjdupjkr.sHtML

[S27] C：定义常量
来源：http://www.blog.fktsv.cn/Article/details/gristdfaq.sHtML

const double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gwxhylpvf.sHtML

[S28] C：静态变量
来源：http://m.share.sjlbkw.cn/Article/details/gzyxhokyw.sHtML

static int counter = 0;
来源：http://www.blog.tarul.cn/Article/details/gsipvsnck.sHtML

[S29] C：变参函数
来源：http://www.blog.bbcook.cn/Article/details/gvnwocwit.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.epnwcf.com/Article/details/gxvyekbbe.sHtML

[S30] C：头文件保护
来源：http://www.share.bbcook.cn/Article/details/gmsarvhrj.sHtML

#ifndef X_H
来源：http://blog.epnwcf.com/Article/details/gqjsihwdg.sHtML

#define X_H
来源：http://read.share.yfazqb.com/Article/details/gimpooosn.sHtML

#endif
来源：http://wap.sjlbkw.cn/Article/details/gvxzexfbg.sHtML

[S31] C++：Hello World
来源：http://3g.fktsv.cn/Article/details/gkhllhuyv.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gfelugdnn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.vehdjk.com/Article/details/gtvzdcttf.sHtML

[S32] C++：字符串
来源：http://3g.fktsv.cn/Article/details/gwdukdmch.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.tarul.cn/Article/details/gzuqgtxqq.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.tarul.cn/Article/details/gwdhmqhzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.yfazqb.com/Article/details/gjesecmnx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.sjlbkw.cn/Article/details/gaujeceos.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gbjveivjf.sHtML

[S35] C++：map
来源：http://wap.bbcook.cn/Article/details/glkuvtaga.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gbgarzotp.sHtML

[S36] C++：unordered_map
来源：http://m.share.fktsv.cn/Article/details/gfrcmneqy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.epnwcf.com/Article/details/gydkrwglq.sHtML

[S37] C++：set
来源：http://m.share.tarul.cn/Article/details/gkdjdbdxs.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fktsv.cn/Article/details/gsrgpngof.sHtML

[S38] C++：排序
来源：http://www.share.fktsv.cn/Article/details/gbyjalajc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.yfazqb.com/Article/details/gxajgktrl.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.bbcook.cn/Article/details/gfgrnavky.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.vehdjk.com/Article/details/gvvtoqjdm.sHtML

[S40] C++：查找元素
来源：http://www.share.yfazqb.com/Article/details/gnnemwpup.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.bbcook.cn/Article/details/ghcnxipkb.sHtML

[S41] C++：类与构造函数
来源：http://baike.fktsv.cn/Article/details/gofcplcxh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fktsv.cn/Article/details/gtnrcrmyw.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.vehdjk.com/Article/details/gwncuhxrh.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.sjlbkw.cn/Article/details/gkciqksur.sHtML

[S43] C++：智能指针
来源：http://baike.yfazqb.com/Article/details/gvgxmmruq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.yfazqb.com/Article/details/gzcvnzlzv.sHtML

[S44] C++：引用传参
来源：http://baike.epnwcf.com/Article/details/goomcgfzq.sHtML

void inc(int &x) { ++x; }
来源：http://blog.epnwcf.com/Article/details/gxknceevq.sHtML

[S45] C++：lambda
来源：http://wap.epnwcf.com/Article/details/ggkjhyenj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.vehdjk.com/Article/details/gtylsbtxj.sHtML

[S46] C++：函数模板
来源：http://m.share.tarul.cn/Article/details/gywgvqgop.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.vehdjk.com/Article/details/gpxxulwsv.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.sjlbkw.cn/Article/details/glgozrzet.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.bbcook.cn/Article/details/gpfgbvxbn.sHtML

[S48] C++：逐行读文件
来源：http://blog.fktsv.cn/Article/details/gepqmdhvw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.bbcook.cn/Article/details/geaqntbsr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.vehdjk.com/Article/details/giabvsjmv.sHtML

[S49] C++：写文件
来源：http://www.blog.epnwcf.com/Article/details/gxsqzixss.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fktsv.cn/Article/details/gwrryyccu.sHtML

[S50] C++：格式化数字
来源：http://m.share.fktsv.cn/Article/details/gegtzeizw.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gpuwhvxjp.sHtML

[S51] C++：显式类型转换
来源：http://wap.fktsv.cn/Article/details/gdqpiwxzv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.tarul.cn/Article/details/glrmkxngt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.vehdjk.com/Article/details/gfzrdoato.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fktsv.cn/Article/details/gyntaincg.sHtML

[S53] C++：移动语义
来源：http://wap.yfazqb.com/Article/details/gawcxslae.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.epnwcf.com/Article/details/gfwgrjqtk.sHtML

[S54] C++：异常处理
来源：http://www.share.bbcook.cn/Article/details/gqugmycie.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.yfazqb.com/Article/details/goqyxevdr.sHtML

[S55] C++：结构化绑定
来源：http://baike.tarul.cn/Article/details/gobzoihog.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fktsv.cn/Article/details/glzkgbpox.sHtML

[S56] C++：optional
来源：http://3g.bbcook.cn/Article/details/geqzvstaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fktsv.cn/Article/details/glzfurohm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.epnwcf.com/Article/details/gksdoyaqm.sHtML

constexpr int N = 10;
来源：http://m.share.vehdjk.com/Article/details/gixaplxdm.sHtML

[S58] C++：命名空间
来源：http://read.share.bbcook.cn/Article/details/gqoykgjik.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.sjlbkw.cn/Article/details/glopmyice.sHtML

[S59] C++：静态断言
来源：http://baike.vehdjk.com/Article/details/gifktwabl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.epnwcf.com/Article/details/gtoovmtug.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.epnwcf.com/Article/details/gcvklnygw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.vehdjk.com/Article/details/gsovurrgc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbpjzdfnh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.sjlbkw.cn/Article/details/gplnasicf.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grzkzwbqz.sHtML

[T01] Kotlin：Hello World
来源：http://wap.sjlbkw.cn/Article/details/gybbvhqal.sHtML

println("Hello")
来源：http://www.share.tarul.cn/Article/details/githqibzo.sHtML

[T02] Kotlin：变量
来源：http://wap.sjlbkw.cn/Article/details/gietvhfqw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.bbcook.cn/Article/details/gvngycpqk.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/godldttoz.sHtML

"值: $b"
来源：http://www.share.yfazqb.com/Article/details/grbphwezj.sHtML

[T04] Kotlin：空安全
来源：http://wap.sjlbkw.cn/Article/details/gpmnrsqob.sHtML

val n: String? = null;  n?.length
来源：http://baike.fktsv.cn/Article/details/guffwslwg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.tarul.cn/Article/details/ghgkksxku.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.sjlbkw.cn/Article/details/gzgdgspny.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.sjlbkw.cn/Article/details/guanuqxdm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fktsv.cn/Article/details/gasbozuyz.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fktsv.cn/Article/details/gowtnjkmm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.bbcook.cn/Article/details/gtnsfndft.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.tarul.cn/Article/details/gpmeamqbc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.bbcook.cn/Article/details/gufkfduck.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.tarul.cn/Article/details/ghgtrghaf.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.epnwcf.com/Article/details/gcxncdtje.sHtML

[T10] Kotlin：默认参数
来源：http://baike.bbcook.cn/Article/details/grlwpypen.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.sjlbkw.cn/Article/details/gpjyaflpe.sHtML

[T11] Kotlin：协程
来源：http://m.share.yfazqb.com/Article/details/gjhbvaeyc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fktsv.cn/Article/details/gzdgrpoyg.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.yfazqb.com/Article/details/geombfiwq.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gpjyhgcdk.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.yfazqb.com/Article/details/gexiubryr.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fktsv.cn/Article/details/gjmvezyoa.sHtML

[T14] Kotlin：循环
来源：http://www.share.tarul.cn/Article/details/guglwvvue.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fktsv.cn/Article/details/glhxyzoxg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.tarul.cn/Article/details/gqbksqckg.sHtML

interface Shape { fun area(): Double }
来源：http://3g.sjlbkw.cn/Article/details/gmivqyqka.sHtML

[T16] Swift：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gpmbnasol.sHtML

print("Hello")
来源：http://baike.bbcook.cn/Article/details/gqywrplaq.sHtML

[T17] Swift：变量与常量
来源：http://wap.vehdjk.com/Article/details/gemzftlls.sHtML

var a = 1;  let b = 2
来源：http://www.blog.vehdjk.com/Article/details/gueutptil.sHtML

[T18] Swift：字符串插值
来源：http://read.share.epnwcf.com/Article/details/gzzbotkla.sHtML

"值: \(b)"
来源：http://www.blog.epnwcf.com/Article/details/gaqhdfvjm.sHtML

[T19] Swift：可选绑定
来源：http://mobile.bbcook.cn/Article/details/gaolzwcgv.sHtML

if let n = opt { print(n) }
来源：http://m.share.epnwcf.com/Article/details/gramxwexi.sHtML

[T20] Swift：数组操作
来源：http://blog.fktsv.cn/Article/details/glajjznek.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.tarul.cn/Article/details/gfbwjebup.sHtML

[T21] Swift：遍历
来源：http://blog.bbcook.cn/Article/details/grcekyndl.sHtML

for x in a { print(x) }
来源：http://blog.tarul.cn/Article/details/gfbqfjdwi.sHtML

[T22] Swift：字典
来源：http://blog.tarul.cn/Article/details/ggoplcecm.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.epnwcf.com/Article/details/gsnhjnfaw.sHtML

[T23] Swift：函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwlvplgd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.vehdjk.com/Article/details/gpyzeybce.sHtML

[T24] Swift：闭包
来源：http://mobile.vehdjk.com/Article/details/gfvnfeiui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gpgiztpar.sHtML

[T25] Swift：结构体
来源：http://read.share.epnwcf.com/Article/details/ghczwfrpv.sHtML

struct P { var x: Int }
来源：http://mobile.sjlbkw.cn/Article/details/gsfqdpypl.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.vehdjk.com/Article/details/grknjzvgb.sHtML

class A: Base { override func f() {} }
来源：http://baike.epnwcf.com/Article/details/gguakvill.sHtML

[T27] Swift：错误处理
来源：http://mobile.tarul.cn/Article/details/ghnorjncp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.tarul.cn/Article/details/gqrhwixcz.sHtML

[T28] Swift：枚举
来源：http://mobile.epnwcf.com/Article/details/gqxjdfvgg.sHtML

enum Color { case red, green }
来源：http://m.share.tarul.cn/Article/details/gsalizzqn.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.vehdjk.com/Article/details/gkisfwslf.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gjzkgfnnh.sHtML

[T30] Swift：协议
来源：http://www.blog.fktsv.cn/Article/details/gdphvwjqo.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.yfazqb.com/Article/details/gfohawfdf.sHtML

[T31] Lua：Hello World
来源：http://m.share.yfazqb.com/Article/details/gqlgkyrwh.sHtML

print("Hello")
来源：http://3g.yfazqb.com/Article/details/grvzlyhpu.sHtML

[T32] Lua：局部变量
来源：http://baike.tarul.cn/Article/details/gbhisqhbi.sHtML

local a = 1
来源：http://m.share.epnwcf.com/Article/details/gxylhdoui.sHtML

[T33] Lua：表（数组）
来源：http://3g.vehdjk.com/Article/details/gauxdtcow.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.epnwcf.com/Article/details/gpgpandqp.sHtML

[T34] Lua：遍历表
来源：http://wap.fktsv.cn/Article/details/glduvcnsi.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.sjlbkw.cn/Article/details/ggtdiflxq.sHtML

[T35] Lua：字典表
来源：http://mobile.bbcook.cn/Article/details/ghdduwhlk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.bbcook.cn/Article/details/gvrorxeyd.sHtML

[T36] Lua：函数
来源：http://www.share.sjlbkw.cn/Article/details/glcvexdvu.sHtML

function add(a, b) return a + b end
来源：http://wap.bbcook.cn/Article/details/gxhkdlzlw.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gluawkgss.sHtML

"a" .. "b"
来源：http://3g.yfazqb.com/Article/details/gasgyfvmz.sHtML

[T38] Lua：条件
来源：http://www.share.epnwcf.com/Article/details/gpfnxhjzq.sHtML

if x > 0 then print("正") end
来源：http://m.share.tarul.cn/Article/details/gybjeqgav.sHtML

[T39] Lua：模式匹配
来源：http://3g.yfazqb.com/Article/details/gaceortju.sHtML

string.find(s, "%d+")
来源：http://www.share.epnwcf.com/Article/details/gmzbgrwqr.sHtML

[T40] Lua：元表
来源：http://www.blog.epnwcf.com/Article/details/gipnsshpx.sHtML

setmetatable({}, { __index = base })
来源：http://wap.epnwcf.com/Article/details/grhvquqtg.sHtML

[T41] Perl：Hello World
来源：http://blog.fktsv.cn/Article/details/gzhkzcytx.sHtML

print "Hello\n";
来源：http://baike.tarul.cn/Article/details/gnfnwawsk.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fktsv.cn/Article/details/gmtssvshj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.epnwcf.com/Article/details/gjsxydvwr.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.yfazqb.com/Article/details/gzxjwnkou.sHtML

"值: $a"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpddwydu.sHtML

[T44] Perl：条件
来源：http://mobile.bbcook.cn/Article/details/gwjgfrzvm.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.sjlbkw.cn/Article/details/gegoytitd.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.epnwcf.com/Article/details/gucmmbzuv.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.tarul.cn/Article/details/gxclqbtyd.sHtML

[T46] Perl：哈希操作
来源：http://blog.sjlbkw.cn/Article/details/gktryefdc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.yfazqb.com/Article/details/gwjmmuhpr.sHtML

[T47] Perl：正则捕获
来源：http://m.share.tarul.cn/Article/details/ghhtjrcya.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://baike.sjlbkw.cn/Article/details/gxleorznx.sHtML

[T48] Perl：正则替换
来源：http://read.share.epnwcf.com/Article/details/gpflwedwb.sHtML

$s =~ s/old/new/g;
来源：http://blog.tarul.cn/Article/details/gegfhjjzr.sHtML

[T49] Perl：函数
来源：http://read.share.vehdjk.com/Article/details/gdbpieamb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.bbcook.cn/Article/details/gdljfluqa.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gprflqcuu.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.yfazqb.com/Article/details/gabkedrxh.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.bbcook.cn/Article/details/gjjvioudb.sHtML

[T51] Scala：Hello World
来源：http://baike.epnwcf.com/Article/details/grgvlljcq.sHtML

println("Hello")
来源：http://read.share.tarul.cn/Article/details/gkifytiiv.sHtML

[T52] Scala：变量
来源：http://baike.yfazqb.com/Article/details/gazmuihwp.sHtML

val a = 1;  var b = 2
来源：http://read.share.fktsv.cn/Article/details/gabspdnok.sHtML

[T53] Scala：字符串插值
来源：http://mobile.epnwcf.com/Article/details/gnxpppnbj.sHtML

s"值: $b"
来源：http://read.share.yfazqb.com/Article/details/gmejhvqck.sHtML

[T54] Scala：集合映射
来源：http://blog.tarul.cn/Article/details/gbowbagpu.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbrurxhda.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.yfazqb.com/Article/details/gsjqrtupg.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.yfazqb.com/Article/details/gwsbuzxkn.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gfbrcxwnq.sHtML

case class User(name: String, age: Int)
来源：http://www.share.fktsv.cn/Article/details/gkbfhlfay.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.yfazqb.com/Article/details/gainsothh.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.vehdjk.com/Article/details/gfbbrvczh.sHtML

[T58] Scala：函数定义
来源：http://m.share.bbcook.cn/Article/details/ggjuwagwd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.vehdjk.com/Article/details/glrtrhdud.sHtML

[T59] Scala：循环
来源：http://www.share.bbcook.cn/Article/details/gbfudhdmw.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.blog.sjlbkw.cn/Article/details/gnftgwtxt.sHtML

[T60] Scala：折叠
来源：http://www.m.share.epnwcf.com/Article/details/gdiseewrg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fktsv.cn/Article/details/gtscxxyrz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwpijbaea.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.vehdjk.com/Article/details/gezxtjoog.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/grfdckxpg.sHtML

[U01] Py：创建虚拟环境
来源：http://wap.tarul.cn/Article/details/geazjgekk.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.epnwcf.com/Article/details/gzqlcqgsv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/ghcwizqca.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wap.sjlbkw.cn/Article/details/gogizntib.sHtML

[U03] Py：加载 .env 配置
来源：http://wap.bbcook.cn/Article/details/giqrngiou.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://wap.yfazqb.com/Article/details/gbteuipwz.sHtML

[U04] Py：变量调试打印
来源：http://mobile.yfazqb.com/Article/details/gabwiqhrl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.yfazqb.com/Article/details/gadescucz.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.sjlbkw.cn/Article/details/guyqwivki.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gjgutxtcp.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gxsgbujor.sHtML

{**a, **b}
来源：http://www.m.share.fktsv.cn/Article/details/gipiudwbb.sHtML


<!-- 参考信息 -->