代发 wailian999

split -l 1000 big.log part_
来源：http://bby.sweek.top

[R74] 批量重命名
来源：http://ehe.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eua.yvedp.cn

[R75] 导出环境变量
来源：http://san.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://gzj.jiagoushi.top

[R76] 使用临时文件
来源：http://tpc.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hwu.birdmap.top

[R77] 读取用户输入
来源：http://ray.316326.xyz

read -rp "请输入: " ans
来源：http://zmp.gzhubu.top

[R78] 交互式菜单
来源：http://noj.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ujb.jinqigufen.top

[R79] 解析命令行选项
来源：http://gjc.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hbo.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://wjj.dianchejie.cn

time ./run.sh
来源：http://vsg.yuanzhike.top

================================================================================
来源：http://wkl.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://rvc.tianlin.xyz

================================================================================
来源：http://tyi.yuxming.cn

[S01] C：Hello World
来源：http://bzq.zhoulong.xyz

#include <stdio.h>
来源：http://rqj.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wea.52xcode.cn

[S02] C：变量与格式化输出
来源：http://huk.gogol.net.cn

int a = 10; printf("%d\n", a);
来源：http://qnp.cucudq.cn

[S03] C：读入整数
来源：http://ryq.sxryk.cn

int x; scanf("%d", &x);
来源：http://sxg.ydzc1.top

[S04] C：字符串复制
来源：http://uij.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://eph.hnxiangtu.top

[S05] C：字符串长度
来源：http://mcc.nanxinkj.top

strlen(s)
来源：http://aqu.xziqi.cn

[S06] C：字符串比较
来源：http://tcp.gzhubu.top

strcmp(a, b) == 0
来源：http://bne.hammf.cn

[S07] C：数组遍历求和
来源：http://fev.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uex.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://mwt.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sbz.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://vdz.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hzk.uphjek.com

[S10] C：指针与解引用
来源：http://fet.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://lol.fehbvm.com

[S11] C：逐行读文件
来源：http://bgg.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://bpm.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fxl.hammf.cn

fclose(f);
来源：http://geg.yj20258888.top

[S12] C：写文件
来源：http://kxl.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fym.jiagoushi.top

[S13] C：宏定义
来源：http://mue.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qmw.guowangkeji.top

[S14] C：枚举
来源：http://pco.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://jnl.hysaishi.cn

[S15] C：类型转换
来源：http://rng.jqgufenzy.top

(double) a / b
来源：http://eli.cqqwz.cn

[S16] C：位操作置位
来源：http://olf.guannengcc.top

x |= (1 << 3);
来源：http://hdq.yvedp.cn

[S17] C：安全拼接字符串
来源：http://oni.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sal.chenzaomai.com

[S18] C：命令行参数
来源：http://fzy.hammf.cn

int main(int argc, char **argv)
来源：http://mdw.cdnleiting.top

[S19] C：快速排序
来源：http://oni.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wxr.kuanghao11.cn

[S20] C：二分查找
来源：http://zsw.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lxz.yfazqb.com

[S21] C：字符类别判断
来源：http://edr.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wah.ydzc1.top

[S22] C：字符串转数字
来源：http://zui.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ymz.sufxvd.cn

[S23] C：随机数
来源：http://gvj.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gvn.hnqzz.top

[S24] C：获取本地时间
来源：http://zxa.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fal.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://hav.dashuyun.cn

memcpy(dst, src, n);
来源：http://yup.guannengcc.top

[S26] C：内存清零
来源：http://vjn.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://eti.ppjwa.cn

[S27] C：定义常量
来源：http://bba.hammf.cn

const double PI = 3.14159;
来源：http://pwu.zhongyouzk.top

[S28] C：静态变量
来源：http://tmu.iojbl.cn

static int counter = 0;
来源：http://eci.shzxlz.cn

[S29] C：变参函数
来源：http://khb.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://got.zdbjq.cn

[S30] C：头文件保护
来源：http://kha.zhongyouzk.top

#ifndef X_H
来源：http://tgy.yuanzhike.top

#define X_H
来源：http://zrt.xziqi.cn

#endif
来源：http://wfb.redwolf501.top

[S31] C++：Hello World
来源：http://lqk.yj202588.top

#include <iostream>
来源：http://uut.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://hon.nanxinkj.top

[S32] C++：字符串
来源：http://vpb.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://cws.hywenlv.cn

[S33] C++：vector 增删
来源：http://vjz.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oqo.ybcxt.top

[S34] C++：遍历 vector
来源：http://gth.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://fwv.jqgufenzy.top

[S35] C++：map
来源：http://gtu.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://etf.nanxinkj.top

[S36] C++：unordered_map
来源：http://atu.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nhn.quarkkingdee.top

[S37] C++：set
来源：http://fsx.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qml.0kj1m.cn

[S38] C++：排序
来源：http://kpt.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://fjc.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://eqx.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uxi.52xcode.cn

[S40] C++：查找元素
来源：http://ijc.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ftc.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://zqp.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fii.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://hfz.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://nkp.chenjidiqi.icu

[S43] C++：智能指针
来源：http://ahl.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://eqw.sysykeji.top

[S44] C++：引用传参
来源：http://ckx.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://eaw.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://lsk.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://fvk.vqdsnc.cn

[S46] C++：函数模板
来源：http://ngv.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://knh.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://htc.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iax.ctjpmb.com

[S48] C++：逐行读文件
来源：http://dvy.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://uip.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://hkw.tian-w.cn

[S49] C++：写文件
来源：http://yxs.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljw.jinqigfzy.top

[S50] C++：格式化数字
来源：http://vew.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pyf.ybcxt.top

[S51] C++：显式类型转换
来源：http://cxp.yonumen.top

static_cast<double>(a) / b
来源：http://kng.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://tuv.smart0.xyz

int size() const noexcept { return n_; }
来源：http://iac.epnwcf.com

[S53] C++：移动语义
来源：http://rmw.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://bun.hysaishi.cn

[S54] C++：异常处理
来源：http://bok.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tdd.zycfv.cn

[S55] C++：结构化绑定
来源：http://ftk.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://gqr.fehbvm.com

[S56] C++：optional
来源：http://qxq.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zgt.cdnleiting.top

[S57] C++：编译期常量
来源：http://xhd.9152youxi.cn

constexpr int N = 10;
来源：http://shn.chenlongwang.top

[S58] C++：命名空间
来源：http://rqw.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://yys.daxiang520.top

[S59] C++：静态断言
来源：http://gsl.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lyp.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://yra.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pvv.zhijiandao.cn

================================================================================
来源：http://htb.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fdb.jyoumei.cn

================================================================================
来源：http://aty.shuidangran.top

[T01] Kotlin：Hello World
来源：http://qyd.mhx1999.top

println("Hello")
来源：http://uyg.aibaodan.cn

[T02] Kotlin：变量
来源：http://atz.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vtw.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://ibn.iojbl.cn

"值: $b"
来源：http://deo.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://nly.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://pjj.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://ecl.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://akb.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://vga.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://adz.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://nuv.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zyz.hywenlv.cn

[T08] Kotlin：数据类
来源：http://wtg.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://uqf.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://jsh.ivvv.top

fun String.exclaim() = this + "!"
来源：http://eik.yvedp.cn

[T10] Kotlin：默认参数
来源：http://srp.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bwm.yj202588.top

[T11] Kotlin：协程
来源：http://kuy.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://ctz.epnwcf.com

[T12] Kotlin：解构声明
来源：http://ela.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://rnx.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://eqx.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://kmn.fzhhl.top

[T14] Kotlin：循环
来源：http://gtk.jianghu66.top

for (i in 1..10) println(i)
来源：http://ogb.shzxlz.cn

[T15] Kotlin：接口
来源：http://wnh.bbcook.cn

interface Shape { fun area(): Double }
来源：http://nod.yuanzhike.top

[T16] Swift：Hello World
来源：http://ibe.hywenlv.cn

print("Hello")
来源：http://jzu.aizwys.cn

[T17] Swift：变量与常量
来源：http://drj.smart0.xyz

var a = 1;  let b = 2
来源：http://aaf.chenzaomai.com

[T18] Swift：字符串插值
来源：http://bip.andypj.xyz

"值: \(b)"
来源：http://jir.aibaodan.cn

[T19] Swift：可选绑定
来源：http://bta.ehwqpu.com

if let n = opt { print(n) }
来源：http://ssq.jqgfzy.top

[T20] Swift：数组操作
来源：http://mxq.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://gwe.yvedp.cn

[T21] Swift：遍历
来源：http://jxc.daxiang520.top

for x in a { print(x) }
来源：http://fjq.hfpthk.cn

[T22] Swift：字典
来源：http://ryd.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://pbl.fengsongda.top

[T23] Swift：函数
来源：http://wbp.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fip.jianghu66.top

[T24] Swift：闭包
来源：http://vod.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zwa.andypj.xyz

[T25] Swift：结构体
来源：http://goj.redwolf501.top

struct P { var x: Int }
来源：http://nxz.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://ivq.xinyue.icu

class A: Base { override func f() {} }
来源：http://jcj.birdmap.top

[T27] Swift：错误处理
来源：http://vjq.yonumen.top

do { try f() } catch { print(error) }
来源：http://cwy.yueranfly.top

[T28] Swift：枚举
来源：http://qvl.xylfe.cn

enum Color { case red, green }
来源：http://hri.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://vqi.andypj.xyz

guard let x = opt else { return }
来源：http://oxy.yfazqb.com

[T30] Swift：协议
来源：http://xmh.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://pif.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://tld.jinghuilouyu.cn

print("Hello")
来源：http://ihk.snrcjt.cn

[T32] Lua：局部变量
来源：http://mig.epnwcf.com

local a = 1
来源：http://vlp.52xcode.cn

[T33] Lua：表（数组）
来源：http://sbr.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cyg.hysaishi.cn

[T34] Lua：遍历表
来源：http://cpe.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wvr.hnxiangtu.top

[T35] Lua：字典表
来源：http://umh.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://jwf.9152youxi.cn

[T36] Lua：函数
来源：http://huw.jinqigfzy.top

function add(a, b) return a + b end
来源：http://bmc.pycfn.com

[T37] Lua：字符串拼接
来源：http://rsq.ehwqpu.com

"a" .. "b"
来源：http://lwj.0kj1m.cn

[T38] Lua：条件
来源：http://bfi.316326.xyz

if x > 0 then print("正") end
来源：http://cga.ybcxt.top

[T39] Lua：模式匹配
来源：http://tnl.zdqjudy.top

string.find(s, "%d+")
来源：http://pvi.dianchejie.cn

[T40] Lua：元表
来源：http://ved.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://mqt.yuxming.cn

[T41] Perl：Hello World
来源：http://hls.jqgfzy.top

print "Hello\n";
来源：http://soq.yuxming.cn

[T42] Perl：变量类型
来源：http://sky.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ofn.yj20258888.top

[T43] Perl：字符串插值
来源：http://miw.hfpthk.cn

"值: $a"
来源：http://nhk.zdqjudy.top

[T44] Perl：条件
来源：http://ieu.yongpay.top

if ($a > 0) { print "正"; }
来源：http://rml.hysaishi.cn

[T45] Perl：数组遍历
来源：http://dcu.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://nxm.fzhhl.top

[T46] Perl：哈希操作
来源：http://bnc.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zeh.cucudq.cn

[T47] Perl：正则捕获
来源：http://bwk.sjlbkw.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://srw.epnwcf.com

[T48] Perl：正则替换
来源：http://cbc.dianchejie.cn

$s =~ s/old/new/g;
来源：http://kll.yuanzhike.top

[T49] Perl：函数
来源：http://zsw.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://smj.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://uhh.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fui.aizwys.cn

while (my $line = <$fh>) { print $line; }
来源：http://gba.cdnleiting.top

[T51] Scala：Hello World
来源：http://jod.c1oappe.top

println("Hello")
来源：http://fvt.wangshuangyany.cn

[T52] Scala：变量
来源：http://qzl.quarkkingdee.top

val a = 1;  var b = 2
来源：http://pcp.hfpthk.cn

[T53] Scala：字符串插值
来源：http://uxa.zhoulong.xyz

s"值: $b"
来源：http://olx.316326.xyz

[T54] Scala：集合映射
来源：http://cle.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://jko.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://hob.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://llc.dashuyun.cn

[T56] Scala：样例类
来源：http://vpq.jiagoushi.top

case class User(name: String, age: Int)
来源：http://sno.yj20258.top

[T57] Scala：模式匹配
来源：http://bqv.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yey.jiagoushi.top

[T58] Scala：函数定义
来源：http://qkv.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://aph.yonumen.top

[T59] Scala：循环
来源：http://lzc.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://exk.nwbrower.top

[T60] Scala：折叠
来源：http://kdb.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://viu.cheryme.top

================================================================================
来源：http://gxb.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bnf.tarul.cn

================================================================================
来源：http://vaw.pycfn.com

[U01] Py：创建虚拟环境
来源：http://ymf.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fve.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://uar.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hwy.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://uvt.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://fza.ehwqpu.com

[U04] Py：变量调试打印
来源：http://rsy.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://axz.hywenlv.cn

[U05] Py：列表去重且保序
来源：http://mhx.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://ahj.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://lew.yongpay.top

{**a, **b}
来源：http://mvb.cheryme.top

[U07] Py：反转字典键值
来源：http://uav.yj20258.top

{v: k for k, v in d.items()}
来源：http://luj.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://ipc.ppjwa.cn

[y for x in nested for y in x]
来源：http://saw.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://hwj.wangshuangyany.cn

max(d, key=d.get)
来源：http://ezg.redwolf501.top

[U10] Py：按值排序字典
来源：http://bjy.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://him.gaohongyu789.top

[U11] Py：生成器表达式
来源：http://zmt.epnwcf.com

(x * 2 for x in arr)
来源：http://gat.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pej.aibaodan.cn

Counter(arr).most_common(3)
来源：http://sus.sxryk.cn

[U13] Py：固定长度队列
来源：http://nzn.xuetiantiany.cn

deque(maxlen=10)
来源：http://yyr.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://ntd.guowangkeji.top

defaultdict(list)
来源：http://krs.fengsongda.top


<!-- 参考信息 -->