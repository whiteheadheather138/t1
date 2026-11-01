代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/gpwdasiei.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gtgdeksay.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.tarul.cn/Article/details/gkeuibqlw.sHtML

[R61] 磁盘占用
来源：http://read.share.tarul.cn/Article/details/grwojvcwz.sHtML

df -h;  du -sh *
来源：http://read.share.yfazqb.com/Article/details/gowfcqozp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.vehdjk.com/Article/details/ghonxroim.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.tarul.cn/Article/details/gnboisjlm.sHtML

[R63] 内存与进程
来源：http://blog.sjlbkw.cn/Article/details/gfywxjkag.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.yfazqb.com/Article/details/gnulzdqzn.sHtML

[R64] 结束进程
来源：http://blog.tarul.cn/Article/details/gujcmeiiq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fktsv.cn/Article/details/gfmeyhjtb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.tarul.cn/Article/details/gbkzcmsuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.vehdjk.com/Article/details/gyrohuztj.sHtML

[R66] 定时任务
来源：http://wap.vehdjk.com/Article/details/glyegbqkd.sHtML

crontab -e;  crontab -l
来源：http://baike.yfazqb.com/Article/details/gkfeahfdd.sHtML

[R67] 生成随机十六进制串
来源：http://wap.vehdjk.com/Article/details/gvtdcdqsv.sHtML

openssl rand -hex 16
来源：http://m.share.fktsv.cn/Article/details/ghzcoalld.sHtML

[R68] 计算文件校验值
来源：http://mobile.yfazqb.com/Article/details/gyyoxuovr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.tarul.cn/Article/details/gcakbzawh.sHtML

[R69] 生成随机密码
来源：http://m.share.bbcook.cn/Article/details/ggqjkdvmc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.vehdjk.com/Article/details/gddijgifo.sHtML

[R70] 时间戳与互转
来源：http://read.share.fktsv.cn/Article/details/glykmebck.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.yfazqb.com/Article/details/gnzosqwcc.sHtML

[R71] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gscldqftn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fktsv.cn/Article/details/gkmoptrha.sHtML

[R72] 等待端口就绪
来源：http://mobile.bbcook.cn/Article/details/gkxjydgmi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gsaiwqnnj.sHtML

[R73] 分割大日志
来源：http://mobile.epnwcf.com/Article/details/gyydotnsg.sHtML

split -l 1000 big.log part_
来源：http://3g.fktsv.cn/Article/details/guznxmlpj.sHtML

[R74] 批量重命名
来源：http://3g.tarul.cn/Article/details/gxzuaqnhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.tarul.cn/Article/details/gsocsjyyu.sHtML

[R75] 导出环境变量
来源：http://read.share.tarul.cn/Article/details/ggyazvtey.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.yfazqb.com/Article/details/gxosueoax.sHtML

[R76] 使用临时文件
来源：http://m.share.bbcook.cn/Article/details/gqsrutjjx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gfzyrresg.sHtML

[R77] 读取用户输入
来源：http://www.blog.vehdjk.com/Article/details/gpysbxzwv.sHtML

read -rp "请输入: " ans
来源：http://3g.sjlbkw.cn/Article/details/gyqrwinfu.sHtML

[R78] 交互式菜单
来源：http://baike.vehdjk.com/Article/details/gwishggtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.epnwcf.com/Article/details/ggnzvmnxp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.yfazqb.com/Article/details/guqnkwrxs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.sjlbkw.cn/Article/details/glulyavou.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.tarul.cn/Article/details/guifiltie.sHtML

time ./run.sh
来源：http://wap.yfazqb.com/Article/details/gmhiotwqr.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gevcfeqnp.sHtML

S. C / C++ 专题
来源：http://www.m.share.yfazqb.com/Article/details/gokqyxjyy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggxnzzcsb.sHtML

[S01] C：Hello World
来源：http://blog.sjlbkw.cn/Article/details/gckiqulgi.sHtML

#include <stdio.h>
来源：http://wap.yfazqb.com/Article/details/gtstoqzia.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.epnwcf.com/Article/details/gvezbdwzm.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.epnwcf.com/Article/details/gaeizmfrl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.bbcook.cn/Article/details/ggycphhwh.sHtML

[S03] C：读入整数
来源：http://www.m.share.tarul.cn/Article/details/gkkrhypyt.sHtML

int x; scanf("%d", &x);
来源：http://baike.epnwcf.com/Article/details/gmjgtcdmq.sHtML

[S04] C：字符串复制
来源：http://baike.tarul.cn/Article/details/gyddxhufc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.epnwcf.com/Article/details/gygcuszll.sHtML

[S05] C：字符串长度
来源：http://wap.epnwcf.com/Article/details/gvbsijhzy.sHtML

strlen(s)
来源：http://blog.vehdjk.com/Article/details/gsecomwjf.sHtML

[S06] C：字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gyqdmhtls.sHtML

strcmp(a, b) == 0
来源：http://read.share.tarul.cn/Article/details/ghtxhjphc.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fktsv.cn/Article/details/gchtcptlu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.bbcook.cn/Article/details/gjpsizdvp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fktsv.cn/Article/details/gjqdtxpam.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.yfazqb.com/Article/details/gnfkufvww.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fktsv.cn/Article/details/geuwfnmqq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.yfazqb.com/Article/details/gjwtjiogk.sHtML

[S10] C：指针与解引用
来源：http://3g.yfazqb.com/Article/details/gmzarovbx.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.tarul.cn/Article/details/gmnsmzzes.sHtML

[S11] C：逐行读文件
来源：http://www.share.tarul.cn/Article/details/gcdcaviuh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.yfazqb.com/Article/details/gyxopvqpl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.bbcook.cn/Article/details/ghicfrfod.sHtML

fclose(f);
来源：http://m.share.yfazqb.com/Article/details/gwnnlqulh.sHtML

[S12] C：写文件
来源：http://www.share.sjlbkw.cn/Article/details/gkocbkwgs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.sjlbkw.cn/Article/details/gbzsimxad.sHtML

[S13] C：宏定义
来源：http://baike.tarul.cn/Article/details/ghjohrxua.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.yfazqb.com/Article/details/gnvifiqol.sHtML

[S14] C：枚举
来源：http://mobile.sjlbkw.cn/Article/details/gduckvtjw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.bbcook.cn/Article/details/giihniqnz.sHtML

[S15] C：类型转换
来源：http://baike.epnwcf.com/Article/details/gdeaslrdl.sHtML

(double) a / b
来源：http://3g.yfazqb.com/Article/details/gagcwajlw.sHtML

[S16] C：位操作置位
来源：http://read.share.vehdjk.com/Article/details/gvdajsxqy.sHtML

x |= (1 << 3);
来源：http://read.share.sjlbkw.cn/Article/details/gqpipzdug.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gtkyvwsdq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.tarul.cn/Article/details/gpykaoebm.sHtML

[S18] C：命令行参数
来源：http://wap.epnwcf.com/Article/details/guxjbvzjf.sHtML

int main(int argc, char **argv)
来源：http://baike.bbcook.cn/Article/details/gaastxlew.sHtML

[S19] C：快速排序
来源：http://3g.bbcook.cn/Article/details/gkgeiwdwt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.bbcook.cn/Article/details/giknxxcno.sHtML

[S20] C：二分查找
来源：http://read.share.yfazqb.com/Article/details/guznyfxjc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.tarul.cn/Article/details/gnkkmvfkq.sHtML

[S21] C：字符类别判断
来源：http://m.share.vehdjk.com/Article/details/ghhmipttq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.yfazqb.com/Article/details/gzzkwoibn.sHtML

[S22] C：字符串转数字
来源：http://m.share.yfazqb.com/Article/details/genceircb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.epnwcf.com/Article/details/gplykeayo.sHtML

[S23] C：随机数
来源：http://wap.fktsv.cn/Article/details/gauxnxesb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.sjlbkw.cn/Article/details/gbbqiuikp.sHtML

[S24] C：获取本地时间
来源：http://wap.vehdjk.com/Article/details/gcblhqriq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.epnwcf.com/Article/details/gmyuacwej.sHtML

[S25] C：内存拷贝
来源：http://baike.tarul.cn/Article/details/gniumgznw.sHtML

memcpy(dst, src, n);
来源：http://read.share.bbcook.cn/Article/details/gkflonuxq.sHtML

[S26] C：内存清零
来源：http://www.m.share.fktsv.cn/Article/details/gcayqdysw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.vehdjk.com/Article/details/golpmyyyu.sHtML

[S27] C：定义常量
来源：http://wap.vehdjk.com/Article/details/gduuoxyky.sHtML

const double PI = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/glsztoqau.sHtML

[S28] C：静态变量
来源：http://baike.epnwcf.com/Article/details/glclnucva.sHtML

static int counter = 0;
来源：http://read.share.vehdjk.com/Article/details/grjfjejdn.sHtML

[S29] C：变参函数
来源：http://www.m.share.yfazqb.com/Article/details/gpptjjhke.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.bbcook.cn/Article/details/gsjtoqmeq.sHtML

[S30] C：头文件保护
来源：http://mobile.yfazqb.com/Article/details/gsaldihme.sHtML

#ifndef X_H
来源：http://baike.yfazqb.com/Article/details/gfeebffad.sHtML

#define X_H
来源：http://wap.epnwcf.com/Article/details/gftmndfdk.sHtML

#endif
来源：http://read.share.vehdjk.com/Article/details/gtgypxavn.sHtML

[S31] C++：Hello World
来源：http://baike.sjlbkw.cn/Article/details/gjjcnqkgc.sHtML

#include <iostream>
来源：http://wap.sjlbkw.cn/Article/details/gwwmeyzuh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.bbcook.cn/Article/details/gavqhdksz.sHtML

[S32] C++：字符串
来源：http://baike.vehdjk.com/Article/details/gzwjpdxyq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.vehdjk.com/Article/details/gcommiisk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fktsv.cn/Article/details/gpqzstuuy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.tarul.cn/Article/details/gwfddksrp.sHtML

[S34] C++：遍历 vector
来源：http://www.share.yfazqb.com/Article/details/gohqfpxue.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.yfazqb.com/Article/details/gjvmfeqsm.sHtML

[S35] C++：map
来源：http://read.share.yfazqb.com/Article/details/gvekzhgcy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gukioojod.sHtML

[S36] C++：unordered_map
来源：http://www.blog.sjlbkw.cn/Article/details/gnxcyheoj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gpjktdyzl.sHtML

[S37] C++：set
来源：http://www.share.tarul.cn/Article/details/gjcpthyxp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.tarul.cn/Article/details/gjltsgqtj.sHtML

[S38] C++：排序
来源：http://blog.sjlbkw.cn/Article/details/gxkmuzdqk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.epnwcf.com/Article/details/gantjsuay.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.vehdjk.com/Article/details/geynkqhvw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.epnwcf.com/Article/details/goiewgwji.sHtML

[S40] C++：查找元素
来源：http://blog.yfazqb.com/Article/details/gqdvzzabh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fktsv.cn/Article/details/gkwynhitt.sHtML

[S41] C++：类与构造函数
来源：http://m.share.vehdjk.com/Article/details/gxoegthsz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.yfazqb.com/Article/details/guyflvfyi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.bbcook.cn/Article/details/gcvwjdtiu.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.vehdjk.com/Article/details/ggdlkwqxt.sHtML

[S43] C++：智能指针
来源：http://read.share.tarul.cn/Article/details/gkszvvlll.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fktsv.cn/Article/details/gittxicww.sHtML

[S44] C++：引用传参
来源：http://m.share.yfazqb.com/Article/details/gsbygegbd.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.yfazqb.com/Article/details/gwmreubqi.sHtML

[S45] C++：lambda
来源：http://read.share.sjlbkw.cn/Article/details/gzdkrvfok.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.vehdjk.com/Article/details/gdxctitlx.sHtML

[S46] C++：函数模板
来源：http://3g.sjlbkw.cn/Article/details/gndvmdxpq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.epnwcf.com/Article/details/gakascvdv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.tarul.cn/Article/details/gygxxysyg.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.epnwcf.com/Article/details/ggqysqaqv.sHtML

[S48] C++：逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/ghxvwtxvo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fktsv.cn/Article/details/gajtrunyi.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.sjlbkw.cn/Article/details/goohnsrmw.sHtML

[S49] C++：写文件
来源：http://www.blog.tarul.cn/Article/details/gsrsjafow.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.vehdjk.com/Article/details/gwktxigpl.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.yfazqb.com/Article/details/gwkgntzhh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.epnwcf.com/Article/details/gqnldgyvd.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fktsv.cn/Article/details/gittalzzb.sHtML

static_cast<double>(a) / b
来源：http://mobile.yfazqb.com/Article/details/gubawwkei.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.yfazqb.com/Article/details/gpignobme.sHtML

int size() const noexcept { return n_; }
来源：http://wap.bbcook.cn/Article/details/glkdrkfdx.sHtML

[S53] C++：移动语义
来源：http://m.share.tarul.cn/Article/details/glhyxvmac.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.sjlbkw.cn/Article/details/gmnpelldw.sHtML

[S54] C++：异常处理
来源：http://wap.bbcook.cn/Article/details/gbrqeslis.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.sjlbkw.cn/Article/details/gdezcwfdj.sHtML

[S55] C++：结构化绑定
来源：http://m.share.epnwcf.com/Article/details/geopwbhgz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.yfazqb.com/Article/details/gahjbbqzt.sHtML

[S56] C++：optional
来源：http://baike.bbcook.cn/Article/details/gfqzhafiu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.sjlbkw.cn/Article/details/gsbedsfht.sHtML

[S57] C++：编译期常量
来源：http://mobile.epnwcf.com/Article/details/ghfwmvctl.sHtML

constexpr int N = 10;
来源：http://mobile.tarul.cn/Article/details/gfdjugfzh.sHtML

[S58] C++：命名空间
来源：http://blog.vehdjk.com/Article/details/ghzdwzgjr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fktsv.cn/Article/details/gkvqfuseu.sHtML

[S59] C++：静态断言
来源：http://mobile.yfazqb.com/Article/details/gvcdokzyo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.tarul.cn/Article/details/guqtfcqcw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fktsv.cn/Article/details/gbxdjqlqy.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.epnwcf.com/Article/details/gycimsndn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gevkfnwqr.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.epnwcf.com/Article/details/ghjjgtnzo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grvaxyqga.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.vehdjk.com/Article/details/guzrpjxow.sHtML

println("Hello")
来源：http://3g.bbcook.cn/Article/details/gjtjcmktv.sHtML

[T02] Kotlin：变量
来源：http://www.share.epnwcf.com/Article/details/glznflhtj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.yfazqb.com/Article/details/gpuhseqok.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fktsv.cn/Article/details/gxwvhetea.sHtML

"值: $b"
来源：http://www.blog.epnwcf.com/Article/details/golyjbcpy.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.bbcook.cn/Article/details/glmxifuqy.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.sjlbkw.cn/Article/details/gwkszynri.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.bbcook.cn/Article/details/gycpxoinv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.bbcook.cn/Article/details/gouemyccd.sHtML

[T06] Kotlin：集合映射
来源：http://blog.yfazqb.com/Article/details/ggviqxkub.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.yfazqb.com/Article/details/gsaychrkn.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.epnwcf.com/Article/details/gmygkqekc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.vehdjk.com/Article/details/gtjfeqnai.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.yfazqb.com/Article/details/gdqlfetsq.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fktsv.cn/Article/details/gqexekodw.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.epnwcf.com/Article/details/gpaxalwho.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.bbcook.cn/Article/details/gkckqnyge.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.sjlbkw.cn/Article/details/gbdmhtzil.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.vehdjk.com/Article/details/gbgkoeorr.sHtML

[T11] Kotlin：协程
来源：http://mobile.yfazqb.com/Article/details/ghxwkvlzq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.sjlbkw.cn/Article/details/gemsgjlhp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.yfazqb.com/Article/details/gvpuxlggq.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gglpowdmy.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fktsv.cn/Article/details/gkrrfnjpk.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.bbcook.cn/Article/details/gxywznvwn.sHtML

[T14] Kotlin：循环
来源：http://blog.fktsv.cn/Article/details/gjspfbwpf.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.vehdjk.com/Article/details/gdluysgzo.sHtML

[T15] Kotlin：接口
来源：http://wap.sjlbkw.cn/Article/details/gvbjpdbgr.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fktsv.cn/Article/details/gnclaugal.sHtML

[T16] Swift：Hello World
来源：http://wap.epnwcf.com/Article/details/gxaljfqfp.sHtML

print("Hello")
来源：http://www.share.vehdjk.com/Article/details/gkwbljlig.sHtML

[T17] Swift：变量与常量
来源：http://mobile.epnwcf.com/Article/details/gubwssinw.sHtML

var a = 1;  let b = 2
来源：http://wap.vehdjk.com/Article/details/gxtkjmhpb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gvkrrfcue.sHtML

"值: \(b)"
来源：http://3g.fktsv.cn/Article/details/gpcipxmtx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.epnwcf.com/Article/details/gptzxvdgi.sHtML

if let n = opt { print(n) }
来源：http://read.share.bbcook.cn/Article/details/gqpbfwbcz.sHtML

[T20] Swift：数组操作
来源：http://3g.vehdjk.com/Article/details/gbexoatmy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fktsv.cn/Article/details/geqkusirl.sHtML

[T21] Swift：遍历
来源：http://www.m.share.epnwcf.com/Article/details/gjqrlqnkn.sHtML

for x in a { print(x) }
来源：http://3g.fktsv.cn/Article/details/gfrotukuc.sHtML

[T22] Swift：字典
来源：http://baike.yfazqb.com/Article/details/gssaugcqh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fktsv.cn/Article/details/gjuaopwxy.sHtML

[T23] Swift：函数
来源：http://m.share.yfazqb.com/Article/details/gmzqzqqcg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fktsv.cn/Article/details/gwlkrfxzd.sHtML

[T24] Swift：闭包
来源：http://m.share.epnwcf.com/Article/details/gfggvksby.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.sjlbkw.cn/Article/details/gignhxxdp.sHtML

[T25] Swift：结构体
来源：http://read.share.sjlbkw.cn/Article/details/gkmgwovob.sHtML

struct P { var x: Int }
来源：http://www.m.share.yfazqb.com/Article/details/ganlflfnm.sHtML

[T26] Swift：类与重写
来源：http://mobile.fktsv.cn/Article/details/gkpsfbcvt.sHtML

class A: Base { override func f() {} }
来源：http://m.share.sjlbkw.cn/Article/details/gfzmdboan.sHtML

[T27] Swift：错误处理
来源：http://blog.yfazqb.com/Article/details/gsjzygrlv.sHtML

do { try f() } catch { print(error) }
来源：http://3g.tarul.cn/Article/details/gnhtychzr.sHtML

[T28] Swift：枚举
来源：http://blog.sjlbkw.cn/Article/details/gxzmirdtf.sHtML

enum Color { case red, green }
来源：http://www.m.share.yfazqb.com/Article/details/glpscxael.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.vehdjk.com/Article/details/govtvxomf.sHtML

guard let x = opt else { return }
来源：http://www.share.fktsv.cn/Article/details/gdahhaplj.sHtML

[T30] Swift：协议
来源：http://read.share.vehdjk.com/Article/details/gjzbkxzsk.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.epnwcf.com/Article/details/gaosppncb.sHtML

[T31] Lua：Hello World
来源：http://blog.fktsv.cn/Article/details/gmhliyqnn.sHtML

print("Hello")
来源：http://baike.fktsv.cn/Article/details/gsnabgkah.sHtML

[T32] Lua：局部变量
来源：http://blog.tarul.cn/Article/details/gfxubfata.sHtML

local a = 1
来源：http://baike.yfazqb.com/Article/details/gniwnlpbn.sHtML

[T33] Lua：表（数组）
来源：http://m.share.vehdjk.com/Article/details/gdvdxslng.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.bbcook.cn/Article/details/gnqkbfbdn.sHtML

[T34] Lua：遍历表
来源：http://3g.vehdjk.com/Article/details/gjbwpzkxy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.tarul.cn/Article/details/goilajwha.sHtML

[T35] Lua：字典表
来源：http://baike.vehdjk.com/Article/details/gdpxrcmrz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.vehdjk.com/Article/details/glyplsxpm.sHtML

[T36] Lua：函数
来源：http://blog.tarul.cn/Article/details/gccyminkc.sHtML

function add(a, b) return a + b end
来源：http://read.share.yfazqb.com/Article/details/gmblpdqyo.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gmgyelgjw.sHtML

"a" .. "b"
来源：http://wap.sjlbkw.cn/Article/details/gleoeazbc.sHtML

[T38] Lua：条件
来源：http://blog.epnwcf.com/Article/details/glvwnkyff.sHtML

if x > 0 then print("正") end
来源：http://blog.bbcook.cn/Article/details/gelavpndy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.bbcook.cn/Article/details/gnwxtvbaf.sHtML

string.find(s, "%d+")
来源：http://mobile.yfazqb.com/Article/details/gbdlrqcee.sHtML

[T40] Lua：元表
来源：http://read.share.sjlbkw.cn/Article/details/gpsjdibip.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fktsv.cn/Article/details/gavwhzhhi.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.epnwcf.com/Article/details/geijhpmer.sHtML

print "Hello\n";
来源：http://www.blog.tarul.cn/Article/details/gwoukvwad.sHtML

[T42] Perl：变量类型
来源：http://wap.yfazqb.com/Article/details/ghcyprrpv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.sjlbkw.cn/Article/details/gvwwdfiki.sHtML

[T43] Perl：字符串插值
来源：http://wap.yfazqb.com/Article/details/gsxxtcvxp.sHtML

"值: $a"
来源：http://read.share.fktsv.cn/Article/details/gnxxrfmrg.sHtML

[T44] Perl：条件
来源：http://www.m.share.bbcook.cn/Article/details/gpppthavy.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.tarul.cn/Article/details/gyqygsmkk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.sjlbkw.cn/Article/details/goubuiuuo.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.tarul.cn/Article/details/glsnciiem.sHtML

[T46] Perl：哈希操作
来源：http://3g.fktsv.cn/Article/details/gemrvsude.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.yfazqb.com/Article/details/glnamifoo.sHtML

[T47] Perl：正则捕获
来源：http://m.share.yfazqb.com/Article/details/gvjykjcmy.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.epnwcf.com/Article/details/gquppnnih.sHtML

[T48] Perl：正则替换
来源：http://baike.tarul.cn/Article/details/glrwnshgo.sHtML

$s =~ s/old/new/g;
来源：http://blog.vehdjk.com/Article/details/gbeczwiqt.sHtML

[T49] Perl：函数
来源：http://m.share.tarul.cn/Article/details/gqqprcnki.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.sjlbkw.cn/Article/details/gjxfngllh.sHtML

[T50] Perl：逐行读文件
来源：http://wap.yfazqb.com/Article/details/gfwjeffsh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxxrqety.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.epnwcf.com/Article/details/gytlnamzn.sHtML

[T51] Scala：Hello World
来源：http://blog.yfazqb.com/Article/details/ggiuhkryv.sHtML

println("Hello")
来源：http://www.share.fktsv.cn/Article/details/gdksipcfl.sHtML

[T52] Scala：变量
来源：http://blog.bbcook.cn/Article/details/ghajgrptn.sHtML

val a = 1;  var b = 2
来源：http://m.share.tarul.cn/Article/details/gsoltibrg.sHtML

[T53] Scala：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gzlvtxybj.sHtML

s"值: $b"
来源：http://wap.tarul.cn/Article/details/ggfqryhpe.sHtML

[T54] Scala：集合映射
来源：http://www.blog.tarul.cn/Article/details/gpqkaqatv.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gcappaafw.sHtML

[T55] Scala：集合过滤
来源：http://mobile.yfazqb.com/Article/details/gyypqewhy.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://3g.epnwcf.com/Article/details/gkzhjjrsd.sHtML

[T56] Scala：样例类
来源：http://www.blog.epnwcf.com/Article/details/gjdgtifri.sHtML

case class User(name: String, age: Int)
来源：http://wap.vehdjk.com/Article/details/gczantgfv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.sjlbkw.cn/Article/details/gonwdnirn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.yfazqb.com/Article/details/gilcwrcii.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.fktsv.cn/Article/details/gutfgwijm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.tarul.cn/Article/details/gukmzylau.sHtML

[T59] Scala：循环
来源：http://baike.sjlbkw.cn/Article/details/gtvnoayty.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fktsv.cn/Article/details/gcdmkngni.sHtML

[T60] Scala：折叠
来源：http://blog.bbcook.cn/Article/details/gyiaqaszm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.tarul.cn/Article/details/glpaqmeiu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpoievpsi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gxmmiinww.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gupnqlvux.sHtML


<!-- 参考信息 -->