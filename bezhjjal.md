代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://okm.c1oappe.top

[S10] C：指针与解引用
来源：http://xaw.bjfxy.top

int *p = &a;  *p = 5;
来源：http://gai.snrcjt.cn

[S11] C：逐行读文件
来源：http://dua.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://nyt.zycfv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yib.fzhhl.top

fclose(f);
来源：http://tqm.ehwqpu.com

[S12] C：写文件
来源：http://wrk.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qgf.sufxvd.cn

[S13] C：宏定义
来源：http://dym.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aol.fanxiaobao.xyz

[S14] C：枚举
来源：http://gpk.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://grp.yanxiufei.cn

[S15] C：类型转换
来源：http://pia.xingfuxueyuan.xyz

(double) a / b
来源：http://lfc.wangdashe.top

[S16] C：位操作置位
来源：http://jui.xuanzx.com

x |= (1 << 3);
来源：http://fqo.316326.xyz

[S17] C：安全拼接字符串
来源：http://usx.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ayc.jianghu66.top

[S18] C：命令行参数
来源：http://qvc.hywenlv.cn

int main(int argc, char **argv)
来源：http://klz.gaohongyu789.top

[S19] C：快速排序
来源：http://diq.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://ftm.ydzc1.top

[S20] C：二分查找
来源：http://ccj.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wav.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://nof.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kwn.chenzaomai.com

[S22] C：字符串转数字
来源：http://qvb.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://azs.fengsongda.top

[S23] C：随机数
来源：http://syt.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dqk.yongpay.top

[S24] C：获取本地时间
来源：http://wkf.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uxt.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://gcg.epnwcf.com

memcpy(dst, src, n);
来源：http://ifo.fktsv.cn

[S26] C：内存清零
来源：http://sni.fktsv.cn

memset(a, 0, sizeof a);
来源：http://fkn.nanxinkj.top

[S27] C：定义常量
来源：http://tui.hongshengwenyu.top

const double PI = 3.14159;
来源：http://nwz.zhijiandao.cn

[S28] C：静态变量
来源：http://uif.hcnkem.com

static int counter = 0;
来源：http://awe.gotoacloud.top

[S29] C：变参函数
来源：http://lqy.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jyj.yj202588.top

[S30] C：头文件保护
来源：http://eyh.jqgufenzy.top

#ifndef X_H
来源：http://obo.shanyushiyangtech.top

#define X_H
来源：http://tno.jinqigfzy.top

#endif
来源：http://gmq.yj20258888.top

[S31] C++：Hello World
来源：http://fnz.zhongyouzk.top

#include <iostream>
来源：http://zmq.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://wzc.chenzaomai.com

[S32] C++：字符串
来源：http://jhf.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://hil.redwolf501.top

[S33] C++：vector 增删
来源：http://rbp.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://npc.yongpay.top

[S34] C++：遍历 vector
来源：http://bjg.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://qer.cashguo.top

[S35] C++：map
来源：http://hai.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://whj.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://qzl.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khk.xinyue.icu

[S37] C++：set
来源：http://cxo.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://glt.yangfankeji.com

[S38] C++：排序
来源：http://njd.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://vtq.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://ksz.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kyc.daria6918.cn

[S40] C++：查找元素
来源：http://wso.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dsv.sufxvd.cn

[S41] C++：类与构造函数
来源：http://tlr.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mih.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://eew.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://jhs.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://oxg.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://vll.cashguo.top

[S44] C++：引用传参
来源：http://oqv.yvedp.cn

void inc(int &x) { ++x; }
来源：http://yrq.aizwys.cn

[S45] C++：lambda
来源：http://baz.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://upy.yj202588.top

[S46] C++：函数模板
来源：http://nyk.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ntn.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://ibj.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://erl.cheryme.top

[S48] C++：逐行读文件
来源：http://vfh.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://qvb.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://yfu.nanxuanxn.top

[S49] C++：写文件
来源：http://miw.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xpe.daxiang520.top

[S50] C++：格式化数字
来源：http://qaw.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oqb.yvedp.cn

[S51] C++：显式类型转换
来源：http://rnn.nanxuanxn.top

static_cast<double>(a) / b
来源：http://pee.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://hij.sysykeji.top

int size() const noexcept { return n_; }
来源：http://sbr.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://vec.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://ool.fengsongda.top

[S54] C++：异常处理
来源：http://dtk.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://voc.chenlongwang.top

[S55] C++：结构化绑定
来源：http://dgv.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://tqn.nanxuanxn.top

[S56] C++：optional
来源：http://fme.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://amy.jiagoushi.top

[S57] C++：编译期常量
来源：http://iaa.xziqi.cn

constexpr int N = 10;
来源：http://fmu.fktsv.cn

[S58] C++：命名空间
来源：http://fsu.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://ixh.epnwcf.com

[S59] C++：静态断言
来源：http://vsr.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ecc.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://tet.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ijr.9152youxi.cn

================================================================================
来源：http://grt.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://igv.shzxlz.cn

================================================================================
来源：http://hzn.yuxming.cn

[T01] Kotlin：Hello World
来源：http://bye.kuanghao11.cn

println("Hello")
来源：http://mep.yongpay.top

[T02] Kotlin：变量
来源：http://fqh.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cei.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://xpx.guowangkeji.top

"值: $b"
来源：http://jqx.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://rhf.yj202588.top

val n: String? = null;  n?.length
来源：http://mzy.sweek.top

[T05] Kotlin：when 表达式
来源：http://cij.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jaz.tarul.cn

[T06] Kotlin：集合映射
来源：http://alx.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yck.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://gob.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jvw.hfpthk.cn

[T08] Kotlin：数据类
来源：http://cws.yj202588.top

data class User(val name: String, val age: Int)
来源：http://fwz.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://bjq.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://equ.cheryme.top

[T10] Kotlin：默认参数
来源：http://rtu.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lix.chenlongwang.top

[T11] Kotlin：协程
来源：http://olv.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hvf.yuxming.cn

[T12] Kotlin：解构声明
来源：http://ger.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://jcu.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://fnr.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://xtf.fengsongda.top

[T14] Kotlin：循环
来源：http://nid.52xcode.cn

for (i in 1..10) println(i)
来源：http://rte.xinyue.icu

[T15] Kotlin：接口
来源：http://oyu.hnqzz.top

interface Shape { fun area(): Double }
来源：http://nvs.cashguo.top

[T16] Swift：Hello World
来源：http://dtn.wangshuangyany.cn

print("Hello")
来源：http://sph.iojbl.cn

[T17] Swift：变量与常量
来源：http://wzo.yangfankeji.com

var a = 1;  let b = 2
来源：http://bjb.yuxming.cn

[T18] Swift：字符串插值
来源：http://yta.shangyingyoupin.top

"值: \(b)"
来源：http://vlo.tarul.cn

[T19] Swift：可选绑定
来源：http://ure.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://pby.yanxiufei.cn

[T20] Swift：数组操作
来源：http://ajy.nanxuanxn.top

var a = [1, 2, 3];  a.append(4)
来源：http://aiq.jlsjyb.cn

[T21] Swift：遍历
来源：http://nlv.gaohongyu789.top

for x in a { print(x) }
来源：http://asd.cdnleiting.top

[T22] Swift：字典
来源：http://rsy.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cbn.sweek.top

[T23] Swift：函数
来源：http://awm.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ezu.hcnkem.com

[T24] Swift：闭包
来源：http://sqq.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qts.wangdashe.top

[T25] Swift：结构体
来源：http://ieg.hnqzz.top

struct P { var x: Int }
来源：http://ecl.zdqjudy.top

[T26] Swift：类与重写
来源：http://elo.jyoumei.cn

class A: Base { override func f() {} }
来源：http://ubs.cdnleiting.top

[T27] Swift：错误处理
来源：http://dla.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://sgy.zhoulong.xyz

[T28] Swift：枚举
来源：http://lsh.epnwcf.com

enum Color { case red, green }
来源：http://yan.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://wtk.jinqigfzy.top

guard let x = opt else { return }
来源：http://gdc.9152youxi.cn

[T30] Swift：协议
来源：http://npv.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://lnc.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://ban.c1oappe.top

print("Hello")
来源：http://akc.pycfn.com

[T32] Lua：局部变量
来源：http://vtv.shzxlz.cn

local a = 1
来源：http://mtj.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://epb.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tdy.zhongyouzk.top

[T34] Lua：遍历表
来源：http://oeu.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vyx.sufxvd.cn

[T35] Lua：字典表
来源：http://tck.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://bng.xinyue.icu

[T36] Lua：函数
来源：http://slt.sysykeji.top

function add(a, b) return a + b end
来源：http://dex.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://dka.hongshengwenyu.top

"a" .. "b"
来源：http://ljk.zhoulong.xyz

[T38] Lua：条件
来源：http://eqb.yonumen.top

if x > 0 then print("正") end
来源：http://ckm.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://yvn.ydzc1.top

string.find(s, "%d+")
来源：http://ibv.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://emm.jqgfzy.top

setmetatable({}, { __index = base })
来源：http://sxk.havefunace.top

[T41] Perl：Hello World
来源：http://enu.fzhhl.top

print "Hello\n";
来源：http://dlk.epnwcf.com

[T42] Perl：变量类型
来源：http://esm.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pyu.quarkkingdee.top

[T43] Perl：字符串插值
来源：http://xcx.hysaishi.cn

"值: $a"
来源：http://gnw.hnqzz.top

[T44] Perl：条件
来源：http://buo.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://fip.dianchejie.cn

[T45] Perl：数组遍历
来源：http://hwj.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://jwo.hfpthk.cn

[T46] Perl：哈希操作
来源：http://cxf.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rkm.yuanzhike.top

[T47] Perl：正则捕获
来源：http://rlj.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://epp.nanxuanxn.top

[T48] Perl：正则替换
来源：http://gnv.bbcook.cn

$s =~ s/old/new/g;
来源：http://mjq.shanyushiyangtech.top

[T49] Perl：函数
来源：http://ajz.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qdi.jinqigufen.top

[T50] Perl：逐行读文件
来源：http://qft.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://pnl.ydzc1.top

while (my $line = <$fh>) { print $line; }
来源：http://jra.yj20258.top

[T51] Scala：Hello World
来源：http://mud.chenjidiqi.icu

println("Hello")
来源：http://jyw.havefunace.top

[T52] Scala：变量
来源：http://ofu.sufxvd.cn

val a = 1;  var b = 2
来源：http://kdz.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://ork.zhoulong.xyz

s"值: $b"
来源：http://gzn.chenlongwang.top

[T54] Scala：集合映射
来源：http://ivv.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://rfj.c1oappe.top

[T55] Scala：集合过滤
来源：http://hfd.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://nfd.birdmap.top

[T56] Scala：样例类
来源：http://mvy.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://dpx.tarul.cn

[T57] Scala：模式匹配
来源：http://tmn.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zsd.zhongyouzk.top

[T58] Scala：函数定义
来源：http://hhu.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wmr.ydjk.org.cn

[T59] Scala：循环
来源：http://ret.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://yyy.sjlbkw.cn

[T60] Scala：折叠
来源：http://xen.tarul.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rct.c1oappe.top

================================================================================
来源：http://gjr.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fur.fanxiaobao.xyz

================================================================================
来源：http://ufn.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://hay.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://smt.xuetiantiany.cn

[U02] Py：导出 / 安装依赖
来源：http://lxl.xylfe.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sai.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://mqx.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://thf.epnwcf.com

[U04] Py：变量调试打印
来源：http://amt.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gpu.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://ptb.haohaochexian.top

list(dict.fromkeys(arr))
来源：http://wcq.sxryk.cn

[U06] Py：合并两个字典
来源：http://tev.quarkkingdee.top

{**a, **b}
来源：http://qab.tanke756.top

[U07] Py：反转字典键值
来源：http://hnw.epnwcf.com

{v: k for k, v in d.items()}
来源：http://rkz.yonumen.top

[U08] Py：展平二维列表
来源：http://wro.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://quq.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://uhi.epnwcf.com

max(d, key=d.get)
来源：http://pna.yongpay.top

[U10] Py：按值排序字典
来源：http://oge.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nwf.cashguo.top

[U11] Py：生成器表达式
来源：http://ivt.snrcjt.cn

(x * 2 for x in arr)
来源：http://yjm.chenzaomai.com

[U12] Py：取出现最多的 3 个元素
来源：http://zfg.fktsv.cn

Counter(arr).most_common(3)
来源：http://umr.zhaomingkeji.xyz

[U13] Py：固定长度队列
来源：http://vmw.cheryme.top

deque(maxlen=10)
来源：http://eiz.hnqzz.top

[U14] Py：分组收集到列表
来源：http://buw.jinyuanbaomall.cn

defaultdict(list)
来源：http://vzy.yfazqb.com

[U15] Py：高精度计时
来源：http://qnh.vehdjk.com

t = time.perf_counter()
来源：http://fox.cucudq.cn

[U16] Py：命令行参数解析
来源：http://bfy.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ghe.shuidangran.top

[U17] Py：初始化日志
来源：http://bqw.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://nbk.sxryk.cn

[U18] Py：预编译正则
来源：http://ved.yvedp.cn

pat = re.compile(r"\d+")
来源：http://ren.yonumen.top

[U19] Py：正则替换带回调
来源：http://izf.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yhh.316326.xyz

[U20] Py：缓存函数结果
来源：http://tav.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://jpe.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://jqb.yj20258888.top

@contextlib.contextmanager
来源：http://ufc.xuanzx.com

[U22] Py：矩阵转置
来源：http://pap.shangyingyoupin.top

list(zip(*m))
来源：http://dle.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://caj.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wwb.shuidangran.top

[U24] Py：路径操作
来源：http://ele.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ypq.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://mdu.svipenyu.cn

csv.DictReader(f)
来源：http://lke.dashuyun.cn

[U26] Py：并发下载
来源：http://akk.sweek.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gyn.hammf.cn

[U27] Py：异步 HTTP
来源：http://asp.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://noh.zhongyouzk.top

[U28] Py：类型别名
来源：http://ubi.tian-w.cn

UserId = int
来源：http://qzk.guowangkeji.top

[U29] Py：属性校验
来源：http://ysa.jinqigufen.top

@property 与 @x.setter 配合
来源：http://nbp.c1oappe.top

[U30] Py：数据类
来源：http://jbk.jinqigufen.top

@dataclass(slots=True)
来源：http://qpy.guowangkeji.top

[U31] Py：单测
来源：http://qjx.jlsjyb.cn

python -m pytest -q
来源：http://vdv.xinyue.icu

[U32] Py：代码格式化
来源：http://aah.yj20258.top

ruff format . && ruff check --fix .
来源：http://puc.nanxinkj.top


<!-- 参考信息 -->