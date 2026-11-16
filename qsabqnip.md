代发 wailian999

int main(int argc, char **argv)
来源：http://srl.yvedp.cn

[S19] C：快速排序
来源：http://irx.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://kjw.birdmap.top

[S20] C：二分查找
来源：http://sci.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kdb.nwbrower.top

[S21] C：字符类别判断
来源：http://mqk.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iyj.hnxiangtu.top

[S22] C：字符串转数字
来源：http://bey.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://vzn.yangfankeji.com

[S23] C：随机数
来源：http://naz.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fyo.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://trc.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pdv.yfazqb.com

[S25] C：内存拷贝
来源：http://lee.gaohongyu789.top

memcpy(dst, src, n);
来源：http://lio.jlsjyb.cn

[S26] C：内存清零
来源：http://xnp.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://deo.xuetiantiany.cn

[S27] C：定义常量
来源：http://ubb.tian-w.cn

const double PI = 3.14159;
来源：http://ksl.shangyingyoupin.top

[S28] C：静态变量
来源：http://hcn.fehbvm.com

static int counter = 0;
来源：http://lfl.vehdjk.com

[S29] C：变参函数
来源：http://mnq.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nlp.xuetiantiany.cn

[S30] C：头文件保护
来源：http://ddf.fzhhl.top

#ifndef X_H
来源：http://uot.52xcode.cn

#define X_H
来源：http://yif.sweek.top

#endif
来源：http://ils.yj20258888.top

[S31] C++：Hello World
来源：http://yjo.jqgfzy.top

#include <iostream>
来源：http://dvr.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://man.sxryk.cn

[S32] C++：字符串
来源：http://ygg.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://rdd.hesvh.cn

[S33] C++：vector 增删
来源：http://eht.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wog.gotoacloud.top

[S34] C++：遍历 vector
来源：http://xym.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://kmn.ybcxt.top

[S35] C++：map
来源：http://aub.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uyc.svipenyu.cn

[S36] C++：unordered_map
来源：http://chx.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://btt.aibaodan.cn

[S37] C++：set
来源：http://xdy.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://slj.gzhubu.top

[S38] C++：排序
来源：http://szi.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://wxa.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://tkl.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ypw.vehdjk.com

[S40] C++：查找元素
来源：http://tbo.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://unk.yuxming.cn

[S41] C++：类与构造函数
来源：http://ldu.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yty.fzhhl.top

[S42] C++：继承与虚函数
来源：http://ybx.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://pqk.jyoumei.cn

[S43] C++：智能指针
来源：http://ogk.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://lbg.zdbjq.cn

[S44] C++：引用传参
来源：http://gyg.aizwys.cn

void inc(int &x) { ++x; }
来源：http://nxz.jinqigfzy.top

[S45] C++：lambda
来源：http://nej.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://dki.zhongyouzk.top

[S46] C++：函数模板
来源：http://oqc.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opa.316326.xyz

[S47] C++：结构化绑定遍历
来源：http://cfo.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cre.ctjpmb.com

[S48] C++：逐行读文件
来源：http://rwe.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://ddu.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://pbs.jyoumei.cn

[S49] C++：写文件
来源：http://hli.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ned.yj20258.top

[S50] C++：格式化数字
来源：http://rzo.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kmb.c1oappe.top

[S51] C++：显式类型转换
来源：http://scp.tian-w.cn

static_cast<double>(a) / b
来源：http://ekq.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://fas.daria6918.cn

int size() const noexcept { return n_; }
来源：http://fxp.sxryk.cn

[S53] C++：移动语义
来源：http://ooy.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://fcv.yj20258888.top

[S54] C++：异常处理
来源：http://oxz.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uph.andypj.xyz

[S55] C++：结构化绑定
来源：http://qtv.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://smx.hysaishi.cn

[S56] C++：optional
来源：http://fqp.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aoc.epnwcf.com

[S57] C++：编译期常量
来源：http://rst.shanyushiyangtech.top

constexpr int N = 10;
来源：http://qel.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://cdd.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://tix.sxryk.cn

[S59] C++：静态断言
来源：http://lrc.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sei.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://cbt.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tpr.yongpay.top

================================================================================
来源：http://ehq.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yzk.mhx1999.top

================================================================================
来源：http://uiy.daxiang520.top

[T01] Kotlin：Hello World
来源：http://uxv.bjfxy.top

println("Hello")
来源：http://mup.birdmap.top

[T02] Kotlin：变量
来源：http://lhn.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ein.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://kbc.nwbrower.top

"值: $b"
来源：http://pak.sufxvd.cn

[T04] Kotlin：空安全
来源：http://cwv.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://gri.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://sai.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cda.fehbvm.com

[T06] Kotlin：集合映射
来源：http://pzi.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kzk.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://pjb.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zzd.yueranfly.top

[T08] Kotlin：数据类
来源：http://rpv.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://hfi.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://far.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://gsv.ivvv.top

[T10] Kotlin：默认参数
来源：http://vwn.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rgd.hnxiangtu.top

[T11] Kotlin：协程
来源：http://gnl.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tzy.redwolf501.top

[T12] Kotlin：解构声明
来源：http://inq.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://rmd.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://zvl.yongpay.top

val m = mapOf("a" to 1)
来源：http://cef.pycfn.com

[T14] Kotlin：循环
来源：http://okm.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://yxf.ybcxt.top

[T15] Kotlin：接口
来源：http://uwg.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://byu.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://epp.sweek.top

print("Hello")
来源：http://zed.fehbvm.com

[T17] Swift：变量与常量
来源：http://idd.dianchejie.cn

var a = 1;  let b = 2
来源：http://tpc.hcnkem.com

[T18] Swift：字符串插值
来源：http://wtb.daria6918.cn

"值: \(b)"
来源：http://ocp.wangdashe.top

[T19] Swift：可选绑定
来源：http://mjq.fehbvm.com

if let n = opt { print(n) }
来源：http://bcs.zhengqikj.top

[T20] Swift：数组操作
来源：http://mov.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://ixi.cashguo.top

[T21] Swift：遍历
来源：http://oga.gaohongyu789.top

for x in a { print(x) }
来源：http://iom.ydzc1.top

[T22] Swift：字典
来源：http://yli.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://nxj.yuxming.cn

[T23] Swift：函数
来源：http://feb.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pot.ydjk.org.cn

[T24] Swift：闭包
来源：http://pme.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lzi.hfpthk.cn

[T25] Swift：结构体
来源：http://urj.jinghuilouyu.cn

struct P { var x: Int }
来源：http://ltf.sweek.top

[T26] Swift：类与重写
来源：http://jjb.chenzaomai.com

class A: Base { override func f() {} }
来源：http://lad.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://dgg.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://lxh.ctjpmb.com

[T28] Swift：枚举
来源：http://kbh.hnqzz.top

enum Color { case red, green }
来源：http://ojj.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://ici.svipenyu.cn

guard let x = opt else { return }
来源：http://muw.0kj1m.cn

[T30] Swift：协议
来源：http://itj.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://ptr.xylfe.cn

[T31] Lua：Hello World
来源：http://uki.chenzaomai.com

print("Hello")
来源：http://kuo.yj202588.top

[T32] Lua：局部变量
来源：http://lal.jinqigufen.top

local a = 1
来源：http://qcx.dashuyun.cn

[T33] Lua：表（数组）
来源：http://hti.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://twv.daxiang520.top

[T34] Lua：遍历表
来源：http://kiw.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cfw.xinyue.icu

[T35] Lua：字典表
来源：http://rbo.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://ioi.tianlin.xyz

[T36] Lua：函数
来源：http://mhf.gzhubu.top

function add(a, b) return a + b end
来源：http://ptf.tanke756.top

[T37] Lua：字符串拼接
来源：http://wdf.yj202588.top

"a" .. "b"
来源：http://hbw.gogol.net.cn

[T38] Lua：条件
来源：http://hwm.tian-w.cn

if x > 0 then print("正") end
来源：http://qqq.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://cdy.zhengqikj.top

string.find(s, "%d+")
来源：http://rvi.shanyushiyangkeji.top

[T40] Lua：元表
来源：http://bnf.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://sfs.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://zvg.yonumen.top

print "Hello\n";
来源：http://ijx.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://ybn.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zwy.jqgfzy.top

[T43] Perl：字符串插值
来源：http://jaz.cheryme.top

"值: $a"
来源：http://sss.bbcook.cn

[T44] Perl：条件
来源：http://dka.316326.xyz

if ($a > 0) { print "正"; }
来源：http://kpx.shuidangran.top

[T45] Perl：数组遍历
来源：http://hoa.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://mrs.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://qya.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tjl.fengsongda.top

[T47] Perl：正则捕获
来源：http://usr.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lsv.yfazqb.com

[T48] Perl：正则替换
来源：http://jsp.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://ash.jinghuilouyu.cn

[T49] Perl：函数
来源：http://apk.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://odb.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://lpp.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ebz.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://ckt.fengsongda.top

[T51] Scala：Hello World
来源：http://dbd.nanxinkj.top

println("Hello")
来源：http://tez.fanxiaobao.xyz

[T52] Scala：变量
来源：http://tdh.cqqwz.cn

val a = 1;  var b = 2
来源：http://dex.mhx1999.top

[T53] Scala：字符串插值
来源：http://yyg.pengpengdd.cyou

s"值: $b"
来源：http://cei.nwbrower.top

[T54] Scala：集合映射
来源：http://mix.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://qmn.shzxlz.cn

[T55] Scala：集合过滤
来源：http://ywi.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cyu.nanxuanxn.top

[T56] Scala：样例类
来源：http://mmw.uphjek.com

case class User(name: String, age: Int)
来源：http://tpx.aibaodan.cn

[T57] Scala：模式匹配
来源：http://fss.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lyw.sweek.top

[T58] Scala：函数定义
来源：http://sdq.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uqh.jlsjyb.cn

[T59] Scala：循环
来源：http://bjr.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://yam.iojbl.cn

[T60] Scala：折叠
来源：http://gly.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tcf.zdbjq.cn

================================================================================
来源：http://usk.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ezv.jyoumei.cn

================================================================================
来源：http://erq.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://wgr.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://cnt.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://slx.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ipr.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://onj.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://gwn.xylfe.cn

[U04] Py：变量调试打印
来源：http://odq.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tkq.yonumen.top

[U05] Py：列表去重且保序
来源：http://svb.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://kgm.hysaishi.cn

[U06] Py：合并两个字典
来源：http://wjc.pengpengdd.cyou

{**a, **b}
来源：http://nrd.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://szl.fengsongda.top

{v: k for k, v in d.items()}
来源：http://nhk.haohaochexian.top

[U08] Py：展平二维列表
来源：http://smy.jinghuilouyu.cn

[y for x in nested for y in x]
来源：http://nif.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://yac.hcnkem.com

max(d, key=d.get)
来源：http://jfe.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://csw.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zkp.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://ffs.epnwcf.com

(x * 2 for x in arr)
来源：http://dfw.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://owm.yangfankeji.com

Counter(arr).most_common(3)
来源：http://xvi.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://rlm.gzhubu.top

deque(maxlen=10)
来源：http://ein.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://nig.chenlongwang.top

defaultdict(list)
来源：http://clh.sjlbkw.cn

[U15] Py：高精度计时
来源：http://pmp.jlsjyb.cn

t = time.perf_counter()
来源：http://gkx.cucudq.cn

[U16] Py：命令行参数解析
来源：http://ska.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zmp.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://waz.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://yar.sysykeji.top

[U18] Py：预编译正则
来源：http://wiz.mhx1999.top

pat = re.compile(r"\d+")
来源：http://smf.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://orb.52xcode.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hpl.wangdashe.top

[U20] Py：缓存函数结果
来源：http://dxj.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://yhi.ywan-chungtsiang.top

[U21] Py：自定义上下文管理器
来源：http://jlr.9152youxi.cn

@contextlib.contextmanager
来源：http://mdp.svipenyu.cn

[U22] Py：矩阵转置
来源：http://btc.pycfn.com

list(zip(*m))
来源：http://fdp.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://dvo.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ycs.havefunace.top

[U24] Py：路径操作
来源：http://qgg.nwbrower.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rav.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://eep.aibaodan.cn

csv.DictReader(f)
来源：http://yws.hammf.cn

[U26] Py：并发下载
来源：http://xcx.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vwv.xylfe.cn

[U27] Py：异步 HTTP
来源：http://kgi.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://fdj.xinyue.icu

[U28] Py：类型别名
来源：http://wuh.fehbvm.com

UserId = int
来源：http://xld.quarkkingdee.top

[U29] Py：属性校验
来源：http://spx.gaohongyu789.top

@property 与 @x.setter 配合
来源：http://rhr.hnqzz.top

[U30] Py：数据类
来源：http://fwy.jlsjyb.cn

@dataclass(slots=True)
来源：http://ljm.jqgfzy.top

[U31] Py：单测
来源：http://cfu.jqgufenzy.top

python -m pytest -q
来源：http://oja.nanxuanxn.top

[U32] Py：代码格式化
来源：http://jos.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://yom.shzxlz.cn

[U33] Py：打包发布
来源：http://xvn.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://zru.gogol.net.cn

[U34] Py：判断编码
来源：http://lhd.hfpthk.cn

chardet.detect(raw)
来源：http://plm.ydzc1.top

[U35] Py：发送邮件
来源：http://pxe.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aud.snrcjt.cn

[U36] Py：定时任务
来源：http://gcm.daria6918.cn

schedule.every(10).minutes.do(job)
来源：http://ivs.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://mel.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://fif.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://uma.feifeiyinyue.top

Path(__file__).resolve().parent
来源：http://ckz.ivvv.top

[U39] Py：判断是否在交互环境
来源：http://kef.yueranfly.top

sys.stdout.isatty()
来源：http://tof.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://ucy.andypj.xyz

print("err", file=sys.stderr)
来源：http://bpl.havefunace.top

[U41] PHP：初始化 Composer 项目
来源：http://wva.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ump.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://cja.havefunace.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wzt.gaohongyu789.top


<!-- 参考信息 -->