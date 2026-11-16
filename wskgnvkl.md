代发 wailian999

read -rp "请输入: " ans
来源：http://xdk.ctjpmb.com

[R78] 交互式菜单
来源：http://nze.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rml.tian-w.cn

[R79] 解析命令行选项
来源：http://rlh.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mbz.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://xad.gzhubu.top

time ./run.sh
来源：http://cob.ydjk.org.cn

================================================================================
来源：http://uug.yj20258888.top

S. C / C++ 专题
来源：http://exb.hammf.cn

================================================================================
来源：http://msh.gaohongyu789.top

[S01] C：Hello World
来源：http://hbc.xylfe.cn

#include <stdio.h>
来源：http://mko.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vll.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://wxp.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://whm.fzhhl.top

[S03] C：读入整数
来源：http://iha.tianlin.xyz

int x; scanf("%d", &x);
来源：http://dwj.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://dto.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://lfs.bbcook.cn

[S05] C：字符串长度
来源：http://kfd.hcnkem.com

strlen(s)
来源：http://fzl.hcnkem.com

[S06] C：字符串比较
来源：http://epu.tanke756.top

strcmp(a, b) == 0
来源：http://yjp.c1oappe.top

[S07] C：数组遍历求和
来源：http://eok.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sgx.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://hlg.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dhj.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://ujc.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uri.zhoulong.xyz

[S10] C：指针与解引用
来源：http://hcv.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://zbm.vqdsnc.cn

[S11] C：逐行读文件
来源：http://lwe.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://vaa.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aio.andypj.xyz

fclose(f);
来源：http://qpe.xuanzx.com

[S12] C：写文件
来源：http://xll.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mps.gzhubu.top

[S13] C：宏定义
来源：http://hor.sufxvd.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ptk.xuanzx.com

[S14] C：枚举
来源：http://auy.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://kyf.c1oappe.top

[S15] C：类型转换
来源：http://uhb.shanyushiyangkeji.top

(double) a / b
来源：http://tjy.cheryme.top

[S16] C：位操作置位
来源：http://kww.uphjek.com

x |= (1 << 3);
来源：http://kqi.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://ilb.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nxi.ctjpmb.com

[S18] C：命令行参数
来源：http://mca.svipenyu.cn

int main(int argc, char **argv)
来源：http://edo.snrcjt.cn

[S19] C：快速排序
来源：http://qkp.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gjn.cashguo.top

[S20] C：二分查找
来源：http://nwh.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qtn.kuanghao11.cn

[S21] C：字符类别判断
来源：http://mee.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://trw.yuanzhike.top

[S22] C：字符串转数字
来源：http://fxs.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rru.yj20258.top

[S23] C：随机数
来源：http://zpj.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://sir.hfpthk.cn

[S24] C：获取本地时间
来源：http://qri.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hnw.redwolf501.top

[S25] C：内存拷贝
来源：http://hkx.redwolf501.top

memcpy(dst, src, n);
来源：http://ykw.hcnkem.com

[S26] C：内存清零
来源：http://pfo.pycfn.com

memset(a, 0, sizeof a);
来源：http://igw.sysykeji.top

[S27] C：定义常量
来源：http://wzs.0kj1m.cn

const double PI = 3.14159;
来源：http://ejd.birdmap.top

[S28] C：静态变量
来源：http://rcn.havefunace.top

static int counter = 0;
来源：http://pjd.daria6918.cn

[S29] C：变参函数
来源：http://joo.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uiv.shzxlz.cn

[S30] C：头文件保护
来源：http://frc.yj202588.top

#ifndef X_H
来源：http://lkj.52xcode.cn

#define X_H
来源：http://ksv.haohaochexian.top

#endif
来源：http://bgo.ppjwa.cn

[S31] C++：Hello World
来源：http://ytf.jinqigufen.top

#include <iostream>
来源：http://yrp.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://bej.zhiwuduotai.top

[S32] C++：字符串
来源：http://ymc.tian-w.cn

std::string s = "hi";  s += "!";
来源：http://xij.jinqigufen.top

[S33] C++：vector 增删
来源：http://nlh.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ztf.gogol.net.cn

[S34] C++：遍历 vector
来源：http://fxo.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://ruz.fehbvm.com

[S35] C++：map
来源：http://hcf.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oqr.yanxiufei.cn

[S36] C++：unordered_map
来源：http://ivy.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://klq.zhoulong.xyz

[S37] C++：set
来源：http://zqy.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://djo.xinyue.icu

[S38] C++：排序
来源：http://fvo.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://fsb.pycfn.com

[S39] C++：自定义比较器排序
来源：http://slx.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ahe.zhixingplan.top

[S40] C++：查找元素
来源：http://rbt.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxz.nanxinkj.top

[S41] C++：类与构造函数
来源：http://vui.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tlr.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://mzr.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://fyu.wangdashe.top

[S43] C++：智能指针
来源：http://ijk.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://iyg.hammf.cn

[S44] C++：引用传参
来源：http://oha.yj202588.top

void inc(int &x) { ++x; }
来源：http://okf.jinqigufen.top

[S45] C++：lambda
来源：http://xqy.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://cax.sufxvd.cn

[S46] C++：函数模板
来源：http://mpc.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://giv.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://giv.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xkk.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://rnf.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://dub.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://dwz.daxiang520.top

[S49] C++：写文件
来源：http://ifp.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tku.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://edm.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://umn.xylfe.cn

[S51] C++：显式类型转换
来源：http://zog.fengsongda.top

static_cast<double>(a) / b
来源：http://erp.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://gsk.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://fqf.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://qvb.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://bgm.0kj1m.cn

[S54] C++：异常处理
来源：http://wuk.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxz.vehdjk.com

[S55] C++：结构化绑定
来源：http://meg.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://alj.yongpay.top

[S56] C++：optional
来源：http://ews.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tes.nwbrower.top

[S57] C++：编译期常量
来源：http://npa.gotoacloud.top

constexpr int N = 10;
来源：http://tey.smart0.xyz

[S58] C++：命名空间
来源：http://lkj.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://kuw.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://ptc.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oec.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://oin.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yso.smart0.xyz

================================================================================
来源：http://btf.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zpl.ppjwa.cn

================================================================================
来源：http://qmg.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://oum.316326.xyz

println("Hello")
来源：http://skv.dashuyun.cn

[T02] Kotlin：变量
来源：http://pww.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgg.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://clw.sxryk.cn

"值: $b"
来源：http://hst.xylfe.cn

[T04] Kotlin：空安全
来源：http://acm.c1oappe.top

val n: String? = null;  n?.length
来源：http://hnn.wangshuangyany.cn

[T05] Kotlin：when 表达式
来源：http://rht.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cbm.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://zjp.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ocn.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://qlw.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kji.yj202588.top

[T08] Kotlin：数据类
来源：http://vjv.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://uii.hammf.cn

[T09] Kotlin：扩展函数
来源：http://uvq.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://tzk.yfazqb.com

[T10] Kotlin：默认参数
来源：http://nbh.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://epu.tianlin.xyz

[T11] Kotlin：协程
来源：http://bjf.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://pql.tanke756.top

[T12] Kotlin：解构声明
来源：http://nxs.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://uoi.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://fgq.ybcxt.top

val m = mapOf("a" to 1)
来源：http://hhl.yj20258888.top

[T14] Kotlin：循环
来源：http://baf.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://ska.jlsjyb.cn

[T15] Kotlin：接口
来源：http://mwh.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://owr.andypj.xyz

[T16] Swift：Hello World
来源：http://jrp.sjlbkw.cn

print("Hello")
来源：http://dls.shuidangran.top

[T17] Swift：变量与常量
来源：http://sci.hfpthk.cn

var a = 1;  let b = 2
来源：http://iwb.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://hyn.andypj.xyz

"值: \(b)"
来源：http://vdo.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://nhq.haohaochexian.top

if let n = opt { print(n) }
来源：http://sas.yj20258.top

[T20] Swift：数组操作
来源：http://ngn.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://zki.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://xsb.wangdashe.top

for x in a { print(x) }
来源：http://vpt.pengpengdd.cyou

[T22] Swift：字典
来源：http://uyj.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nre.gzhubu.top

[T23] Swift：函数
来源：http://qwx.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fkg.cashguo.top

[T24] Swift：闭包
来源：http://hnf.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ori.ehwqpu.com

[T25] Swift：结构体
来源：http://zoj.yuanzhike.top

struct P { var x: Int }
来源：http://vtu.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://wsi.chenlongwang.top

class A: Base { override func f() {} }
来源：http://ahk.zhaomingkeji.xyz

[T27] Swift：错误处理
来源：http://qkq.birdmap.top

do { try f() } catch { print(error) }
来源：http://rph.shzxlz.cn

[T28] Swift：枚举
来源：http://raq.tanke756.top

enum Color { case red, green }
来源：http://pgf.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://wrg.meibo888.top

guard let x = opt else { return }
来源：http://fes.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://ggl.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://hfx.aizwys.cn

[T31] Lua：Hello World
来源：http://tte.shzxlz.cn

print("Hello")
来源：http://uzh.zdbjq.cn

[T32] Lua：局部变量
来源：http://cvw.sysykeji.top

local a = 1
来源：http://gyz.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://qqa.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pag.hnqzz.top

[T34] Lua：遍历表
来源：http://irz.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ylc.jyoumei.cn

[T35] Lua：字典表
来源：http://fur.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://byh.pycfn.com

[T36] Lua：函数
来源：http://who.kuanghao11.cn

function add(a, b) return a + b end
来源：http://ztm.hnxiangtu.top

[T37] Lua：字符串拼接
来源：http://cgk.yuxming.cn

"a" .. "b"
来源：http://oqs.jinghuilouyu.cn

[T38] Lua：条件
来源：http://iah.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://yei.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://ozi.meibo888.top

string.find(s, "%d+")
来源：http://kqg.cqqwz.cn

[T40] Lua：元表
来源：http://qvi.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://xht.zhongyouzk.top

[T41] Perl：Hello World
来源：http://eik.bjfxy.top

print "Hello\n";
来源：http://xuc.birdmap.top

[T42] Perl：变量类型
来源：http://mew.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nsq.hammf.cn

[T43] Perl：字符串插值
来源：http://plu.yonumen.top

"值: $a"
来源：http://czk.fengsongda.top

[T44] Perl：条件
来源：http://slh.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://nmr.birdmap.top

[T45] Perl：数组遍历
来源：http://rzo.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://pbu.hywenlv.cn

[T46] Perl：哈希操作
来源：http://lhc.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jzq.yfazqb.com

[T47] Perl：正则捕获
来源：http://zyw.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qzr.jinqigufen.top

[T48] Perl：正则替换
来源：http://jxw.ivvv.top

$s =~ s/old/new/g;
来源：http://alt.hnxiangtu.top

[T49] Perl：函数
来源：http://bmp.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eir.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://nrt.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://hsm.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://ydj.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://kgi.fanxiaobao.xyz

println("Hello")
来源：http://qqq.sxryk.cn

[T52] Scala：变量
来源：http://kwe.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://qmz.wangdashe.top

[T53] Scala：字符串插值
来源：http://gzy.pengpengdd.cyou

s"值: $b"
来源：http://etv.hnqzz.top

[T54] Scala：集合映射
来源：http://kcy.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://kpa.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://tvv.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qhl.zhengqikj.top

[T56] Scala：样例类
来源：http://cbf.cucudq.cn

case class User(name: String, age: Int)
来源：http://ufj.redwolf501.top

[T57] Scala：模式匹配
来源：http://riq.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rhd.sufxvd.cn

[T58] Scala：函数定义
来源：http://ohu.ctjpmb.com

def add(a: Int, b: Int): Int = a + b
来源：http://gdn.chenlongwang.top

[T59] Scala：循环
来源：http://mnn.sxryk.cn

for (i <- 1 to 10) println(i)
来源：http://ood.nanxinkj.top

[T60] Scala：折叠
来源：http://gnw.yuxming.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://clr.sufxvd.cn

================================================================================
来源：http://yfp.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pak.feifeiyinyue.top

================================================================================
来源：http://yrf.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://phz.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pau.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://rxh.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uof.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://czd.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zff.daxiang520.top

[U04] Py：变量调试打印
来源：http://bgh.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iav.cashguo.top

[U05] Py：列表去重且保序
来源：http://ojw.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://hvx.yvedp.cn

[U06] Py：合并两个字典
来源：http://opf.yangfankeji.com

{**a, **b}
来源：http://qkm.chenlongwang.top

[U07] Py：反转字典键值
来源：http://dbv.52xcode.cn

{v: k for k, v in d.items()}
来源：http://igd.tianlin.xyz

[U08] Py：展平二维列表
来源：http://icw.ivvv.top

[y for x in nested for y in x]
来源：http://bhj.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://zhx.aizwys.cn

max(d, key=d.get)
来源：http://wpz.cdnleiting.top

[U10] Py：按值排序字典
来源：http://rwi.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://piy.zdqjudy.top

[U11] Py：生成器表达式
来源：http://klb.gogol.net.cn

(x * 2 for x in arr)
来源：http://cyh.ppjwa.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mqg.mhx1999.top

Counter(arr).most_common(3)
来源：http://xsc.guowangkeji.top

[U13] Py：固定长度队列
来源：http://yqz.snrcjt.cn

deque(maxlen=10)
来源：http://axn.shuidangran.top

[U14] Py：分组收集到列表
来源：http://sfb.andypj.xyz

defaultdict(list)
来源：http://rzz.yvedp.cn

[U15] Py：高精度计时
来源：http://hlx.ydjk.org.cn

t = time.perf_counter()
来源：http://bdn.wangdashe.top

[U16] Py：命令行参数解析
来源：http://ylm.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vmw.jyoumei.cn

[U17] Py：初始化日志
来源：http://fzi.9152youxi.cn

logging.basicConfig(level=logging.INFO)
来源：http://rgs.jinqigfzy.top

[U18] Py：预编译正则
来源：http://vnz.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://aan.cucudq.cn


<!-- 参考信息 -->