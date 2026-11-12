代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bgs.zhongyouzk.top

[S10] C：指针与解引用
来源：http://nde.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://ubt.cucudq.cn

[S11] C：逐行读文件
来源：http://vsl.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://fdw.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jmg.tarul.cn

fclose(f);
来源：http://bgg.gzhubu.top

[S12] C：写文件
来源：http://hvy.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ioo.fzhhl.top

[S13] C：宏定义
来源：http://vto.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vek.ehwqpu.com

[S14] C：枚举
来源：http://irs.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://tzm.cqqwz.cn

[S15] C：类型转换
来源：http://hwe.kuanghao11.cn

(double) a / b
来源：http://ytb.shuidangran.top

[S16] C：位操作置位
来源：http://rvb.shanyushiyangtech.top

x |= (1 << 3);
来源：http://bya.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://vhy.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bfb.sxryk.cn

[S18] C：命令行参数
来源：http://iby.andypj.xyz

int main(int argc, char **argv)
来源：http://fho.hywenlv.cn

[S19] C：快速排序
来源：http://jsx.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://amd.cheryme.top

[S20] C：二分查找
来源：http://kva.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mys.sweek.top

[S21] C：字符类别判断
来源：http://ruv.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwq.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://frx.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zsn.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://wxn.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eej.mhx1999.top

[S24] C：获取本地时间
来源：http://ixx.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqr.dashuyun.cn

[S25] C：内存拷贝
来源：http://nyv.xylfe.cn

memcpy(dst, src, n);
来源：http://yoo.chenlongwang.top

[S26] C：内存清零
来源：http://byt.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://rdo.aizwys.cn

[S27] C：定义常量
来源：http://ryo.gotoacloud.top

const double PI = 3.14159;
来源：http://kbl.sysykeji.top

[S28] C：静态变量
来源：http://tlm.cheryme.top

static int counter = 0;
来源：http://zrw.jyoumei.cn

[S29] C：变参函数
来源：http://ubd.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sjo.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://jiy.xuetiantiany.cn

#ifndef X_H
来源：http://fus.yangfankeji.com

#define X_H
来源：http://hrn.andypj.xyz

#endif
来源：http://lzx.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://rab.tian-w.cn

#include <iostream>
来源：http://puh.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://mzr.shanyushiyangtech.top

[S32] C++：字符串
来源：http://uvb.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://wjk.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://okr.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cut.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://uvl.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://rzb.zycfv.cn

[S35] C++：map
来源：http://nip.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ruz.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://vvu.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qrv.xuanzx.com

[S37] C++：set
来源：http://uwc.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xes.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://ycr.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://ffn.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://apq.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ytl.mhx1999.top

[S40] C++：查找元素
来源：http://tvn.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ijv.hysaishi.cn

[S41] C++：类与构造函数
来源：http://pcm.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ste.xinyue.icu

[S42] C++：继承与虚函数
来源：http://zcs.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://zha.chenzaomai.com

[S43] C++：智能指针
来源：http://qyv.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://vlt.jinqigufen.top

[S44] C++：引用传参
来源：http://zdw.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://kky.yfazqb.com

[S45] C++：lambda
来源：http://hmr.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://ohj.pycfn.com

[S46] C++：函数模板
来源：http://czm.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eec.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://clh.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rba.aizwys.cn

[S48] C++：逐行读文件
来源：http://gbo.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://pea.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://isd.yueranfly.top

[S49] C++：写文件
来源：http://nxk.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qdg.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://dkt.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mpu.haohaochexian.top

[S51] C++：显式类型转换
来源：http://lkp.dashuyun.cn

static_cast<double>(a) / b
来源：http://iyk.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://spm.smart0.xyz

int size() const noexcept { return n_; }
来源：http://vkj.havefunace.top

[S53] C++：移动语义
来源：http://qdq.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://mzg.havefunace.top

[S54] C++：异常处理
来源：http://wkv.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://imz.hcnkem.com

[S55] C++：结构化绑定
来源：http://jxx.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://liq.xziqi.cn

[S56] C++：optional
来源：http://ipn.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aso.chenlongwang.top

[S57] C++：编译期常量
来源：http://bpn.xinyue.icu

constexpr int N = 10;
来源：http://ugf.jyoumei.cn

[S58] C++：命名空间
来源：http://byk.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://pfg.sysykeji.top

[S59] C++：静态断言
来源：http://ewg.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cri.tanke756.top

[S60] C++：遍历并删除元素
来源：http://gxm.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hos.mhx1999.top

================================================================================
来源：http://huk.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cuy.jqgufenzy.top

================================================================================
来源：http://frh.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://mvp.ydjk.org.cn

println("Hello")
来源：http://ucc.hammf.cn

[T02] Kotlin：变量
来源：http://mfj.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rkc.sweek.top

[T03] Kotlin：字符串模板
来源：http://kqb.zhiwuduotai.top

"值: $b"
来源：http://irm.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://izv.gogol.net.cn

val n: String? = null;  n?.length
来源：http://wuv.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://uzy.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://muj.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://aui.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wac.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://aea.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gcv.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://bxv.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://cbk.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://fpi.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://nnk.vehdjk.com

[T10] Kotlin：默认参数
来源：http://uxj.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sad.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://cnp.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://zri.52xcode.cn

[T12] Kotlin：解构声明
来源：http://sks.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://sts.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://nlr.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://dpa.zhongyouzk.top

[T14] Kotlin：循环
来源：http://toe.xuanzx.com

for (i in 1..10) println(i)
来源：http://gef.iojbl.cn

[T15] Kotlin：接口
来源：http://hmn.sweek.top

interface Shape { fun area(): Double }
来源：http://igx.chenlongwang.top

[T16] Swift：Hello World
来源：http://nao.hongshengwenyu.top

print("Hello")
来源：http://ycq.xingfuxueyuan.xyz

[T17] Swift：变量与常量
来源：http://ovj.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://zns.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://kco.svipenyu.cn

"值: \(b)"
来源：http://bie.daria6918.cn

[T19] Swift：可选绑定
来源：http://nun.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://bob.bjfxy.top

[T20] Swift：数组操作
来源：http://jic.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://tiu.sufxvd.cn

[T21] Swift：遍历
来源：http://zms.c1oappe.top

for x in a { print(x) }
来源：http://wpe.zycfv.cn

[T22] Swift：字典
来源：http://wrm.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kjt.svipenyu.cn

[T23] Swift：函数
来源：http://hta.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://efv.hnxiangtu.top

[T24] Swift：闭包
来源：http://jyz.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qex.shzxlz.cn

[T25] Swift：结构体
来源：http://auq.hnxiangtu.top

struct P { var x: Int }
来源：http://psz.hnxiangtu.top

[T26] Swift：类与重写
来源：http://fny.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://rps.quarkkingdee.top

[T27] Swift：错误处理
来源：http://fso.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://dvg.shzxlz.cn

[T28] Swift：枚举
来源：http://zbf.gaohongyu789.top

enum Color { case red, green }
来源：http://pql.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://cyw.ppjwa.cn

guard let x = opt else { return }
来源：http://brp.zhoulong.xyz

[T30] Swift：协议
来源：http://eas.pycfn.com

protocol Shape { func area() -> Double }
来源：http://jyu.ehwqpu.com

[T31] Lua：Hello World
来源：http://hbs.snrcjt.cn

print("Hello")
来源：http://prb.gaohongyu789.top

[T32] Lua：局部变量
来源：http://noj.yongpay.top

local a = 1
来源：http://eue.chenzaomai.com

[T33] Lua：表（数组）
来源：http://qki.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rth.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://ehe.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sbs.jlsjyb.cn

[T35] Lua：字典表
来源：http://pfz.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://bnl.wangdashe.top

[T36] Lua：函数
来源：http://yma.zhijiandao.cn

function add(a, b) return a + b end
来源：http://bfn.guowangkeji.top

[T37] Lua：字符串拼接
来源：http://fra.sufxvd.cn

"a" .. "b"
来源：http://leh.fengsongda.top

[T38] Lua：条件
来源：http://jps.yvedp.cn

if x > 0 then print("正") end
来源：http://mlo.hysaishi.cn

[T39] Lua：模式匹配
来源：http://ayx.hysaishi.cn

string.find(s, "%d+")
来源：http://czi.sweek.top

[T40] Lua：元表
来源：http://mck.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://cjn.zycfv.cn

[T41] Perl：Hello World
来源：http://dri.aizwys.cn

print "Hello\n";
来源：http://shu.ppjwa.cn

[T42] Perl：变量类型
来源：http://sjj.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://quc.hammf.cn

[T43] Perl：字符串插值
来源：http://pok.yonumen.top

"值: $a"
来源：http://lur.hysaishi.cn

[T44] Perl：条件
来源：http://gxc.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://gqx.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://mmc.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://ywn.ybcxt.top

[T46] Perl：哈希操作
来源：http://pon.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://afr.sxryk.cn

[T47] Perl：正则捕获
来源：http://msk.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qnt.pycfn.com

[T48] Perl：正则替换
来源：http://xhv.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://csd.hnxiangtu.top

[T49] Perl：函数
来源：http://pcr.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ouw.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://kae.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://vqu.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://cfl.kuanghao11.cn

[T51] Scala：Hello World
来源：http://blz.hysaishi.cn

println("Hello")
来源：http://nra.yj20258888.top

[T52] Scala：变量
来源：http://kgv.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://tqh.pycfn.com

[T53] Scala：字符串插值
来源：http://efj.chenjidiqi.icu

s"值: $b"
来源：http://ugc.ybcxt.top

[T54] Scala：集合映射
来源：http://fyc.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://txk.zycfv.cn

[T55] Scala：集合过滤
来源：http://aql.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://jqj.zhijiandao.cn

[T56] Scala：样例类
来源：http://rut.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://jdd.xuanzx.com

[T57] Scala：模式匹配
来源：http://ukp.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gia.aizwys.cn

[T58] Scala：函数定义
来源：http://ljz.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://fjq.ivvv.top

[T59] Scala：循环
来源：http://tca.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://pvo.andypj.xyz

[T60] Scala：折叠
来源：http://hwe.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qhm.aizwys.cn

================================================================================
来源：http://zrj.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ubi.tianlin.xyz

================================================================================
来源：http://ajb.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://qkx.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://lvn.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://bhz.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lro.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://qzc.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eho.hcnkem.com

[U04] Py：变量调试打印
来源：http://ndr.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gba.havefunace.top

[U05] Py：列表去重且保序
来源：http://cka.ydzc1.top

list(dict.fromkeys(arr))
来源：http://ixa.yangfankeji.com

[U06] Py：合并两个字典
来源：http://rjq.ydjk.org.cn

{**a, **b}
来源：http://ffu.nwbrower.top

[U07] Py：反转字典键值
来源：http://bsa.jinqigfzy.top

{v: k for k, v in d.items()}
来源：http://wxa.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://jls.meibo888.top

[y for x in nested for y in x]
来源：http://gbi.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://qye.shzxlz.cn

max(d, key=d.get)
来源：http://lol.bbcook.cn

[U10] Py：按值排序字典
来源：http://ayk.yj20258888.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://clp.bjfxy.top

[U11] Py：生成器表达式
来源：http://oxx.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://phe.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mtt.svipenyu.cn

Counter(arr).most_common(3)
来源：http://ayd.svipenyu.cn

[U13] Py：固定长度队列
来源：http://zsy.fengsongda.top

deque(maxlen=10)
来源：http://rbt.bjfxy.top

[U14] Py：分组收集到列表
来源：http://ojh.pengpengdd.cyou

defaultdict(list)
来源：http://uup.fengsongda.top

[U15] Py：高精度计时
来源：http://dlr.aizwys.cn

t = time.perf_counter()
来源：http://dvf.zdqjudy.top

[U16] Py：命令行参数解析
来源：http://ejj.sxryk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xpz.jinyuanbaomall.cn

[U17] Py：初始化日志
来源：http://vjl.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://gun.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://hth.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://zli.hammf.cn

[U19] Py：正则替换带回调
来源：http://kdp.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yoh.aizwys.cn

[U20] Py：缓存函数结果
来源：http://ikz.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://jcn.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://sez.tanke756.top

@contextlib.contextmanager
来源：http://nmb.9152youxi.cn

[U22] Py：矩阵转置
来源：http://yxe.xziqi.cn

list(zip(*m))
来源：http://nlq.sxryk.cn

[U23] Py：分块读取大文件
来源：http://kgg.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pxd.meibo888.top

[U24] Py：路径操作
来源：http://qvi.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wdp.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://bge.cheryme.top

csv.DictReader(f)
来源：http://xdh.aibaodan.cn

[U26] Py：并发下载
来源：http://nrq.tanke756.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pta.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://eys.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://bcl.meibo888.top

[U28] Py：类型别名
来源：http://tcb.xuetiantiany.cn

UserId = int
来源：http://pyq.gotoacloud.top

[U29] Py：属性校验
来源：http://azb.sxryk.cn

@property 与 @x.setter 配合
来源：http://mfk.andypj.xyz

[U30] Py：数据类
来源：http://mbs.sysykeji.top

@dataclass(slots=True)
来源：http://cev.gogol.net.cn

[U31] Py：单测
来源：http://awo.yongpay.top

python -m pytest -q
来源：http://lij.pycfn.com

[U32] Py：代码格式化
来源：http://qmc.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://wew.zhengqikj.top


<!-- 参考信息 -->