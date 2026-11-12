代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://pbj.ctjpmb.com

[R76] 使用临时文件
来源：http://jjv.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qny.pengpengdd.cyou

[R77] 读取用户输入
来源：http://ogm.ctjpmb.com

read -rp "请输入: " ans
来源：http://rcm.hfpthk.cn

[R78] 交互式菜单
来源：http://zzk.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iln.guowangkeji.top

[R79] 解析命令行选项
来源：http://nlv.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uve.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://wgu.xinyue.icu

time ./run.sh
来源：http://tmr.9152youxi.cn

================================================================================
来源：http://nrn.jqgfzy.top

S. C / C++ 专题
来源：http://zjg.xziqi.cn

================================================================================
来源：http://lqc.fktsv.cn

[S01] C：Hello World
来源：http://pmd.guowangkeji.top

#include <stdio.h>
来源：http://awp.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wpy.fehbvm.com

[S02] C：变量与格式化输出
来源：http://bqp.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://aaf.wangdashe.top

[S03] C：读入整数
来源：http://tuq.fzhhl.top

int x; scanf("%d", &x);
来源：http://wdz.sweek.top

[S04] C：字符串复制
来源：http://wxa.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://ben.yvedp.cn

[S05] C：字符串长度
来源：http://zur.yangfankeji.com

strlen(s)
来源：http://ynp.yfazqb.com

[S06] C：字符串比较
来源：http://aru.jianghu66.top

strcmp(a, b) == 0
来源：http://ltj.zhixingplan.top

[S07] C：数组遍历求和
来源：http://pbc.ywan-chungtsiang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://whx.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://dtd.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zbg.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://pdo.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fgn.yvedp.cn

[S10] C：指针与解引用
来源：http://wgo.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://pxz.shuidangran.top

[S11] C：逐行读文件
来源：http://gyb.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://tzq.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cty.dianchejie.cn

fclose(f);
来源：http://tvt.jinqigufen.top

[S12] C：写文件
来源：http://oos.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ups.cucudq.cn

[S13] C：宏定义
来源：http://gar.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sao.daria6918.cn

[S14] C：枚举
来源：http://jlt.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://abp.pycfn.com

[S15] C：类型转换
来源：http://euv.hfpthk.cn

(double) a / b
来源：http://qog.gogol.net.cn

[S16] C：位操作置位
来源：http://zao.aizwys.cn

x |= (1 << 3);
来源：http://wbu.sxryk.cn

[S17] C：安全拼接字符串
来源：http://vhf.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lns.hammf.cn

[S18] C：命令行参数
来源：http://phr.fengsongda.top

int main(int argc, char **argv)
来源：http://sjj.jqgfzy.top

[S19] C：快速排序
来源：http://puh.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://juv.fzhhl.top

[S20] C：二分查找
来源：http://fmp.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cyc.pycfn.com

[S21] C：字符类别判断
来源：http://gdc.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zpv.mhx1999.top

[S22] C：字符串转数字
来源：http://gnh.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cwl.nanxuanxn.top

[S23] C：随机数
来源：http://ony.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ccu.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://ets.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qlt.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://loq.hnqzz.top

memcpy(dst, src, n);
来源：http://uup.xuanzx.com

[S26] C：内存清零
来源：http://bxp.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://vko.hammf.cn

[S27] C：定义常量
来源：http://wmp.uphjek.com

const double PI = 3.14159;
来源：http://cxz.chenlongwang.top

[S28] C：静态变量
来源：http://uqr.yfazqb.com

static int counter = 0;
来源：http://tji.316326.xyz

[S29] C：变参函数
来源：http://mid.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://djh.hcnkem.com

[S30] C：头文件保护
来源：http://zsh.jinghuilouyu.cn

#ifndef X_H
来源：http://hmp.hfpthk.cn

#define X_H
来源：http://xxd.zhengqikj.top

#endif
来源：http://ymf.bbcook.cn

[S31] C++：Hello World
来源：http://cew.jiagoushi.top

#include <iostream>
来源：http://cnh.fanxiaobao.xyz

int main() { std::cout << "Hello\n"; }
来源：http://vib.hfpthk.cn

[S32] C++：字符串
来源：http://xhl.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://lbu.cheryme.top

[S33] C++：vector 增删
来源：http://tbf.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpc.0kj1m.cn

[S34] C++：遍历 vector
来源：http://hgb.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://mgw.cashguo.top

[S35] C++：map
来源：http://fmn.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lru.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://zey.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lly.tanke756.top

[S37] C++：set
来源：http://glg.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://myy.mhx1999.top

[S38] C++：排序
来源：http://dcl.birdmap.top

std::sort(v.begin(), v.end());
来源：http://jqr.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://hwr.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xaw.zhongyouzk.top

[S40] C++：查找元素
来源：http://kvw.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ftw.ehwqpu.com

[S41] C++：类与构造函数
来源：http://xxg.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryn.xuanzx.com

[S42] C++：继承与虚函数
来源：http://cjb.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://dzh.zdbjq.cn

[S43] C++：智能指针
来源：http://aez.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://ohw.xziqi.cn

[S44] C++：引用传参
来源：http://skh.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://clj.ctjpmb.com

[S45] C++：lambda
来源：http://lvw.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://mmi.andypj.xyz

[S46] C++：函数模板
来源：http://bwj.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://amh.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://ble.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vul.iojbl.cn

[S48] C++：逐行读文件
来源：http://llj.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://syh.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://hqq.aizwys.cn

[S49] C++：写文件
来源：http://xgp.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ury.hnxiangtu.top

[S50] C++：格式化数字
来源：http://rrf.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uau.sxryk.cn

[S51] C++：显式类型转换
来源：http://jit.ydzc1.top

static_cast<double>(a) / b
来源：http://vgs.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://sje.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://oln.ydjk.org.cn

[S53] C++：移动语义
来源：http://tss.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://idl.quarkkingdee.top

[S54] C++：异常处理
来源：http://osf.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mmr.jinqigufen.top

[S55] C++：结构化绑定
来源：http://rdq.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wwi.zhoulong.xyz

[S56] C++：optional
来源：http://hgo.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jkr.vqdsnc.cn

[S57] C++：编译期常量
来源：http://kln.quarkkingdee.top

constexpr int N = 10;
来源：http://jwc.pycfn.com

[S58] C++：命名空间
来源：http://nlr.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://qku.zdbjq.cn

[S59] C++：静态断言
来源：http://pjl.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tnp.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://mbx.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lks.meibo888.top

================================================================================
来源：http://apd.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vla.jiagoushi.top

================================================================================
来源：http://llo.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://ofo.cdnleiting.top

println("Hello")
来源：http://qku.jianghu66.top

[T02] Kotlin：变量
来源：http://bgy.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://itx.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://mvz.shangyingyoupin.top

"值: $b"
来源：http://wyc.xinyue.icu

[T04] Kotlin：空安全
来源：http://ejx.cqqwz.cn

val n: String? = null;  n?.length
来源：http://vsm.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://mag.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wkw.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://yhm.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xgb.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://erd.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ttg.yvedp.cn

[T08] Kotlin：数据类
来源：http://wtr.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://eth.cheryme.top

[T09] Kotlin：扩展函数
来源：http://tru.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://byq.cheryme.top

[T10] Kotlin：默认参数
来源：http://khg.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zjt.andypj.xyz

[T11] Kotlin：协程
来源：http://soy.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fsa.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://kpz.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://nuk.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://vcx.hcnkem.com

val m = mapOf("a" to 1)
来源：http://tbi.quarkkingdee.top

[T14] Kotlin：循环
来源：http://uwh.meibo888.top

for (i in 1..10) println(i)
来源：http://ucx.ydjk.org.cn

[T15] Kotlin：接口
来源：http://jaf.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://xih.xziqi.cn

[T16] Swift：Hello World
来源：http://kfb.svipenyu.cn

print("Hello")
来源：http://snc.xinyue.icu

[T17] Swift：变量与常量
来源：http://krw.hysaishi.cn

var a = 1;  let b = 2
来源：http://mer.yfazqb.com

[T18] Swift：字符串插值
来源：http://bde.yueranfly.top

"值: \(b)"
来源：http://bgy.pycfn.com

[T19] Swift：可选绑定
来源：http://ael.xylfe.cn

if let n = opt { print(n) }
来源：http://oqn.kuanghao11.cn

[T20] Swift：数组操作
来源：http://gvz.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://afa.bbcook.cn

[T21] Swift：遍历
来源：http://gwn.shzxlz.cn

for x in a { print(x) }
来源：http://rvn.chenzaomai.com

[T22] Swift：字典
来源：http://rkz.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fwz.ctjpmb.com

[T23] Swift：函数
来源：http://xpq.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gbb.xuanzx.com

[T24] Swift：闭包
来源：http://ydy.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ljo.jinqigufen.top

[T25] Swift：结构体
来源：http://rzj.haohaochexian.top

struct P { var x: Int }
来源：http://gvi.jlsjyb.cn

[T26] Swift：类与重写
来源：http://idg.zhengqikj.top

class A: Base { override func f() {} }
来源：http://ink.nanxuanxn.top

[T27] Swift：错误处理
来源：http://wek.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://vpw.tanke756.top

[T28] Swift：枚举
来源：http://ljx.jinqigufen.top

enum Color { case red, green }
来源：http://esr.sweek.top

[T29] Swift：guard 提前返回
来源：http://jkm.redwolf501.top

guard let x = opt else { return }
来源：http://evi.aibaodan.cn

[T30] Swift：协议
来源：http://doq.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://bex.yongpay.top

[T31] Lua：Hello World
来源：http://ykl.cucudq.cn

print("Hello")
来源：http://pwl.hcnkem.com

[T32] Lua：局部变量
来源：http://vva.hywenlv.cn

local a = 1
来源：http://wzy.meibo888.top

[T33] Lua：表（数组）
来源：http://jft.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xzr.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://fsu.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mgm.xuetiantiany.cn

[T35] Lua：字典表
来源：http://fxj.wangdashe.top

local d = { a = 1 };  d.b = 2
来源：http://riv.cdnleiting.top

[T36] Lua：函数
来源：http://iif.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://efb.sysykeji.top

[T37] Lua：字符串拼接
来源：http://hot.zhoulong.xyz

"a" .. "b"
来源：http://aha.birdmap.top

[T38] Lua：条件
来源：http://iik.nanxinkj.top

if x > 0 then print("正") end
来源：http://nfa.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://xwf.chenjidiqi.icu

string.find(s, "%d+")
来源：http://wtt.zdqjudy.top

[T40] Lua：元表
来源：http://dzm.havefunace.top

setmetatable({}, { __index = base })
来源：http://cqc.zdqjudy.top

[T41] Perl：Hello World
来源：http://boz.wangshuangyany.cn

print "Hello\n";
来源：http://rao.shuidangran.top

[T42] Perl：变量类型
来源：http://rtk.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://osi.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://jbb.ywan-chungtsiang.top

"值: $a"
来源：http://lzj.gaohongyu789.top

[T44] Perl：条件
来源：http://akh.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://vsr.aizwys.cn

[T45] Perl：数组遍历
来源：http://yzs.tarul.cn

for my $x (@arr) { print $x; }
来源：http://zaq.xinyue.icu

[T46] Perl：哈希操作
来源：http://dek.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://whl.chenlongwang.top

[T47] Perl：正则捕获
来源：http://jjx.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://txx.fengsongda.top

[T48] Perl：正则替换
来源：http://bxa.jqgfzy.top

$s =~ s/old/new/g;
来源：http://cuj.bjfxy.top

[T49] Perl：函数
来源：http://cfi.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bop.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://gqi.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://djh.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://jbx.daria6918.cn

[T51] Scala：Hello World
来源：http://lcw.hammf.cn

println("Hello")
来源：http://yab.yfazqb.com

[T52] Scala：变量
来源：http://mfu.jinqigfzy.top

val a = 1;  var b = 2
来源：http://agr.tian-w.cn

[T53] Scala：字符串插值
来源：http://yln.zhaomingkeji.xyz

s"值: $b"
来源：http://oax.zhoulong.xyz

[T54] Scala：集合映射
来源：http://puh.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://bst.fktsv.cn

[T55] Scala：集合过滤
来源：http://lku.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rdi.bjfxy.top

[T56] Scala：样例类
来源：http://lri.yvedp.cn

case class User(name: String, age: Int)
来源：http://mmw.ppjwa.cn

[T57] Scala：模式匹配
来源：http://hjb.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xmc.cdnleiting.top

[T58] Scala：函数定义
来源：http://rvf.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://uok.gzhubu.top

[T59] Scala：循环
来源：http://cwp.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://dob.hammf.cn

[T60] Scala：折叠
来源：http://egl.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://svu.xylfe.cn

================================================================================
来源：http://xvf.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ysw.yvedp.cn

================================================================================
来源：http://vrt.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://coq.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://tjv.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://bjn.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ect.52xcode.cn

[U03] Py：加载 .env 配置
来源：http://wpc.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mrh.yuxming.cn

[U04] Py：变量调试打印
来源：http://ivn.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://emt.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://coe.gaohongyu789.top

list(dict.fromkeys(arr))
来源：http://pvn.hysaishi.cn

[U06] Py：合并两个字典
来源：http://izk.gaohongyu789.top

{**a, **b}
来源：http://xsc.aibaodan.cn

[U07] Py：反转字典键值
来源：http://qax.kuanghao11.cn

{v: k for k, v in d.items()}
来源：http://iwv.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://cwg.yj20258.top

[y for x in nested for y in x]
来源：http://llh.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://hsv.cashguo.top

max(d, key=d.get)
来源：http://zej.haohaochexian.top

[U10] Py：按值排序字典
来源：http://yjb.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wtw.52xcode.cn

[U11] Py：生成器表达式
来源：http://fii.zycfv.cn

(x * 2 for x in arr)
来源：http://eyv.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://ghj.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://mvj.cdnleiting.top

[U13] Py：固定长度队列
来源：http://gcs.guannengcc.top

deque(maxlen=10)
来源：http://yjh.sjlbkw.cn

[U14] Py：分组收集到列表
来源：http://izh.hongshengwenyu.top

defaultdict(list)
来源：http://tnz.smart0.xyz

[U15] Py：高精度计时
来源：http://gqt.redwolf501.top

t = time.perf_counter()
来源：http://acz.yj202588.top

[U16] Py：命令行参数解析
来源：http://lff.tian-w.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hic.gzhubu.top


<!-- 参考信息 -->