代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nqy.hysaishi.cn

[S21] C：字符类别判断
来源：http://smw.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bln.uphjek.com

[S22] C：字符串转数字
来源：http://pjc.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ulh.svipenyu.cn

[S23] C：随机数
来源：http://tff.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eyc.mhx1999.top

[S24] C：获取本地时间
来源：http://vtv.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vrp.yj202588.top

[S25] C：内存拷贝
来源：http://zhr.yanxiufei.cn

memcpy(dst, src, n);
来源：http://dxj.mhx1999.top

[S26] C：内存清零
来源：http://gqt.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://nqj.dashuyun.cn

[S27] C：定义常量
来源：http://usa.havefunace.top

const double PI = 3.14159;
来源：http://kdi.zdqjudy.top

[S28] C：静态变量
来源：http://qng.sweek.top

static int counter = 0;
来源：http://xpd.feifeiyinyue.top

[S29] C：变参函数
来源：http://sbv.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://swr.uphjek.com

[S30] C：头文件保护
来源：http://vzw.jiagoushi.top

#ifndef X_H
来源：http://ych.jyoumei.cn

#define X_H
来源：http://rjt.hfpthk.cn

#endif
来源：http://ycc.zhiwuduotai.top

[S31] C++：Hello World
来源：http://epb.jqgufenzy.top

#include <iostream>
来源：http://mgf.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://gfi.gaohongyu789.top

[S32] C++：字符串
来源：http://vsx.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://sjn.ctjpmb.com

[S33] C++：vector 增删
来源：http://udk.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wfe.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://wyt.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://zug.jinqigufen.top

[S35] C++：map
来源：http://mhx.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wdw.mhx1999.top

[S36] C++：unordered_map
来源：http://eqq.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dmu.9152youxi.cn

[S37] C++：set
来源：http://gvs.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mdm.feifeiyinyue.top

[S38] C++：排序
来源：http://jji.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://lst.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://ufe.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qpm.zhixingplan.top

[S40] C++：查找元素
来源：http://bzt.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oco.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://dwf.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jud.havefunace.top

[S42] C++：继承与虚函数
来源：http://isq.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://jvq.sysykeji.top

[S43] C++：智能指针
来源：http://jof.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://lkd.ctjpmb.com

[S44] C++：引用传参
来源：http://vmu.fktsv.cn

void inc(int &x) { ++x; }
来源：http://nea.uphjek.com

[S45] C++：lambda
来源：http://tun.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://gph.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://eub.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rau.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://mfw.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lyx.hesvh.cn

[S48] C++：逐行读文件
来源：http://cph.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://rnb.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://bjq.ehwqpu.com

[S49] C++：写文件
来源：http://imh.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ati.c1oappe.top

[S50] C++：格式化数字
来源：http://evz.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hcd.bjfxy.top

[S51] C++：显式类型转换
来源：http://sho.zhongyouzk.top

static_cast<double>(a) / b
来源：http://yxs.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://fdg.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://qni.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://bjc.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://tjr.hfpthk.cn

[S54] C++：异常处理
来源：http://uiq.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qep.ybcxt.top

[S55] C++：结构化绑定
来源：http://kqs.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wny.epnwcf.com

[S56] C++：optional
来源：http://gjs.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jue.sufxvd.cn

[S57] C++：编译期常量
来源：http://ayl.cdnleiting.top

constexpr int N = 10;
来源：http://rrc.yueranfly.top

[S58] C++：命名空间
来源：http://wvx.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://njv.hfpthk.cn

[S59] C++：静态断言
来源：http://zvf.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eve.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://wox.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zpx.fengsongda.top

================================================================================
来源：http://kdf.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fjd.jinqigufen.top

================================================================================
来源：http://wud.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://fqc.zhijiandao.cn

println("Hello")
来源：http://zab.yangfankeji.com

[T02] Kotlin：变量
来源：http://xzf.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://plt.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://etf.zhijiandao.cn

"值: $b"
来源：http://srq.yvedp.cn

[T04] Kotlin：空安全
来源：http://dte.uphjek.com

val n: String? = null;  n?.length
来源：http://ufn.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://amo.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmd.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://xag.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rvb.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://anx.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://may.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://pio.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://yss.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://yeb.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://bbg.yj202588.top

[T10] Kotlin：默认参数
来源：http://oqj.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wwf.c1oappe.top

[T11] Kotlin：协程
来源：http://ugm.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://pju.meibo888.top

[T12] Kotlin：解构声明
来源：http://faz.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://ewu.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://cte.xuanzx.com

val m = mapOf("a" to 1)
来源：http://rcl.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://rwy.shuidangran.top

for (i in 1..10) println(i)
来源：http://cwz.sxryk.cn

[T15] Kotlin：接口
来源：http://wwq.xylfe.cn

interface Shape { fun area(): Double }
来源：http://ikq.hfpthk.cn

[T16] Swift：Hello World
来源：http://bqx.jyoumei.cn

print("Hello")
来源：http://aok.sxryk.cn

[T17] Swift：变量与常量
来源：http://ufh.sufxvd.cn

var a = 1;  let b = 2
来源：http://xfb.0kj1m.cn

[T18] Swift：字符串插值
来源：http://oli.hcnkem.com

"值: \(b)"
来源：http://vpg.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://xur.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://gix.tian-w.cn

[T20] Swift：数组操作
来源：http://edj.jqgufenzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://pip.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://bxy.aizwys.cn

for x in a { print(x) }
来源：http://rci.nanxuanxn.top

[T22] Swift：字典
来源：http://jxg.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://cpo.havefunace.top

[T23] Swift：函数
来源：http://shm.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gdq.c1oappe.top

[T24] Swift：闭包
来源：http://poi.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://avt.pengpengdd.cyou

[T25] Swift：结构体
来源：http://cox.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://qjl.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://fyd.pycfn.com

class A: Base { override func f() {} }
来源：http://lbl.epnwcf.com

[T27] Swift：错误处理
来源：http://nra.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://lzj.ydzc1.top

[T28] Swift：枚举
来源：http://pni.jianghu66.top

enum Color { case red, green }
来源：http://xqo.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://biy.iojbl.cn

guard let x = opt else { return }
来源：http://hmf.316326.xyz

[T30] Swift：协议
来源：http://lxv.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://wbf.gogol.net.cn

[T31] Lua：Hello World
来源：http://cdr.wangshuangyany.cn

print("Hello")
来源：http://pyt.meibo888.top

[T32] Lua：局部变量
来源：http://abl.fehbvm.com

local a = 1
来源：http://eqc.xziqi.cn

[T33] Lua：表（数组）
来源：http://gmb.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mgp.xuanzx.com

[T34] Lua：遍历表
来源：http://qwc.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tpd.zhixingplan.top

[T35] Lua：字典表
来源：http://enz.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://pfe.xuetiantiany.cn

[T36] Lua：函数
来源：http://ymn.cdnleiting.top

function add(a, b) return a + b end
来源：http://hpy.vehdjk.com

[T37] Lua：字符串拼接
来源：http://yui.9152youxi.cn

"a" .. "b"
来源：http://ytb.gzhubu.top

[T38] Lua：条件
来源：http://emp.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://apx.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://mcc.ctjpmb.com

string.find(s, "%d+")
来源：http://biq.tarul.cn

[T40] Lua：元表
来源：http://ums.epnwcf.com

setmetatable({}, { __index = base })
来源：http://bcw.jyoumei.cn

[T41] Perl：Hello World
来源：http://jal.ivvv.top

print "Hello\n";
来源：http://oto.yj20258.top

[T42] Perl：变量类型
来源：http://nzg.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://omr.gotoacloud.top

[T43] Perl：字符串插值
来源：http://bmt.jqgufenzy.top

"值: $a"
来源：http://ava.zhixingplan.top

[T44] Perl：条件
来源：http://fpi.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://qyc.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://ofp.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://rub.andypj.xyz

[T46] Perl：哈希操作
来源：http://tmz.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ykj.tianlin.xyz

[T47] Perl：正则捕获
来源：http://jwq.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zid.zhixingplan.top

[T48] Perl：正则替换
来源：http://ilb.hywenlv.cn

$s =~ s/old/new/g;
来源：http://fea.birdmap.top

[T49] Perl：函数
来源：http://sbz.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xxe.hesvh.cn

[T50] Perl：逐行读文件
来源：http://csd.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://amw.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://hdg.haohaochexian.top

[T51] Scala：Hello World
来源：http://drk.yfazqb.com

println("Hello")
来源：http://ycr.xinyue.icu

[T52] Scala：变量
来源：http://wex.ehwqpu.com

val a = 1;  var b = 2
来源：http://dzp.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://mby.fanxiaobao.xyz

s"值: $b"
来源：http://fir.ydjk.org.cn

[T54] Scala：集合映射
来源：http://gst.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://tqf.gotoacloud.top

[T55] Scala：集合过滤
来源：http://bqw.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://jry.chenjidiqi.icu

[T56] Scala：样例类
来源：http://pso.shzxlz.cn

case class User(name: String, age: Int)
来源：http://fzt.havefunace.top

[T57] Scala：模式匹配
来源：http://oli.bbcook.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gdi.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://qtc.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kbj.iojbl.cn

[T59] Scala：循环
来源：http://kct.gotoacloud.top

for (i <- 1 to 10) println(i)
来源：http://dxo.gotoacloud.top

[T60] Scala：折叠
来源：http://bcb.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ohh.tianlin.xyz

================================================================================
来源：http://gqr.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yfq.snrcjt.cn

================================================================================
来源：http://lte.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://nlx.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://blx.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://bvp.fzhhl.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mnl.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://uhd.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://sfw.sweek.top

[U04] Py：变量调试打印
来源：http://lek.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kui.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://ral.zhengqikj.top

list(dict.fromkeys(arr))
来源：http://uci.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://ebl.ivvv.top

{**a, **b}
来源：http://ddd.tian-w.cn

[U07] Py：反转字典键值
来源：http://gxs.ctjpmb.com

{v: k for k, v in d.items()}
来源：http://obl.yfazqb.com

[U08] Py：展平二维列表
来源：http://grf.fktsv.cn

[y for x in nested for y in x]
来源：http://zoj.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://inl.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://vtd.cqqwz.cn

[U10] Py：按值排序字典
来源：http://xon.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mze.chenlongwang.top

[U11] Py：生成器表达式
来源：http://wlv.svipenyu.cn

(x * 2 for x in arr)
来源：http://stp.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ule.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://urf.dashuyun.cn

[U13] Py：固定长度队列
来源：http://xgg.gogol.net.cn

deque(maxlen=10)
来源：http://pio.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://mva.cdnleiting.top

defaultdict(list)
来源：http://itw.hnxiangtu.top

[U15] Py：高精度计时
来源：http://lxe.ydzc1.top

t = time.perf_counter()
来源：http://aqf.jianghu66.top

[U16] Py：命令行参数解析
来源：http://xxx.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://asf.yangfankeji.com

[U17] Py：初始化日志
来源：http://onw.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://xrq.yj20258888.top

[U18] Py：预编译正则
来源：http://zzm.hcnkem.com

pat = re.compile(r"\d+")
来源：http://jzq.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://unp.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tuz.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://fll.mhx1999.top

@functools.lru_cache(maxsize=None)
来源：http://yvk.haohaochexian.top

[U21] Py：自定义上下文管理器
来源：http://jyy.wangshuangyany.cn

@contextlib.contextmanager
来源：http://qfv.yuanzhike.top

[U22] Py：矩阵转置
来源：http://ruy.zdbjq.cn

list(zip(*m))
来源：http://diq.wangdashe.top

[U23] Py：分块读取大文件
来源：http://jxm.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vwm.cucudq.cn

[U24] Py：路径操作
来源：http://ltz.pengpengdd.cyou

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zum.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://okk.redwolf501.top

csv.DictReader(f)
来源：http://pcb.yj202588.top

[U26] Py：并发下载
来源：http://vcr.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fxj.sysykeji.top

[U27] Py：异步 HTTP
来源：http://voj.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://dxf.redwolf501.top

[U28] Py：类型别名
来源：http://jyt.52xcode.cn

UserId = int
来源：http://rbp.xziqi.cn

[U29] Py：属性校验
来源：http://acu.hfpthk.cn

@property 与 @x.setter 配合
来源：http://zkm.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://bvd.xuetiantiany.cn

@dataclass(slots=True)
来源：http://aja.tianlin.xyz

[U31] Py：单测
来源：http://yum.52xcode.cn

python -m pytest -q
来源：http://vij.vqdsnc.cn

[U32] Py：代码格式化
来源：http://wys.fengsongda.top

ruff format . && ruff check --fix .
来源：http://jaw.fanxiaobao.xyz

[U33] Py：打包发布
来源：http://mxd.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://tyb.xylfe.cn

[U34] Py：判断编码
来源：http://bkz.nwbrower.top

chardet.detect(raw)
来源：http://slb.ctjpmb.com

[U35] Py：发送邮件
来源：http://mms.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pxv.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://rbv.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://lig.ehwqpu.com

[U37] Py：读写 Excel
来源：http://trt.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://yug.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://ldd.hesvh.cn

Path(__file__).resolve().parent
来源：http://qlh.snrcjt.cn

[U39] Py：判断是否在交互环境
来源：http://pez.daxiang520.top

sys.stdout.isatty()
来源：http://epu.havefunace.top

[U40] Py：打印到标准错误
来源：http://tjn.tanke756.top

print("err", file=sys.stderr)
来源：http://ybx.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://tca.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://srn.zhongyouzk.top

[U42] PHP：PSR-4 自动加载
来源：http://zed.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wmq.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://ovo.daxiang520.top

namespace App\Http;
来源：http://wvv.daria6918.cn

[U44] PHP：开启严格类型
来源：http://gbe.feifeiyinyue.top

declare(strict_types=1);
来源：http://mxb.9152youxi.cn


<!-- 参考信息 -->