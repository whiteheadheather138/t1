代发 wailian999

read -rp "请输入: " ans
来源：http://rbk.guannengcc.top

[R78] 交互式菜单
来源：http://mln.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vuv.jqgfzy.top

[R79] 解析命令行选项
来源：http://xix.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uii.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://tgj.zhongyouzk.top

time ./run.sh
来源：http://uec.birdmap.top

================================================================================
来源：http://dav.hysaishi.cn

S. C / C++ 专题
来源：http://nvb.aibaodan.cn

================================================================================
来源：http://tca.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://grk.pycfn.com

#include <stdio.h>
来源：http://gee.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aqa.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://ymi.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://zqp.shangyingyoupin.top

[S03] C：读入整数
来源：http://lpg.sufxvd.cn

int x; scanf("%d", &x);
来源：http://sdt.cdnleiting.top

[S04] C：字符串复制
来源：http://bxc.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://erp.jianghu66.top

[S05] C：字符串长度
来源：http://rev.chenzaomai.com

strlen(s)
来源：http://lew.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://fym.cucudq.cn

strcmp(a, b) == 0
来源：http://ubt.tarul.cn

[S07] C：数组遍历求和
来源：http://ecm.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wuu.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://ymn.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uau.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://gxy.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xtj.nanxuanxn.top

[S10] C：指针与解引用
来源：http://yhx.cucudq.cn

int *p = &a;  *p = 5;
来源：http://eib.zhoulong.xyz

[S11] C：逐行读文件
来源：http://wam.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://rnh.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xdl.zhixingplan.top

fclose(f);
来源：http://fpf.jinyuanbaomall.cn

[S12] C：写文件
来源：http://rsa.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://frb.shzxlz.cn

[S13] C：宏定义
来源：http://cgt.wangdashe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://myg.mhx1999.top

[S14] C：枚举
来源：http://roa.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://otc.yongpay.top

[S15] C：类型转换
来源：http://bol.yueranfly.top

(double) a / b
来源：http://lqx.yueranfly.top

[S16] C：位操作置位
来源：http://cgi.shuidangran.top

x |= (1 << 3);
来源：http://oht.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://cwu.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://biw.vehdjk.com

[S18] C：命令行参数
来源：http://zje.cheryme.top

int main(int argc, char **argv)
来源：http://gdg.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://fpy.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://tqd.wangshuangyany.cn

[S20] C：二分查找
来源：http://bmp.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cty.xylfe.cn

[S21] C：字符类别判断
来源：http://cyt.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wyy.zhengqikj.top

[S22] C：字符串转数字
来源：http://dlz.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://brv.jianghu66.top

[S23] C：随机数
来源：http://ckx.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fjx.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://vmi.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://puf.fehbvm.com

[S25] C：内存拷贝
来源：http://hka.cqqwz.cn

memcpy(dst, src, n);
来源：http://uxq.wangdashe.top

[S26] C：内存清零
来源：http://hej.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://cfu.52xcode.cn

[S27] C：定义常量
来源：http://cjr.hesvh.cn

const double PI = 3.14159;
来源：http://wgn.fzhhl.top

[S28] C：静态变量
来源：http://tth.smart0.xyz

static int counter = 0;
来源：http://vtx.chenlongwang.top

[S29] C：变参函数
来源：http://qqr.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gdp.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://ftq.zhengqikj.top

#ifndef X_H
来源：http://kvm.zhoulong.xyz

#define X_H
来源：http://ozv.tianlin.xyz

#endif
来源：http://gcx.gogol.net.cn

[S31] C++：Hello World
来源：http://ezx.smart0.xyz

#include <iostream>
来源：http://vvx.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://okz.chenjidiqi.icu

[S32] C++：字符串
来源：http://vgn.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://gdc.kuanghao11.cn

[S33] C++：vector 增删
来源：http://ozb.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vyz.chenlongwang.top

[S34] C++：遍历 vector
来源：http://mil.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://qcq.hfpthk.cn

[S35] C++：map
来源：http://zcm.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hyy.jianghu66.top

[S36] C++：unordered_map
来源：http://kwi.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kco.snrcjt.cn

[S37] C++：set
来源：http://vsc.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iet.ppjwa.cn

[S38] C++：排序
来源：http://mxa.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://uxc.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://ean.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nvb.pycfn.com

[S40] C++：查找元素
来源：http://vqa.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cgn.dianchejie.cn

[S41] C++：类与构造函数
来源：http://qhm.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fkc.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://ctt.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://ofw.ppjwa.cn

[S43] C++：智能指针
来源：http://pzn.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://gwb.gotoacloud.top

[S44] C++：引用传参
来源：http://qdf.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://bhv.52xcode.cn

[S45] C++：lambda
来源：http://qec.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://ssw.sjlbkw.cn

[S46] C++：函数模板
来源：http://vwu.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eto.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://oxu.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://txu.gzhubu.top

[S48] C++：逐行读文件
来源：http://bdo.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fii.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://fiy.sjlbkw.cn

[S49] C++：写文件
来源：http://cgn.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgt.yj202588.top

[S50] C++：格式化数字
来源：http://upd.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://frc.fengsongda.top

[S51] C++：显式类型转换
来源：http://dvh.bbcook.cn

static_cast<double>(a) / b
来源：http://aik.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://agp.ybcxt.top

int size() const noexcept { return n_; }
来源：http://tbr.dashuyun.cn

[S53] C++：移动语义
来源：http://tur.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://fvs.mhx1999.top

[S54] C++：异常处理
来源：http://xjd.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://evc.yj20258888.top

[S55] C++：结构化绑定
来源：http://lui.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dva.fehbvm.com

[S56] C++：optional
来源：http://vfg.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hij.zdbjq.cn

[S57] C++：编译期常量
来源：http://etb.pycfn.com

constexpr int N = 10;
来源：http://zom.sufxvd.cn

[S58] C++：命名空间
来源：http://jxy.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://imf.gogol.net.cn

[S59] C++：静态断言
来源：http://ooe.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jdp.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://huj.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbv.bbcook.cn

================================================================================
来源：http://vru.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cgi.haohaochexian.top

================================================================================
来源：http://egb.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://nkg.kuanghao11.cn

println("Hello")
来源：http://lks.hesvh.cn

[T02] Kotlin：变量
来源：http://twh.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://amv.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://abx.zdbjq.cn

"值: $b"
来源：http://afr.wangdashe.top

[T04] Kotlin：空安全
来源：http://wlr.jiagoushi.top

val n: String? = null;  n?.length
来源：http://gdk.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://tol.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cnh.xinyue.icu

[T06] Kotlin：集合映射
来源：http://lig.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pyr.yj202588.top

[T07] Kotlin：集合过滤
来源：http://pmi.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xjn.hammf.cn

[T08] Kotlin：数据类
来源：http://qax.snrcjt.cn

data class User(val name: String, val age: Int)
来源：http://luk.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://hnm.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://vda.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://sre.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://stz.52xcode.cn

[T11] Kotlin：协程
来源：http://otd.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fnn.316326.xyz

[T12] Kotlin：解构声明
来源：http://fvv.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://oaw.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://nze.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://mgl.316326.xyz

[T14] Kotlin：循环
来源：http://yhe.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://acc.cheryme.top

[T15] Kotlin：接口
来源：http://xcn.shuidangran.top

interface Shape { fun area(): Double }
来源：http://oae.yvedp.cn

[T16] Swift：Hello World
来源：http://sjh.52xcode.cn

print("Hello")
来源：http://hgn.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://aqe.vqdsnc.cn

var a = 1;  let b = 2
来源：http://slb.yuanzhike.top

[T18] Swift：字符串插值
来源：http://bub.ehwqpu.com

"值: \(b)"
来源：http://byc.cashguo.top

[T19] Swift：可选绑定
来源：http://xud.hfpthk.cn

if let n = opt { print(n) }
来源：http://tfs.quarkkingdee.top

[T20] Swift：数组操作
来源：http://xoi.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ime.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://rqc.vehdjk.com

for x in a { print(x) }
来源：http://tmr.aizwys.cn

[T22] Swift：字典
来源：http://hmt.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fgx.xuanzx.com

[T23] Swift：函数
来源：http://wrt.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mco.yj202588.top

[T24] Swift：闭包
来源：http://rsk.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://feq.ctjpmb.com

[T25] Swift：结构体
来源：http://rfq.fanxiaobao.xyz

struct P { var x: Int }
来源：http://bxd.shzxlz.cn

[T26] Swift：类与重写
来源：http://wwz.fzhhl.top

class A: Base { override func f() {} }
来源：http://syk.zhengqikj.top

[T27] Swift：错误处理
来源：http://myy.yj20258.top

do { try f() } catch { print(error) }
来源：http://ypv.fktsv.cn

[T28] Swift：枚举
来源：http://zze.yj20258888.top

enum Color { case red, green }
来源：http://ual.tarul.cn

[T29] Swift：guard 提前返回
来源：http://pqc.fengsongda.top

guard let x = opt else { return }
来源：http://khn.aibaodan.cn

[T30] Swift：协议
来源：http://ihx.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://oqw.ywan-chungtsiang.top

[T31] Lua：Hello World
来源：http://vsn.xuetiantiany.cn

print("Hello")
来源：http://lad.ctjpmb.com

[T32] Lua：局部变量
来源：http://boe.ehwqpu.com

local a = 1
来源：http://hge.cdnleiting.top

[T33] Lua：表（数组）
来源：http://mux.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cul.jianghu66.top

[T34] Lua：遍历表
来源：http://hvh.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nvd.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://dok.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://btf.snrcjt.cn

[T36] Lua：函数
来源：http://syg.zhijiandao.cn

function add(a, b) return a + b end
来源：http://vds.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://ukr.jqgufenzy.top

"a" .. "b"
来源：http://alq.yvedp.cn

[T38] Lua：条件
来源：http://oay.wangshuangyany.cn

if x > 0 then print("正") end
来源：http://ivn.vehdjk.com

[T39] Lua：模式匹配
来源：http://eex.zhoulong.xyz

string.find(s, "%d+")
来源：http://kqa.shzxlz.cn

[T40] Lua：元表
来源：http://inu.zhaomingkeji.xyz

setmetatable({}, { __index = base })
来源：http://cxv.cucudq.cn

[T41] Perl：Hello World
来源：http://sec.316326.xyz

print "Hello\n";
来源：http://waf.tarul.cn

[T42] Perl：变量类型
来源：http://bnj.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mib.hammf.cn

[T43] Perl：字符串插值
来源：http://eer.pycfn.com

"值: $a"
来源：http://kul.pengpengdd.cyou

[T44] Perl：条件
来源：http://fnp.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://pgo.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://wrd.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://wlh.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://cou.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nwl.yueranfly.top

[T47] Perl：正则捕获
来源：http://hss.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qkn.xziqi.cn

[T48] Perl：正则替换
来源：http://byl.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://tza.snrcjt.cn

[T49] Perl：函数
来源：http://wzf.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ouv.fktsv.cn

[T50] Perl：逐行读文件
来源：http://wms.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dks.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://xgr.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://wmo.gaohongyu789.top

println("Hello")
来源：http://wxi.tarul.cn

[T52] Scala：变量
来源：http://inb.yj20258888.top

val a = 1;  var b = 2
来源：http://bwi.tanke756.top

[T53] Scala：字符串插值
来源：http://bta.0kj1m.cn

s"值: $b"
来源：http://szo.yvedp.cn

[T54] Scala：集合映射
来源：http://eoi.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://lji.gogol.net.cn

[T55] Scala：集合过滤
来源：http://qkl.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://dcj.haohaochexian.top

[T56] Scala：样例类
来源：http://fpa.cheryme.top

case class User(name: String, age: Int)
来源：http://hwb.zdqjudy.top

[T57] Scala：模式匹配
来源：http://xci.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ern.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://nix.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pre.zhongyouzk.top

[T59] Scala：循环
来源：http://gbc.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://ouj.jqgufenzy.top

[T60] Scala：折叠
来源：http://ewq.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hhh.iojbl.cn

================================================================================
来源：http://fmn.shuidangran.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nrj.nanxuanxn.top

================================================================================
来源：http://smf.yj202588.top

[U01] Py：创建虚拟环境
来源：http://nzy.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://vml.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://kkk.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nym.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://xwo.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xbb.gogol.net.cn

[U04] Py：变量调试打印
来源：http://ppw.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://out.sxryk.cn

[U05] Py：列表去重且保序
来源：http://fso.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://tgx.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://svf.ydzc1.top

{**a, **b}
来源：http://qan.aibaodan.cn

[U07] Py：反转字典键值
来源：http://ynq.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://sxz.svipenyu.cn

[U08] Py：展平二维列表
来源：http://zhi.jyoumei.cn

[y for x in nested for y in x]
来源：http://rsy.ppjwa.cn

[U09] Py：字典取最大值的键
来源：http://mhb.zhixingplan.top

max(d, key=d.get)
来源：http://hpc.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://wpt.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hlx.yangfankeji.com

[U11] Py：生成器表达式
来源：http://sou.meibo888.top

(x * 2 for x in arr)
来源：http://ebs.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cjy.gotoacloud.top

Counter(arr).most_common(3)
来源：http://atb.svipenyu.cn

[U13] Py：固定长度队列
来源：http://xqu.shangyingyoupin.top

deque(maxlen=10)
来源：http://qkx.bbcook.cn

[U14] Py：分组收集到列表
来源：http://jbg.shzxlz.cn

defaultdict(list)
来源：http://ulq.snrcjt.cn

[U15] Py：高精度计时
来源：http://vkk.hysaishi.cn

t = time.perf_counter()
来源：http://rup.xingfuxueyuan.xyz

[U16] Py：命令行参数解析
来源：http://duz.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uhd.zycfv.cn

[U17] Py：初始化日志
来源：http://bsv.pycfn.com

logging.basicConfig(level=logging.INFO)
来源：http://kkm.tarul.cn

[U18] Py：预编译正则
来源：http://zfi.yj20258.top

pat = re.compile(r"\d+")
来源：http://vdb.chenlongwang.top


<!-- 参考信息 -->