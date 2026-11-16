代发 wailian999

int main(int argc, char **argv)
来源：http://hyx.yj20258888.top

[S19] C：快速排序
来源：http://nbi.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://jha.vehdjk.com

[S20] C：二分查找
来源：http://fpd.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ugl.yfazqb.com

[S21] C：字符类别判断
来源：http://xcd.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qtr.chenzaomai.com

[S22] C：字符串转数字
来源：http://fxz.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://reu.snrcjt.cn

[S23] C：随机数
来源：http://atd.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wxm.zhengqikj.top

[S24] C：获取本地时间
来源：http://jmg.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lrw.hywenlv.cn

[S25] C：内存拷贝
来源：http://wtb.meibo888.top

memcpy(dst, src, n);
来源：http://mge.hfpthk.cn

[S26] C：内存清零
来源：http://rfl.pycfn.com

memset(a, 0, sizeof a);
来源：http://qyc.yj202588.top

[S27] C：定义常量
来源：http://mpj.zycfv.cn

const double PI = 3.14159;
来源：http://bwh.pengpengdd.cyou

[S28] C：静态变量
来源：http://mem.zdqjudy.top

static int counter = 0;
来源：http://klb.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://itt.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://puf.yueranfly.top

[S30] C：头文件保护
来源：http://efr.hywenlv.cn

#ifndef X_H
来源：http://jhd.ppjwa.cn

#define X_H
来源：http://grc.yj202588.top

#endif
来源：http://tlg.redwolf501.top

[S31] C++：Hello World
来源：http://sxr.fzhhl.top

#include <iostream>
来源：http://uin.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://vqn.epnwcf.com

[S32] C++：字符串
来源：http://kzg.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://vtl.daria6918.cn

[S33] C++：vector 增删
来源：http://hsm.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lln.ivvv.top

[S34] C++：遍历 vector
来源：http://btb.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://vkl.chenzaomai.com

[S35] C++：map
来源：http://vyn.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qrl.xylfe.cn

[S36] C++：unordered_map
来源：http://msk.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mrp.nanxuanxn.top

[S37] C++：set
来源：http://qxp.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqz.jyoumei.cn

[S38] C++：排序
来源：http://hko.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://ewe.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://tks.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ihx.vehdjk.com

[S40] C++：查找元素
来源：http://wmn.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ugd.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://yhi.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bvh.ybcxt.top

[S42] C++：继承与虚函数
来源：http://aas.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://kao.ivvv.top

[S43] C++：智能指针
来源：http://jko.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://skf.nanxinkj.top

[S44] C++：引用传参
来源：http://jbc.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://dxa.feifeiyinyue.top

[S45] C++：lambda
来源：http://ldb.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nfw.cucudq.cn

[S46] C++：函数模板
来源：http://zrw.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tox.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://fzd.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hjo.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://rfd.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://iqz.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://qpj.yanxiufei.cn

[S49] C++：写文件
来源：http://fpt.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sbw.fengsongda.top

[S50] C++：格式化数字
来源：http://gnz.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tmf.sufxvd.cn

[S51] C++：显式类型转换
来源：http://axe.nwbrower.top

static_cast<double>(a) / b
来源：http://qhd.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://sao.iojbl.cn

int size() const noexcept { return n_; }
来源：http://dko.jqgufenzy.top

[S53] C++：移动语义
来源：http://zdg.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://yrq.sufxvd.cn

[S54] C++：异常处理
来源：http://qhz.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oel.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://hyo.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jul.svipenyu.cn

[S56] C++：optional
来源：http://sjl.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lyd.0kj1m.cn

[S57] C++：编译期常量
来源：http://goz.0kj1m.cn

constexpr int N = 10;
来源：http://ptn.vqdsnc.cn

[S58] C++：命名空间
来源：http://tht.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://vpb.feifeiyinyue.top

[S59] C++：静态断言
来源：http://cxt.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://djg.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://rvs.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bqs.zdbjq.cn

================================================================================
来源：http://ttx.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mwk.hongshengwenyu.top

================================================================================
来源：http://tit.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://sss.gaohongyu789.top

println("Hello")
来源：http://mzl.yfazqb.com

[T02] Kotlin：变量
来源：http://vop.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://idw.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://spx.meibo888.top

"值: $b"
来源：http://rsk.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://lau.hysaishi.cn

val n: String? = null;  n?.length
来源：http://acg.316326.xyz

[T05] Kotlin：when 表达式
来源：http://vxu.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cip.bjfxy.top

[T06] Kotlin：集合映射
来源：http://dea.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pgu.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://uzg.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wyh.ppjwa.cn

[T08] Kotlin：数据类
来源：http://vvc.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://ppi.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://zgd.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://qjp.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://cyn.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jsm.yvedp.cn

[T11] Kotlin：协程
来源：http://owx.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://urq.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://xxh.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://ahu.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://sqg.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://iop.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://hwl.tanke756.top

for (i in 1..10) println(i)
来源：http://lby.meibo888.top

[T15] Kotlin：接口
来源：http://nnq.yj20258888.top

interface Shape { fun area(): Double }
来源：http://bgc.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://cbc.gogol.net.cn

print("Hello")
来源：http://bvj.shuidangran.top

[T17] Swift：变量与常量
来源：http://dmt.birdmap.top

var a = 1;  let b = 2
来源：http://xdc.zhengqikj.top

[T18] Swift：字符串插值
来源：http://mbk.fzhhl.top

"值: \(b)"
来源：http://cqd.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://oxf.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://bce.cheryme.top

[T20] Swift：数组操作
来源：http://sah.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cny.feifeiyinyue.top

[T21] Swift：遍历
来源：http://rcw.xuanzx.com

for x in a { print(x) }
来源：http://ltj.zhengqikj.top

[T22] Swift：字典
来源：http://gpo.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://zms.vqdsnc.cn

[T23] Swift：函数
来源：http://mrg.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qxj.yj202588.top

[T24] Swift：闭包
来源：http://plk.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qye.pengpengdd.cyou

[T25] Swift：结构体
来源：http://muu.meibo888.top

struct P { var x: Int }
来源：http://mfr.bbcook.cn

[T26] Swift：类与重写
来源：http://ncw.aizwys.cn

class A: Base { override func f() {} }
来源：http://gbv.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://nsu.fzhhl.top

do { try f() } catch { print(error) }
来源：http://efd.sweek.top

[T28] Swift：枚举
来源：http://ggg.yj20258888.top

enum Color { case red, green }
来源：http://rzv.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://hul.zhongyouzk.top

guard let x = opt else { return }
来源：http://byv.cqqwz.cn

[T30] Swift：协议
来源：http://eqa.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://bbo.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://hjr.yongpay.top

print("Hello")
来源：http://eke.nwbrower.top

[T32] Lua：局部变量
来源：http://mfb.sweek.top

local a = 1
来源：http://otd.yuanzhike.top

[T33] Lua：表（数组）
来源：http://bly.jinghuilouyu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gzm.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://syq.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tao.shzxlz.cn

[T35] Lua：字典表
来源：http://wyi.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://qdq.uphjek.com

[T36] Lua：函数
来源：http://tzg.ydjk.org.cn

function add(a, b) return a + b end
来源：http://nhb.daxiang520.top

[T37] Lua：字符串拼接
来源：http://oud.shangyingyoupin.top

"a" .. "b"
来源：http://rhj.ivvv.top

[T38] Lua：条件
来源：http://vbb.ctjpmb.com

if x > 0 then print("正") end
来源：http://oos.yvedp.cn

[T39] Lua：模式匹配
来源：http://uso.cqqwz.cn

string.find(s, "%d+")
来源：http://tfh.jinqigfzy.top

[T40] Lua：元表
来源：http://zch.yonumen.top

setmetatable({}, { __index = base })
来源：http://gun.meibo888.top

[T41] Perl：Hello World
来源：http://stz.yvedp.cn

print "Hello\n";
来源：http://hyi.ppjwa.cn

[T42] Perl：变量类型
来源：http://qje.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zmo.svipenyu.cn

[T43] Perl：字符串插值
来源：http://nuo.epnwcf.com

"值: $a"
来源：http://dxu.meibo888.top

[T44] Perl：条件
来源：http://plw.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://lvb.chenlongwang.top

[T45] Perl：数组遍历
来源：http://sfh.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://bvy.nwbrower.top

[T46] Perl：哈希操作
来源：http://abp.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kxr.yvedp.cn

[T47] Perl：正则捕获
来源：http://hpq.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rzh.sysykeji.top

[T48] Perl：正则替换
来源：http://qaa.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://fvz.feifeiyinyue.top

[T49] Perl：函数
来源：http://wns.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ftb.iojbl.cn

[T50] Perl：逐行读文件
来源：http://fpl.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://ybj.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://ooe.zhongyouzk.top

[T51] Scala：Hello World
来源：http://hjf.hammf.cn

println("Hello")
来源：http://hop.zdbjq.cn

[T52] Scala：变量
来源：http://vtq.nwbrower.top

val a = 1;  var b = 2
来源：http://pwo.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://bsb.xuetiantiany.cn

s"值: $b"
来源：http://jjz.cheryme.top

[T54] Scala：集合映射
来源：http://elg.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://tbx.316326.xyz

[T55] Scala：集合过滤
来源：http://dib.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://cfj.tarul.cn

[T56] Scala：样例类
来源：http://raa.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://ver.ppjwa.cn

[T57] Scala：模式匹配
来源：http://rmg.fehbvm.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://rng.nanxinkj.top

[T58] Scala：函数定义
来源：http://oua.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://apz.cashguo.top

[T59] Scala：循环
来源：http://zzw.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://edr.ctjpmb.com

[T60] Scala：折叠
来源：http://pen.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vts.gogol.net.cn

================================================================================
来源：http://idy.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ser.cucudq.cn

================================================================================
来源：http://fuv.snrcjt.cn

[U01] Py：创建虚拟环境
来源：http://pwk.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://mjs.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://fsh.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ypk.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://vby.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://csw.yueranfly.top

[U04] Py：变量调试打印
来源：http://ynb.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sdg.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://ohi.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://mzg.pycfn.com

[U06] Py：合并两个字典
来源：http://ydw.nanxinkj.top

{**a, **b}
来源：http://ilg.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://sea.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://yhc.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://lba.havefunace.top

[y for x in nested for y in x]
来源：http://aff.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://ydf.kuanghao11.cn

max(d, key=d.get)
来源：http://mnk.haohaochexian.top

[U10] Py：按值排序字典
来源：http://mio.daxiang520.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gev.c1oappe.top

[U11] Py：生成器表达式
来源：http://zar.yanxiufei.cn

(x * 2 for x in arr)
来源：http://zrp.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://qfm.shanyushiyangtech.top

Counter(arr).most_common(3)
来源：http://nzr.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://ktm.xingfuxueyuan.xyz

deque(maxlen=10)
来源：http://hdp.tanke756.top

[U14] Py：分组收集到列表
来源：http://fqz.yueranfly.top

defaultdict(list)
来源：http://qkb.cashguo.top

[U15] Py：高精度计时
来源：http://nqx.chenzaomai.com

t = time.perf_counter()
来源：http://tlx.wangdashe.top

[U16] Py：命令行参数解析
来源：http://bwd.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://obm.yj202588.top

[U17] Py：初始化日志
来源：http://hrm.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://jvl.mhx1999.top

[U18] Py：预编译正则
来源：http://tsd.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://ozj.ydzc1.top

[U19] Py：正则替换带回调
来源：http://xor.zhongyouzk.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cnj.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://nvt.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://pyo.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://scw.hcnkem.com

@contextlib.contextmanager
来源：http://rmt.fehbvm.com

[U22] Py：矩阵转置
来源：http://bxv.hfpthk.cn

list(zip(*m))
来源：http://cpy.havefunace.top

[U23] Py：分块读取大文件
来源：http://ytk.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kgy.feifeiyinyue.top

[U24] Py：路径操作
来源：http://dmq.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rbq.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://tkt.tanke756.top

csv.DictReader(f)
来源：http://lqp.meibo888.top

[U26] Py：并发下载
来源：http://bvn.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://raw.hnxiangtu.top

[U27] Py：异步 HTTP
来源：http://bwn.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://rad.hongshengwenyu.top

[U28] Py：类型别名
来源：http://dnc.fanxiaobao.xyz

UserId = int
来源：http://hbd.zhengqikj.top

[U29] Py：属性校验
来源：http://stj.quarkkingdee.top

@property 与 @x.setter 配合
来源：http://nqz.snrcjt.cn

[U30] Py：数据类
来源：http://zkb.jyoumei.cn

@dataclass(slots=True)
来源：http://elm.iojbl.cn

[U31] Py：单测
来源：http://euy.xuanzx.com

python -m pytest -q
来源：http://vfs.nanxinkj.top

[U32] Py：代码格式化
来源：http://hyk.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://lyu.feifeiyinyue.top

[U33] Py：打包发布
来源：http://qrj.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://qcl.shangyingyoupin.top

[U34] Py：判断编码
来源：http://ytt.cdnleiting.top

chardet.detect(raw)
来源：http://nbt.xziqi.cn

[U35] Py：发送邮件
来源：http://pyt.ydzc1.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bwd.epnwcf.com

[U36] Py：定时任务
来源：http://nir.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://uzj.gzhubu.top

[U37] Py：读写 Excel
来源：http://lxo.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://kif.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://pvz.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://qzd.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://pku.jqgufenzy.top

sys.stdout.isatty()
来源：http://mqk.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://acb.zhengqikj.top

print("err", file=sys.stderr)
来源：http://joy.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://gni.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cur.bjfxy.top

[U42] PHP：PSR-4 自动加载
来源：http://wio.hnxiangtu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ipm.daxiang520.top


<!-- 参考信息 -->