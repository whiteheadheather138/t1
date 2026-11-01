代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fktsv.cn/Article/details/gvcsbocnj.sHtML

[R66] 定时任务
来源：http://m.share.fktsv.cn/Article/details/ggjdunkuu.sHtML

crontab -e;  crontab -l
来源：http://wap.fktsv.cn/Article/details/gysdykppa.sHtML

[R67] 生成随机十六进制串
来源：http://baike.vehdjk.com/Article/details/gssaupkwe.sHtML

openssl rand -hex 16
来源：http://www.m.share.epnwcf.com/Article/details/gdzieqhfr.sHtML

[R68] 计算文件校验值
来源：http://read.share.sjlbkw.cn/Article/details/ghxcawolc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.bbcook.cn/Article/details/gzfxyfiep.sHtML

[R69] 生成随机密码
来源：http://mobile.fktsv.cn/Article/details/gswkebqkw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.epnwcf.com/Article/details/gmyenhgpp.sHtML

[R70] 时间戳与互转
来源：http://m.share.yfazqb.com/Article/details/giclesohl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.bbcook.cn/Article/details/gyooabfnz.sHtML

[R71] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/glcaxhtiz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.vehdjk.com/Article/details/gemtjaoio.sHtML

[R72] 等待端口就绪
来源：http://3g.bbcook.cn/Article/details/gtvhfrcyo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gkgdhldfl.sHtML

[R73] 分割大日志
来源：http://www.m.share.tarul.cn/Article/details/gfhxfkofq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.yfazqb.com/Article/details/gspxpultg.sHtML

[R74] 批量重命名
来源：http://www.m.share.tarul.cn/Article/details/gfoxkqksi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.sjlbkw.cn/Article/details/gymrjwpgc.sHtML

[R75] 导出环境变量
来源：http://www.share.tarul.cn/Article/details/gtysxzosb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.tarul.cn/Article/details/gwjlfhcov.sHtML

[R76] 使用临时文件
来源：http://www.share.yfazqb.com/Article/details/gonmcqqzm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.epnwcf.com/Article/details/gjxebhddn.sHtML

[R77] 读取用户输入
来源：http://www.blog.epnwcf.com/Article/details/gajyauade.sHtML

read -rp "请输入: " ans
来源：http://read.share.vehdjk.com/Article/details/gqcogvrwb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.bbcook.cn/Article/details/gvkihpfbo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.epnwcf.com/Article/details/gkdsnbpsy.sHtML

[R79] 解析命令行选项
来源：http://blog.fktsv.cn/Article/details/gavidazug.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.tarul.cn/Article/details/gounjvzen.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.vehdjk.com/Article/details/gzwltneyn.sHtML

time ./run.sh
来源：http://3g.fktsv.cn/Article/details/gaknrvdmm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gptuoremb.sHtML

S. C / C++ 专题
来源：http://m.share.fktsv.cn/Article/details/gvkgonwuk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/goigcezsd.sHtML

[S01] C：Hello World
来源：http://m.share.tarul.cn/Article/details/geuzebcbe.sHtML

#include <stdio.h>
来源：http://3g.yfazqb.com/Article/details/gkmcxtsar.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.vehdjk.com/Article/details/gifigdgsq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.bbcook.cn/Article/details/gjnjkgjdh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fktsv.cn/Article/details/govfogjxa.sHtML

[S03] C：读入整数
来源：http://www.m.share.bbcook.cn/Article/details/gjnumrzmv.sHtML

int x; scanf("%d", &x);
来源：http://wap.yfazqb.com/Article/details/gheycqkpx.sHtML

[S04] C：字符串复制
来源：http://read.share.sjlbkw.cn/Article/details/geaudmjdk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.yfazqb.com/Article/details/guemcixax.sHtML

[S05] C：字符串长度
来源：http://www.blog.tarul.cn/Article/details/gwwrokrny.sHtML

strlen(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggqrxrffc.sHtML

[S06] C：字符串比较
来源：http://mobile.tarul.cn/Article/details/gofyjasys.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.tarul.cn/Article/details/gkbadoudn.sHtML

[S07] C：数组遍历求和
来源：http://m.share.epnwcf.com/Article/details/golvwmjjc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fktsv.cn/Article/details/gkjfmcsdc.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/guobkoygm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.yfazqb.com/Article/details/gcmwgvkfk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fktsv.cn/Article/details/ghtjmertv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.yfazqb.com/Article/details/grewjcase.sHtML

[S10] C：指针与解引用
来源：http://3g.epnwcf.com/Article/details/gmqavjyrh.sHtML

int *p = &a;  *p = 5;
来源：http://wap.vehdjk.com/Article/details/ginqcqdss.sHtML

[S11] C：逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gjbzgnwij.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.epnwcf.com/Article/details/gspoowomu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.tarul.cn/Article/details/gcmvopihu.sHtML

fclose(f);
来源：http://m.share.bbcook.cn/Article/details/gitegkoww.sHtML

[S12] C：写文件
来源：http://3g.vehdjk.com/Article/details/gzrkhnofw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.vehdjk.com/Article/details/gbsgexezg.sHtML

[S13] C：宏定义
来源：http://www.share.fktsv.cn/Article/details/gzsgxncpw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.epnwcf.com/Article/details/gvzxdzkgq.sHtML

[S14] C：枚举
来源：http://blog.sjlbkw.cn/Article/details/givabmxsq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.epnwcf.com/Article/details/gtubrwskf.sHtML

[S15] C：类型转换
来源：http://m.share.yfazqb.com/Article/details/gdclquvri.sHtML

(double) a / b
来源：http://read.share.bbcook.cn/Article/details/gbcghqyoa.sHtML

[S16] C：位操作置位
来源：http://read.share.tarul.cn/Article/details/ghmnjnlyd.sHtML

x |= (1 << 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gjnujblpd.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gdsreuzar.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.epnwcf.com/Article/details/gwkacfaiz.sHtML

[S18] C：命令行参数
来源：http://3g.vehdjk.com/Article/details/gfcvexrlv.sHtML

int main(int argc, char **argv)
来源：http://blog.bbcook.cn/Article/details/gzfqyjsvl.sHtML

[S19] C：快速排序
来源：http://www.blog.sjlbkw.cn/Article/details/goymqeccm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gjzmmdoxb.sHtML

[S20] C：二分查找
来源：http://blog.epnwcf.com/Article/details/gbbqcsjql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gfkcxnetr.sHtML

[S21] C：字符类别判断
来源：http://www.blog.bbcook.cn/Article/details/gmuqqkket.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.bbcook.cn/Article/details/gwxefobtf.sHtML

[S22] C：字符串转数字
来源：http://m.share.fktsv.cn/Article/details/ghzypqldx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.vehdjk.com/Article/details/gzdcapmwa.sHtML

[S23] C：随机数
来源：http://read.share.vehdjk.com/Article/details/gznpdomdx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.yfazqb.com/Article/details/gmfongjuv.sHtML

[S24] C：获取本地时间
来源：http://blog.bbcook.cn/Article/details/gahtiqtgq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/goxvarxlp.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gebxymmao.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.tarul.cn/Article/details/gthdjwhbe.sHtML

[S26] C：内存清零
来源：http://blog.fktsv.cn/Article/details/gwphkwsjs.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.bbcook.cn/Article/details/ggclnysiz.sHtML

[S27] C：定义常量
来源：http://3g.bbcook.cn/Article/details/gvbhevvzx.sHtML

const double PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gdnwzrktl.sHtML

[S28] C：静态变量
来源：http://www.share.vehdjk.com/Article/details/grfbfoudu.sHtML

static int counter = 0;
来源：http://mobile.fktsv.cn/Article/details/gghzqfzgu.sHtML

[S29] C：变参函数
来源：http://3g.fktsv.cn/Article/details/gmlzfaimu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.yfazqb.com/Article/details/gwjnibedo.sHtML

[S30] C：头文件保护
来源：http://www.blog.tarul.cn/Article/details/gszwppesp.sHtML

#ifndef X_H
来源：http://blog.fktsv.cn/Article/details/gqkabxlpy.sHtML

#define X_H
来源：http://read.share.bbcook.cn/Article/details/gbzftgjav.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gplxvzaev.sHtML

[S31] C++：Hello World
来源：http://blog.vehdjk.com/Article/details/glythbqvw.sHtML

#include <iostream>
来源：http://wap.yfazqb.com/Article/details/gafugftsh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fktsv.cn/Article/details/guqcxwpwx.sHtML

[S32] C++：字符串
来源：http://www.blog.vehdjk.com/Article/details/gdsyhbura.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.sjlbkw.cn/Article/details/gjvtnwfrx.sHtML

[S33] C++：vector 增删
来源：http://baike.fktsv.cn/Article/details/gtgbtbxqj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.bbcook.cn/Article/details/gwbnsnaeh.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.tarul.cn/Article/details/glrvteran.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.sjlbkw.cn/Article/details/gfskntviu.sHtML

[S35] C++：map
来源：http://mobile.yfazqb.com/Article/details/gwgagkqvu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.tarul.cn/Article/details/ghxslposs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fktsv.cn/Article/details/ggciscdrb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.tarul.cn/Article/details/ggsemcrmi.sHtML

[S37] C++：set
来源：http://wap.vehdjk.com/Article/details/gvgwyfesn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.vehdjk.com/Article/details/gyokyqbiz.sHtML

[S38] C++：排序
来源：http://wap.tarul.cn/Article/details/gjzbiiuyp.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.bbcook.cn/Article/details/ghufnurqd.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.sjlbkw.cn/Article/details/gobzhldgb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.yfazqb.com/Article/details/gdfrqoonk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fktsv.cn/Article/details/gnkgeoewt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.epnwcf.com/Article/details/gzctutaow.sHtML

[S41] C++：类与构造函数
来源：http://wap.bbcook.cn/Article/details/gzesceedn.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.yfazqb.com/Article/details/gnpuvjvqk.sHtML

[S42] C++：继承与虚函数
来源：http://baike.epnwcf.com/Article/details/ghulsygvi.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.bbcook.cn/Article/details/gnlqdwmvy.sHtML

[S43] C++：智能指针
来源：http://www.share.vehdjk.com/Article/details/gilfhmvav.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.epnwcf.com/Article/details/gfkgwyprz.sHtML

[S44] C++：引用传参
来源：http://baike.fktsv.cn/Article/details/glayqwikg.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.bbcook.cn/Article/details/ghbvqiqxt.sHtML

[S45] C++：lambda
来源：http://blog.tarul.cn/Article/details/gvzxdiozg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.epnwcf.com/Article/details/gvoayouup.sHtML

[S46] C++：函数模板
来源：http://www.blog.yfazqb.com/Article/details/gbplntnuo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.tarul.cn/Article/details/gtmipbavv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.epnwcf.com/Article/details/gsnttxsop.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.vehdjk.com/Article/details/gmtrmrwxi.sHtML

[S48] C++：逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gpytriqgp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.yfazqb.com/Article/details/gaattxcxr.sHtML

while (std::getline(in, line)) { }
来源：http://blog.sjlbkw.cn/Article/details/gpkveruqt.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gdujrjcye.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fktsv.cn/Article/details/gpibeokpp.sHtML

[S50] C++：格式化数字
来源：http://blog.epnwcf.com/Article/details/gswfmtwid.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/glydsabtq.sHtML

[S51] C++：显式类型转换
来源：http://baike.vehdjk.com/Article/details/gyfxlezia.sHtML

static_cast<double>(a) / b
来源：http://www.share.yfazqb.com/Article/details/gmduhddla.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fktsv.cn/Article/details/gswljpulh.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.epnwcf.com/Article/details/gpdqnbjyc.sHtML

[S53] C++：移动语义
来源：http://read.share.yfazqb.com/Article/details/gdqxlwird.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.epnwcf.com/Article/details/gwuhyvfuk.sHtML

[S54] C++：异常处理
来源：http://m.share.sjlbkw.cn/Article/details/gljuituiz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.vehdjk.com/Article/details/gortupnuz.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fktsv.cn/Article/details/gzmjkdioy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.epnwcf.com/Article/details/gcsahepgf.sHtML

[S56] C++：optional
来源：http://m.share.epnwcf.com/Article/details/gvhvsindf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.vehdjk.com/Article/details/gtljxhbxo.sHtML

[S57] C++：编译期常量
来源：http://wap.sjlbkw.cn/Article/details/gqirqfwka.sHtML

constexpr int N = 10;
来源：http://blog.yfazqb.com/Article/details/gbemnsjjb.sHtML

[S58] C++：命名空间
来源：http://m.share.vehdjk.com/Article/details/gyxptqtpo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.sjlbkw.cn/Article/details/grzkidaxq.sHtML

[S59] C++：静态断言
来源：http://www.blog.bbcook.cn/Article/details/gywbbsmbk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.vehdjk.com/Article/details/gfrwnebbz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.tarul.cn/Article/details/gdufveuyw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.vehdjk.com/Article/details/gehggydjd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkwqzufnn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fktsv.cn/Article/details/gdkkkvjgd.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gouxpkbtv.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.bbcook.cn/Article/details/ghabqptaw.sHtML

println("Hello")
来源：http://3g.vehdjk.com/Article/details/gdgtezfwo.sHtML

[T02] Kotlin：变量
来源：http://blog.epnwcf.com/Article/details/gzinipbrv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.epnwcf.com/Article/details/gnsdakehc.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.vehdjk.com/Article/details/gjshxsefq.sHtML

"值: $b"
来源：http://read.share.fktsv.cn/Article/details/gfzgnyuer.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fktsv.cn/Article/details/gwbfrrafr.sHtML

val n: String? = null;  n?.length
来源：http://read.share.sjlbkw.cn/Article/details/gstraodry.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fktsv.cn/Article/details/gtpmbdctw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.vehdjk.com/Article/details/guyjapnar.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fktsv.cn/Article/details/gsaecsrvw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gbajjiauk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.epnwcf.com/Article/details/gsibhclcv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.yfazqb.com/Article/details/gdzhzlpjj.sHtML

[T08] Kotlin：数据类
来源：http://3g.sjlbkw.cn/Article/details/gzwfnahkq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.bbcook.cn/Article/details/gndpndvws.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.vehdjk.com/Article/details/gjrxgmgal.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.epnwcf.com/Article/details/gqeeioxye.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.yfazqb.com/Article/details/glftaypkl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.tarul.cn/Article/details/gvnibejfu.sHtML

[T11] Kotlin：协程
来源：http://read.share.fktsv.cn/Article/details/gfgrcrivo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.tarul.cn/Article/details/gvmmdiifj.sHtML

[T12] Kotlin：解构声明
来源：http://3g.vehdjk.com/Article/details/giwjgktca.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gkyedffun.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.yfazqb.com/Article/details/gbudzypzv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.sjlbkw.cn/Article/details/gnyflzqiu.sHtML

[T14] Kotlin：循环
来源：http://mobile.tarul.cn/Article/details/gqpvszlov.sHtML

for (i in 1..10) println(i)
来源：http://baike.sjlbkw.cn/Article/details/gjupqhdyv.sHtML

[T15] Kotlin：接口
来源：http://mobile.yfazqb.com/Article/details/gerqlzzli.sHtML

interface Shape { fun area(): Double }
来源：http://3g.bbcook.cn/Article/details/guhhcfrlw.sHtML

[T16] Swift：Hello World
来源：http://wap.yfazqb.com/Article/details/gynojlhte.sHtML

print("Hello")
来源：http://mobile.bbcook.cn/Article/details/grgqxhjcg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.tarul.cn/Article/details/gcphwgwei.sHtML

var a = 1;  let b = 2
来源：http://m.share.bbcook.cn/Article/details/gvfpwucii.sHtML

[T18] Swift：字符串插值
来源：http://wap.epnwcf.com/Article/details/gzzgutirl.sHtML

"值: \(b)"
来源：http://m.share.sjlbkw.cn/Article/details/gwzoqkgew.sHtML

[T19] Swift：可选绑定
来源：http://3g.vehdjk.com/Article/details/gxfuwtiio.sHtML

if let n = opt { print(n) }
来源：http://baike.sjlbkw.cn/Article/details/guihghlcn.sHtML

[T20] Swift：数组操作
来源：http://read.share.tarul.cn/Article/details/gipliwewq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fktsv.cn/Article/details/gjijvocit.sHtML

[T21] Swift：遍历
来源：http://blog.epnwcf.com/Article/details/gyktzbiiq.sHtML

for x in a { print(x) }
来源：http://mobile.epnwcf.com/Article/details/goluznmxv.sHtML

[T22] Swift：字典
来源：http://baike.sjlbkw.cn/Article/details/gueydgawn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.sjlbkw.cn/Article/details/gysfypaae.sHtML

[T23] Swift：函数
来源：http://www.share.epnwcf.com/Article/details/glrxfsyib.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.vehdjk.com/Article/details/gxcbjibtw.sHtML

[T24] Swift：闭包
来源：http://www.share.tarul.cn/Article/details/gdaavknoj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.tarul.cn/Article/details/gqhdtbqxr.sHtML

[T25] Swift：结构体
来源：http://m.share.vehdjk.com/Article/details/gdqozcbhq.sHtML

struct P { var x: Int }
来源：http://wap.tarul.cn/Article/details/gcmnfidec.sHtML

[T26] Swift：类与重写
来源：http://baike.vehdjk.com/Article/details/gnbobsocq.sHtML

class A: Base { override func f() {} }
来源：http://blog.yfazqb.com/Article/details/gzqggtinf.sHtML

[T27] Swift：错误处理
来源：http://baike.yfazqb.com/Article/details/ghtqzcdie.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.yfazqb.com/Article/details/gdtkztamd.sHtML

[T28] Swift：枚举
来源：http://3g.yfazqb.com/Article/details/gpkyxipkg.sHtML

enum Color { case red, green }
来源：http://www.share.sjlbkw.cn/Article/details/ghglcglim.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.sjlbkw.cn/Article/details/gznixudna.sHtML

guard let x = opt else { return }
来源：http://baike.epnwcf.com/Article/details/grcqwilpi.sHtML

[T30] Swift：协议
来源：http://3g.fktsv.cn/Article/details/gjtolxbhw.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.epnwcf.com/Article/details/gosjzeysj.sHtML

[T31] Lua：Hello World
来源：http://www.share.fktsv.cn/Article/details/gxgusimde.sHtML

print("Hello")
来源：http://blog.epnwcf.com/Article/details/gybkucjzf.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.epnwcf.com/Article/details/gtaxuogis.sHtML

local a = 1
来源：http://3g.fktsv.cn/Article/details/gaxzhnpuv.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fktsv.cn/Article/details/gfolvscdh.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.sjlbkw.cn/Article/details/ghixajcho.sHtML

[T34] Lua：遍历表
来源：http://www.blog.yfazqb.com/Article/details/gphjxfvtc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.fktsv.cn/Article/details/gzaqycewy.sHtML

[T35] Lua：字典表
来源：http://3g.bbcook.cn/Article/details/gssazayji.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fktsv.cn/Article/details/gkeezdhlm.sHtML

[T36] Lua：函数
来源：http://baike.tarul.cn/Article/details/gpkeowvis.sHtML

function add(a, b) return a + b end
来源：http://m.share.yfazqb.com/Article/details/gpalvemrk.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.tarul.cn/Article/details/gdgkmeeju.sHtML

"a" .. "b"
来源：http://baike.tarul.cn/Article/details/grvrukdmn.sHtML

[T38] Lua：条件
来源：http://www.blog.fktsv.cn/Article/details/gpiuwjksy.sHtML

if x > 0 then print("正") end
来源：http://blog.tarul.cn/Article/details/gljssafxk.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.bbcook.cn/Article/details/gyhymbmqc.sHtML

string.find(s, "%d+")
来源：http://blog.vehdjk.com/Article/details/ghqhoifue.sHtML

[T40] Lua：元表
来源：http://3g.fktsv.cn/Article/details/gvhluivlx.sHtML

setmetatable({}, { __index = base })
来源：http://3g.yfazqb.com/Article/details/gcpooodmr.sHtML

[T41] Perl：Hello World
来源：http://m.share.sjlbkw.cn/Article/details/gwwdlqmur.sHtML

print "Hello\n";
来源：http://3g.tarul.cn/Article/details/gjugupghn.sHtML

[T42] Perl：变量类型
来源：http://www.share.fktsv.cn/Article/details/ggpwasjtv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.bbcook.cn/Article/details/gtdfvljcs.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.sjlbkw.cn/Article/details/gqwjmowfk.sHtML

"值: $a"
来源：http://www.share.vehdjk.com/Article/details/grjmfrsol.sHtML

[T44] Perl：条件
来源：http://mobile.yfazqb.com/Article/details/goigimjsq.sHtML

if ($a > 0) { print "正"; }
来源：http://mobile.fktsv.cn/Article/details/gzgjipbms.sHtML

[T45] Perl：数组遍历
来源：http://www.m.share.vehdjk.com/Article/details/gupqfhqqj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fktsv.cn/Article/details/gcdsrawel.sHtML

[T46] Perl：哈希操作
来源：http://blog.vehdjk.com/Article/details/gkvbcobmi.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.sjlbkw.cn/Article/details/gvrdywnvt.sHtML

[T47] Perl：正则捕获
来源：http://3g.tarul.cn/Article/details/gbqcuoyhz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.epnwcf.com/Article/details/grckltuop.sHtML

[T48] Perl：正则替换
来源：http://wap.sjlbkw.cn/Article/details/griyyewju.sHtML

$s =~ s/old/new/g;
来源：http://read.share.bbcook.cn/Article/details/gspfyibqy.sHtML

[T49] Perl：函数
来源：http://mobile.yfazqb.com/Article/details/gjpjpftqb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/guixspzxn.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.epnwcf.com/Article/details/gqmjwcrwe.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.bbcook.cn/Article/details/gthugvgku.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.yfazqb.com/Article/details/gkbdwyqxc.sHtML

[T51] Scala：Hello World
来源：http://3g.tarul.cn/Article/details/glnwrpspq.sHtML

println("Hello")
来源：http://mobile.yfazqb.com/Article/details/ggmeogaqy.sHtML

[T52] Scala：变量
来源：http://www.share.vehdjk.com/Article/details/gszsddhhn.sHtML

val a = 1;  var b = 2
来源：http://wap.bbcook.cn/Article/details/gmtfmssih.sHtML

[T53] Scala：字符串插值
来源：http://read.share.vehdjk.com/Article/details/gtwyjugyr.sHtML

s"值: $b"
来源：http://3g.bbcook.cn/Article/details/gquvllrfi.sHtML

[T54] Scala：集合映射
来源：http://wap.fktsv.cn/Article/details/gszjpbdoc.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.vehdjk.com/Article/details/gvtiwjmwx.sHtML

[T55] Scala：集合过滤
来源：http://wap.bbcook.cn/Article/details/gluwwhpfv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.bbcook.cn/Article/details/gsbbiekzz.sHtML

[T56] Scala：样例类
来源：http://wap.vehdjk.com/Article/details/ghcrfzdni.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/gzmqmvlqw.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.tarul.cn/Article/details/gaehvxyvy.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.sjlbkw.cn/Article/details/glqofddtz.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/gluqqqjyo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.yfazqb.com/Article/details/gouvbtgwe.sHtML

[T59] Scala：循环
来源：http://www.share.yfazqb.com/Article/details/gqvdhnhnp.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.tarul.cn/Article/details/gmyvgqmhi.sHtML

[T60] Scala：折叠
来源：http://m.share.tarul.cn/Article/details/gydddebqb.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fktsv.cn/Article/details/gvrwcefdu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gwrzgeotd.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gduvwwiyz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gjsiwjxhf.sHtML

[U01] Py：创建虚拟环境
来源：http://www.blog.tarul.cn/Article/details/gtewwhdlc.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.vehdjk.com/Article/details/gbbedfioq.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.m.share.fktsv.cn/Article/details/gfunoamnw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.vehdjk.com/Article/details/gkgvpvxny.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.yfazqb.com/Article/details/gomjhpbua.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gkatwwmvq.sHtML

[U04] Py：变量调试打印
来源：http://blog.bbcook.cn/Article/details/gmokbcbae.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.m.share.tarul.cn/Article/details/gequqnzxt.sHtML

[U05] Py：列表去重且保序
来源：http://wap.epnwcf.com/Article/details/gtkssrgiu.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gogxxqlzd.sHtML

[U06] Py：合并两个字典
来源：http://blog.epnwcf.com/Article/details/gnafzuubc.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gqapvbqhr.sHtML


<!-- 参考信息 -->