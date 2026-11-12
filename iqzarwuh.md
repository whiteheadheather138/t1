代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://lhj.quarkkingdee.top

[R76] 使用临时文件
来源：http://sww.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bef.jianghu66.top

[R77] 读取用户输入
来源：http://par.ivvv.top

read -rp "请输入: " ans
来源：http://nwa.nanxinkj.top

[R78] 交互式菜单
来源：http://its.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fqi.cashguo.top

[R79] 解析命令行选项
来源：http://mow.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kce.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://bdl.fzhhl.top

time ./run.sh
来源：http://qki.feifeiyinyue.top

================================================================================
来源：http://nve.cdnleiting.top

S. C / C++ 专题
来源：http://jdt.yueranfly.top

================================================================================
来源：http://zqz.shuidangran.top

[S01] C：Hello World
来源：http://xgy.sufxvd.cn

#include <stdio.h>
来源：http://vod.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vnp.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://fdb.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://gzn.jlsjyb.cn

[S03] C：读入整数
来源：http://ilb.ybcxt.top

int x; scanf("%d", &x);
来源：http://anw.zhengqikj.top

[S04] C：字符串复制
来源：http://xoc.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xtl.hcnkem.com

[S05] C：字符串长度
来源：http://qgz.nanxinkj.top

strlen(s)
来源：http://jyi.sxryk.cn

[S06] C：字符串比较
来源：http://ukf.daria6918.cn

strcmp(a, b) == 0
来源：http://fwp.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://fxk.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tnm.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://asb.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rmk.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://ldv.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jlo.hcnkem.com

[S10] C：指针与解引用
来源：http://ckt.ybcxt.top

int *p = &a;  *p = 5;
来源：http://blq.mhx1999.top

[S11] C：逐行读文件
来源：http://bpp.hywenlv.cn

FILE *f = fopen("a.txt", "r");
来源：http://aqn.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://muz.gotoacloud.top

fclose(f);
来源：http://nak.zycfv.cn

[S12] C：写文件
来源：http://xya.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zll.nwbrower.top

[S13] C：宏定义
来源：http://fgj.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ywx.kuanghao11.cn

[S14] C：枚举
来源：http://ktz.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://fie.316326.xyz

[S15] C：类型转换
来源：http://foe.shangyingyoupin.top

(double) a / b
来源：http://qiv.yongpay.top

[S16] C：位操作置位
来源：http://ybr.guowangkeji.top

x |= (1 << 3);
来源：http://qpb.pycfn.com

[S17] C：安全拼接字符串
来源：http://azx.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qwq.ppjwa.cn

[S18] C：命令行参数
来源：http://oau.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://jfz.fengsongda.top

[S19] C：快速排序
来源：http://jfq.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://gde.pengpengdd.cyou

[S20] C：二分查找
来源：http://lio.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wcc.gzhubu.top

[S21] C：字符类别判断
来源：http://fxv.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lpo.cucudq.cn

[S22] C：字符串转数字
来源：http://rfx.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://ctb.vehdjk.com

[S23] C：随机数
来源：http://cde.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yhs.jlsjyb.cn

[S24] C：获取本地时间
来源：http://rhr.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rcc.xziqi.cn

[S25] C：内存拷贝
来源：http://zsq.wangdashe.top

memcpy(dst, src, n);
来源：http://rbl.jqgufenzy.top

[S26] C：内存清零
来源：http://azm.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://zrr.yj20258888.top

[S27] C：定义常量
来源：http://phy.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://vdt.hcnkem.com

[S28] C：静态变量
来源：http://qrx.yj202588.top

static int counter = 0;
来源：http://cxv.zhiwuduotai.top

[S29] C：变参函数
来源：http://htv.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://boq.mhx1999.top

[S30] C：头文件保护
来源：http://mjm.xuetiantiany.cn

#ifndef X_H
来源：http://qbn.cucudq.cn

#define X_H
来源：http://tcf.snrcjt.cn

#endif
来源：http://uce.yanxiufei.cn

[S31] C++：Hello World
来源：http://mru.wangdashe.top

#include <iostream>
来源：http://dpn.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://cov.yanxiufei.cn

[S32] C++：字符串
来源：http://iir.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://plc.9152youxi.cn

[S33] C++：vector 增删
来源：http://tfe.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jvp.aizwys.cn

[S34] C++：遍历 vector
来源：http://fti.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://gyu.redwolf501.top

[S35] C++：map
来源：http://krj.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dwh.gotoacloud.top

[S36] C++：unordered_map
来源：http://dtk.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odc.hywenlv.cn

[S37] C++：set
来源：http://jzm.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lnt.yanxiufei.cn

[S38] C++：排序
来源：http://pxr.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://osd.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://dai.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://snf.gzhubu.top

[S40] C++：查找元素
来源：http://tat.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kgn.9152youxi.cn

[S41] C++：类与构造函数
来源：http://pdp.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ykx.c1oappe.top

[S42] C++：继承与虚函数
来源：http://eox.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://wll.feifeiyinyue.top

[S43] C++：智能指针
来源：http://rhn.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://clk.vqdsnc.cn

[S44] C++：引用传参
来源：http://ojd.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://ixn.tarul.cn

[S45] C++：lambda
来源：http://inn.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://dno.daria6918.cn

[S46] C++：函数模板
来源：http://val.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ogk.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://pca.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://srl.guowangkeji.top

[S48] C++：逐行读文件
来源：http://zko.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tfs.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://nsy.0kj1m.cn

[S49] C++：写文件
来源：http://bnu.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jwl.yanxiufei.cn

[S50] C++：格式化数字
来源：http://eqj.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nek.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://lub.birdmap.top

static_cast<double>(a) / b
来源：http://wiw.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://yis.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://dbx.vehdjk.com

[S53] C++：移动语义
来源：http://vag.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://bxd.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://hry.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wjr.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://wgg.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://oxl.hcnkem.com

[S56] C++：optional
来源：http://iic.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ugv.xziqi.cn

[S57] C++：编译期常量
来源：http://seg.cashguo.top

constexpr int N = 10;
来源：http://zbm.feifeiyinyue.top

[S58] C++：命名空间
来源：http://azk.sweek.top

namespace ns { int f() { return 1; } }
来源：http://qui.hammf.cn

[S59] C++：静态断言
来源：http://dwo.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://npn.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://rzl.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://otl.zhaomingkeji.xyz

================================================================================
来源：http://hnz.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bed.fanxiaobao.xyz

================================================================================
来源：http://pjg.epnwcf.com

[T01] Kotlin：Hello World
来源：http://xwd.wangdashe.top

println("Hello")
来源：http://xdi.sysykeji.top

[T02] Kotlin：变量
来源：http://vra.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dnb.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://qen.zhiwuduotai.top

"值: $b"
来源：http://wdw.gogol.net.cn

[T04] Kotlin：空安全
来源：http://ggq.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://qjq.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://lud.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://acl.yfazqb.com

[T06] Kotlin：集合映射
来源：http://bmq.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sas.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://mvp.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bal.c1oappe.top

[T08] Kotlin：数据类
来源：http://wqu.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://ezn.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://ucg.meibo888.top

fun String.exclaim() = this + "!"
来源：http://pde.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://dmc.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rhw.ppjwa.cn

[T11] Kotlin：协程
来源：http://aiv.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lri.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ice.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://vdf.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://anf.aizwys.cn

val m = mapOf("a" to 1)
来源：http://jbs.hcnkem.com

[T14] Kotlin：循环
来源：http://zoo.yongpay.top

for (i in 1..10) println(i)
来源：http://khk.hysaishi.cn

[T15] Kotlin：接口
来源：http://qmi.redwolf501.top

interface Shape { fun area(): Double }
来源：http://hyi.tian-w.cn

[T16] Swift：Hello World
来源：http://vec.gogol.net.cn

print("Hello")
来源：http://owu.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://sli.yj20258888.top

var a = 1;  let b = 2
来源：http://mtu.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://xcj.cucudq.cn

"值: \(b)"
来源：http://szr.xziqi.cn

[T19] Swift：可选绑定
来源：http://dho.chenlongwang.top

if let n = opt { print(n) }
来源：http://krj.52xcode.cn

[T20] Swift：数组操作
来源：http://fbw.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://jbq.birdmap.top

[T21] Swift：遍历
来源：http://xax.iojbl.cn

for x in a { print(x) }
来源：http://hup.ybcxt.top

[T22] Swift：字典
来源：http://mil.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://bwk.52xcode.cn

[T23] Swift：函数
来源：http://alb.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://isb.zhengqikj.top

[T24] Swift：闭包
来源：http://zno.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qms.ehwqpu.com

[T25] Swift：结构体
来源：http://uje.yj20258.top

struct P { var x: Int }
来源：http://xkd.fehbvm.com

[T26] Swift：类与重写
来源：http://jbb.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://lya.0kj1m.cn

[T27] Swift：错误处理
来源：http://sus.wangshuangyany.cn

do { try f() } catch { print(error) }
来源：http://aug.yangfankeji.com

[T28] Swift：枚举
来源：http://nni.quarkkingdee.top

enum Color { case red, green }
来源：http://qwd.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://vkr.haohaochexian.top

guard let x = opt else { return }
来源：http://qgp.gotoacloud.top

[T30] Swift：协议
来源：http://ngb.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://cxr.ppjwa.cn

[T31] Lua：Hello World
来源：http://ulu.316326.xyz

print("Hello")
来源：http://jua.sjlbkw.cn

[T32] Lua：局部变量
来源：http://lvr.jinyuanbaomall.cn

local a = 1
来源：http://sid.cashguo.top

[T33] Lua：表（数组）
来源：http://swp.zdqjudy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sih.jiagoushi.top

[T34] Lua：遍历表
来源：http://muu.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://ydw.yonumen.top

[T35] Lua：字典表
来源：http://ezi.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://fhi.jianghu66.top

[T36] Lua：函数
来源：http://whk.sxryk.cn

function add(a, b) return a + b end
来源：http://igl.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://lij.ywan-chungtsiang.top

"a" .. "b"
来源：http://pqj.bbcook.cn

[T38] Lua：条件
来源：http://tju.redwolf501.top

if x > 0 then print("正") end
来源：http://qly.yvedp.cn

[T39] Lua：模式匹配
来源：http://zjm.zhoulong.xyz

string.find(s, "%d+")
来源：http://myb.iojbl.cn

[T40] Lua：元表
来源：http://uen.sweek.top

setmetatable({}, { __index = base })
来源：http://eyo.tanke756.top

[T41] Perl：Hello World
来源：http://ers.kuanghao11.cn

print "Hello\n";
来源：http://zbj.gzhubu.top

[T42] Perl：变量类型
来源：http://zcp.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hbv.chenzaomai.com

[T43] Perl：字符串插值
来源：http://dbo.ydjk.org.cn

"值: $a"
来源：http://lje.hesvh.cn

[T44] Perl：条件
来源：http://lrg.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://xzh.fehbvm.com

[T45] Perl：数组遍历
来源：http://vmt.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://agv.daria6918.cn

[T46] Perl：哈希操作
来源：http://sph.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mke.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://hrp.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fsm.tanke756.top

[T48] Perl：正则替换
来源：http://ile.iojbl.cn

$s =~ s/old/new/g;
来源：http://mgj.xuetiantiany.cn

[T49] Perl：函数
来源：http://ynr.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://old.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://hpx.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ssi.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://zbb.gotoacloud.top

[T51] Scala：Hello World
来源：http://idi.gotoacloud.top

println("Hello")
来源：http://njr.ppjwa.cn

[T52] Scala：变量
来源：http://toe.zhijiandao.cn

val a = 1;  var b = 2
来源：http://wex.nwbrower.top

[T53] Scala：字符串插值
来源：http://ubc.yvedp.cn

s"值: $b"
来源：http://yow.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://qrk.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://ndu.hysaishi.cn

[T55] Scala：集合过滤
来源：http://guv.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://yid.pycfn.com

[T56] Scala：样例类
来源：http://dxw.cqqwz.cn

case class User(name: String, age: Int)
来源：http://wos.jqgfzy.top

[T57] Scala：模式匹配
来源：http://lce.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsn.yangfankeji.com

[T58] Scala：函数定义
来源：http://qva.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://giz.epnwcf.com

[T59] Scala：循环
来源：http://uhs.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://oww.pycfn.com

[T60] Scala：折叠
来源：http://put.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xhu.jinqigufen.top

================================================================================
来源：http://qch.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jrr.jiagoushi.top

================================================================================
来源：http://ran.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://gxn.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://kxx.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://haw.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://meu.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://mkx.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sfl.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://vad.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zsq.redwolf501.top

[U05] Py：列表去重且保序
来源：http://sps.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://wit.pycfn.com

[U06] Py：合并两个字典
来源：http://ngy.sxryk.cn

{**a, **b}
来源：http://zrd.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://cgq.cucudq.cn

{v: k for k, v in d.items()}
来源：http://aus.yongpay.top

[U08] Py：展平二维列表
来源：http://zmx.chenzaomai.com

[y for x in nested for y in x]
来源：http://suc.hammf.cn

[U09] Py：字典取最大值的键
来源：http://zaj.ivvv.top

max(d, key=d.get)
来源：http://cil.cdnleiting.top

[U10] Py：按值排序字典
来源：http://bds.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lld.ydjk.org.cn

[U11] Py：生成器表达式
来源：http://fce.zdbjq.cn

(x * 2 for x in arr)
来源：http://ytp.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://iet.cqqwz.cn

Counter(arr).most_common(3)
来源：http://dwl.hammf.cn

[U13] Py：固定长度队列
来源：http://cod.haohaochexian.top

deque(maxlen=10)
来源：http://ukt.hesvh.cn

[U14] Py：分组收集到列表
来源：http://abu.sufxvd.cn

defaultdict(list)
来源：http://kza.epnwcf.com

[U15] Py：高精度计时
来源：http://rgo.chenjidiqi.icu

t = time.perf_counter()
来源：http://frx.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://geh.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sty.xuetiantiany.cn


<!-- 参考信息 -->