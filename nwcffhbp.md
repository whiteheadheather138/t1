代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://mhm.0kj1m.cn

[R76] 使用临时文件
来源：http://jvk.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kkf.yangfankeji.com

[R77] 读取用户输入
来源：http://wrc.zdqjudy.top

read -rp "请输入: " ans
来源：http://cay.gaohongyu789.top

[R78] 交互式菜单
来源：http://key.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cgy.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://xne.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zgc.pycfn.com

[R80] 查看脚本执行耗时
来源：http://fva.yj20258.top

time ./run.sh
来源：http://lni.xylfe.cn

================================================================================
来源：http://wil.vqdsnc.cn

S. C / C++ 专题
来源：http://pqb.hongshengwenyu.top

================================================================================
来源：http://zdm.haohaochexian.top

[S01] C：Hello World
来源：http://iha.zhengqikj.top

#include <stdio.h>
来源：http://szv.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ydy.yongpay.top

[S02] C：变量与格式化输出
来源：http://tsu.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://ooo.zdbjq.cn

[S03] C：读入整数
来源：http://hec.jianghu66.top

int x; scanf("%d", &x);
来源：http://voc.yuxming.cn

[S04] C：字符串复制
来源：http://qgw.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://cvt.yvedp.cn

[S05] C：字符串长度
来源：http://zqe.guannengcc.top

strlen(s)
来源：http://hbi.vqdsnc.cn

[S06] C：字符串比较
来源：http://mqd.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://rgz.dianchejie.cn

[S07] C：数组遍历求和
来源：http://vtg.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ble.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://nje.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iny.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://nxz.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rar.zhengqikj.top

[S10] C：指针与解引用
来源：http://gwc.pycfn.com

int *p = &a;  *p = 5;
来源：http://nau.zhixingplan.top

[S11] C：逐行读文件
来源：http://kfc.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://qlk.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://olq.shanyushiyangtech.top

fclose(f);
来源：http://wfj.jinyuanbaomall.cn

[S12] C：写文件
来源：http://bho.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ewi.xuanzx.com

[S13] C：宏定义
来源：http://cum.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://plq.cashguo.top

[S14] C：枚举
来源：http://qdw.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://kny.yj20258.top

[S15] C：类型转换
来源：http://uuz.jinghuilouyu.cn

(double) a / b
来源：http://elq.jqgfzy.top

[S16] C：位操作置位
来源：http://ymk.zhixingplan.top

x |= (1 << 3);
来源：http://ezq.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://ose.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pvh.sufxvd.cn

[S18] C：命令行参数
来源：http://gac.daria6918.cn

int main(int argc, char **argv)
来源：http://vbd.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://ufj.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qhg.hongshengwenyu.top

[S20] C：二分查找
来源：http://bii.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jtw.xylfe.cn

[S21] C：字符类别判断
来源：http://kgm.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://udv.uphjek.com

[S22] C：字符串转数字
来源：http://eny.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://fxa.sweek.top

[S23] C：随机数
来源：http://msl.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yrw.yongpay.top

[S24] C：获取本地时间
来源：http://qdr.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kwy.shuidangran.top

[S25] C：内存拷贝
来源：http://ecp.epnwcf.com

memcpy(dst, src, n);
来源：http://wkv.cdnleiting.top

[S26] C：内存清零
来源：http://ief.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://scm.nanxuanxn.top

[S27] C：定义常量
来源：http://wyc.snrcjt.cn

const double PI = 3.14159;
来源：http://ybo.snrcjt.cn

[S28] C：静态变量
来源：http://hmz.nanxuanxn.top

static int counter = 0;
来源：http://vzv.fktsv.cn

[S29] C：变参函数
来源：http://utq.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fnd.yueranfly.top

[S30] C：头文件保护
来源：http://ijt.sysykeji.top

#ifndef X_H
来源：http://yqh.andypj.xyz

#define X_H
来源：http://tap.yueranfly.top

#endif
来源：http://xed.hnxiangtu.top

[S31] C++：Hello World
来源：http://yxz.cashguo.top

#include <iostream>
来源：http://jui.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://fuh.bjfxy.top

[S32] C++：字符串
来源：http://miw.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://hle.shzxlz.cn

[S33] C++：vector 增删
来源：http://cts.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ujk.birdmap.top

[S34] C++：遍历 vector
来源：http://vep.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rlv.quarkkingdee.top

[S35] C++：map
来源：http://ahh.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tsa.gotoacloud.top

[S36] C++：unordered_map
来源：http://zrx.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ptd.jqgufenzy.top

[S37] C++：set
来源：http://ubu.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://igh.vehdjk.com

[S38] C++：排序
来源：http://agx.birdmap.top

std::sort(v.begin(), v.end());
来源：http://zzb.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://wgt.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oon.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://kbs.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xjk.sysykeji.top

[S41] C++：类与构造函数
来源：http://lkd.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kbc.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://cnn.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://qkn.xylfe.cn

[S43] C++：智能指针
来源：http://hjd.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://utr.wangdashe.top

[S44] C++：引用传参
来源：http://aoy.tanke756.top

void inc(int &x) { ++x; }
来源：http://tpj.c1oappe.top

[S45] C++：lambda
来源：http://rdt.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mqx.yongpay.top

[S46] C++：函数模板
来源：http://laz.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ugs.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://htl.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zpp.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://trm.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://gyy.sxryk.cn

while (std::getline(in, line)) { }
来源：http://idg.xinyue.icu

[S49] C++：写文件
来源：http://xtc.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gsw.nanxinkj.top

[S50] C++：格式化数字
来源：http://mpd.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cqb.svipenyu.cn

[S51] C++：显式类型转换
来源：http://wov.dianchejie.cn

static_cast<double>(a) / b
来源：http://cul.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://xbl.bbcook.cn

int size() const noexcept { return n_; }
来源：http://wya.zycfv.cn

[S53] C++：移动语义
来源：http://fka.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://gyf.jyoumei.cn

[S54] C++：异常处理
来源：http://zwc.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ilu.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://wbw.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vfj.nanxuanxn.top

[S56] C++：optional
来源：http://syz.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sxw.ivvv.top

[S57] C++：编译期常量
来源：http://phg.havefunace.top

constexpr int N = 10;
来源：http://aqc.hnxiangtu.top

[S58] C++：命名空间
来源：http://vvx.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://ebw.hammf.cn

[S59] C++：静态断言
来源：http://nkx.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kch.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://mxq.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xuj.wangshuangyany.cn

================================================================================
来源：http://qae.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krv.nanxinkj.top

================================================================================
来源：http://dts.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://tzr.sysykeji.top

println("Hello")
来源：http://rdz.zhoulong.xyz

[T02] Kotlin：变量
来源：http://sfg.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vxk.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://wpi.nwbrower.top

"值: $b"
来源：http://dcn.havefunace.top

[T04] Kotlin：空安全
来源：http://pii.gogol.net.cn

val n: String? = null;  n?.length
来源：http://zps.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://fdk.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ino.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://icd.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yuc.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://lkq.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://wge.fengsongda.top

[T08] Kotlin：数据类
来源：http://yhd.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://mqn.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://tnx.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://aqb.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://ndc.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yhr.birdmap.top

[T11] Kotlin：协程
来源：http://iyl.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vtw.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://heg.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://stq.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://geh.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://qui.zdqjudy.top

[T14] Kotlin：循环
来源：http://tkx.gotoacloud.top

for (i in 1..10) println(i)
来源：http://bll.haohaochexian.top

[T15] Kotlin：接口
来源：http://vkp.yj202588.top

interface Shape { fun area(): Double }
来源：http://yeu.ppjwa.cn

[T16] Swift：Hello World
来源：http://wve.zhijiandao.cn

print("Hello")
来源：http://kls.ppjwa.cn

[T17] Swift：变量与常量
来源：http://uua.tanke756.top

var a = 1;  let b = 2
来源：http://lxt.yuxming.cn

[T18] Swift：字符串插值
来源：http://vhh.yueranfly.top

"值: \(b)"
来源：http://exu.ppjwa.cn

[T19] Swift：可选绑定
来源：http://zjd.fengsongda.top

if let n = opt { print(n) }
来源：http://bdb.jinqigfzy.top

[T20] Swift：数组操作
来源：http://fwp.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nme.0kj1m.cn

[T21] Swift：遍历
来源：http://xuz.zhijiandao.cn

for x in a { print(x) }
来源：http://vtg.pycfn.com

[T22] Swift：字典
来源：http://fxv.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://dsw.nwbrower.top

[T23] Swift：函数
来源：http://cou.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dpl.hnqzz.top

[T24] Swift：闭包
来源：http://yhb.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://clr.tarul.cn

[T25] Swift：结构体
来源：http://rjb.daxiang520.top

struct P { var x: Int }
来源：http://hsf.yuanzhike.top

[T26] Swift：类与重写
来源：http://zuo.aibaodan.cn

class A: Base { override func f() {} }
来源：http://vtw.pycfn.com

[T27] Swift：错误处理
来源：http://bpp.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://wrx.zhixingplan.top

[T28] Swift：枚举
来源：http://kta.yj20258888.top

enum Color { case red, green }
来源：http://det.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://won.ivvv.top

guard let x = opt else { return }
来源：http://jjr.dashuyun.cn

[T30] Swift：协议
来源：http://bxs.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://uyt.nwbrower.top

[T31] Lua：Hello World
来源：http://htj.jqgufenzy.top

print("Hello")
来源：http://fim.zhoulong.xyz

[T32] Lua：局部变量
来源：http://vov.yangfankeji.com

local a = 1
来源：http://lyn.cucudq.cn

[T33] Lua：表（数组）
来源：http://adh.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eqk.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://mfx.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hyc.zhiwuduotai.top

[T35] Lua：字典表
来源：http://ntv.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://siy.yonumen.top

[T36] Lua：函数
来源：http://wlh.haohaochexian.top

function add(a, b) return a + b end
来源：http://ogv.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://ouy.meibo888.top

"a" .. "b"
来源：http://ncb.shangyingyoupin.top

[T38] Lua：条件
来源：http://hcb.havefunace.top

if x > 0 then print("正") end
来源：http://iiq.sysykeji.top

[T39] Lua：模式匹配
来源：http://iet.iojbl.cn

string.find(s, "%d+")
来源：http://bcn.jqgufenzy.top

[T40] Lua：元表
来源：http://hfg.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://ddu.hnxiangtu.top

[T41] Perl：Hello World
来源：http://ejh.chenjidiqi.icu

print "Hello\n";
来源：http://tzj.cdnleiting.top

[T42] Perl：变量类型
来源：http://fkn.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pnf.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://jtv.quarkkingdee.top

"值: $a"
来源：http://mtd.svipenyu.cn

[T44] Perl：条件
来源：http://rti.haohaochexian.top

if ($a > 0) { print "正"; }
来源：http://vir.316326.xyz

[T45] Perl：数组遍历
来源：http://acv.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://ovq.redwolf501.top

[T46] Perl：哈希操作
来源：http://kan.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cbs.gotoacloud.top

[T47] Perl：正则捕获
来源：http://dfe.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oot.sjlbkw.cn

[T48] Perl：正则替换
来源：http://caq.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://bih.epnwcf.com

[T49] Perl：函数
来源：http://tqr.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ujf.gzhubu.top

[T50] Perl：逐行读文件
来源：http://xee.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://elk.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://dwr.jianghu66.top

[T51] Scala：Hello World
来源：http://vxq.snrcjt.cn

println("Hello")
来源：http://ihm.9152youxi.cn

[T52] Scala：变量
来源：http://saz.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://yhd.chenzaomai.com

[T53] Scala：字符串插值
来源：http://hsa.bbcook.cn

s"值: $b"
来源：http://kek.uphjek.com

[T54] Scala：集合映射
来源：http://emb.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://qkk.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://jmx.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gev.ctjpmb.com

[T56] Scala：样例类
来源：http://juj.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://vns.bjfxy.top

[T57] Scala：模式匹配
来源：http://wvn.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://red.0kj1m.cn

[T58] Scala：函数定义
来源：http://lvh.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://naq.c1oappe.top

[T59] Scala：循环
来源：http://clx.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://xmt.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://tli.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bhg.hnxiangtu.top

================================================================================
来源：http://len.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vcz.yvedp.cn

================================================================================
来源：http://vsb.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://rdh.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://wju.zhiwuduotai.top

[U02] Py：导出 / 安装依赖
来源：http://wrc.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sot.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://kny.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wtb.xuanzx.com

[U04] Py：变量调试打印
来源：http://ack.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ztq.hnqzz.top

[U05] Py：列表去重且保序
来源：http://znn.birdmap.top

list(dict.fromkeys(arr))
来源：http://cmb.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://ckv.jinqigfzy.top

{**a, **b}
来源：http://sku.cdnleiting.top

[U07] Py：反转字典键值
来源：http://cdt.sweek.top

{v: k for k, v in d.items()}
来源：http://xqv.dianchejie.cn

[U08] Py：展平二维列表
来源：http://ygb.tarul.cn

[y for x in nested for y in x]
来源：http://wpr.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://yly.xuetiantiany.cn

max(d, key=d.get)
来源：http://pzq.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://gsm.svipenyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wqw.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://qnx.chenlongwang.top

(x * 2 for x in arr)
来源：http://pmn.ydjk.org.cn

[U12] Py：取出现最多的 3 个元素
来源：http://plb.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://fga.smart0.xyz

[U13] Py：固定长度队列
来源：http://yqh.chenzaomai.com

deque(maxlen=10)
来源：http://eyo.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://zsi.shangyingyoupin.top

defaultdict(list)
来源：http://qqt.shuidangran.top

[U15] Py：高精度计时
来源：http://byb.nwbrower.top

t = time.perf_counter()
来源：http://wxv.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://usr.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lwd.chenlongwang.top


<!-- 参考信息 -->