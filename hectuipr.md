代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ksh.shuidangran.top

[R70] 时间戳与互转
来源：http://fbe.bjfxy.top

date +%s;  date -d @1700000000
来源：http://scs.jlsjyb.cn

[R71] 日期格式化
来源：http://ehe.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mxf.pycfn.com

[R72] 等待端口就绪
来源：http://qcj.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esq.ydjk.org.cn

[R73] 分割大日志
来源：http://oel.havefunace.top

split -l 1000 big.log part_
来源：http://cqg.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://kjd.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aky.cashguo.top

[R75] 导出环境变量
来源：http://cni.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://cue.haohaochexian.top

[R76] 使用临时文件
来源：http://pca.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ams.quarkkingdee.top

[R77] 读取用户输入
来源：http://xuk.sysykeji.top

read -rp "请输入: " ans
来源：http://jxj.hysaishi.cn

[R78] 交互式菜单
来源：http://xxe.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://toq.bjfxy.top

[R79] 解析命令行选项
来源：http://vgf.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zwq.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://jhp.sysykeji.top

time ./run.sh
来源：http://glg.svipenyu.cn

================================================================================
来源：http://ckt.jyoumei.cn

S. C / C++ 专题
来源：http://tbn.gogol.net.cn

================================================================================
来源：http://skc.jinqigfzy.top

[S01] C：Hello World
来源：http://hzr.xuetiantiany.cn

#include <stdio.h>
来源：http://avy.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nmh.andypj.xyz

[S02] C：变量与格式化输出
来源：http://jls.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://puw.daria6918.cn

[S03] C：读入整数
来源：http://rak.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://gbw.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://enm.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dwm.tianlin.xyz

[S05] C：字符串长度
来源：http://vtt.cdnleiting.top

strlen(s)
来源：http://aqe.shuidangran.top

[S06] C：字符串比较
来源：http://ejb.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://czs.snrcjt.cn

[S07] C：数组遍历求和
来源：http://msu.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bmv.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://oeh.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wjy.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://kax.zycfv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oxk.yanxiufei.cn

[S10] C：指针与解引用
来源：http://fnc.fzhhl.top

int *p = &a;  *p = 5;
来源：http://ufp.9152youxi.cn

[S11] C：逐行读文件
来源：http://jcm.wangdashe.top

FILE *f = fopen("a.txt", "r");
来源：http://uln.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vph.yuanzhike.top

fclose(f);
来源：http://tbb.yj20258.top

[S12] C：写文件
来源：http://grf.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ykf.9152youxi.cn

[S13] C：宏定义
来源：http://xis.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bsw.shangyingyoupin.top

[S14] C：枚举
来源：http://mvn.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://swa.tanke756.top

[S15] C：类型转换
来源：http://ril.xuetiantiany.cn

(double) a / b
来源：http://vtd.chenlongwang.top

[S16] C：位操作置位
来源：http://bkp.pengpengdd.cyou

x |= (1 << 3);
来源：http://htz.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://pij.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aum.xuetiantiany.cn

[S18] C：命令行参数
来源：http://nar.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://tcn.bbcook.cn

[S19] C：快速排序
来源：http://cxn.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bxz.cashguo.top

[S20] C：二分查找
来源：http://lmi.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tsv.gaohongyu789.top

[S21] C：字符类别判断
来源：http://ydz.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tmc.hysaishi.cn

[S22] C：字符串转数字
来源：http://ekl.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://tdj.jinghuilouyu.cn

[S23] C：随机数
来源：http://jyq.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zcv.yangfankeji.com

[S24] C：获取本地时间
来源：http://fmi.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://crk.uphjek.com

[S25] C：内存拷贝
来源：http://vpp.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://rao.quarkkingdee.top

[S26] C：内存清零
来源：http://euf.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://egk.gogol.net.cn

[S27] C：定义常量
来源：http://clk.0kj1m.cn

const double PI = 3.14159;
来源：http://uke.feifeiyinyue.top

[S28] C：静态变量
来源：http://akj.cucudq.cn

static int counter = 0;
来源：http://ahe.birdmap.top

[S29] C：变参函数
来源：http://vys.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sfq.jinqigufen.top

[S30] C：头文件保护
来源：http://frw.guannengcc.top

#ifndef X_H
来源：http://xmk.jiagoushi.top

#define X_H
来源：http://tji.sufxvd.cn

#endif
来源：http://jcy.shzxlz.cn

[S31] C++：Hello World
来源：http://ckw.aizwys.cn

#include <iostream>
来源：http://cdf.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://tty.jqgufenzy.top

[S32] C++：字符串
来源：http://iti.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://nuy.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://slj.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ctg.jiagoushi.top

[S34] C++：遍历 vector
来源：http://pib.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://sqc.hnxiangtu.top

[S35] C++：map
来源：http://agw.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cyo.yj20258888.top

[S36] C++：unordered_map
来源：http://bdu.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kgb.shzxlz.cn

[S37] C++：set
来源：http://uhj.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iar.nwbrower.top

[S38] C++：排序
来源：http://wlq.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://kuf.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://rnk.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://slr.hysaishi.cn

[S40] C++：查找元素
来源：http://wso.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tdu.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://mpo.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ike.sysykeji.top

[S42] C++：继承与虚函数
来源：http://cwj.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://rxd.mhx1999.top

[S43] C++：智能指针
来源：http://vab.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://doe.xuetiantiany.cn

[S44] C++：引用传参
来源：http://ars.hesvh.cn

void inc(int &x) { ++x; }
来源：http://wrl.jqgufenzy.top

[S45] C++：lambda
来源：http://eeu.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://rsp.chenlongwang.top

[S46] C++：函数模板
来源：http://voo.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fsm.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://wbc.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eng.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://doi.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://pyl.yueranfly.top

while (std::getline(in, line)) { }
来源：http://dei.guannengcc.top

[S49] C++：写文件
来源：http://izn.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jsz.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://mcc.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rje.zdqjudy.top

[S51] C++：显式类型转换
来源：http://lpy.yj202588.top

static_cast<double>(a) / b
来源：http://wcb.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://ytj.xuanzx.com

int size() const noexcept { return n_; }
来源：http://kyg.nanxuanxn.top

[S53] C++：移动语义
来源：http://qks.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://bfd.zhiwuduotai.top

[S54] C++：异常处理
来源：http://djg.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fub.snrcjt.cn

[S55] C++：结构化绑定
来源：http://hjv.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mtf.xylfe.cn

[S56] C++：optional
来源：http://xkr.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mfk.xylfe.cn

[S57] C++：编译期常量
来源：http://jmf.cheryme.top

constexpr int N = 10;
来源：http://mhg.chenjidiqi.icu

[S58] C++：命名空间
来源：http://zyr.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://lse.jqgufenzy.top

[S59] C++：静态断言
来源：http://stx.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vul.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://exp.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xmb.yanxiufei.cn

================================================================================
来源：http://fha.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://elh.quarkkingdee.top

================================================================================
来源：http://jqg.nwbrower.top

[T01] Kotlin：Hello World
来源：http://smg.chenzaomai.com

println("Hello")
来源：http://qxz.yfazqb.com

[T02] Kotlin：变量
来源：http://pjm.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fdn.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://mju.gaohongyu789.top

"值: $b"
来源：http://owi.hfpthk.cn

[T04] Kotlin：空安全
来源：http://hwg.yvedp.cn

val n: String? = null;  n?.length
来源：http://pio.cashguo.top

[T05] Kotlin：when 表达式
来源：http://ire.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fbp.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://cgq.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uji.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://glj.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fze.fktsv.cn

[T08] Kotlin：数据类
来源：http://ofq.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://tdj.hammf.cn

[T09] Kotlin：扩展函数
来源：http://jew.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://ypc.zhixingplan.top

[T10] Kotlin：默认参数
来源：http://mrb.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://gru.andypj.xyz

[T11] Kotlin：协程
来源：http://xlh.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dne.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://wnq.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://cff.birdmap.top

[T13] Kotlin：只读 Map
来源：http://qqp.yj20258.top

val m = mapOf("a" to 1)
来源：http://htk.jqgfzy.top

[T14] Kotlin：循环
来源：http://ivj.epnwcf.com

for (i in 1..10) println(i)
来源：http://nkm.haohaochexian.top

[T15] Kotlin：接口
来源：http://roc.fengsongda.top

interface Shape { fun area(): Double }
来源：http://ojp.zhixingplan.top

[T16] Swift：Hello World
来源：http://niv.c1oappe.top

print("Hello")
来源：http://bdq.epnwcf.com

[T17] Swift：变量与常量
来源：http://ckv.hfpthk.cn

var a = 1;  let b = 2
来源：http://dil.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://ahs.zhixingplan.top

"值: \(b)"
来源：http://plb.nwbrower.top

[T19] Swift：可选绑定
来源：http://ibu.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://syc.jqgufenzy.top

[T20] Swift：数组操作
来源：http://hib.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://znt.meibo888.top

[T21] Swift：遍历
来源：http://tvt.xuetiantiany.cn

for x in a { print(x) }
来源：http://aew.yuxming.cn

[T22] Swift：字典
来源：http://lby.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://hjc.hammf.cn

[T23] Swift：函数
来源：http://nlw.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://luu.xinyue.icu

[T24] Swift：闭包
来源：http://hqb.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://niz.uphjek.com

[T25] Swift：结构体
来源：http://rnu.hesvh.cn

struct P { var x: Int }
来源：http://ubq.daria6918.cn

[T26] Swift：类与重写
来源：http://gwx.fzhhl.top

class A: Base { override func f() {} }
来源：http://elc.fktsv.cn

[T27] Swift：错误处理
来源：http://ufp.hnqzz.top

do { try f() } catch { print(error) }
来源：http://ybm.quarkkingdee.top

[T28] Swift：枚举
来源：http://qlt.ctjpmb.com

enum Color { case red, green }
来源：http://fby.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://unb.jinqigfzy.top

guard let x = opt else { return }
来源：http://fbt.hongshengwenyu.top

[T30] Swift：协议
来源：http://kcr.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://hgb.zycfv.cn

[T31] Lua：Hello World
来源：http://ajq.nanxuanxn.top

print("Hello")
来源：http://zvj.haohaochexian.top

[T32] Lua：局部变量
来源：http://bbx.yueranfly.top

local a = 1
来源：http://cmn.c1oappe.top

[T33] Lua：表（数组）
来源：http://svc.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bce.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://etl.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://dwh.jqgfzy.top

[T35] Lua：字典表
来源：http://cyv.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://ban.jiagoushi.top

[T36] Lua：函数
来源：http://gjc.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://zae.vehdjk.com

[T37] Lua：字符串拼接
来源：http://jlm.gaohongyu789.top

"a" .. "b"
来源：http://aze.fengsongda.top

[T38] Lua：条件
来源：http://lvf.nanxinkj.top

if x > 0 then print("正") end
来源：http://osy.gotoacloud.top

[T39] Lua：模式匹配
来源：http://abf.sufxvd.cn

string.find(s, "%d+")
来源：http://kts.sweek.top

[T40] Lua：元表
来源：http://moz.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://lrf.9152youxi.cn

[T41] Perl：Hello World
来源：http://tpp.hnqzz.top

print "Hello\n";
来源：http://ddw.jlsjyb.cn

[T42] Perl：变量类型
来源：http://rsi.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dwn.nwbrower.top

[T43] Perl：字符串插值
来源：http://zvn.chenlongwang.top

"值: $a"
来源：http://scd.hnxiangtu.top

[T44] Perl：条件
来源：http://ivw.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://eik.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://shu.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://cwu.meibo888.top

[T46] Perl：哈希操作
来源：http://lnu.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://raq.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://ybi.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://loj.bjfxy.top

[T48] Perl：正则替换
来源：http://qpo.jyoumei.cn

$s =~ s/old/new/g;
来源：http://noa.tanke756.top

[T49] Perl：函数
来源：http://qyg.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lha.sufxvd.cn

[T50] Perl：逐行读文件
来源：http://qms.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uqz.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://hjw.shuidangran.top

[T51] Scala：Hello World
来源：http://doo.xinyue.icu

println("Hello")
来源：http://ggv.epnwcf.com

[T52] Scala：变量
来源：http://piu.jiagoushi.top

val a = 1;  var b = 2
来源：http://gdc.dianchejie.cn

[T53] Scala：字符串插值
来源：http://mfb.smart0.xyz

s"值: $b"
来源：http://gkn.xuanzx.com

[T54] Scala：集合映射
来源：http://soe.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://pud.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://umt.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tdj.haohaochexian.top

[T56] Scala：样例类
来源：http://kxn.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://wwz.316326.xyz

[T57] Scala：模式匹配
来源：http://aqj.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fwo.havefunace.top

[T58] Scala：函数定义
来源：http://jvd.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://lru.fzhhl.top

[T59] Scala：循环
来源：http://lar.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://fkr.wangshuangyany.cn

[T60] Scala：折叠
来源：http://kch.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://luu.wangshuangyany.cn

================================================================================
来源：http://reb.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kxe.tanke756.top

================================================================================
来源：http://puq.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://ezg.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://tks.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://qxm.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bye.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://lgd.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://joa.zdqjudy.top

[U04] Py：变量调试打印
来源：http://kyy.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xyo.andypj.xyz

[U05] Py：列表去重且保序
来源：http://ici.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://vzx.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://ojk.vqdsnc.cn

{**a, **b}
来源：http://jhr.sysykeji.top

[U07] Py：反转字典键值
来源：http://pqw.jqgfzy.top

{v: k for k, v in d.items()}
来源：http://rro.cdnleiting.top

[U08] Py：展平二维列表
来源：http://azl.kuanghao11.cn

[y for x in nested for y in x]
来源：http://qco.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://aro.tian-w.cn

max(d, key=d.get)
来源：http://tim.jqgfzy.top

[U10] Py：按值排序字典
来源：http://bjv.yueranfly.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hjk.jinqigufen.top


<!-- 参考信息 -->