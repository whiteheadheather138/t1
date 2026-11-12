代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://fji.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://gqs.yongpay.top

fclose(f);
来源：http://wvq.52xcode.cn

[S12] C：写文件
来源：http://rbw.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mvu.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://eun.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fns.jinyuanbaomall.cn

[S14] C：枚举
来源：http://vof.hammf.cn

enum Color { RED, GREEN, BLUE };
来源：http://zyc.daria6918.cn

[S15] C：类型转换
来源：http://ckj.dashuyun.cn

(double) a / b
来源：http://vta.smart0.xyz

[S16] C：位操作置位
来源：http://kod.kuanghao11.cn

x |= (1 << 3);
来源：http://zdi.aizwys.cn

[S17] C：安全拼接字符串
来源：http://jwv.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jox.316326.xyz

[S18] C：命令行参数
来源：http://qkt.jqgfzy.top

int main(int argc, char **argv)
来源：http://bxv.ehwqpu.com

[S19] C：快速排序
来源：http://khm.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vbp.smart0.xyz

[S20] C：二分查找
来源：http://dsz.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mwv.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://fdv.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://emu.nwbrower.top

[S22] C：字符串转数字
来源：http://soy.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://kgo.ywan-chungtsiang.top

[S23] C：随机数
来源：http://dwv.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xmk.yongpay.top

[S24] C：获取本地时间
来源：http://kjs.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vjp.tarul.cn

[S25] C：内存拷贝
来源：http://ohk.yfazqb.com

memcpy(dst, src, n);
来源：http://afq.jinghuilouyu.cn

[S26] C：内存清零
来源：http://nyh.yonumen.top

memset(a, 0, sizeof a);
来源：http://qez.daria6918.cn

[S27] C：定义常量
来源：http://yon.jiagoushi.top

const double PI = 3.14159;
来源：http://ekj.iojbl.cn

[S28] C：静态变量
来源：http://spg.hywenlv.cn

static int counter = 0;
来源：http://btt.yangfankeji.com

[S29] C：变参函数
来源：http://krt.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qdx.zdqjudy.top

[S30] C：头文件保护
来源：http://pln.sjlbkw.cn

#ifndef X_H
来源：http://jwv.andypj.xyz

#define X_H
来源：http://ayl.zhongyouzk.top

#endif
来源：http://hul.shangyingyoupin.top

[S31] C++：Hello World
来源：http://ilt.shzxlz.cn

#include <iostream>
来源：http://urc.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://dah.gotoacloud.top

[S32] C++：字符串
来源：http://oei.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://fvj.tarul.cn

[S33] C++：vector 增删
来源：http://phg.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fli.hysaishi.cn

[S34] C++：遍历 vector
来源：http://pss.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://lhf.zhixingplan.top

[S35] C++：map
来源：http://wph.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmp.cdnleiting.top

[S36] C++：unordered_map
来源：http://ceq.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aim.ivvv.top

[S37] C++：set
来源：http://znq.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aml.yj20258.top

[S38] C++：排序
来源：http://nlv.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://hgc.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://hyd.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://goz.ppjwa.cn

[S40] C++：查找元素
来源：http://myl.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xqk.hfpthk.cn

[S41] C++：类与构造函数
来源：http://tme.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ewy.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://csw.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://cra.haohaochexian.top

[S43] C++：智能指针
来源：http://ure.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://aid.sufxvd.cn

[S44] C++：引用传参
来源：http://hql.jianghu66.top

void inc(int &x) { ++x; }
来源：http://mzh.zhixingplan.top

[S45] C++：lambda
来源：http://fgc.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fmi.jinqigfzy.top

[S46] C++：函数模板
来源：http://ubb.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ccg.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://lgi.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tdv.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://hxf.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ddw.epnwcf.com

while (std::getline(in, line)) { }
来源：http://jva.aizwys.cn

[S49] C++：写文件
来源：http://xrv.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://opp.hammf.cn

[S50] C++：格式化数字
来源：http://fzz.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uix.fengsongda.top

[S51] C++：显式类型转换
来源：http://bqh.hywenlv.cn

static_cast<double>(a) / b
来源：http://gva.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://tnz.ybcxt.top

int size() const noexcept { return n_; }
来源：http://ean.zhongyouzk.top

[S53] C++：移动语义
来源：http://ans.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://hgy.pengpengdd.cyou

[S54] C++：异常处理
来源：http://lap.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ncu.shuidangran.top

[S55] C++：结构化绑定
来源：http://fno.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://sjt.shanyushiyangkeji.top

[S56] C++：optional
来源：http://kal.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uxi.xziqi.cn

[S57] C++：编译期常量
来源：http://qbz.chenjidiqi.icu

constexpr int N = 10;
来源：http://qkv.pycfn.com

[S58] C++：命名空间
来源：http://haz.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://ytf.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://pjg.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hul.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://hsn.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isj.mhx1999.top

================================================================================
来源：http://hdc.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nbd.zdqjudy.top

================================================================================
来源：http://dri.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://gte.cdnleiting.top

println("Hello")
来源：http://ovs.ppjwa.cn

[T02] Kotlin：变量
来源：http://wps.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://npk.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://gaq.jyoumei.cn

"值: $b"
来源：http://ekb.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://hjw.dashuyun.cn

val n: String? = null;  n?.length
来源：http://pss.cashguo.top

[T05] Kotlin：when 表达式
来源：http://qfm.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oug.316326.xyz

[T06] Kotlin：集合映射
来源：http://ojq.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ivw.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://gmr.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://koz.daria6918.cn

[T08] Kotlin：数据类
来源：http://hjl.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://voq.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://pdz.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://crl.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://nit.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rbr.fzhhl.top

[T11] Kotlin：协程
来源：http://dlq.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://aty.bjfxy.top

[T12] Kotlin：解构声明
来源：http://eqo.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://ana.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://xye.nwbrower.top

val m = mapOf("a" to 1)
来源：http://lbq.cucudq.cn

[T14] Kotlin：循环
来源：http://nha.316326.xyz

for (i in 1..10) println(i)
来源：http://dyu.hnqzz.top

[T15] Kotlin：接口
来源：http://pmm.smart0.xyz

interface Shape { fun area(): Double }
来源：http://mie.ydjk.org.cn

[T16] Swift：Hello World
来源：http://sjd.fehbvm.com

print("Hello")
来源：http://uez.ivvv.top

[T17] Swift：变量与常量
来源：http://tqv.zhijiandao.cn

var a = 1;  let b = 2
来源：http://yre.yj20258888.top

[T18] Swift：字符串插值
来源：http://anr.jiagoushi.top

"值: \(b)"
来源：http://plr.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://uwf.hammf.cn

if let n = opt { print(n) }
来源：http://fdl.havefunace.top

[T20] Swift：数组操作
来源：http://reh.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fyx.zdbjq.cn

[T21] Swift：遍历
来源：http://pyl.tanke756.top

for x in a { print(x) }
来源：http://brj.iojbl.cn

[T22] Swift：字典
来源：http://flz.hfpthk.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mte.hcnkem.com

[T23] Swift：函数
来源：http://oej.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wao.chenzaomai.com

[T24] Swift：闭包
来源：http://xtn.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rfs.xuanzx.com

[T25] Swift：结构体
来源：http://mfb.hesvh.cn

struct P { var x: Int }
来源：http://hqg.jlsjyb.cn

[T26] Swift：类与重写
来源：http://ipj.yangfankeji.com

class A: Base { override func f() {} }
来源：http://fkp.sweek.top

[T27] Swift：错误处理
来源：http://voi.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://hwx.gzhubu.top

[T28] Swift：枚举
来源：http://pvl.hnqzz.top

enum Color { case red, green }
来源：http://nzw.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://mha.smart0.xyz

guard let x = opt else { return }
来源：http://ebz.aibaodan.cn

[T30] Swift：协议
来源：http://cpk.yongpay.top

protocol Shape { func area() -> Double }
来源：http://vvm.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://cbo.yuanzhike.top

print("Hello")
来源：http://hfc.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://xze.sjlbkw.cn

local a = 1
来源：http://ntx.yuxming.cn

[T33] Lua：表（数组）
来源：http://jib.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://btc.ydzc1.top

[T34] Lua：遍历表
来源：http://bkv.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://jnl.fengsongda.top

[T35] Lua：字典表
来源：http://tqs.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://wep.zdbjq.cn

[T36] Lua：函数
来源：http://god.zhoulong.xyz

function add(a, b) return a + b end
来源：http://meg.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://jmw.guowangkeji.top

"a" .. "b"
来源：http://fyc.zhengqikj.top

[T38] Lua：条件
来源：http://xde.wangdashe.top

if x > 0 then print("正") end
来源：http://gny.daxiang520.top

[T39] Lua：模式匹配
来源：http://jog.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://exv.jianghu66.top

[T40] Lua：元表
来源：http://mmc.aizwys.cn

setmetatable({}, { __index = base })
来源：http://cag.cashguo.top

[T41] Perl：Hello World
来源：http://tzp.hammf.cn

print "Hello\n";
来源：http://xvc.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://asb.svipenyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bzk.ctjpmb.com

[T43] Perl：字符串插值
来源：http://ruv.fktsv.cn

"值: $a"
来源：http://ofu.52xcode.cn

[T44] Perl：条件
来源：http://wui.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://unk.ppjwa.cn

[T45] Perl：数组遍历
来源：http://blv.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://tgu.gzhubu.top

[T46] Perl：哈希操作
来源：http://rzr.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ffz.fzhhl.top

[T47] Perl：正则捕获
来源：http://cqn.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cel.yuxming.cn

[T48] Perl：正则替换
来源：http://msl.fzhhl.top

$s =~ s/old/new/g;
来源：http://hct.yj20258888.top

[T49] Perl：函数
来源：http://nbg.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxv.sxryk.cn

[T50] Perl：逐行读文件
来源：http://skh.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wfk.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://omc.jqgufenzy.top

[T51] Scala：Hello World
来源：http://ziy.sjlbkw.cn

println("Hello")
来源：http://bgy.nanxinkj.top

[T52] Scala：变量
来源：http://iow.havefunace.top

val a = 1;  var b = 2
来源：http://gio.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://uou.hnxiangtu.top

s"值: $b"
来源：http://dpz.nwbrower.top

[T54] Scala：集合映射
来源：http://ydx.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://cga.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://ape.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://ucm.snrcjt.cn

[T56] Scala：样例类
来源：http://tzq.yonumen.top

case class User(name: String, age: Int)
来源：http://dur.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://byb.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jzz.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://lxt.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://pix.chenjidiqi.icu

[T59] Scala：循环
来源：http://uuv.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://wcg.uphjek.com

[T60] Scala：折叠
来源：http://cwi.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gml.zhijiandao.cn

================================================================================
来源：http://lir.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zbg.feifeiyinyue.top

================================================================================
来源：http://got.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://cyg.hysaishi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kbo.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://ais.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fjr.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://tsl.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xzq.daria6918.cn

[U04] Py：变量调试打印
来源：http://vjf.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ykh.yanxiufei.cn

[U05] Py：列表去重且保序
来源：http://ezc.sweek.top

list(dict.fromkeys(arr))
来源：http://apu.bbcook.cn

[U06] Py：合并两个字典
来源：http://frt.xuanzx.com

{**a, **b}
来源：http://omb.0kj1m.cn

[U07] Py：反转字典键值
来源：http://usz.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://kpq.zhixingplan.top

[U08] Py：展平二维列表
来源：http://lav.epnwcf.com

[y for x in nested for y in x]
来源：http://kqe.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://ipo.cheryme.top

max(d, key=d.get)
来源：http://rmh.sysykeji.top

[U10] Py：按值排序字典
来源：http://pmt.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wyn.ppjwa.cn

[U11] Py：生成器表达式
来源：http://qrt.shuidangran.top

(x * 2 for x in arr)
来源：http://yeh.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://wfw.yuanzhike.top

Counter(arr).most_common(3)
来源：http://xga.jqgfzy.top

[U13] Py：固定长度队列
来源：http://msz.0kj1m.cn

deque(maxlen=10)
来源：http://uxu.yueranfly.top

[U14] Py：分组收集到列表
来源：http://yba.nwbrower.top

defaultdict(list)
来源：http://omg.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://lxt.cdnleiting.top

t = time.perf_counter()
来源：http://zed.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://mdg.hywenlv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cbr.yanxiufei.cn

[U17] Py：初始化日志
来源：http://okb.yuanzhike.top

logging.basicConfig(level=logging.INFO)
来源：http://unl.chenlongwang.top

[U18] Py：预编译正则
来源：http://qxg.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://ywk.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://buu.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ops.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://cwy.shanyushiyangtech.top

@functools.lru_cache(maxsize=None)
来源：http://crj.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://qfw.9152youxi.cn

@contextlib.contextmanager
来源：http://syi.zhengqikj.top

[U22] Py：矩阵转置
来源：http://xeg.ppjwa.cn

list(zip(*m))
来源：http://eop.andypj.xyz

[U23] Py：分块读取大文件
来源：http://htx.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://djb.chenlongwang.top

[U24] Py：路径操作
来源：http://zok.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sek.fktsv.cn

[U25] Py：CSV 按字典读
来源：http://for.pengpengdd.cyou

csv.DictReader(f)
来源：http://llf.vehdjk.com

[U26] Py：并发下载
来源：http://hwr.shuidangran.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gwh.xylfe.cn

[U27] Py：异步 HTTP
来源：http://acl.uphjek.com

aiohttp.ClientSession() 配合 async with
来源：http://ivk.yonumen.top

[U28] Py：类型别名
来源：http://upy.zhengqikj.top

UserId = int
来源：http://oyl.shanyushiyangkeji.top

[U29] Py：属性校验
来源：http://nzd.haohaochexian.top

@property 与 @x.setter 配合
来源：http://fxk.nwbrower.top

[U30] Py：数据类
来源：http://cgh.meibo888.top

@dataclass(slots=True)
来源：http://qbf.jinyuanbaomall.cn

[U31] Py：单测
来源：http://ugd.zhiwuduotai.top

python -m pytest -q
来源：http://rpk.zhixingplan.top

[U32] Py：代码格式化
来源：http://khb.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://vbm.52xcode.cn

[U33] Py：打包发布
来源：http://pod.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://jbp.hysaishi.cn

[U34] Py：判断编码
来源：http://tiy.shangyingyoupin.top

chardet.detect(raw)
来源：http://lft.tianlin.xyz


<!-- 参考信息 -->