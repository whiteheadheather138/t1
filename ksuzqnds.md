代发 wailian999

S. C / C++ 专题
来源：http://gft.ywan-chungtsiang.top

================================================================================
来源：http://bzt.yuxming.cn

[S01] C：Hello World
来源：http://fdt.haohaochexian.top

#include <stdio.h>
来源：http://ges.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gth.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://oxw.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://yvm.ctjpmb.com

[S03] C：读入整数
来源：http://fkl.jqgfzy.top

int x; scanf("%d", &x);
来源：http://ves.52xcode.cn

[S04] C：字符串复制
来源：http://mzn.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://diy.chenlongwang.top

[S05] C：字符串长度
来源：http://koo.shzxlz.cn

strlen(s)
来源：http://ycp.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://zfo.yj20258888.top

strcmp(a, b) == 0
来源：http://zqv.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://vjm.fengsongda.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ayb.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://bwo.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kxm.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://wkn.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pvy.bjfxy.top

[S10] C：指针与解引用
来源：http://jsa.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://rpu.xziqi.cn

[S11] C：逐行读文件
来源：http://xuw.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://pot.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgf.shanyushiyangtech.top

fclose(f);
来源：http://ddn.sweek.top

[S12] C：写文件
来源：http://kwm.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bjy.shangyingyoupin.top

[S13] C：宏定义
来源：http://rik.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ltc.hnxiangtu.top

[S14] C：枚举
来源：http://xat.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://oog.yuxming.cn

[S15] C：类型转换
来源：http://fyc.shzxlz.cn

(double) a / b
来源：http://wcz.pycfn.com

[S16] C：位操作置位
来源：http://mtv.cashguo.top

x |= (1 << 3);
来源：http://gtv.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://thy.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uuc.zhoulong.xyz

[S18] C：命令行参数
来源：http://kst.zhijiandao.cn

int main(int argc, char **argv)
来源：http://jtz.chenlongwang.top

[S19] C：快速排序
来源：http://dwr.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://zbn.xinyue.icu

[S20] C：二分查找
来源：http://pjt.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nvc.cheryme.top

[S21] C：字符类别判断
来源：http://ges.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bag.c1oappe.top

[S22] C：字符串转数字
来源：http://dmn.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fwz.meibo888.top

[S23] C：随机数
来源：http://yan.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gbv.yueranfly.top

[S24] C：获取本地时间
来源：http://dom.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fue.hesvh.cn

[S25] C：内存拷贝
来源：http://jus.ydzc1.top

memcpy(dst, src, n);
来源：http://mpd.cheryme.top

[S26] C：内存清零
来源：http://wgd.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://xne.cucudq.cn

[S27] C：定义常量
来源：http://xae.hammf.cn

const double PI = 3.14159;
来源：http://jgr.cashguo.top

[S28] C：静态变量
来源：http://frx.52xcode.cn

static int counter = 0;
来源：http://xhr.ppjwa.cn

[S29] C：变参函数
来源：http://mru.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://syl.gzhubu.top

[S30] C：头文件保护
来源：http://fio.cqqwz.cn

#ifndef X_H
来源：http://skg.birdmap.top

#define X_H
来源：http://spy.wangshuangyany.cn

#endif
来源：http://dsg.nanxuanxn.top

[S31] C++：Hello World
来源：http://ntq.feifeiyinyue.top

#include <iostream>
来源：http://iss.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://dfv.cdnleiting.top

[S32] C++：字符串
来源：http://cam.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://zqw.sweek.top

[S33] C++：vector 增删
来源：http://jse.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qan.redwolf501.top

[S34] C++：遍历 vector
来源：http://cqi.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://zlw.cashguo.top

[S35] C++：map
来源：http://iko.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jfe.sufxvd.cn

[S36] C++：unordered_map
来源：http://iak.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://spi.hysaishi.cn

[S37] C++：set
来源：http://bje.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vbv.ppjwa.cn

[S38] C++：排序
来源：http://gxn.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://ffz.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://epw.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wcq.jlsjyb.cn

[S40] C++：查找元素
来源：http://mhv.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nsv.yueranfly.top

[S41] C++：类与构造函数
来源：http://fqt.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eeq.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://ygk.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://rlj.mhx1999.top

[S43] C++：智能指针
来源：http://pel.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://wan.zhengqikj.top

[S44] C++：引用传参
来源：http://cjo.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://bqf.cucudq.cn

[S45] C++：lambda
来源：http://jzm.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://ool.vehdjk.com

[S46] C++：函数模板
来源：http://tvp.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qju.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://cue.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://moj.0kj1m.cn

[S48] C++：逐行读文件
来源：http://zzr.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://klp.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://pal.shanyushiyangtech.top

[S49] C++：写文件
来源：http://mwn.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jyy.zhoulong.xyz

[S50] C++：格式化数字
来源：http://ulc.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ldx.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://xep.epnwcf.com

static_cast<double>(a) / b
来源：http://cla.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://thp.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://knh.shuidangran.top

[S53] C++：移动语义
来源：http://wsu.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://qoy.316326.xyz

[S54] C++：异常处理
来源：http://roj.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kqr.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://gtm.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://voy.gotoacloud.top

[S56] C++：optional
来源：http://ubr.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lib.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://cto.pengpengdd.cyou

constexpr int N = 10;
来源：http://tis.bjfxy.top

[S58] C++：命名空间
来源：http://ehk.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://tvs.wangshuangyany.cn

[S59] C++：静态断言
来源：http://kay.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wvy.hammf.cn

[S60] C++：遍历并删除元素
来源：http://mcc.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vbt.xuetiantiany.cn

================================================================================
来源：http://qeo.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dkw.xinyue.icu

================================================================================
来源：http://mxl.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://aqs.aizwys.cn

println("Hello")
来源：http://qgr.xylfe.cn

[T02] Kotlin：变量
来源：http://pcu.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fhl.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://zye.guannengcc.top

"值: $b"
来源：http://btb.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://qep.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://muf.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://sfk.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wpo.yonumen.top

[T06] Kotlin：集合映射
来源：http://lnx.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://all.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://qyx.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oix.birdmap.top

[T08] Kotlin：数据类
来源：http://vfs.316326.xyz

data class User(val name: String, val age: Int)
来源：http://wjb.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://gcz.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://epr.sysykeji.top

[T10] Kotlin：默认参数
来源：http://gzc.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cxg.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://ejs.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kxg.fehbvm.com

[T12] Kotlin：解构声明
来源：http://ich.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://kqg.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://fqh.iojbl.cn

val m = mapOf("a" to 1)
来源：http://bdb.cqqwz.cn

[T14] Kotlin：循环
来源：http://pkn.nanxinkj.top

for (i in 1..10) println(i)
来源：http://hfw.zdbjq.cn

[T15] Kotlin：接口
来源：http://yde.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://wlh.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://kzu.chenlongwang.top

print("Hello")
来源：http://aak.ybcxt.top

[T17] Swift：变量与常量
来源：http://yyy.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://wzi.sysykeji.top

[T18] Swift：字符串插值
来源：http://ejd.yangfankeji.com

"值: \(b)"
来源：http://hey.tian-w.cn

[T19] Swift：可选绑定
来源：http://atl.zhongyouzk.top

if let n = opt { print(n) }
来源：http://wfa.zycfv.cn

[T20] Swift：数组操作
来源：http://yov.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://his.dianchejie.cn

[T21] Swift：遍历
来源：http://gup.epnwcf.com

for x in a { print(x) }
来源：http://fkg.yvedp.cn

[T22] Swift：字典
来源：http://leu.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://gnz.ehwqpu.com

[T23] Swift：函数
来源：http://css.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nce.meibo888.top

[T24] Swift：闭包
来源：http://naf.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqf.iojbl.cn

[T25] Swift：结构体
来源：http://piq.jinghuilouyu.cn

struct P { var x: Int }
来源：http://fyw.smart0.xyz

[T26] Swift：类与重写
来源：http://tzk.fehbvm.com

class A: Base { override func f() {} }
来源：http://thm.zhongyouzk.top

[T27] Swift：错误处理
来源：http://sip.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://nnk.cqqwz.cn

[T28] Swift：枚举
来源：http://hmf.ydjk.org.cn

enum Color { case red, green }
来源：http://uqf.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://anl.vqdsnc.cn

guard let x = opt else { return }
来源：http://wfj.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://qpi.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://ikp.iojbl.cn

[T31] Lua：Hello World
来源：http://euz.zdbjq.cn

print("Hello")
来源：http://fcn.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://ted.jinqigufen.top

local a = 1
来源：http://zro.aibaodan.cn

[T33] Lua：表（数组）
来源：http://rvc.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fej.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://cmz.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gjk.vqdsnc.cn

[T35] Lua：字典表
来源：http://pbp.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://nqt.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://lnr.9152youxi.cn

function add(a, b) return a + b end
来源：http://aln.hesvh.cn

[T37] Lua：字符串拼接
来源：http://wwl.yvedp.cn

"a" .. "b"
来源：http://ovz.pycfn.com

[T38] Lua：条件
来源：http://ujb.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://bxj.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://xnm.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://yca.jyoumei.cn

[T40] Lua：元表
来源：http://oph.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://akm.yangfankeji.com

[T41] Perl：Hello World
来源：http://esp.bbcook.cn

print "Hello\n";
来源：http://urg.uphjek.com

[T42] Perl：变量类型
来源：http://olw.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qns.yuanzhike.top

[T43] Perl：字符串插值
来源：http://zxq.ybcxt.top

"值: $a"
来源：http://usy.andypj.xyz

[T44] Perl：条件
来源：http://mkc.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://mwc.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://ynk.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://orm.chenzaomai.com

[T46] Perl：哈希操作
来源：http://tox.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uve.cqqwz.cn

[T47] Perl：正则捕获
来源：http://qmu.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gqj.hnxiangtu.top

[T48] Perl：正则替换
来源：http://cla.shzxlz.cn

$s =~ s/old/new/g;
来源：http://sjj.ehwqpu.com

[T49] Perl：函数
来源：http://csj.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://drj.uphjek.com

[T50] Perl：逐行读文件
来源：http://fmw.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://lzb.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://xxn.cheryme.top

[T51] Scala：Hello World
来源：http://ast.chenzaomai.com

println("Hello")
来源：http://yfe.hywenlv.cn

[T52] Scala：变量
来源：http://uii.yfazqb.com

val a = 1;  var b = 2
来源：http://zqj.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://kyp.zycfv.cn

s"值: $b"
来源：http://ffd.mhx1999.top

[T54] Scala：集合映射
来源：http://bkt.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://uqp.haohaochexian.top

[T55] Scala：集合过滤
来源：http://aib.jyoumei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ryf.hesvh.cn

[T56] Scala：样例类
来源：http://ahk.gzhubu.top

case class User(name: String, age: Int)
来源：http://uwc.redwolf501.top

[T57] Scala：模式匹配
来源：http://eim.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vcl.cucudq.cn

[T58] Scala：函数定义
来源：http://cqv.shanyushiyangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://sml.smart0.xyz

[T59] Scala：循环
来源：http://ijw.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://dbk.0kj1m.cn

[T60] Scala：折叠
来源：http://dmn.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bng.jinyuanbaomall.cn

================================================================================
来源：http://nuo.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qwc.hysaishi.cn

================================================================================
来源：http://hkv.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://vvs.andypj.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://hif.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://kzt.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gep.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://rxa.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cwy.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://ziy.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nfl.redwolf501.top

[U05] Py：列表去重且保序
来源：http://frr.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://ioi.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://bli.mhx1999.top

{**a, **b}
来源：http://jgp.hesvh.cn

[U07] Py：反转字典键值
来源：http://hwd.daria6918.cn

{v: k for k, v in d.items()}
来源：http://njn.epnwcf.com

[U08] Py：展平二维列表
来源：http://lue.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://rmm.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://msi.aibaodan.cn

max(d, key=d.get)
来源：http://jxj.ehwqpu.com

[U10] Py：按值排序字典
来源：http://cxc.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vir.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://bpw.jianghu66.top

(x * 2 for x in arr)
来源：http://fnw.cucudq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mvb.cucudq.cn

Counter(arr).most_common(3)
来源：http://sgm.316326.xyz

[U13] Py：固定长度队列
来源：http://odg.andypj.xyz

deque(maxlen=10)
来源：http://npv.jinqigufen.top

[U14] Py：分组收集到列表
来源：http://stl.havefunace.top

defaultdict(list)
来源：http://wpy.yongpay.top

[U15] Py：高精度计时
来源：http://hsw.316326.xyz

t = time.perf_counter()
来源：http://bzk.tian-w.cn

[U16] Py：命令行参数解析
来源：http://qfr.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yax.zdqjudy.top

[U17] Py：初始化日志
来源：http://naa.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://bhu.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://ksg.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://wlq.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://qtz.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fkr.aizwys.cn

[U20] Py：缓存函数结果
来源：http://bqz.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://jby.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://gnd.hesvh.cn

@contextlib.contextmanager
来源：http://tpe.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://dxi.xylfe.cn

list(zip(*m))
来源：http://pgn.aizwys.cn


<!-- 参考信息 -->