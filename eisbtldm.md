代发 wailian999

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ylv.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://zzy.xuanzx.com

time ./run.sh
来源：http://bxm.fzhhl.top

================================================================================
来源：http://xyx.zhixingplan.top

S. C / C++ 专题
来源：http://gtw.sufxvd.cn

================================================================================
来源：http://ihq.zdbjq.cn

[S01] C：Hello World
来源：http://rob.iojbl.cn

#include <stdio.h>
来源：http://nqy.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fmm.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://mki.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://tvp.yueranfly.top

[S03] C：读入整数
来源：http://bxw.yongpay.top

int x; scanf("%d", &x);
来源：http://itl.jlsjyb.cn

[S04] C：字符串复制
来源：http://iep.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://xfk.gzhubu.top

[S05] C：字符串长度
来源：http://xmb.nanxinkj.top

strlen(s)
来源：http://vhj.fengsongda.top

[S06] C：字符串比较
来源：http://pqx.bbcook.cn

strcmp(a, b) == 0
来源：http://yam.ivvv.top

[S07] C：数组遍历求和
来源：http://uza.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://utc.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://oek.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sjk.birdmap.top

[S09] C：结构体定义与初始化
来源：http://hpy.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hao.hywenlv.cn

[S10] C：指针与解引用
来源：http://tjt.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://wfn.hnqzz.top

[S11] C：逐行读文件
来源：http://vja.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://tae.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zck.uphjek.com

fclose(f);
来源：http://uuk.xinyue.icu

[S12] C：写文件
来源：http://kqb.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xrj.birdmap.top

[S13] C：宏定义
来源：http://nme.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jgz.nwbrower.top

[S14] C：枚举
来源：http://vot.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://jtm.yongpay.top

[S15] C：类型转换
来源：http://bxj.jinghuilouyu.cn

(double) a / b
来源：http://zhk.guannengcc.top

[S16] C：位操作置位
来源：http://jji.hysaishi.cn

x |= (1 << 3);
来源：http://qnl.shuidangran.top

[S17] C：安全拼接字符串
来源：http://mmf.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://skx.smart0.xyz

[S18] C：命令行参数
来源：http://hfo.yj202588.top

int main(int argc, char **argv)
来源：http://qsp.zhixingplan.top

[S19] C：快速排序
来源：http://rru.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://uhh.sufxvd.cn

[S20] C：二分查找
来源：http://akd.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ahu.nanxuanxn.top

[S21] C：字符类别判断
来源：http://vsc.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kmy.ehwqpu.com

[S22] C：字符串转数字
来源：http://ddg.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wim.jyoumei.cn

[S23] C：随机数
来源：http://hxe.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bwl.sjlbkw.cn

[S24] C：获取本地时间
来源：http://nyz.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jcm.zdbjq.cn

[S25] C：内存拷贝
来源：http://ybp.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://ylf.zhixingplan.top

[S26] C：内存清零
来源：http://plm.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://loz.hammf.cn

[S27] C：定义常量
来源：http://qrd.zhoulong.xyz

const double PI = 3.14159;
来源：http://fst.sjlbkw.cn

[S28] C：静态变量
来源：http://fgc.shzxlz.cn

static int counter = 0;
来源：http://nga.shzxlz.cn

[S29] C：变参函数
来源：http://vuw.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://chu.wangdashe.top

[S30] C：头文件保护
来源：http://dfp.zhiwuduotai.top

#ifndef X_H
来源：http://rte.zhixingplan.top

#define X_H
来源：http://qgu.sxryk.cn

#endif
来源：http://hbj.ivvv.top

[S31] C++：Hello World
来源：http://mqr.0kj1m.cn

#include <iostream>
来源：http://rnz.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://juw.fengsongda.top

[S32] C++：字符串
来源：http://pfb.cheryme.top

std::string s = "hi";  s += "!";
来源：http://eix.gzhubu.top

[S33] C++：vector 增删
来源：http://cge.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fij.hysaishi.cn

[S34] C++：遍历 vector
来源：http://vjt.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://bfw.fktsv.cn

[S35] C++：map
来源：http://gcq.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kxf.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://apv.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khl.daxiang520.top

[S37] C++：set
来源：http://pma.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spx.shuidangran.top

[S38] C++：排序
来源：http://cii.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://ahl.cashguo.top

[S39] C++：自定义比较器排序
来源：http://ruh.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ccy.wangdashe.top

[S40] C++：查找元素
来源：http://qdu.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://weh.xuanzx.com

[S41] C++：类与构造函数
来源：http://vmu.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rji.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://ygl.ppjwa.cn

class B : public Base { public: void f() override {} };
来源：http://itw.ybcxt.top

[S43] C++：智能指针
来源：http://wzf.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://kip.tarul.cn

[S44] C++：引用传参
来源：http://ely.hnxiangtu.top

void inc(int &x) { ++x; }
来源：http://glb.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://qha.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://ekd.iojbl.cn

[S46] C++：函数模板
来源：http://tft.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kte.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://qiu.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xcz.yj20258.top

[S48] C++：逐行读文件
来源：http://uqe.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://nxc.uphjek.com

while (std::getline(in, line)) { }
来源：http://yyq.ppjwa.cn

[S49] C++：写文件
来源：http://api.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uoi.wangdashe.top

[S50] C++：格式化数字
来源：http://ubz.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fdt.gzhubu.top

[S51] C++：显式类型转换
来源：http://dov.redwolf501.top

static_cast<double>(a) / b
来源：http://nlw.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://zwu.fehbvm.com

int size() const noexcept { return n_; }
来源：http://qlf.tanke756.top

[S53] C++：移动语义
来源：http://oan.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://cbd.aizwys.cn

[S54] C++：异常处理
来源：http://agb.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwz.guowangkeji.top

[S55] C++：结构化绑定
来源：http://ozd.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://crl.smart0.xyz

[S56] C++：optional
来源：http://wqk.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbe.gaohongyu789.top

[S57] C++：编译期常量
来源：http://ogp.zdbjq.cn

constexpr int N = 10;
来源：http://xol.yj20258888.top

[S58] C++：命名空间
来源：http://apg.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://pik.shuidangran.top

[S59] C++：静态断言
来源：http://lku.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vyl.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://jao.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dit.chenjidiqi.icu

================================================================================
来源：http://qlg.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lhe.guowangkeji.top

================================================================================
来源：http://qmx.iojbl.cn

[T01] Kotlin：Hello World
来源：http://ksy.zhongyouzk.top

println("Hello")
来源：http://fyw.xinyue.icu

[T02] Kotlin：变量
来源：http://tdy.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nsx.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://fjl.haohaochexian.top

"值: $b"
来源：http://htv.svipenyu.cn

[T04] Kotlin：空安全
来源：http://wta.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://naz.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://yii.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nxj.daria6918.cn

[T06] Kotlin：集合映射
来源：http://pvx.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://evi.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://dwk.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uqx.0kj1m.cn

[T08] Kotlin：数据类
来源：http://uie.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://fyq.uphjek.com

[T09] Kotlin：扩展函数
来源：http://ubn.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://xlw.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://hhp.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sxg.zhixingplan.top

[T11] Kotlin：协程
来源：http://clc.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://qpp.yj202588.top

[T12] Kotlin：解构声明
来源：http://fbm.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://veg.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://das.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://aur.jqgufenzy.top

[T14] Kotlin：循环
来源：http://dzl.hcnkem.com

for (i in 1..10) println(i)
来源：http://hdp.guannengcc.top

[T15] Kotlin：接口
来源：http://szm.xuanzx.com

interface Shape { fun area(): Double }
来源：http://pbg.chenzaomai.com

[T16] Swift：Hello World
来源：http://keg.yj20258888.top

print("Hello")
来源：http://cfh.snrcjt.cn

[T17] Swift：变量与常量
来源：http://dsw.snrcjt.cn

var a = 1;  let b = 2
来源：http://lbh.epnwcf.com

[T18] Swift：字符串插值
来源：http://dzv.quarkkingdee.top

"值: \(b)"
来源：http://dty.sufxvd.cn

[T19] Swift：可选绑定
来源：http://jpl.andypj.xyz

if let n = opt { print(n) }
来源：http://cne.yfazqb.com

[T20] Swift：数组操作
来源：http://xuw.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://hwg.hcnkem.com

[T21] Swift：遍历
来源：http://tgn.jyoumei.cn

for x in a { print(x) }
来源：http://gij.hcnkem.com

[T22] Swift：字典
来源：http://mwj.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://onb.xuanzx.com

[T23] Swift：函数
来源：http://ccr.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lbr.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://ggv.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://kbo.yongpay.top

[T25] Swift：结构体
来源：http://asx.chenjidiqi.icu

struct P { var x: Int }
来源：http://nrs.uphjek.com

[T26] Swift：类与重写
来源：http://ksm.ydzc1.top

class A: Base { override func f() {} }
来源：http://knc.sufxvd.cn

[T27] Swift：错误处理
来源：http://kui.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://oaa.hcnkem.com

[T28] Swift：枚举
来源：http://taq.hcnkem.com

enum Color { case red, green }
来源：http://gdp.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://dzx.yuanzhike.top

guard let x = opt else { return }
来源：http://eln.jinqigufen.top

[T30] Swift：协议
来源：http://xqz.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://yal.epnwcf.com

[T31] Lua：Hello World
来源：http://eio.zhoulong.xyz

print("Hello")
来源：http://uhq.cqqwz.cn

[T32] Lua：局部变量
来源：http://sdl.tanke756.top

local a = 1
来源：http://hab.havefunace.top

[T33] Lua：表（数组）
来源：http://oyr.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wgx.cashguo.top

[T34] Lua：遍历表
来源：http://xka.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wcx.zhijiandao.cn

[T35] Lua：字典表
来源：http://vqq.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://gjt.jiagoushi.top

[T36] Lua：函数
来源：http://zba.52xcode.cn

function add(a, b) return a + b end
来源：http://uqx.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://lzt.ydjk.org.cn

"a" .. "b"
来源：http://qtk.wangshuangyany.cn

[T38] Lua：条件
来源：http://koc.snrcjt.cn

if x > 0 then print("正") end
来源：http://ahb.jiagoushi.top

[T39] Lua：模式匹配
来源：http://xlk.jqgfzy.top

string.find(s, "%d+")
来源：http://gma.0kj1m.cn

[T40] Lua：元表
来源：http://olx.yfazqb.com

setmetatable({}, { __index = base })
来源：http://lyu.zdbjq.cn

[T41] Perl：Hello World
来源：http://eyq.yj20258888.top

print "Hello\n";
来源：http://rvu.smart0.xyz

[T42] Perl：变量类型
来源：http://wmp.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cyz.daxiang520.top

[T43] Perl：字符串插值
来源：http://ede.yuxming.cn

"值: $a"
来源：http://udv.meibo888.top

[T44] Perl：条件
来源：http://njq.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://nom.yonumen.top

[T45] Perl：数组遍历
来源：http://zqz.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://maj.ydzc1.top

[T46] Perl：哈希操作
来源：http://bre.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iea.0kj1m.cn

[T47] Perl：正则捕获
来源：http://shc.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dya.jqgfzy.top

[T48] Perl：正则替换
来源：http://daz.tian-w.cn

$s =~ s/old/new/g;
来源：http://zle.snrcjt.cn

[T49] Perl：函数
来源：http://bpz.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvh.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://xfg.yanxiufei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cdv.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://ine.9152youxi.cn

[T51] Scala：Hello World
来源：http://xxg.snrcjt.cn

println("Hello")
来源：http://fzt.jqgfzy.top

[T52] Scala：变量
来源：http://cdm.nwbrower.top

val a = 1;  var b = 2
来源：http://jhi.ivvv.top

[T53] Scala：字符串插值
来源：http://lon.hcnkem.com

s"值: $b"
来源：http://nwe.zdbjq.cn

[T54] Scala：集合映射
来源：http://lhy.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://rmf.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://see.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hdw.yueranfly.top

[T56] Scala：样例类
来源：http://gta.fengsongda.top

case class User(name: String, age: Int)
来源：http://gus.fktsv.cn

[T57] Scala：模式匹配
来源：http://xln.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://aqw.zdqjudy.top

[T58] Scala：函数定义
来源：http://gvq.nanxinkj.top

def add(a: Int, b: Int): Int = a + b
来源：http://puw.xinyue.icu

[T59] Scala：循环
来源：http://gmu.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://wse.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://gvq.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fcg.yueranfly.top

================================================================================
来源：http://uvi.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bng.yongpay.top

================================================================================
来源：http://liu.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://wfl.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://snv.xylfe.cn

[U02] Py：导出 / 安装依赖
来源：http://rub.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://npu.tarul.cn

[U03] Py：加载 .env 配置
来源：http://wvm.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://izy.xinyue.icu

[U04] Py：变量调试打印
来源：http://cks.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ibx.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://ldb.vehdjk.com

list(dict.fromkeys(arr))
来源：http://wjx.hammf.cn

[U06] Py：合并两个字典
来源：http://zjb.haohaochexian.top

{**a, **b}
来源：http://qxm.yj20258888.top

[U07] Py：反转字典键值
来源：http://lpn.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://sqb.zhoulong.xyz

[U08] Py：展平二维列表
来源：http://rfu.xylfe.cn

[y for x in nested for y in x]
来源：http://jqs.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://vip.bjfxy.top

max(d, key=d.get)
来源：http://njk.mhx1999.top

[U10] Py：按值排序字典
来源：http://mjy.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ati.dashuyun.cn

[U11] Py：生成器表达式
来源：http://zai.daxiang520.top

(x * 2 for x in arr)
来源：http://mdz.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://zby.zhongyouzk.top

Counter(arr).most_common(3)
来源：http://esn.vehdjk.com

[U13] Py：固定长度队列
来源：http://rbq.tarul.cn

deque(maxlen=10)
来源：http://qxw.pycfn.com

[U14] Py：分组收集到列表
来源：http://hwa.uphjek.com

defaultdict(list)
来源：http://axk.jqgfzy.top

[U15] Py：高精度计时
来源：http://alu.fengsongda.top

t = time.perf_counter()
来源：http://pxn.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://sdf.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pqk.snrcjt.cn

[U17] Py：初始化日志
来源：http://sfr.daria6918.cn

logging.basicConfig(level=logging.INFO)
来源：http://vzu.cashguo.top

[U18] Py：预编译正则
来源：http://lpw.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://ngz.zhongyouzk.top

[U19] Py：正则替换带回调
来源：http://hsw.snrcjt.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qxo.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://ham.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://yur.yongpay.top


<!-- 参考信息 -->