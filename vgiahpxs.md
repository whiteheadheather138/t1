代发 wailian999

int main(int argc, char **argv)
来源：http://akk.tianlin.xyz

[S19] C：快速排序
来源：http://etn.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://cpw.yongpay.top

[S20] C：二分查找
来源：http://wym.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dev.c1oappe.top

[S21] C：字符类别判断
来源：http://xmx.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cig.shuidangran.top

[S22] C：字符串转数字
来源：http://hjn.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://gre.ctjpmb.com

[S23] C：随机数
来源：http://bjw.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yvy.ehwqpu.com

[S24] C：获取本地时间
来源：http://dct.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aug.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://bvr.kuanghao11.cn

memcpy(dst, src, n);
来源：http://mej.zhiwuduotai.top

[S26] C：内存清零
来源：http://gan.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://xli.gotoacloud.top

[S27] C：定义常量
来源：http://sne.zhiwuduotai.top

const double PI = 3.14159;
来源：http://rvl.nanxuanxn.top

[S28] C：静态变量
来源：http://ymk.zhengqikj.top

static int counter = 0;
来源：http://mhw.hfpthk.cn

[S29] C：变参函数
来源：http://fgt.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cfj.nwbrower.top

[S30] C：头文件保护
来源：http://uun.smart0.xyz

#ifndef X_H
来源：http://eww.wangshuangyany.cn

#define X_H
来源：http://pdc.shuidangran.top

#endif
来源：http://vaq.pengpengdd.cyou

[S31] C++：Hello World
来源：http://wjm.daxiang520.top

#include <iostream>
来源：http://hlf.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://jkg.havefunace.top

[S32] C++：字符串
来源：http://wbz.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://fqy.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://bfv.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zoj.aibaodan.cn

[S34] C++：遍历 vector
来源：http://ecp.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://zeo.xingfuxueyuan.xyz

[S35] C++：map
来源：http://zbv.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uip.yj202588.top

[S36] C++：unordered_map
来源：http://cqe.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qzk.nanxuanxn.top

[S37] C++：set
来源：http://cca.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eeq.hongshengwenyu.top

[S38] C++：排序
来源：http://upw.birdmap.top

std::sort(v.begin(), v.end());
来源：http://xcs.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://ptx.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qbr.sufxvd.cn

[S40] C++：查找元素
来源：http://cgb.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vqr.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://hsu.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pae.tanke756.top

[S42] C++：继承与虚函数
来源：http://mwm.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://nwt.ctjpmb.com

[S43] C++：智能指针
来源：http://lut.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://oqe.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://cuv.yj20258888.top

void inc(int &x) { ++x; }
来源：http://fkh.c1oappe.top

[S45] C++：lambda
来源：http://hvl.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qbs.bbcook.cn

[S46] C++：函数模板
来源：http://opx.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yav.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://ceg.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xgj.ydzc1.top

[S48] C++：逐行读文件
来源：http://cnl.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://dun.smart0.xyz

while (std::getline(in, line)) { }
来源：http://cmv.jiagoushi.top

[S49] C++：写文件
来源：http://whb.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gdd.guannengcc.top

[S50] C++：格式化数字
来源：http://lka.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rgd.yonumen.top

[S51] C++：显式类型转换
来源：http://vlj.yuxming.cn

static_cast<double>(a) / b
来源：http://noz.tanke756.top

[S52] C++：const 与 noexcept
来源：http://qah.mhx1999.top

int size() const noexcept { return n_; }
来源：http://crx.mhx1999.top

[S53] C++：移动语义
来源：http://fbd.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://mdu.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://gxo.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dxk.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://yaz.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rpq.vehdjk.com

[S56] C++：optional
来源：http://htc.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ktk.sweek.top

[S57] C++：编译期常量
来源：http://npl.yueranfly.top

constexpr int N = 10;
来源：http://tmy.uphjek.com

[S58] C++：命名空间
来源：http://rdk.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://udb.cashguo.top

[S59] C++：静态断言
来源：http://orq.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yom.tanke756.top

[S60] C++：遍历并删除元素
来源：http://twg.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ohm.wangdashe.top

================================================================================
来源：http://pqq.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gov.yanxiufei.cn

================================================================================
来源：http://yqm.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://jcl.yuanzhike.top

println("Hello")
来源：http://kux.jqgfzy.top

[T02] Kotlin：变量
来源：http://sxk.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mrx.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://owr.iojbl.cn

"值: $b"
来源：http://gyu.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://flr.9152youxi.cn

val n: String? = null;  n?.length
来源：http://nzt.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://mqy.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hbn.smart0.xyz

[T06] Kotlin：集合映射
来源：http://pvz.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hfc.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://yow.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://suq.yangfankeji.com

[T08] Kotlin：数据类
来源：http://fzj.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://ofd.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://fpl.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://oum.havefunace.top

[T10] Kotlin：默认参数
来源：http://gxv.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://pwu.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://ehz.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://uqu.havefunace.top

[T12] Kotlin：解构声明
来源：http://div.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://hux.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://iwq.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://iqs.snrcjt.cn

[T14] Kotlin：循环
来源：http://znx.zhixingplan.top

for (i in 1..10) println(i)
来源：http://yrg.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://aug.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://daj.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://ewc.sjlbkw.cn

print("Hello")
来源：http://aqn.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://zhu.yangfankeji.com

var a = 1;  let b = 2
来源：http://ooo.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://zlp.pengpengdd.cyou

"值: \(b)"
来源：http://hoa.bbcook.cn

[T19] Swift：可选绑定
来源：http://wiv.vehdjk.com

if let n = opt { print(n) }
来源：http://mqc.yvedp.cn

[T20] Swift：数组操作
来源：http://nsd.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://vql.shangyingyoupin.top

[T21] Swift：遍历
来源：http://jcn.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://jho.quarkkingdee.top

[T22] Swift：字典
来源：http://vhk.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://rwl.52xcode.cn

[T23] Swift：函数
来源：http://jws.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tee.cashguo.top

[T24] Swift：闭包
来源：http://jit.ywan-chungtsiang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xew.xuetiantiany.cn

[T25] Swift：结构体
来源：http://zfh.0kj1m.cn

struct P { var x: Int }
来源：http://cvu.zycfv.cn

[T26] Swift：类与重写
来源：http://xxk.yongpay.top

class A: Base { override func f() {} }
来源：http://gfb.jqgufenzy.top

[T27] Swift：错误处理
来源：http://bav.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://pnv.jianghu66.top

[T28] Swift：枚举
来源：http://qna.zhixingplan.top

enum Color { case red, green }
来源：http://xhl.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://pkb.jinqigfzy.top

guard let x = opt else { return }
来源：http://hpb.zhijiandao.cn

[T30] Swift：协议
来源：http://ncq.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://zyk.epnwcf.com

[T31] Lua：Hello World
来源：http://msn.zhengqikj.top

print("Hello")
来源：http://fxl.c1oappe.top

[T32] Lua：局部变量
来源：http://cqz.jinqigufen.top

local a = 1
来源：http://slq.iojbl.cn

[T33] Lua：表（数组）
来源：http://xhj.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bwj.cashguo.top

[T34] Lua：遍历表
来源：http://uqb.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://umx.yongpay.top

[T35] Lua：字典表
来源：http://hsw.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://bhy.zycfv.cn

[T36] Lua：函数
来源：http://lgi.c1oappe.top

function add(a, b) return a + b end
来源：http://rtr.hcnkem.com

[T37] Lua：字符串拼接
来源：http://xri.pycfn.com

"a" .. "b"
来源：http://kvt.fktsv.cn

[T38] Lua：条件
来源：http://sac.sweek.top

if x > 0 then print("正") end
来源：http://lok.jiagoushi.top

[T39] Lua：模式匹配
来源：http://ave.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://pvf.jyoumei.cn

[T40] Lua：元表
来源：http://zsz.52xcode.cn

setmetatable({}, { __index = base })
来源：http://yiw.jlsjyb.cn

[T41] Perl：Hello World
来源：http://vvu.xingfuxueyuan.xyz

print "Hello\n";
来源：http://zbc.svipenyu.cn

[T42] Perl：变量类型
来源：http://lkw.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xbq.hnqzz.top

[T43] Perl：字符串插值
来源：http://rih.sxryk.cn

"值: $a"
来源：http://fjh.ybcxt.top

[T44] Perl：条件
来源：http://grr.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://uqn.sweek.top

[T45] Perl：数组遍历
来源：http://uks.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://uyx.yongpay.top

[T46] Perl：哈希操作
来源：http://llk.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uje.yvedp.cn

[T47] Perl：正则捕获
来源：http://hvk.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rvj.guowangkeji.top

[T48] Perl：正则替换
来源：http://gzx.ppjwa.cn

$s =~ s/old/new/g;
来源：http://nth.ivvv.top

[T49] Perl：函数
来源：http://sci.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mqh.gzhubu.top

[T50] Perl：逐行读文件
来源：http://pgh.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ane.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://xww.meibo888.top

[T51] Scala：Hello World
来源：http://ulb.shanyushiyangkeji.top

println("Hello")
来源：http://fbn.jinqigfzy.top

[T52] Scala：变量
来源：http://tbe.guannengcc.top

val a = 1;  var b = 2
来源：http://zow.chenzaomai.com

[T53] Scala：字符串插值
来源：http://cpz.bbcook.cn

s"值: $b"
来源：http://nvx.xinyue.icu

[T54] Scala：集合映射
来源：http://qpk.hcnkem.com

List(1, 2, 3).map(_ * 2)
来源：http://mms.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://aps.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://fxd.snrcjt.cn

[T56] Scala：样例类
来源：http://zyu.bbcook.cn

case class User(name: String, age: Int)
来源：http://uui.hfpthk.cn

[T57] Scala：模式匹配
来源：http://wtd.fktsv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hov.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://oxn.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://oct.redwolf501.top

[T59] Scala：循环
来源：http://moh.sweek.top

for (i <- 1 to 10) println(i)
来源：http://dur.kuanghao11.cn

[T60] Scala：折叠
来源：http://ffs.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lkr.daxiang520.top

================================================================================
来源：http://qtt.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fwr.sjlbkw.cn

================================================================================
来源：http://ohi.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://eyk.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qqx.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://xcr.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hlg.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://hdo.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://dul.tianlin.xyz

[U04] Py：变量调试打印
来源：http://ppc.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ivl.birdmap.top

[U05] Py：列表去重且保序
来源：http://kiy.fengsongda.top

list(dict.fromkeys(arr))
来源：http://gzn.gotoacloud.top

[U06] Py：合并两个字典
来源：http://cja.shanyushiyangtech.top

{**a, **b}
来源：http://nba.cucudq.cn

[U07] Py：反转字典键值
来源：http://ekg.yj20258888.top

{v: k for k, v in d.items()}
来源：http://gil.cdnleiting.top

[U08] Py：展平二维列表
来源：http://yho.aibaodan.cn

[y for x in nested for y in x]
来源：http://aaf.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://ymb.yonumen.top

max(d, key=d.get)
来源：http://zov.52xcode.cn

[U10] Py：按值排序字典
来源：http://nxs.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gjt.svipenyu.cn

[U11] Py：生成器表达式
来源：http://jky.jinqigufen.top

(x * 2 for x in arr)
来源：http://iui.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xyk.iojbl.cn

Counter(arr).most_common(3)
来源：http://lqk.snrcjt.cn

[U13] Py：固定长度队列
来源：http://qxl.cheryme.top

deque(maxlen=10)
来源：http://dhs.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://gln.ivvv.top

defaultdict(list)
来源：http://wtx.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://aiy.zhijiandao.cn

t = time.perf_counter()
来源：http://gza.tarul.cn

[U16] Py：命令行参数解析
来源：http://epx.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ydy.zhengqikj.top

[U17] Py：初始化日志
来源：http://rog.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://fww.epnwcf.com

[U18] Py：预编译正则
来源：http://qdq.meibo888.top

pat = re.compile(r"\d+")
来源：http://oiw.yj20258888.top

[U19] Py：正则替换带回调
来源：http://ioz.bbcook.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zyi.tarul.cn

[U20] Py：缓存函数结果
来源：http://mst.yj20258.top

@functools.lru_cache(maxsize=None)
来源：http://eky.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://ywq.yj202588.top

@contextlib.contextmanager
来源：http://gtz.wangdashe.top

[U22] Py：矩阵转置
来源：http://cyz.vqdsnc.cn

list(zip(*m))
来源：http://kns.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://vke.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yqy.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://ztt.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bga.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://xrp.sjlbkw.cn

csv.DictReader(f)
来源：http://vgk.hnxiangtu.top

[U26] Py：并发下载
来源：http://hau.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kqi.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://dsp.jinqigfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://lir.9152youxi.cn

[U28] Py：类型别名
来源：http://lff.yuanzhike.top

UserId = int
来源：http://sos.ivvv.top

[U29] Py：属性校验
来源：http://vqx.daria6918.cn

@property 与 @x.setter 配合
来源：http://bdj.hysaishi.cn

[U30] Py：数据类
来源：http://vxr.tianlin.xyz

@dataclass(slots=True)
来源：http://rfc.vehdjk.com

[U31] Py：单测
来源：http://uac.jinyuanbaomall.cn

python -m pytest -q
来源：http://yme.guannengcc.top

[U32] Py：代码格式化
来源：http://bfv.bjfxy.top

ruff format . && ruff check --fix .
来源：http://npc.xylfe.cn

[U33] Py：打包发布
来源：http://rcy.feifeiyinyue.top

python -m build  （依赖 pyproject.toml）
来源：http://llk.hysaishi.cn

[U34] Py：判断编码
来源：http://zaw.kuanghao11.cn

chardet.detect(raw)
来源：http://ceo.0kj1m.cn

[U35] Py：发送邮件
来源：http://vlp.hnxiangtu.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rqz.pycfn.com

[U36] Py：定时任务
来源：http://ive.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://cbh.shuidangran.top

[U37] Py：读写 Excel
来源：http://qhg.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://itx.cashguo.top

[U38] Py：获取脚本所在目录
来源：http://ftc.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://ssi.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://cyf.fktsv.cn

sys.stdout.isatty()
来源：http://evv.aizwys.cn

[U40] Py：打印到标准错误
来源：http://zcj.havefunace.top

print("err", file=sys.stderr)
来源：http://vat.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://wro.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mzb.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://nwx.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cno.ivvv.top


<!-- 参考信息 -->