代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://uha.shuidangran.top

[S02] C：变量与格式化输出
来源：http://bci.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://vep.hnqzz.top

[S03] C：读入整数
来源：http://tsh.zhixingplan.top

int x; scanf("%d", &x);
来源：http://skh.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://vur.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://pza.sxryk.cn

[S05] C：字符串长度
来源：http://iak.gotoacloud.top

strlen(s)
来源：http://haz.vehdjk.com

[S06] C：字符串比较
来源：http://len.redwolf501.top

strcmp(a, b) == 0
来源：http://agr.zdbjq.cn

[S07] C：数组遍历求和
来源：http://hqs.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://knr.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://gdg.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rex.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://zyj.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qtj.sxryk.cn

[S10] C：指针与解引用
来源：http://jza.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://oeg.cashguo.top

[S11] C：逐行读文件
来源：http://lgb.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://lbh.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nbt.hywenlv.cn

fclose(f);
来源：http://hxh.jinghuilouyu.cn

[S12] C：写文件
来源：http://qoe.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lxk.ybcxt.top

[S13] C：宏定义
来源：http://sxb.bjfxy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ifl.iojbl.cn

[S14] C：枚举
来源：http://cya.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://ywi.sjlbkw.cn

[S15] C：类型转换
来源：http://cmq.jinqigfzy.top

(double) a / b
来源：http://cun.zhoulong.xyz

[S16] C：位操作置位
来源：http://msr.fanxiaobao.xyz

x |= (1 << 3);
来源：http://tjj.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://spx.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grv.redwolf501.top

[S18] C：命令行参数
来源：http://kkg.cucudq.cn

int main(int argc, char **argv)
来源：http://ylo.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://dai.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uqr.mhx1999.top

[S20] C：二分查找
来源：http://iyq.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qvn.hfpthk.cn

[S21] C：字符类别判断
来源：http://aqp.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vtl.haohaochexian.top

[S22] C：字符串转数字
来源：http://wji.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://pnk.smart0.xyz

[S23] C：随机数
来源：http://thq.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jdx.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://qfh.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aeq.mhx1999.top

[S25] C：内存拷贝
来源：http://eam.daxiang520.top

memcpy(dst, src, n);
来源：http://jmz.cucudq.cn

[S26] C：内存清零
来源：http://bjp.yonumen.top

memset(a, 0, sizeof a);
来源：http://dvq.0kj1m.cn

[S27] C：定义常量
来源：http://buw.havefunace.top

const double PI = 3.14159;
来源：http://dos.yonumen.top

[S28] C：静态变量
来源：http://rnl.wangshuangyany.cn

static int counter = 0;
来源：http://djt.redwolf501.top

[S29] C：变参函数
来源：http://src.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gqc.xinyue.icu

[S30] C：头文件保护
来源：http://mai.yueranfly.top

#ifndef X_H
来源：http://amw.nanxinkj.top

#define X_H
来源：http://zya.feifeiyinyue.top

#endif
来源：http://qof.tarul.cn

[S31] C++：Hello World
来源：http://yus.epnwcf.com

#include <iostream>
来源：http://cfb.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://lis.shuidangran.top

[S32] C++：字符串
来源：http://dox.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://sll.zhongyouzk.top

[S33] C++：vector 增删
来源：http://ljf.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ioc.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://vzz.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://vba.zhaomingkeji.xyz

[S35] C++：map
来源：http://fmi.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hlo.aibaodan.cn

[S36] C++：unordered_map
来源：http://wrx.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgw.cucudq.cn

[S37] C++：set
来源：http://nmj.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eod.meibo888.top

[S38] C++：排序
来源：http://ikn.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://gbs.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://hje.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qek.cucudq.cn

[S40] C++：查找元素
来源：http://usi.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://anr.yangfankeji.com

[S41] C++：类与构造函数
来源：http://ufq.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zxu.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://rjk.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://ikx.xuetiantiany.cn

[S43] C++：智能指针
来源：http://ilu.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://nvp.bjfxy.top

[S44] C++：引用传参
来源：http://lbf.guannengcc.top

void inc(int &x) { ++x; }
来源：http://sgl.nanxuanxn.top

[S45] C++：lambda
来源：http://ggr.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://qjm.xuetiantiany.cn

[S46] C++：函数模板
来源：http://ehi.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zat.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://qpi.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mrs.gotoacloud.top

[S48] C++：逐行读文件
来源：http://vek.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://xyu.wangdashe.top

while (std::getline(in, line)) { }
来源：http://dqv.sjlbkw.cn

[S49] C++：写文件
来源：http://gcg.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xzy.wangdashe.top

[S50] C++：格式化数字
来源：http://yqx.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ipa.mhx1999.top

[S51] C++：显式类型转换
来源：http://xjq.xinyue.icu

static_cast<double>(a) / b
来源：http://mfr.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://dth.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://oka.vqdsnc.cn

[S53] C++：移动语义
来源：http://jot.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://lfi.kuanghao11.cn

[S54] C++：异常处理
来源：http://qsj.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcs.tarul.cn

[S55] C++：结构化绑定
来源：http://zqa.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fst.epnwcf.com

[S56] C++：optional
来源：http://skq.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wmr.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://nnw.vehdjk.com

constexpr int N = 10;
来源：http://reu.sufxvd.cn

[S58] C++：命名空间
来源：http://epb.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://hrx.c1oappe.top

[S59] C++：静态断言
来源：http://fbe.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nrg.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://gnj.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://opj.redwolf501.top

================================================================================
来源：http://uzf.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ngs.snrcjt.cn

================================================================================
来源：http://xqc.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://vpj.jinqigufen.top

println("Hello")
来源：http://bfo.cucudq.cn

[T02] Kotlin：变量
来源：http://mmi.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rey.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://lzt.cashguo.top

"值: $b"
来源：http://lqz.pycfn.com

[T04] Kotlin：空安全
来源：http://tig.birdmap.top

val n: String? = null;  n?.length
来源：http://sxo.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://jde.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ofy.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://zcv.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ufe.pycfn.com

[T07] Kotlin：集合过滤
来源：http://ibh.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jlu.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://qzt.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://tde.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://hrh.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://oof.52xcode.cn

[T10] Kotlin：默认参数
来源：http://pcd.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uxo.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://obr.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kec.epnwcf.com

[T12] Kotlin：解构声明
来源：http://zsk.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://gmw.yj20258.top

[T13] Kotlin：只读 Map
来源：http://fyy.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://bqm.zdbjq.cn

[T14] Kotlin：循环
来源：http://xar.tianlin.xyz

for (i in 1..10) println(i)
来源：http://sej.cqqwz.cn

[T15] Kotlin：接口
来源：http://fnt.sysykeji.top

interface Shape { fun area(): Double }
来源：http://lfi.shzxlz.cn

[T16] Swift：Hello World
来源：http://lky.jlsjyb.cn

print("Hello")
来源：http://tjc.zhengqikj.top

[T17] Swift：变量与常量
来源：http://zif.kuanghao11.cn

var a = 1;  let b = 2
来源：http://yse.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://sqh.tarul.cn

"值: \(b)"
来源：http://dpf.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://frf.yuanzhike.top

if let n = opt { print(n) }
来源：http://eui.sjlbkw.cn

[T20] Swift：数组操作
来源：http://pua.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://cqz.wangdashe.top

[T21] Swift：遍历
来源：http://xhb.xuanzx.com

for x in a { print(x) }
来源：http://ajl.xylfe.cn

[T22] Swift：字典
来源：http://zxw.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://cbo.nanxinkj.top

[T23] Swift：函数
来源：http://dgr.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://usj.zhiwuduotai.top

[T24] Swift：闭包
来源：http://tui.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uxr.bbcook.cn

[T25] Swift：结构体
来源：http://upf.aizwys.cn

struct P { var x: Int }
来源：http://sxs.kuanghao11.cn

[T26] Swift：类与重写
来源：http://cme.ehwqpu.com

class A: Base { override func f() {} }
来源：http://zzi.tianlin.xyz

[T27] Swift：错误处理
来源：http://wyo.yj20258.top

do { try f() } catch { print(error) }
来源：http://inh.ctjpmb.com

[T28] Swift：枚举
来源：http://rro.52xcode.cn

enum Color { case red, green }
来源：http://dsb.yj202588.top

[T29] Swift：guard 提前返回
来源：http://kvf.shuidangran.top

guard let x = opt else { return }
来源：http://vfc.yj20258888.top

[T30] Swift：协议
来源：http://jsn.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://fev.havefunace.top

[T31] Lua：Hello World
来源：http://hru.daxiang520.top

print("Hello")
来源：http://nny.shuidangran.top

[T32] Lua：局部变量
来源：http://bem.yanxiufei.cn

local a = 1
来源：http://iol.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://rqh.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ibw.chenzaomai.com

[T34] Lua：遍历表
来源：http://bbq.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vwj.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://ghn.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://rgf.tian-w.cn

[T36] Lua：函数
来源：http://jem.mhx1999.top

function add(a, b) return a + b end
来源：http://cpm.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://dln.jinqigfzy.top

"a" .. "b"
来源：http://tkt.xylfe.cn

[T38] Lua：条件
来源：http://ayj.aizwys.cn

if x > 0 then print("正") end
来源：http://hvn.nwbrower.top

[T39] Lua：模式匹配
来源：http://aue.yj20258.top

string.find(s, "%d+")
来源：http://fnb.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://lak.zycfv.cn

setmetatable({}, { __index = base })
来源：http://klt.yj202588.top

[T41] Perl：Hello World
来源：http://okf.fzhhl.top

print "Hello\n";
来源：http://yym.zdbjq.cn

[T42] Perl：变量类型
来源：http://kbu.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nbd.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://swq.gotoacloud.top

"值: $a"
来源：http://kbm.zdbjq.cn

[T44] Perl：条件
来源：http://jxt.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://wgh.xziqi.cn

[T45] Perl：数组遍历
来源：http://yzu.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://wgg.yuxming.cn

[T46] Perl：哈希操作
来源：http://bbn.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ymj.chenlongwang.top

[T47] Perl：正则捕获
来源：http://hrs.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tsc.mhx1999.top

[T48] Perl：正则替换
来源：http://gcv.zycfv.cn

$s =~ s/old/new/g;
来源：http://joh.ydzc1.top

[T49] Perl：函数
来源：http://qvx.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yhf.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://poc.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://rwf.yangfankeji.com

while (my $line = <$fh>) { print $line; }
来源：http://ocm.316326.xyz

[T51] Scala：Hello World
来源：http://cim.aibaodan.cn

println("Hello")
来源：http://doa.snrcjt.cn

[T52] Scala：变量
来源：http://bmi.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://zoq.c1oappe.top

[T53] Scala：字符串插值
来源：http://ugq.9152youxi.cn

s"值: $b"
来源：http://tzd.zhongyouzk.top

[T54] Scala：集合映射
来源：http://fpk.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://aqz.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://tvl.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://wjb.hammf.cn

[T56] Scala：样例类
来源：http://dqb.ydzc1.top

case class User(name: String, age: Int)
来源：http://oyt.meibo888.top

[T57] Scala：模式匹配
来源：http://xws.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jyx.sweek.top

[T58] Scala：函数定义
来源：http://dbr.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gol.uphjek.com

[T59] Scala：循环
来源：http://tst.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://kue.tanke756.top

[T60] Scala：折叠
来源：http://xhz.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gfg.yangfankeji.com

================================================================================
来源：http://cuv.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qjh.yj20258888.top

================================================================================
来源：http://zqc.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://aoz.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://zkx.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://ell.tianlin.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iei.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://eik.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ujg.daria6918.cn

[U04] Py：变量调试打印
来源：http://eel.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pte.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://gfx.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://ijz.fanxiaobao.xyz

[U06] Py：合并两个字典
来源：http://hub.smart0.xyz

{**a, **b}
来源：http://owj.jinqigufen.top

[U07] Py：反转字典键值
来源：http://qml.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://znr.tanke756.top

[U08] Py：展平二维列表
来源：http://ncg.shzxlz.cn

[y for x in nested for y in x]
来源：http://rhu.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://enh.guowangkeji.top

max(d, key=d.get)
来源：http://kjm.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://vnr.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kct.jqgfzy.top

[U11] Py：生成器表达式
来源：http://azk.uphjek.com

(x * 2 for x in arr)
来源：http://evd.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yqr.yj20258.top

Counter(arr).most_common(3)
来源：http://tpj.hysaishi.cn

[U13] Py：固定长度队列
来源：http://eko.guowangkeji.top

deque(maxlen=10)
来源：http://qbi.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://dle.jqgfzy.top

defaultdict(list)
来源：http://uyl.yueranfly.top

[U15] Py：高精度计时
来源：http://pid.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://oxp.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://zpr.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sgm.xuanzx.com

[U17] Py：初始化日志
来源：http://aqt.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://wdx.dashuyun.cn

[U18] Py：预编译正则
来源：http://mrl.aibaodan.cn

pat = re.compile(r"\d+")
来源：http://lwd.yj202588.top

[U19] Py：正则替换带回调
来源：http://vqt.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nxe.fengsongda.top

[U20] Py：缓存函数结果
来源：http://bba.zdbjq.cn

@functools.lru_cache(maxsize=None)
来源：http://gut.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://cxv.gogol.net.cn

@contextlib.contextmanager
来源：http://gtp.jqgfzy.top

[U22] Py：矩阵转置
来源：http://ite.ydjk.org.cn

list(zip(*m))
来源：http://hhs.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://jsf.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lsf.epnwcf.com

[U24] Py：路径操作
来源：http://rvr.shzxlz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zgi.tanke756.top


<!-- 参考信息 -->