代发 wailian999

x |= (1 << 3);
来源：http://bzk.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://dvq.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tud.jianghu66.top

[S18] C：命令行参数
来源：http://cmg.zhixingplan.top

int main(int argc, char **argv)
来源：http://iep.pengpengdd.cyou

[S19] C：快速排序
来源：http://rpt.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://ozv.vqdsnc.cn

[S20] C：二分查找
来源：http://vto.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kge.zycfv.cn

[S21] C：字符类别判断
来源：http://olj.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://okn.jlsjyb.cn

[S22] C：字符串转数字
来源：http://wys.xziqi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nvf.shzxlz.cn

[S23] C：随机数
来源：http://xze.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yao.zycfv.cn

[S24] C：获取本地时间
来源：http://zuw.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lpn.zdbjq.cn

[S25] C：内存拷贝
来源：http://hyi.andypj.xyz

memcpy(dst, src, n);
来源：http://urn.vqdsnc.cn

[S26] C：内存清零
来源：http://cvz.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://ell.zdqjudy.top

[S27] C：定义常量
来源：http://lnz.jqgfzy.top

const double PI = 3.14159;
来源：http://ejj.ydjk.org.cn

[S28] C：静态变量
来源：http://cxe.sufxvd.cn

static int counter = 0;
来源：http://mkz.xziqi.cn

[S29] C：变参函数
来源：http://mrr.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nch.ehwqpu.com

[S30] C：头文件保护
来源：http://vgu.yueranfly.top

#ifndef X_H
来源：http://yjd.yuanzhike.top

#define X_H
来源：http://eqf.dashuyun.cn

#endif
来源：http://flz.jiagoushi.top

[S31] C++：Hello World
来源：http://apj.xuetiantiany.cn

#include <iostream>
来源：http://yiw.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://gng.xziqi.cn

[S32] C++：字符串
来源：http://xoy.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://clk.hywenlv.cn

[S33] C++：vector 增删
来源：http://flm.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjl.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://hml.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://pvo.hammf.cn

[S35] C++：map
来源：http://uwz.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://frq.yvedp.cn

[S36] C++：unordered_map
来源：http://xrj.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://muy.9152youxi.cn

[S37] C++：set
来源：http://xod.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sek.yfazqb.com

[S38] C++：排序
来源：http://qpo.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://wtb.havefunace.top

[S39] C++：自定义比较器排序
来源：http://xbj.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qve.52xcode.cn

[S40] C++：查找元素
来源：http://jlg.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xev.hammf.cn

[S41] C++：类与构造函数
来源：http://lqy.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ypo.sxryk.cn

[S42] C++：继承与虚函数
来源：http://sgt.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://zhe.zhoulong.xyz

[S43] C++：智能指针
来源：http://kpe.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://onh.cashguo.top

[S44] C++：引用传参
来源：http://sru.fengsongda.top

void inc(int &x) { ++x; }
来源：http://mwy.shzxlz.cn

[S45] C++：lambda
来源：http://ozj.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://jks.yj20258888.top

[S46] C++：函数模板
来源：http://gky.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://efs.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://brr.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aic.yj20258.top

[S48] C++：逐行读文件
来源：http://goh.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://qfz.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://dhm.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://avu.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qzu.daxiang520.top

[S50] C++：格式化数字
来源：http://haj.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hgf.0kj1m.cn

[S51] C++：显式类型转换
来源：http://tak.yuxming.cn

static_cast<double>(a) / b
来源：http://nip.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://kll.meibo888.top

int size() const noexcept { return n_; }
来源：http://jbq.316326.xyz

[S53] C++：移动语义
来源：http://dda.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://tmn.yonumen.top

[S54] C++：异常处理
来源：http://dys.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xxr.birdmap.top

[S55] C++：结构化绑定
来源：http://bbd.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wko.shangyingyoupin.top

[S56] C++：optional
来源：http://wen.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iug.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://fyy.hysaishi.cn

constexpr int N = 10;
来源：http://kaj.vehdjk.com

[S58] C++：命名空间
来源：http://qms.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://kzb.gaohongyu789.top

[S59] C++：静态断言
来源：http://bca.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tnq.tarul.cn

[S60] C++：遍历并删除元素
来源：http://lhb.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pom.yj202588.top

================================================================================
来源：http://ich.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uur.yangfankeji.com

================================================================================
来源：http://mqq.yvedp.cn

[T01] Kotlin：Hello World
来源：http://ylt.zhiwuduotai.top

println("Hello")
来源：http://wir.hfpthk.cn

[T02] Kotlin：变量
来源：http://rkk.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tbh.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://zow.cheryme.top

"值: $b"
来源：http://fyb.ivvv.top

[T04] Kotlin：空安全
来源：http://zqj.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://xng.yj202588.top

[T05] Kotlin：when 表达式
来源：http://uvx.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rdt.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://hwk.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fle.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://gda.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dsp.daria6918.cn

[T08] Kotlin：数据类
来源：http://fce.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://ulr.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://dyn.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://hvf.ydzc1.top

[T10] Kotlin：默认参数
来源：http://ybi.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lvo.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://mdn.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mjd.tian-w.cn

[T12] Kotlin：解构声明
来源：http://qjp.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://kgl.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://yah.sysykeji.top

val m = mapOf("a" to 1)
来源：http://xjz.xziqi.cn

[T14] Kotlin：循环
来源：http://rlu.gzhubu.top

for (i in 1..10) println(i)
来源：http://qjd.sjlbkw.cn

[T15] Kotlin：接口
来源：http://pmn.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://fqo.andypj.xyz

[T16] Swift：Hello World
来源：http://yjr.hcnkem.com

print("Hello")
来源：http://rbe.uphjek.com

[T17] Swift：变量与常量
来源：http://wwd.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://igj.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://acb.ybcxt.top

"值: \(b)"
来源：http://tiz.sxryk.cn

[T19] Swift：可选绑定
来源：http://czf.ehwqpu.com

if let n = opt { print(n) }
来源：http://jgd.sweek.top

[T20] Swift：数组操作
来源：http://gmd.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sqn.yuxming.cn

[T21] Swift：遍历
来源：http://lny.cdnleiting.top

for x in a { print(x) }
来源：http://ryp.cheryme.top

[T22] Swift：字典
来源：http://wyi.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kfk.aibaodan.cn

[T23] Swift：函数
来源：http://ncz.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wje.redwolf501.top

[T24] Swift：闭包
来源：http://yhf.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cbk.havefunace.top

[T25] Swift：结构体
来源：http://hwi.9152youxi.cn

struct P { var x: Int }
来源：http://mqn.hesvh.cn

[T26] Swift：类与重写
来源：http://xiv.hysaishi.cn

class A: Base { override func f() {} }
来源：http://lvs.vqdsnc.cn

[T27] Swift：错误处理
来源：http://clq.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://ubd.yueranfly.top

[T28] Swift：枚举
来源：http://eqz.ctjpmb.com

enum Color { case red, green }
来源：http://gcd.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://awn.jqgfzy.top

guard let x = opt else { return }
来源：http://chp.andypj.xyz

[T30] Swift：协议
来源：http://bap.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://tgv.hysaishi.cn

[T31] Lua：Hello World
来源：http://vpy.tarul.cn

print("Hello")
来源：http://xvu.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://nof.tian-w.cn

local a = 1
来源：http://fvd.hcnkem.com

[T33] Lua：表（数组）
来源：http://zxz.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ubg.cheryme.top

[T34] Lua：遍历表
来源：http://zvj.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://xhm.sxryk.cn

[T35] Lua：字典表
来源：http://obt.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://jcp.cashguo.top

[T36] Lua：函数
来源：http://vkm.zhengqikj.top

function add(a, b) return a + b end
来源：http://ofb.shuidangran.top

[T37] Lua：字符串拼接
来源：http://uko.wangshuangyany.cn

"a" .. "b"
来源：http://grj.yj20258.top

[T38] Lua：条件
来源：http://bgq.daxiang520.top

if x > 0 then print("正") end
来源：http://nll.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://ojy.pengpengdd.cyou

string.find(s, "%d+")
来源：http://lnl.quarkkingdee.top

[T40] Lua：元表
来源：http://gdy.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://ijn.zdbjq.cn

[T41] Perl：Hello World
来源：http://dkp.kuanghao11.cn

print "Hello\n";
来源：http://bal.9152youxi.cn

[T42] Perl：变量类型
来源：http://ogc.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vzz.yuxming.cn

[T43] Perl：字符串插值
来源：http://kaf.xingfuxueyuan.xyz

"值: $a"
来源：http://hlu.xuanzx.com

[T44] Perl：条件
来源：http://url.uphjek.com

if ($a > 0) { print "正"; }
来源：http://hkw.uphjek.com

[T45] Perl：数组遍历
来源：http://ltv.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://abo.snrcjt.cn

[T46] Perl：哈希操作
来源：http://crp.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vno.daxiang520.top

[T47] Perl：正则捕获
来源：http://mqb.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibh.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://tep.havefunace.top

$s =~ s/old/new/g;
来源：http://jyw.jianghu66.top

[T49] Perl：函数
来源：http://yae.jinyuanbaomall.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ddy.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://fdl.wangshuangyany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oql.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://awr.jqgfzy.top

[T51] Scala：Hello World
来源：http://rll.9152youxi.cn

println("Hello")
来源：http://yph.hnxiangtu.top

[T52] Scala：变量
来源：http://nxc.ehwqpu.com

val a = 1;  var b = 2
来源：http://chm.yvedp.cn

[T53] Scala：字符串插值
来源：http://but.jinqigufen.top

s"值: $b"
来源：http://sxj.dianchejie.cn

[T54] Scala：集合映射
来源：http://qzr.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://ixe.yj20258888.top

[T55] Scala：集合过滤
来源：http://gxe.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://dcr.hfpthk.cn

[T56] Scala：样例类
来源：http://ssj.fktsv.cn

case class User(name: String, age: Int)
来源：http://kfk.havefunace.top

[T57] Scala：模式匹配
来源：http://bvh.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vhx.ydzc1.top

[T58] Scala：函数定义
来源：http://uhp.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://fgv.ivvv.top

[T59] Scala：循环
来源：http://mym.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://udy.hysaishi.cn

[T60] Scala：折叠
来源：http://qfj.xingfuxueyuan.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://myb.hysaishi.cn

================================================================================
来源：http://zlu.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gkq.xylfe.cn

================================================================================
来源：http://pae.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://npv.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nvd.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://qdf.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mwo.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://yjq.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://itr.yuxming.cn

[U04] Py：变量调试打印
来源：http://ior.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zlq.gzhubu.top

[U05] Py：列表去重且保序
来源：http://sad.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://fat.xuanzx.com

[U06] Py：合并两个字典
来源：http://sqd.guannengcc.top

{**a, **b}
来源：http://qbt.52xcode.cn

[U07] Py：反转字典键值
来源：http://toj.meibo888.top

{v: k for k, v in d.items()}
来源：http://wyy.hammf.cn

[U08] Py：展平二维列表
来源：http://xqg.52xcode.cn

[y for x in nested for y in x]
来源：http://qtz.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://wum.sxryk.cn

max(d, key=d.get)
来源：http://epu.aibaodan.cn

[U10] Py：按值排序字典
来源：http://iuq.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sne.ppjwa.cn

[U11] Py：生成器表达式
来源：http://ffl.ppjwa.cn

(x * 2 for x in arr)
来源：http://afr.aizwys.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qbf.gogol.net.cn

Counter(arr).most_common(3)
来源：http://bcd.sysykeji.top

[U13] Py：固定长度队列
来源：http://fes.svipenyu.cn

deque(maxlen=10)
来源：http://rgj.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://cru.sysykeji.top

defaultdict(list)
来源：http://jdn.zhixingplan.top

[U15] Py：高精度计时
来源：http://alt.yuanzhike.top

t = time.perf_counter()
来源：http://als.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://irn.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nnd.xingfuxueyuan.xyz

[U17] Py：初始化日志
来源：http://pun.havefunace.top

logging.basicConfig(level=logging.INFO)
来源：http://pmw.snrcjt.cn

[U18] Py：预编译正则
来源：http://lsn.yfazqb.com

pat = re.compile(r"\d+")
来源：http://qgc.fehbvm.com

[U19] Py：正则替换带回调
来源：http://tjt.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ysx.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://jze.andypj.xyz

@functools.lru_cache(maxsize=None)
来源：http://qac.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://kwv.yj20258888.top

@contextlib.contextmanager
来源：http://mmu.52xcode.cn

[U22] Py：矩阵转置
来源：http://kjt.zhaomingkeji.xyz

list(zip(*m))
来源：http://ojc.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://qoe.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vlg.yangfankeji.com

[U24] Py：路径操作
来源：http://rqv.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://imr.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://fkm.meibo888.top

csv.DictReader(f)
来源：http://inj.jyoumei.cn

[U26] Py：并发下载
来源：http://pjw.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vcj.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://uvv.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://dxw.iojbl.cn

[U28] Py：类型别名
来源：http://gmi.yonumen.top

UserId = int
来源：http://gnt.zhoulong.xyz

[U29] Py：属性校验
来源：http://koq.zycfv.cn

@property 与 @x.setter 配合
来源：http://hmk.yuanzhike.top

[U30] Py：数据类
来源：http://ekf.zdqjudy.top

@dataclass(slots=True)
来源：http://dss.hywenlv.cn

[U31] Py：单测
来源：http://pmc.hywenlv.cn

python -m pytest -q
来源：http://jup.cashguo.top

[U32] Py：代码格式化
来源：http://mts.wangdashe.top

ruff format . && ruff check --fix .
来源：http://okk.guannengcc.top

[U33] Py：打包发布
来源：http://lvm.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://wme.tarul.cn

[U34] Py：判断编码
来源：http://vwi.hongshengwenyu.top

chardet.detect(raw)
来源：http://bpu.shuidangran.top

[U35] Py：发送邮件
来源：http://dbd.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://alj.tianlin.xyz

[U36] Py：定时任务
来源：http://lbd.sweek.top

schedule.every(10).minutes.do(job)
来源：http://vdt.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://upm.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://hxd.tanke756.top

[U38] Py：获取脚本所在目录
来源：http://oqf.hysaishi.cn

Path(__file__).resolve().parent
来源：http://ejw.0kj1m.cn

[U39] Py：判断是否在交互环境
来源：http://wsx.shanyushiyangtech.top

sys.stdout.isatty()
来源：http://ntf.yj20258.top

[U40] Py：打印到标准错误
来源：http://vkq.xuanzx.com

print("err", file=sys.stderr)
来源：http://jsa.ywan-chungtsiang.top


<!-- 参考信息 -->