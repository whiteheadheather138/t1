代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://fvx.ydzc1.top

[S15] C：类型转换
来源：http://htk.yj202588.top

(double) a / b
来源：http://sad.fzhhl.top

[S16] C：位操作置位
来源：http://foj.pengpengdd.cyou

x |= (1 << 3);
来源：http://hva.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://oap.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://puv.c1oappe.top

[S18] C：命令行参数
来源：http://sra.vehdjk.com

int main(int argc, char **argv)
来源：http://pbd.feifeiyinyue.top

[S19] C：快速排序
来源：http://kmu.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://biy.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://ily.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://frz.aizwys.cn

[S21] C：字符类别判断
来源：http://crv.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sys.jinqigufen.top

[S22] C：字符串转数字
来源：http://gqg.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://pym.dashuyun.cn

[S23] C：随机数
来源：http://rzu.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mrs.yueranfly.top

[S24] C：获取本地时间
来源：http://exd.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ilo.sweek.top

[S25] C：内存拷贝
来源：http://uww.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://fel.wangdashe.top

[S26] C：内存清零
来源：http://thg.fktsv.cn

memset(a, 0, sizeof a);
来源：http://ddk.tanke756.top

[S27] C：定义常量
来源：http://klo.hysaishi.cn

const double PI = 3.14159;
来源：http://rgm.sysykeji.top

[S28] C：静态变量
来源：http://wec.yj20258888.top

static int counter = 0;
来源：http://vcw.jlsjyb.cn

[S29] C：变参函数
来源：http://dsm.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wyf.ydjk.org.cn

[S30] C：头文件保护
来源：http://pmu.hnxiangtu.top

#ifndef X_H
来源：http://aka.uphjek.com

#define X_H
来源：http://ldu.fengsongda.top

#endif
来源：http://krr.sxryk.cn

[S31] C++：Hello World
来源：http://kyk.tarul.cn

#include <iostream>
来源：http://ayx.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://xlj.zhijiandao.cn

[S32] C++：字符串
来源：http://llc.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://ypy.c1oappe.top

[S33] C++：vector 增删
来源：http://rtn.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nit.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://sod.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://efl.yvedp.cn

[S35] C++：map
来源：http://uuw.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://avu.nanxuanxn.top

[S36] C++：unordered_map
来源：http://els.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gbe.hnxiangtu.top

[S37] C++：set
来源：http://wzy.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbg.fzhhl.top

[S38] C++：排序
来源：http://uts.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://ugb.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://gfh.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fri.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://ytm.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://izw.dashuyun.cn

[S41] C++：类与构造函数
来源：http://kwj.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://imw.uphjek.com

[S42] C++：继承与虚函数
来源：http://nvi.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://rug.yueranfly.top

[S43] C++：智能指针
来源：http://kvp.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://jju.aizwys.cn

[S44] C++：引用传参
来源：http://ajx.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://npp.fehbvm.com

[S45] C++：lambda
来源：http://iwh.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ruz.ehwqpu.com

[S46] C++：函数模板
来源：http://lqw.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oeo.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://vbb.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wyb.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://mkd.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uzc.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://ksm.shanyushiyangtech.top

[S49] C++：写文件
来源：http://szn.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pee.jinqigufen.top

[S50] C++：格式化数字
来源：http://ruo.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wuj.dashuyun.cn

[S51] C++：显式类型转换
来源：http://ryf.tianlin.xyz

static_cast<double>(a) / b
来源：http://xyv.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://lol.yfazqb.com

int size() const noexcept { return n_; }
来源：http://qwt.ydjk.org.cn

[S53] C++：移动语义
来源：http://pmn.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://ipy.fehbvm.com

[S54] C++：异常处理
来源：http://jrt.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kqy.tianlin.xyz

[S55] C++：结构化绑定
来源：http://atj.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://wxd.sxryk.cn

[S56] C++：optional
来源：http://abx.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tmq.316326.xyz

[S57] C++：编译期常量
来源：http://mzq.cucudq.cn

constexpr int N = 10;
来源：http://iqq.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://fpp.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://xde.yvedp.cn

[S59] C++：静态断言
来源：http://mkl.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://quz.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://yae.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ibi.sweek.top

================================================================================
来源：http://nvm.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wxj.jianghu66.top

================================================================================
来源：http://vhk.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://lir.yj20258.top

println("Hello")
来源：http://anm.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://rlf.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cyc.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://yjn.gotoacloud.top

"值: $b"
来源：http://smu.xinyue.icu

[T04] Kotlin：空安全
来源：http://wnd.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://gie.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://zcq.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lxe.c1oappe.top

[T06] Kotlin：集合映射
来源：http://bkl.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vqo.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://bra.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://afy.yj20258888.top

[T08] Kotlin：数据类
来源：http://xtd.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://app.yonumen.top

[T09] Kotlin：扩展函数
来源：http://wtn.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://ply.tian-w.cn

[T10] Kotlin：默认参数
来源：http://qpf.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nlr.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://nzm.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gjl.bjfxy.top

[T12] Kotlin：解构声明
来源：http://mlr.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://hel.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://lfz.cqqwz.cn

val m = mapOf("a" to 1)
来源：http://abo.dashuyun.cn

[T14] Kotlin：循环
来源：http://jke.sufxvd.cn

for (i in 1..10) println(i)
来源：http://cet.hfpthk.cn

[T15] Kotlin：接口
来源：http://cpt.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://vdz.yj20258.top

[T16] Swift：Hello World
来源：http://dtt.zhaomingkeji.xyz

print("Hello")
来源：http://msx.52xcode.cn

[T17] Swift：变量与常量
来源：http://zct.nanxinkj.top

var a = 1;  let b = 2
来源：http://skv.bbcook.cn

[T18] Swift：字符串插值
来源：http://gas.yongpay.top

"值: \(b)"
来源：http://coz.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://hgh.guannengcc.top

if let n = opt { print(n) }
来源：http://rrs.hnxiangtu.top

[T20] Swift：数组操作
来源：http://poa.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uam.yanxiufei.cn

[T21] Swift：遍历
来源：http://bke.andypj.xyz

for x in a { print(x) }
来源：http://wut.ctjpmb.com

[T22] Swift：字典
来源：http://jei.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://jlq.chenzaomai.com

[T23] Swift：函数
来源：http://bgh.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hrk.sxryk.cn

[T24] Swift：闭包
来源：http://ttj.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xmt.epnwcf.com

[T25] Swift：结构体
来源：http://juj.hongshengwenyu.top

struct P { var x: Int }
来源：http://nqd.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://iqu.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://znl.sxryk.cn

[T27] Swift：错误处理
来源：http://hbu.sweek.top

do { try f() } catch { print(error) }
来源：http://oxs.jqgufenzy.top

[T28] Swift：枚举
来源：http://prt.quarkkingdee.top

enum Color { case red, green }
来源：http://njl.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://gkr.meibo888.top

guard let x = opt else { return }
来源：http://hfu.yongpay.top

[T30] Swift：协议
来源：http://vyq.cashguo.top

protocol Shape { func area() -> Double }
来源：http://nfc.mhx1999.top

[T31] Lua：Hello World
来源：http://egh.sxryk.cn

print("Hello")
来源：http://zen.sufxvd.cn

[T32] Lua：局部变量
来源：http://duw.chenlongwang.top

local a = 1
来源：http://bmw.yuxming.cn

[T33] Lua：表（数组）
来源：http://ycy.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://tqc.yangfankeji.com

[T34] Lua：遍历表
来源：http://maj.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fyb.jqgfzy.top

[T35] Lua：字典表
来源：http://sua.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://zrq.hnxiangtu.top

[T36] Lua：函数
来源：http://lnl.nwbrower.top

function add(a, b) return a + b end
来源：http://ekm.316326.xyz

[T37] Lua：字符串拼接
来源：http://sok.jianghu66.top

"a" .. "b"
来源：http://phu.zhengqikj.top

[T38] Lua：条件
来源：http://jpk.gogol.net.cn

if x > 0 then print("正") end
来源：http://ita.snrcjt.cn

[T39] Lua：模式匹配
来源：http://fcd.zhengqikj.top

string.find(s, "%d+")
来源：http://aoj.ydzc1.top

[T40] Lua：元表
来源：http://uma.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://rov.hesvh.cn

[T41] Perl：Hello World
来源：http://fsk.yuxming.cn

print "Hello\n";
来源：http://sfe.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://jlg.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qtn.pycfn.com

[T43] Perl：字符串插值
来源：http://prh.hfpthk.cn

"值: $a"
来源：http://tcy.shuidangran.top

[T44] Perl：条件
来源：http://mld.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://oqb.redwolf501.top

[T45] Perl：数组遍历
来源：http://suj.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://jat.bbcook.cn

[T46] Perl：哈希操作
来源：http://bot.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ocr.yj20258888.top

[T47] Perl：正则捕获
来源：http://ejs.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zhi.uphjek.com

[T48] Perl：正则替换
来源：http://jgw.dashuyun.cn

$s =~ s/old/new/g;
来源：http://npp.zdqjudy.top

[T49] Perl：函数
来源：http://dln.cucudq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iqu.nanxuanxn.top

[T50] Perl：逐行读文件
来源：http://keh.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mhg.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://sth.yvedp.cn

[T51] Scala：Hello World
来源：http://bca.zhengqikj.top

println("Hello")
来源：http://mru.zdqjudy.top

[T52] Scala：变量
来源：http://fpv.quarkkingdee.top

val a = 1;  var b = 2
来源：http://edm.daxiang520.top

[T53] Scala：字符串插值
来源：http://uzc.aizwys.cn

s"值: $b"
来源：http://aje.jqgufenzy.top

[T54] Scala：集合映射
来源：http://ran.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://mup.xuanzx.com

[T55] Scala：集合过滤
来源：http://pmy.fzhhl.top

List(1, 2, 3).filter(_ > 1)
来源：http://ubr.yuxming.cn

[T56] Scala：样例类
来源：http://szd.shuidangran.top

case class User(name: String, age: Int)
来源：http://ogp.yueranfly.top

[T57] Scala：模式匹配
来源：http://plg.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zme.aibaodan.cn

[T58] Scala：函数定义
来源：http://ell.zycfv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tyg.zdqjudy.top

[T59] Scala：循环
来源：http://eff.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://osc.tian-w.cn

[T60] Scala：折叠
来源：http://xst.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vjy.havefunace.top

================================================================================
来源：http://rpq.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bpk.nanxinkj.top

================================================================================
来源：http://pkg.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://zer.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://ytk.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://iue.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lsp.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://pij.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xtw.hesvh.cn

[U04] Py：变量调试打印
来源：http://yhe.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ysx.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://hqe.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://lyn.zhiwuduotai.top

[U06] Py：合并两个字典
来源：http://bcq.cdnleiting.top

{**a, **b}
来源：http://xqj.shuidangran.top

[U07] Py：反转字典键值
来源：http://aan.guannengcc.top

{v: k for k, v in d.items()}
来源：http://fnj.cqqwz.cn

[U08] Py：展平二维列表
来源：http://ztd.hesvh.cn

[y for x in nested for y in x]
来源：http://jke.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://taq.jqgufenzy.top

max(d, key=d.get)
来源：http://ila.hnxiangtu.top

[U10] Py：按值排序字典
来源：http://fkj.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xea.haohaochexian.top

[U11] Py：生成器表达式
来源：http://qej.mhx1999.top

(x * 2 for x in arr)
来源：http://sfd.yj20258888.top

[U12] Py：取出现最多的 3 个元素
来源：http://pln.sxryk.cn

Counter(arr).most_common(3)
来源：http://psg.xziqi.cn

[U13] Py：固定长度队列
来源：http://izq.pycfn.com

deque(maxlen=10)
来源：http://byf.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://sai.svipenyu.cn

defaultdict(list)
来源：http://ddk.tarul.cn

[U15] Py：高精度计时
来源：http://voa.yvedp.cn

t = time.perf_counter()
来源：http://unp.hnqzz.top

[U16] Py：命令行参数解析
来源：http://jgi.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://swt.jianghu66.top

[U17] Py：初始化日志
来源：http://nvq.shzxlz.cn

logging.basicConfig(level=logging.INFO)
来源：http://qpq.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://mwm.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://tma.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://our.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://veu.fzhhl.top

[U20] Py：缓存函数结果
来源：http://xib.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://fvk.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://spq.uphjek.com

@contextlib.contextmanager
来源：http://lna.fzhhl.top

[U22] Py：矩阵转置
来源：http://ant.9152youxi.cn

list(zip(*m))
来源：http://myr.uphjek.com

[U23] Py：分块读取大文件
来源：http://ktj.xylfe.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://otj.dashuyun.cn

[U24] Py：路径操作
来源：http://hnm.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nkx.tianlin.xyz

[U25] Py：CSV 按字典读
来源：http://mey.zhongyouzk.top

csv.DictReader(f)
来源：http://zit.meibo888.top

[U26] Py：并发下载
来源：http://zvg.vqdsnc.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rqa.yvedp.cn

[U27] Py：异步 HTTP
来源：http://rjw.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://non.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://hfb.tarul.cn

UserId = int
来源：http://rwp.jinqigufen.top

[U29] Py：属性校验
来源：http://ukh.cdnleiting.top

@property 与 @x.setter 配合
来源：http://onc.ivvv.top

[U30] Py：数据类
来源：http://awv.ivvv.top

@dataclass(slots=True)
来源：http://soo.yongpay.top

[U31] Py：单测
来源：http://cul.hesvh.cn

python -m pytest -q
来源：http://jsf.uphjek.com

[U32] Py：代码格式化
来源：http://nsa.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://luf.jiagoushi.top

[U33] Py：打包发布
来源：http://xkl.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://meg.tarul.cn

[U34] Py：判断编码
来源：http://uky.birdmap.top

chardet.detect(raw)
来源：http://ras.zdqjudy.top

[U35] Py：发送邮件
来源：http://wnp.hongshengwenyu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qop.jinqigfzy.top

[U36] Py：定时任务
来源：http://qoh.epnwcf.com

schedule.every(10).minutes.do(job)
来源：http://uud.bjfxy.top

[U37] Py：读写 Excel
来源：http://ktt.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://ydd.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://ugq.hnqzz.top

Path(__file__).resolve().parent
来源：http://duf.guannengcc.top


<!-- 参考信息 -->