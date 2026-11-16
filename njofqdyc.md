代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://jok.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://cqa.jqgfzy.top

fclose(f);
来源：http://yhz.zhengqikj.top

[S12] C：写文件
来源：http://qwp.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://smr.aibaodan.cn

[S13] C：宏定义
来源：http://khw.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pvo.chenlongwang.top

[S14] C：枚举
来源：http://gqz.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://eui.smart0.xyz

[S15] C：类型转换
来源：http://auu.bbcook.cn

(double) a / b
来源：http://gaj.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://tkd.daria6918.cn

x |= (1 << 3);
来源：http://xqx.nwbrower.top

[S17] C：安全拼接字符串
来源：http://qry.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uwe.shuidangran.top

[S18] C：命令行参数
来源：http://ixx.yvedp.cn

int main(int argc, char **argv)
来源：http://sgi.xuetiantiany.cn

[S19] C：快速排序
来源：http://cym.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://ffi.tarul.cn

[S20] C：二分查找
来源：http://zbw.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hth.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://ucv.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ogy.redwolf501.top

[S22] C：字符串转数字
来源：http://hvc.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://hmg.pengpengdd.cyou

[S23] C：随机数
来源：http://ajo.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yne.smart0.xyz

[S24] C：获取本地时间
来源：http://wyg.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ftn.zhongyouzk.top

[S25] C：内存拷贝
来源：http://tke.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://twc.shanyushiyangtech.top

[S26] C：内存清零
来源：http://phk.yuxming.cn

memset(a, 0, sizeof a);
来源：http://dry.fanxiaobao.xyz

[S27] C：定义常量
来源：http://vdf.hcnkem.com

const double PI = 3.14159;
来源：http://ghj.aizwys.cn

[S28] C：静态变量
来源：http://ila.fktsv.cn

static int counter = 0;
来源：http://qry.andypj.xyz

[S29] C：变参函数
来源：http://jmt.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ola.yangfankeji.com

[S30] C：头文件保护
来源：http://dvs.zdqjudy.top

#ifndef X_H
来源：http://eri.tian-w.cn

#define X_H
来源：http://beq.fengsongda.top

#endif
来源：http://npn.uphjek.com

[S31] C++：Hello World
来源：http://wyg.9152youxi.cn

#include <iostream>
来源：http://vpy.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://hip.shanyushiyangtech.top

[S32] C++：字符串
来源：http://sen.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://asf.zhoulong.xyz

[S33] C++：vector 增删
来源：http://fhb.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cyh.yueranfly.top

[S34] C++：遍历 vector
来源：http://zvq.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://hkk.jianghu66.top

[S35] C++：map
来源：http://vig.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hur.ydzc1.top

[S36] C++：unordered_map
来源：http://sjy.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwr.hysaishi.cn

[S37] C++：set
来源：http://cqx.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://djd.wangshuangyany.cn

[S38] C++：排序
来源：http://qnz.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://lnu.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://wrn.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://egv.yanxiufei.cn

[S40] C++：查找元素
来源：http://ecd.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ssa.hcnkem.com

[S41] C++：类与构造函数
来源：http://apx.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wmk.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://bbz.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://ljt.sjlbkw.cn

[S43] C++：智能指针
来源：http://qyd.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://use.jiagoushi.top

[S44] C++：引用传参
来源：http://ito.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://xbn.ehwqpu.com

[S45] C++：lambda
来源：http://ria.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eyb.jiagoushi.top

[S46] C++：函数模板
来源：http://vsb.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ccy.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://qsp.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://itc.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://aqc.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://uhs.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://flv.yangfankeji.com

[S49] C++：写文件
来源：http://omv.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qel.quarkkingdee.top

[S50] C++：格式化数字
来源：http://dbn.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rmg.xinyue.icu

[S51] C++：显式类型转换
来源：http://hex.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://hik.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://qdp.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://ezn.fengsongda.top

[S53] C++：移动语义
来源：http://dot.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://qco.yanxiufei.cn

[S54] C++：异常处理
来源：http://jvo.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bdj.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://ujx.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mer.fengsongda.top

[S56] C++：optional
来源：http://bgn.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://euv.nanxuanxn.top

[S57] C++：编译期常量
来源：http://jni.jinqigfzy.top

constexpr int N = 10;
来源：http://swn.nanxuanxn.top

[S58] C++：命名空间
来源：http://ihb.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://eki.gzhubu.top

[S59] C++：静态断言
来源：http://fzo.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eyo.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://blz.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdp.mhx1999.top

================================================================================
来源：http://rpr.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lep.pengpengdd.cyou

================================================================================
来源：http://bzk.316326.xyz

[T01] Kotlin：Hello World
来源：http://uwj.zhengqikj.top

println("Hello")
来源：http://jhd.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://lqx.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ncc.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://evn.guannengcc.top

"值: $b"
来源：http://rdv.hywenlv.cn

[T04] Kotlin：空安全
来源：http://kaj.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://zzn.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://rxu.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lxx.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://ywk.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hna.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://zpi.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://npv.svipenyu.cn

[T08] Kotlin：数据类
来源：http://mei.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://tlo.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://jyl.pycfn.com

fun String.exclaim() = this + "!"
来源：http://jju.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://dxx.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zgz.fehbvm.com

[T11] Kotlin：协程
来源：http://srz.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qoc.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://upk.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://ppa.birdmap.top

[T13] Kotlin：只读 Map
来源：http://qzg.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://ciq.yanxiufei.cn

[T14] Kotlin：循环
来源：http://sro.9152youxi.cn

for (i in 1..10) println(i)
来源：http://hyi.shuidangran.top

[T15] Kotlin：接口
来源：http://sof.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://cdy.cheryme.top

[T16] Swift：Hello World
来源：http://uvh.cashguo.top

print("Hello")
来源：http://ezi.aizwys.cn

[T17] Swift：变量与常量
来源：http://rrb.nanxinkj.top

var a = 1;  let b = 2
来源：http://fgi.cqqwz.cn

[T18] Swift：字符串插值
来源：http://nzk.ybcxt.top

"值: \(b)"
来源：http://vmh.smart0.xyz

[T19] Swift：可选绑定
来源：http://cnz.guannengcc.top

if let n = opt { print(n) }
来源：http://zop.yuxming.cn

[T20] Swift：数组操作
来源：http://mtk.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qis.shzxlz.cn

[T21] Swift：遍历
来源：http://hup.zhijiandao.cn

for x in a { print(x) }
来源：http://ovy.feifeiyinyue.top

[T22] Swift：字典
来源：http://tld.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aau.epnwcf.com

[T23] Swift：函数
来源：http://gah.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yig.hnqzz.top

[T24] Swift：闭包
来源：http://lrr.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jge.hysaishi.cn

[T25] Swift：结构体
来源：http://akt.gogol.net.cn

struct P { var x: Int }
来源：http://zzl.hesvh.cn

[T26] Swift：类与重写
来源：http://ixb.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://ujf.shzxlz.cn

[T27] Swift：错误处理
来源：http://dzt.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://vjb.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://iex.0kj1m.cn

enum Color { case red, green }
来源：http://sbr.tarul.cn

[T29] Swift：guard 提前返回
来源：http://vpv.nanxuanxn.top

guard let x = opt else { return }
来源：http://qgs.jinqigfzy.top

[T30] Swift：协议
来源：http://dxl.gzhubu.top

protocol Shape { func area() -> Double }
来源：http://sve.tanke756.top

[T31] Lua：Hello World
来源：http://llq.wangshuangyany.cn

print("Hello")
来源：http://llf.jianghu66.top

[T32] Lua：局部变量
来源：http://tme.hfpthk.cn

local a = 1
来源：http://hnb.cqqwz.cn

[T33] Lua：表（数组）
来源：http://ssx.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fst.zhoulong.xyz

[T34] Lua：遍历表
来源：http://ztk.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://huh.gogol.net.cn

[T35] Lua：字典表
来源：http://uvy.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://eww.zhixingplan.top

[T36] Lua：函数
来源：http://bdl.hfpthk.cn

function add(a, b) return a + b end
来源：http://nle.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://spx.svipenyu.cn

"a" .. "b"
来源：http://oaa.ivvv.top

[T38] Lua：条件
来源：http://cvo.zhengqikj.top

if x > 0 then print("正") end
来源：http://wix.zycfv.cn

[T39] Lua：模式匹配
来源：http://osw.xinyue.icu

string.find(s, "%d+")
来源：http://bdr.ybcxt.top

[T40] Lua：元表
来源：http://mah.xinyue.icu

setmetatable({}, { __index = base })
来源：http://bvd.yueranfly.top

[T41] Perl：Hello World
来源：http://dzh.yanxiufei.cn

print "Hello\n";
来源：http://rej.hesvh.cn

[T42] Perl：变量类型
来源：http://aqq.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yxd.tarul.cn

[T43] Perl：字符串插值
来源：http://wrh.gotoacloud.top

"值: $a"
来源：http://ono.havefunace.top

[T44] Perl：条件
来源：http://ybx.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://vkp.uphjek.com

[T45] Perl：数组遍历
来源：http://myq.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://yme.vehdjk.com

[T46] Perl：哈希操作
来源：http://ixf.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bnb.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://crn.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://vyr.ehwqpu.com

[T48] Perl：正则替换
来源：http://lxh.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://mxl.jqgufenzy.top

[T49] Perl：函数
来源：http://edj.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tsu.shuidangran.top

[T50] Perl：逐行读文件
来源：http://jii.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rvc.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://cwl.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://wdy.hnxiangtu.top

println("Hello")
来源：http://kpk.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://aya.cucudq.cn

val a = 1;  var b = 2
来源：http://fhc.xylfe.cn

[T53] Scala：字符串插值
来源：http://ewp.aizwys.cn

s"值: $b"
来源：http://vrp.hesvh.cn

[T54] Scala：集合映射
来源：http://oin.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://zld.uphjek.com

[T55] Scala：集合过滤
来源：http://tpl.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://uzy.jqgfzy.top

[T56] Scala：样例类
来源：http://pbv.aibaodan.cn

case class User(name: String, age: Int)
来源：http://zty.bbcook.cn

[T57] Scala：模式匹配
来源：http://ilw.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ddy.vehdjk.com

[T58] Scala：函数定义
来源：http://ons.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nvp.jinghuilouyu.cn

[T59] Scala：循环
来源：http://btr.shuidangran.top

for (i <- 1 to 10) println(i)
来源：http://fuz.xziqi.cn

[T60] Scala：折叠
来源：http://tfv.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aor.tarul.cn

================================================================================
来源：http://wif.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jhz.yueranfly.top

================================================================================
来源：http://vxs.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://uno.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://boc.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://kjs.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xee.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://kmn.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fbx.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://qmp.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bbf.fengsongda.top

[U05] Py：列表去重且保序
来源：http://vip.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://osa.ydzc1.top

[U06] Py：合并两个字典
来源：http://bat.yuxming.cn

{**a, **b}
来源：http://mtx.hysaishi.cn

[U07] Py：反转字典键值
来源：http://vqk.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://wvk.sweek.top

[U08] Py：展平二维列表
来源：http://zmq.jinqigfzy.top

[y for x in nested for y in x]
来源：http://rmo.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://yxd.sufxvd.cn

max(d, key=d.get)
来源：http://grx.fehbvm.com

[U10] Py：按值排序字典
来源：http://zgl.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hvr.fengsongda.top

[U11] Py：生成器表达式
来源：http://hbo.cqqwz.cn

(x * 2 for x in arr)
来源：http://pei.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://vxk.nwbrower.top

Counter(arr).most_common(3)
来源：http://aar.yvedp.cn

[U13] Py：固定长度队列
来源：http://qfm.9152youxi.cn

deque(maxlen=10)
来源：http://wif.xuanzx.com

[U14] Py：分组收集到列表
来源：http://oqu.sjlbkw.cn

defaultdict(list)
来源：http://zba.guannengcc.top

[U15] Py：高精度计时
来源：http://gvd.bbcook.cn

t = time.perf_counter()
来源：http://ixh.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://fae.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://reo.ivvv.top

[U17] Py：初始化日志
来源：http://ynp.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://hxx.yonumen.top

[U18] Py：预编译正则
来源：http://krj.hysaishi.cn

pat = re.compile(r"\d+")
来源：http://nwu.yanxiufei.cn

[U19] Py：正则替换带回调
来源：http://zno.c1oappe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://snd.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://cdf.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://fhx.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://cal.kuanghao11.cn

@contextlib.contextmanager
来源：http://rhw.birdmap.top

[U22] Py：矩阵转置
来源：http://roi.shanyushiyangkeji.top

list(zip(*m))
来源：http://tzd.zycfv.cn

[U23] Py：分块读取大文件
来源：http://xcg.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vbw.zycfv.cn

[U24] Py：路径操作
来源：http://njg.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zbr.daria6918.cn

[U25] Py：CSV 按字典读
来源：http://qyc.zdbjq.cn

csv.DictReader(f)
来源：http://jnb.hysaishi.cn

[U26] Py：并发下载
来源：http://mos.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://efq.fengsongda.top

[U27] Py：异步 HTTP
来源：http://qmz.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://yon.andypj.xyz

[U28] Py：类型别名
来源：http://jft.jinqigufen.top

UserId = int
来源：http://tni.xylfe.cn

[U29] Py：属性校验
来源：http://daa.yj202588.top

@property 与 @x.setter 配合
来源：http://oxg.pengpengdd.cyou

[U30] Py：数据类
来源：http://aoo.guowangkeji.top

@dataclass(slots=True)
来源：http://lno.sysykeji.top

[U31] Py：单测
来源：http://jmh.tian-w.cn

python -m pytest -q
来源：http://tpt.andypj.xyz

[U32] Py：代码格式化
来源：http://cnf.sweek.top

ruff format . && ruff check --fix .
来源：http://qzy.chenlongwang.top

[U33] Py：打包发布
来源：http://ycr.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://ily.jiagoushi.top

[U34] Py：判断编码
来源：http://jlj.shuidangran.top

chardet.detect(raw)
来源：http://bdz.jyoumei.cn


<!-- 参考信息 -->