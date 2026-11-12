代发 wailian999

int main(int argc, char **argv)
来源：http://utn.chenjidiqi.icu

[S19] C：快速排序
来源：http://vca.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://aar.sxryk.cn

[S20] C：二分查找
来源：http://bkj.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rxt.zhongyouzk.top

[S21] C：字符类别判断
来源：http://wdn.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sne.cdnleiting.top

[S22] C：字符串转数字
来源：http://aqb.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://xme.hywenlv.cn

[S23] C：随机数
来源：http://efr.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hnq.ppjwa.cn

[S24] C：获取本地时间
来源：http://jhg.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ifm.redwolf501.top

[S25] C：内存拷贝
来源：http://vmy.ydjk.org.cn

memcpy(dst, src, n);
来源：http://mco.cqqwz.cn

[S26] C：内存清零
来源：http://awm.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://npo.hnqzz.top

[S27] C：定义常量
来源：http://cil.hnxiangtu.top

const double PI = 3.14159;
来源：http://fty.jlsjyb.cn

[S28] C：静态变量
来源：http://bow.316326.xyz

static int counter = 0;
来源：http://lks.zdbjq.cn

[S29] C：变参函数
来源：http://vbg.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmq.fktsv.cn

[S30] C：头文件保护
来源：http://lfk.jqgufenzy.top

#ifndef X_H
来源：http://kko.sxryk.cn

#define X_H
来源：http://mdi.iojbl.cn

#endif
来源：http://xjo.yuanzhike.top

[S31] C++：Hello World
来源：http://pom.xuetiantiany.cn

#include <iostream>
来源：http://ihw.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://zyr.gotoacloud.top

[S32] C++：字符串
来源：http://hxk.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://psf.0kj1m.cn

[S33] C++：vector 增删
来源：http://ymu.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gfs.316326.xyz

[S34] C++：遍历 vector
来源：http://cxp.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://lef.wangshuangyany.cn

[S35] C++：map
来源：http://ovh.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxs.jinqigfzy.top

[S36] C++：unordered_map
来源：http://qre.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uxg.fzhhl.top

[S37] C++：set
来源：http://brp.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lra.sweek.top

[S38] C++：排序
来源：http://xtb.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://mdl.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://xlw.quarkkingdee.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hgr.aibaodan.cn

[S40] C++：查找元素
来源：http://svv.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yyj.hnqzz.top

[S41] C++：类与构造函数
来源：http://yvm.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xzs.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://zwq.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://fhw.shangyingyoupin.top

[S43] C++：智能指针
来源：http://ffz.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://eop.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://hza.cucudq.cn

void inc(int &x) { ++x; }
来源：http://xri.ivvv.top

[S45] C++：lambda
来源：http://jqd.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://nqm.yonumen.top

[S46] C++：函数模板
来源：http://dsp.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dlh.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://gfl.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fbe.hcnkem.com

[S48] C++：逐行读文件
来源：http://fmk.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://khu.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://cok.bbcook.cn

[S49] C++：写文件
来源：http://dbn.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tmy.iojbl.cn

[S50] C++：格式化数字
来源：http://ceq.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cbp.zycfv.cn

[S51] C++：显式类型转换
来源：http://hns.epnwcf.com

static_cast<double>(a) / b
来源：http://fmx.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://jyz.cheryme.top

int size() const noexcept { return n_; }
来源：http://nns.hcnkem.com

[S53] C++：移动语义
来源：http://rty.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://xuk.redwolf501.top

[S54] C++：异常处理
来源：http://yeb.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vhw.guannengcc.top

[S55] C++：结构化绑定
来源：http://jrs.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bxn.nanxinkj.top

[S56] C++：optional
来源：http://jyb.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jyz.andypj.xyz

[S57] C++：编译期常量
来源：http://czp.zhixingplan.top

constexpr int N = 10;
来源：http://twl.sweek.top

[S58] C++：命名空间
来源：http://iki.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://pxq.uphjek.com

[S59] C++：静态断言
来源：http://udi.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ilc.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://oya.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rkt.yuxming.cn

================================================================================
来源：http://fzi.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fes.hongshengwenyu.top

================================================================================
来源：http://krp.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://rwj.ppjwa.cn

println("Hello")
来源：http://uch.0kj1m.cn

[T02] Kotlin：变量
来源：http://qao.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzk.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://hnc.ydjk.org.cn

"值: $b"
来源：http://qdd.redwolf501.top

[T04] Kotlin：空安全
来源：http://ivn.jiagoushi.top

val n: String? = null;  n?.length
来源：http://xve.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://vny.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://enz.meibo888.top

[T06] Kotlin：集合映射
来源：http://ybz.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ops.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://jme.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://abf.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://nbs.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://ktx.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://dew.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://ybd.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://eqh.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sxn.gogol.net.cn

[T11] Kotlin：协程
来源：http://dhh.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://udg.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://xfe.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://hee.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://qnm.yfazqb.com

val m = mapOf("a" to 1)
来源：http://mvm.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://zjl.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://qms.zhixingplan.top

[T15] Kotlin：接口
来源：http://usa.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://uwr.zdbjq.cn

[T16] Swift：Hello World
来源：http://ain.yuanzhike.top

print("Hello")
来源：http://nga.hesvh.cn

[T17] Swift：变量与常量
来源：http://hgv.9152youxi.cn

var a = 1;  let b = 2
来源：http://zcb.yj20258888.top

[T18] Swift：字符串插值
来源：http://zti.zdqjudy.top

"值: \(b)"
来源：http://ibw.bbcook.cn

[T19] Swift：可选绑定
来源：http://esg.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://bla.yongpay.top

[T20] Swift：数组操作
来源：http://jep.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://myu.zhoulong.xyz

[T21] Swift：遍历
来源：http://rri.yangfankeji.com

for x in a { print(x) }
来源：http://kii.dashuyun.cn

[T22] Swift：字典
来源：http://xln.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://dij.bjfxy.top

[T23] Swift：函数
来源：http://qah.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fal.fengsongda.top

[T24] Swift：闭包
来源：http://uxn.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aap.tarul.cn

[T25] Swift：结构体
来源：http://civ.bjfxy.top

struct P { var x: Int }
来源：http://sku.gotoacloud.top

[T26] Swift：类与重写
来源：http://ufy.0kj1m.cn

class A: Base { override func f() {} }
来源：http://yvz.zhiwuduotai.top

[T27] Swift：错误处理
来源：http://nhq.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://wle.nwbrower.top

[T28] Swift：枚举
来源：http://mud.jyoumei.cn

enum Color { case red, green }
来源：http://cxl.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://vaj.zycfv.cn

guard let x = opt else { return }
来源：http://igd.tarul.cn

[T30] Swift：协议
来源：http://bdm.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://epr.zhongyouzk.top

[T31] Lua：Hello World
来源：http://hlx.xuanzx.com

print("Hello")
来源：http://whz.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://rel.dashuyun.cn

local a = 1
来源：http://cth.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://hpy.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://aos.jinqigfzy.top

[T34] Lua：遍历表
来源：http://fzd.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://api.yuanzhike.top

[T35] Lua：字典表
来源：http://azx.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://fmy.nwbrower.top

[T36] Lua：函数
来源：http://yev.jqgfzy.top

function add(a, b) return a + b end
来源：http://yrp.yj20258.top

[T37] Lua：字符串拼接
来源：http://eif.feifeiyinyue.top

"a" .. "b"
来源：http://aci.dashuyun.cn

[T38] Lua：条件
来源：http://xbx.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://wom.yuanzhike.top

[T39] Lua：模式匹配
来源：http://gkk.tanke756.top

string.find(s, "%d+")
来源：http://fvw.jyoumei.cn

[T40] Lua：元表
来源：http://gwl.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://jtd.havefunace.top

[T41] Perl：Hello World
来源：http://vyt.feifeiyinyue.top

print "Hello\n";
来源：http://gfa.yj20258.top

[T42] Perl：变量类型
来源：http://jfb.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vqp.fengsongda.top

[T43] Perl：字符串插值
来源：http://vqj.hysaishi.cn

"值: $a"
来源：http://ihb.haohaochexian.top

[T44] Perl：条件
来源：http://icb.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://diz.meibo888.top

[T45] Perl：数组遍历
来源：http://rmf.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://szg.xylfe.cn

[T46] Perl：哈希操作
来源：http://azj.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mlz.iojbl.cn

[T47] Perl：正则捕获
来源：http://hba.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bdy.sjlbkw.cn

[T48] Perl：正则替换
来源：http://juj.svipenyu.cn

$s =~ s/old/new/g;
来源：http://rcx.hnqzz.top

[T49] Perl：函数
来源：http://pbw.snrcjt.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tlo.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://zqh.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ukk.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://mpv.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://vfy.hongshengwenyu.top

println("Hello")
来源：http://kcr.xuanzx.com

[T52] Scala：变量
来源：http://ods.dashuyun.cn

val a = 1;  var b = 2
来源：http://qbi.fktsv.cn

[T53] Scala：字符串插值
来源：http://wad.meibo888.top

s"值: $b"
来源：http://kjf.fktsv.cn

[T54] Scala：集合映射
来源：http://kbr.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://smo.xziqi.cn

[T55] Scala：集合过滤
来源：http://ugh.shanyushiyangtech.top

List(1, 2, 3).filter(_ > 1)
来源：http://bdq.yuanzhike.top

[T56] Scala：样例类
来源：http://mji.fanxiaobao.xyz

case class User(name: String, age: Int)
来源：http://pxv.redwolf501.top

[T57] Scala：模式匹配
来源：http://zca.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zte.jinqigfzy.top

[T58] Scala：函数定义
来源：http://pxl.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://dkk.hammf.cn

[T59] Scala：循环
来源：http://fsu.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://kdo.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://jcz.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mlc.jqgufenzy.top

================================================================================
来源：http://xdt.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oum.yj20258.top

================================================================================
来源：http://nfs.chenjidiqi.icu

[U01] Py：创建虚拟环境
来源：http://xtf.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zke.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://fuu.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sqn.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://jsq.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upk.sysykeji.top

[U04] Py：变量调试打印
来源：http://vhl.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bie.pycfn.com

[U05] Py：列表去重且保序
来源：http://vxn.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://fom.snrcjt.cn

[U06] Py：合并两个字典
来源：http://vxe.zhongyouzk.top

{**a, **b}
来源：http://ask.nwbrower.top

[U07] Py：反转字典键值
来源：http://bqk.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://fgp.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://dxo.chenzaomai.com

[y for x in nested for y in x]
来源：http://sic.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://kqi.yangfankeji.com

max(d, key=d.get)
来源：http://vpc.hnqzz.top

[U10] Py：按值排序字典
来源：http://gxe.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bzw.sxryk.cn

[U11] Py：生成器表达式
来源：http://waq.sxryk.cn

(x * 2 for x in arr)
来源：http://xyx.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tbz.tianlin.xyz

Counter(arr).most_common(3)
来源：http://zbz.shzxlz.cn

[U13] Py：固定长度队列
来源：http://ekb.yj20258888.top

deque(maxlen=10)
来源：http://rfd.guannengcc.top

[U14] Py：分组收集到列表
来源：http://vje.tianlin.xyz

defaultdict(list)
来源：http://hhg.cqqwz.cn

[U15] Py：高精度计时
来源：http://nyr.ydzc1.top

t = time.perf_counter()
来源：http://meb.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://zcy.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wpq.meibo888.top

[U17] Py：初始化日志
来源：http://zay.sweek.top

logging.basicConfig(level=logging.INFO)
来源：http://zvt.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://raa.jianghu66.top

pat = re.compile(r"\d+")
来源：http://ion.gotoacloud.top

[U19] Py：正则替换带回调
来源：http://kdl.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nzn.hysaishi.cn

[U20] Py：缓存函数结果
来源：http://gzm.hesvh.cn

@functools.lru_cache(maxsize=None)
来源：http://cqm.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://kcm.9152youxi.cn

@contextlib.contextmanager
来源：http://kui.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://hmq.bbcook.cn

list(zip(*m))
来源：http://xui.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://buu.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hjx.zhaomingkeji.xyz

[U24] Py：路径操作
来源：http://tuy.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nej.jinqigufen.top

[U25] Py：CSV 按字典读
来源：http://six.sufxvd.cn

csv.DictReader(f)
来源：http://ysr.tianlin.xyz

[U26] Py：并发下载
来源：http://mcy.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eoh.birdmap.top

[U27] Py：异步 HTTP
来源：http://tyc.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://uzq.hammf.cn

[U28] Py：类型别名
来源：http://syl.0kj1m.cn

UserId = int
来源：http://wbe.snrcjt.cn

[U29] Py：属性校验
来源：http://ddy.ydzc1.top

@property 与 @x.setter 配合
来源：http://foq.sjlbkw.cn

[U30] Py：数据类
来源：http://vib.gaohongyu789.top

@dataclass(slots=True)
来源：http://lbd.haohaochexian.top

[U31] Py：单测
来源：http://vjr.andypj.xyz

python -m pytest -q
来源：http://zmi.kuanghao11.cn

[U32] Py：代码格式化
来源：http://svg.9152youxi.cn

ruff format . && ruff check --fix .
来源：http://xqk.jlsjyb.cn

[U33] Py：打包发布
来源：http://vfp.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://rqz.fzhhl.top

[U34] Py：判断编码
来源：http://ive.hesvh.cn

chardet.detect(raw)
来源：http://ymm.tarul.cn

[U35] Py：发送邮件
来源：http://kpi.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mwb.zdbjq.cn

[U36] Py：定时任务
来源：http://aov.yonumen.top

schedule.every(10).minutes.do(job)
来源：http://mry.hongshengwenyu.top

[U37] Py：读写 Excel
来源：http://fak.mhx1999.top

pandas.read_excel / DataFrame.to_excel
来源：http://dbp.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://abv.zhixingplan.top

Path(__file__).resolve().parent
来源：http://vxm.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://drs.jinqigfzy.top

sys.stdout.isatty()
来源：http://yds.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://ket.wangdashe.top

print("err", file=sys.stderr)
来源：http://fxd.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://gli.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tta.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://nhb.tian-w.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xqj.jianghu66.top


<!-- 参考信息 -->