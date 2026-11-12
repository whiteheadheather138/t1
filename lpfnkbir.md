代发 wailian999

S. C / C++ 专题
来源：http://yjq.316326.xyz

================================================================================
来源：http://pll.yonumen.top

[S01] C：Hello World
来源：http://asz.cashguo.top

#include <stdio.h>
来源：http://mcb.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://awm.bjfxy.top

[S02] C：变量与格式化输出
来源：http://oot.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://lgq.zdbjq.cn

[S03] C：读入整数
来源：http://hvg.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://kjc.dianchejie.cn

[S04] C：字符串复制
来源：http://aat.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://opn.birdmap.top

[S05] C：字符串长度
来源：http://rfn.xingfuxueyuan.xyz

strlen(s)
来源：http://khk.wangshuangyany.cn

[S06] C：字符串比较
来源：http://mqt.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://tgl.9152youxi.cn

[S07] C：数组遍历求和
来源：http://yhz.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uik.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://auj.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rtc.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://hss.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pkt.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://nfe.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://irb.sufxvd.cn

[S11] C：逐行读文件
来源：http://wmv.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://tms.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://icf.vqdsnc.cn

fclose(f);
来源：http://rff.sysykeji.top

[S12] C：写文件
来源：http://til.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rix.tian-w.cn

[S13] C：宏定义
来源：http://grj.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bvb.yongpay.top

[S14] C：枚举
来源：http://jvw.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://lve.zhiwuduotai.top

[S15] C：类型转换
来源：http://ire.guannengcc.top

(double) a / b
来源：http://cnw.zhoulong.xyz

[S16] C：位操作置位
来源：http://bpn.yongpay.top

x |= (1 << 3);
来源：http://iix.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://baq.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sfk.sjlbkw.cn

[S18] C：命令行参数
来源：http://bbb.tianlin.xyz

int main(int argc, char **argv)
来源：http://erp.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://ldx.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://sas.ivvv.top

[S20] C：二分查找
来源：http://nxm.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wjt.epnwcf.com

[S21] C：字符类别判断
来源：http://zes.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipf.yuanzhike.top

[S22] C：字符串转数字
来源：http://rle.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://wqd.birdmap.top

[S23] C：随机数
来源：http://izn.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://abp.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://gip.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fes.sjlbkw.cn

[S25] C：内存拷贝
来源：http://stu.sxryk.cn

memcpy(dst, src, n);
来源：http://klw.feifeiyinyue.top

[S26] C：内存清零
来源：http://dvd.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://cke.shuidangran.top

[S27] C：定义常量
来源：http://zem.jinqigfzy.top

const double PI = 3.14159;
来源：http://vkx.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://sfy.hywenlv.cn

static int counter = 0;
来源：http://anz.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://dnt.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://woj.0kj1m.cn

[S30] C：头文件保护
来源：http://ehz.gogol.net.cn

#ifndef X_H
来源：http://nji.sweek.top

#define X_H
来源：http://fxc.gaohongyu789.top

#endif
来源：http://viq.nanxuanxn.top

[S31] C++：Hello World
来源：http://mpg.fanxiaobao.xyz

#include <iostream>
来源：http://llb.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://tzb.hywenlv.cn

[S32] C++：字符串
来源：http://sde.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://dtu.svipenyu.cn

[S33] C++：vector 增删
来源：http://uom.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ume.vehdjk.com

[S34] C++：遍历 vector
来源：http://tvs.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://jhd.vqdsnc.cn

[S35] C++：map
来源：http://lrm.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bud.hywenlv.cn

[S36] C++：unordered_map
来源：http://mrs.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dog.andypj.xyz

[S37] C++：set
来源：http://dlx.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mnl.hfpthk.cn

[S38] C++：排序
来源：http://rqr.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://jqp.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://weq.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://van.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://avb.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://liv.ydzc1.top

[S41] C++：类与构造函数
来源：http://xmh.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nwh.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://lxi.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://wsx.feifeiyinyue.top

[S43] C++：智能指针
来源：http://zhr.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://xup.gzhubu.top

[S44] C++：引用传参
来源：http://ssc.yongpay.top

void inc(int &x) { ++x; }
来源：http://wlk.wangdashe.top

[S45] C++：lambda
来源：http://yza.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://xuh.yfazqb.com

[S46] C++：函数模板
来源：http://ouw.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cxv.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://lfl.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cdh.yj202588.top

[S48] C++：逐行读文件
来源：http://xrh.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iuf.fengsongda.top

while (std::getline(in, line)) { }
来源：http://fle.birdmap.top

[S49] C++：写文件
来源：http://gak.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jsi.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://puo.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://opp.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://hzb.andypj.xyz

static_cast<double>(a) / b
来源：http://jtf.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://wma.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://whi.smart0.xyz

[S53] C++：移动语义
来源：http://fdj.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://syr.hfpthk.cn

[S54] C++：异常处理
来源：http://byh.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sbi.yuanzhike.top

[S55] C++：结构化绑定
来源：http://dln.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zif.xylfe.cn

[S56] C++：optional
来源：http://stq.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dik.zhongyouzk.top

[S57] C++：编译期常量
来源：http://gur.fengsongda.top

constexpr int N = 10;
来源：http://yjs.birdmap.top

[S58] C++：命名空间
来源：http://mct.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://mim.bjfxy.top

[S59] C++：静态断言
来源：http://yoj.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vmg.316326.xyz

[S60] C++：遍历并删除元素
来源：http://haw.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejn.nanxuanxn.top

================================================================================
来源：http://grt.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bpu.yvedp.cn

================================================================================
来源：http://fch.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://xtl.sysykeji.top

println("Hello")
来源：http://hjq.hnqzz.top

[T02] Kotlin：变量
来源：http://ftw.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sjy.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://oad.hysaishi.cn

"值: $b"
来源：http://wyg.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://xwp.havefunace.top

val n: String? = null;  n?.length
来源：http://lqm.ehwqpu.com

[T05] Kotlin：when 表达式
来源：http://zkr.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qzw.yongpay.top

[T06] Kotlin：集合映射
来源：http://wcx.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dkj.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://wuk.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lfl.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://nwk.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://pnl.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://fyk.pycfn.com

fun String.exclaim() = this + "!"
来源：http://mjb.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://kgh.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vzs.xinyue.icu

[T11] Kotlin：协程
来源：http://qzv.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mlg.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://srg.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://xis.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://gcb.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://fpy.jianghu66.top

[T14] Kotlin：循环
来源：http://jyp.jiagoushi.top

for (i in 1..10) println(i)
来源：http://mdl.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://jxw.tian-w.cn

interface Shape { fun area(): Double }
来源：http://hrj.daria6918.cn

[T16] Swift：Hello World
来源：http://cwr.dianchejie.cn

print("Hello")
来源：http://bkr.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://afo.guowangkeji.top

var a = 1;  let b = 2
来源：http://ias.jyoumei.cn

[T18] Swift：字符串插值
来源：http://jpl.c1oappe.top

"值: \(b)"
来源：http://unt.shzxlz.cn

[T19] Swift：可选绑定
来源：http://ies.yj202588.top

if let n = opt { print(n) }
来源：http://vgd.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://any.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://lus.52xcode.cn

[T21] Swift：遍历
来源：http://nql.shangyingyoupin.top

for x in a { print(x) }
来源：http://rgv.mhx1999.top

[T22] Swift：字典
来源：http://wlz.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hpj.havefunace.top

[T23] Swift：函数
来源：http://iby.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hvs.sxryk.cn

[T24] Swift：闭包
来源：http://cnb.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://swu.hnqzz.top

[T25] Swift：结构体
来源：http://lgb.jqgufenzy.top

struct P { var x: Int }
来源：http://waf.jqgfzy.top

[T26] Swift：类与重写
来源：http://lfg.yonumen.top

class A: Base { override func f() {} }
来源：http://gbd.gogol.net.cn

[T27] Swift：错误处理
来源：http://tnj.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://yih.jqgfzy.top

[T28] Swift：枚举
来源：http://ouf.wangdashe.top

enum Color { case red, green }
来源：http://njo.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://utq.shangyingyoupin.top

guard let x = opt else { return }
来源：http://sgc.ctjpmb.com

[T30] Swift：协议
来源：http://xao.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://krw.chenlongwang.top

[T31] Lua：Hello World
来源：http://jqo.9152youxi.cn

print("Hello")
来源：http://wmn.ydzc1.top

[T32] Lua：局部变量
来源：http://scp.shangyingyoupin.top

local a = 1
来源：http://jnx.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://vsu.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://irb.pycfn.com

[T34] Lua：遍历表
来源：http://tfw.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zix.xylfe.cn

[T35] Lua：字典表
来源：http://wpy.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://ehi.sweek.top

[T36] Lua：函数
来源：http://los.gotoacloud.top

function add(a, b) return a + b end
来源：http://cqq.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://uam.ydzc1.top

"a" .. "b"
来源：http://eti.yvedp.cn

[T38] Lua：条件
来源：http://ldd.fzhhl.top

if x > 0 then print("正") end
来源：http://ukb.yj20258888.top

[T39] Lua：模式匹配
来源：http://vtw.cqqwz.cn

string.find(s, "%d+")
来源：http://yrf.jinqigufen.top

[T40] Lua：元表
来源：http://rot.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://uga.tarul.cn

[T41] Perl：Hello World
来源：http://erb.hesvh.cn

print "Hello\n";
来源：http://bwq.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://gcz.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mrf.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://gnv.hcnkem.com

"值: $a"
来源：http://ozy.vqdsnc.cn

[T44] Perl：条件
来源：http://ehh.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://chi.hnqzz.top

[T45] Perl：数组遍历
来源：http://myu.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://kds.tarul.cn

[T46] Perl：哈希操作
来源：http://ixp.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://otz.zhaomingkeji.xyz

[T47] Perl：正则捕获
来源：http://hgd.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xfg.sufxvd.cn

[T48] Perl：正则替换
来源：http://mah.meibo888.top

$s =~ s/old/new/g;
来源：http://cyq.yueranfly.top

[T49] Perl：函数
来源：http://xak.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eob.mhx1999.top

[T50] Perl：逐行读文件
来源：http://mcs.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dlx.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://euv.gzhubu.top

[T51] Scala：Hello World
来源：http://exf.daxiang520.top

println("Hello")
来源：http://wnk.ydzc1.top

[T52] Scala：变量
来源：http://kzu.yonumen.top

val a = 1;  var b = 2
来源：http://svj.zhengqikj.top

[T53] Scala：字符串插值
来源：http://ggw.jinyuanbaomall.cn

s"值: $b"
来源：http://txi.andypj.xyz

[T54] Scala：集合映射
来源：http://kmj.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://sbk.meibo888.top

[T55] Scala：集合过滤
来源：http://rhg.fengsongda.top

List(1, 2, 3).filter(_ > 1)
来源：http://rdm.chenzaomai.com

[T56] Scala：样例类
来源：http://vmu.tanke756.top

case class User(name: String, age: Int)
来源：http://nxj.yuanzhike.top

[T57] Scala：模式匹配
来源：http://poz.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mvq.ydjk.org.cn

[T58] Scala：函数定义
来源：http://bcr.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://lpw.nwbrower.top

[T59] Scala：循环
来源：http://tkn.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://cgz.ybcxt.top

[T60] Scala：折叠
来源：http://osn.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wfp.aizwys.cn

================================================================================
来源：http://ujp.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xcn.snrcjt.cn

================================================================================
来源：http://xxb.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://wfj.cqqwz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uvk.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://xai.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wbm.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://jko.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://juu.aibaodan.cn

[U04] Py：变量调试打印
来源：http://pht.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zzy.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://ylj.hysaishi.cn

list(dict.fromkeys(arr))
来源：http://vxj.guowangkeji.top

[U06] Py：合并两个字典
来源：http://lxl.hnqzz.top

{**a, **b}
来源：http://cjf.hywenlv.cn

[U07] Py：反转字典键值
来源：http://kwi.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://zeg.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://tkd.cucudq.cn

[y for x in nested for y in x]
来源：http://czj.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://zgf.hongshengwenyu.top

max(d, key=d.get)
来源：http://vxy.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://ogf.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zqy.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://yea.vqdsnc.cn

(x * 2 for x in arr)
来源：http://tha.shanyushiyangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://xao.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://xay.wangdashe.top

[U13] Py：固定长度队列
来源：http://kbw.hammf.cn

deque(maxlen=10)
来源：http://fzm.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://xth.zhengqikj.top

defaultdict(list)
来源：http://kzk.fzhhl.top

[U15] Py：高精度计时
来源：http://kqq.jyoumei.cn

t = time.perf_counter()
来源：http://vhp.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://tev.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ybu.gaohongyu789.top

[U17] Py：初始化日志
来源：http://vau.fengsongda.top

logging.basicConfig(level=logging.INFO)
来源：http://gds.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://osf.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://ofb.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://afq.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yjh.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://usg.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://ykt.yuxming.cn

[U21] Py：自定义上下文管理器
来源：http://rpf.chenjidiqi.icu

@contextlib.contextmanager
来源：http://yaq.hnqzz.top

[U22] Py：矩阵转置
来源：http://sjh.cqqwz.cn

list(zip(*m))
来源：http://yrx.uphjek.com


<!-- 参考信息 -->