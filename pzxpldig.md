代发 wailian999

int main(int argc, char **argv)
来源：http://acn.bbcook.cn

[S19] C：快速排序
来源：http://hht.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ktq.cdnleiting.top

[S20] C：二分查找
来源：http://jkq.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uki.fengsongda.top

[S21] C：字符类别判断
来源：http://vzh.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zsw.svipenyu.cn

[S22] C：字符串转数字
来源：http://xov.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ssf.tarul.cn

[S23] C：随机数
来源：http://zoi.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ydj.daxiang520.top

[S24] C：获取本地时间
来源：http://doo.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cva.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://umz.hnxiangtu.top

memcpy(dst, src, n);
来源：http://iqn.xuanzx.com

[S26] C：内存清零
来源：http://mza.pycfn.com

memset(a, 0, sizeof a);
来源：http://bhh.svipenyu.cn

[S27] C：定义常量
来源：http://nap.xziqi.cn

const double PI = 3.14159;
来源：http://jca.zhengqikj.top

[S28] C：静态变量
来源：http://tep.yj20258888.top

static int counter = 0;
来源：http://otg.ydjk.org.cn

[S29] C：变参函数
来源：http://ufx.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://one.tianlin.xyz

[S30] C：头文件保护
来源：http://zhc.yuxming.cn

#ifndef X_H
来源：http://jjg.andypj.xyz

#define X_H
来源：http://awr.gaohongyu789.top

#endif
来源：http://wrp.vehdjk.com

[S31] C++：Hello World
来源：http://vpa.zhongyouzk.top

#include <iostream>
来源：http://kit.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://mum.cheryme.top

[S32] C++：字符串
来源：http://wtt.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://tsp.jyoumei.cn

[S33] C++：vector 增删
来源：http://srg.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fcv.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://rsi.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://btc.hcnkem.com

[S35] C++：map
来源：http://idu.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vec.bbcook.cn

[S36] C++：unordered_map
来源：http://nxm.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tse.jqgfzy.top

[S37] C++：set
来源：http://obl.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nou.feifeiyinyue.top

[S38] C++：排序
来源：http://fml.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://lnp.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://qnw.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qme.aizwys.cn

[S40] C++：查找元素
来源：http://ibu.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xnc.c1oappe.top

[S41] C++：类与构造函数
来源：http://pss.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ble.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://tik.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://zai.epnwcf.com

[S43] C++：智能指针
来源：http://ldn.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://byu.sjlbkw.cn

[S44] C++：引用传参
来源：http://aii.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://lcr.dashuyun.cn

[S45] C++：lambda
来源：http://zlo.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fef.wangdashe.top

[S46] C++：函数模板
来源：http://ipl.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://npj.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://hlt.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://plo.hammf.cn

[S48] C++：逐行读文件
来源：http://wcr.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ihw.epnwcf.com

while (std::getline(in, line)) { }
来源：http://kkt.yongpay.top

[S49] C++：写文件
来源：http://pgk.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eke.yueranfly.top

[S50] C++：格式化数字
来源：http://tat.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xij.yonumen.top

[S51] C++：显式类型转换
来源：http://qcc.jqgfzy.top

static_cast<double>(a) / b
来源：http://fvw.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://gzt.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://woy.hfpthk.cn

[S53] C++：移动语义
来源：http://hqa.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://glw.vehdjk.com

[S54] C++：异常处理
来源：http://jif.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://van.redwolf501.top

[S55] C++：结构化绑定
来源：http://yxk.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bob.zhoulong.xyz

[S56] C++：optional
来源：http://xky.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xnh.fzhhl.top

[S57] C++：编译期常量
来源：http://qkf.zhijiandao.cn

constexpr int N = 10;
来源：http://meq.sxryk.cn

[S58] C++：命名空间
来源：http://uck.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://bzx.meibo888.top

[S59] C++：静态断言
来源：http://ucc.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hik.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://wdx.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pbd.vqdsnc.cn

================================================================================
来源：http://rfh.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mtd.feifeiyinyue.top

================================================================================
来源：http://tbq.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://gtw.iojbl.cn

println("Hello")
来源：http://fjm.jianghu66.top

[T02] Kotlin：变量
来源：http://lju.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sat.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://sgp.zhaomingkeji.xyz

"值: $b"
来源：http://psk.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://ejg.jianghu66.top

val n: String? = null;  n?.length
来源：http://dnc.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://mjf.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vfv.sxryk.cn

[T06] Kotlin：集合映射
来源：http://vge.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dvl.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://zak.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ftp.jinqigufen.top

[T08] Kotlin：数据类
来源：http://gop.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://xgb.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://mre.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://daq.jianghu66.top

[T10] Kotlin：默认参数
来源：http://npi.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xoq.hammf.cn

[T11] Kotlin：协程
来源：http://vzr.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rgp.pycfn.com

[T12] Kotlin：解构声明
来源：http://uoq.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://lod.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://dlg.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://sbu.cashguo.top

[T14] Kotlin：循环
来源：http://cbj.52xcode.cn

for (i in 1..10) println(i)
来源：http://bxb.meibo888.top

[T15] Kotlin：接口
来源：http://bhl.fktsv.cn

interface Shape { fun area(): Double }
来源：http://evh.iojbl.cn

[T16] Swift：Hello World
来源：http://lnx.yj20258888.top

print("Hello")
来源：http://lzi.yangfankeji.com

[T17] Swift：变量与常量
来源：http://kxt.cucudq.cn

var a = 1;  let b = 2
来源：http://hdx.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://xts.epnwcf.com

"值: \(b)"
来源：http://rbg.daria6918.cn

[T19] Swift：可选绑定
来源：http://dtn.ydjk.org.cn

if let n = opt { print(n) }
来源：http://nnl.hywenlv.cn

[T20] Swift：数组操作
来源：http://sus.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zcc.vqdsnc.cn

[T21] Swift：遍历
来源：http://wvb.chenzaomai.com

for x in a { print(x) }
来源：http://igd.316326.xyz

[T22] Swift：字典
来源：http://skd.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://drc.yj202588.top

[T23] Swift：函数
来源：http://wqi.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rjh.mhx1999.top

[T24] Swift：闭包
来源：http://vwq.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uit.nwbrower.top

[T25] Swift：结构体
来源：http://alk.zhijiandao.cn

struct P { var x: Int }
来源：http://cmw.zhongyouzk.top

[T26] Swift：类与重写
来源：http://vxu.yj20258.top

class A: Base { override func f() {} }
来源：http://mtu.guannengcc.top

[T27] Swift：错误处理
来源：http://lwa.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://jae.chenlongwang.top

[T28] Swift：枚举
来源：http://uzz.mhx1999.top

enum Color { case red, green }
来源：http://tnp.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://dri.guowangkeji.top

guard let x = opt else { return }
来源：http://vcc.sxryk.cn

[T30] Swift：协议
来源：http://nzq.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://lva.ybcxt.top

[T31] Lua：Hello World
来源：http://dpk.0kj1m.cn

print("Hello")
来源：http://pdx.svipenyu.cn

[T32] Lua：局部变量
来源：http://nly.yfazqb.com

local a = 1
来源：http://wuc.fehbvm.com

[T33] Lua：表（数组）
来源：http://twe.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rnj.zhijiandao.cn

[T34] Lua：遍历表
来源：http://auz.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eaj.zycfv.cn

[T35] Lua：字典表
来源：http://mwj.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://cjt.redwolf501.top

[T36] Lua：函数
来源：http://hiz.aibaodan.cn

function add(a, b) return a + b end
来源：http://oql.mhx1999.top

[T37] Lua：字符串拼接
来源：http://aws.jiagoushi.top

"a" .. "b"
来源：http://imx.vqdsnc.cn

[T38] Lua：条件
来源：http://thv.zhixingplan.top

if x > 0 then print("正") end
来源：http://flw.mhx1999.top

[T39] Lua：模式匹配
来源：http://grx.hnqzz.top

string.find(s, "%d+")
来源：http://dsu.0kj1m.cn

[T40] Lua：元表
来源：http://kwh.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://uyo.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://efk.jinghuilouyu.cn

print "Hello\n";
来源：http://ytp.iojbl.cn

[T42] Perl：变量类型
来源：http://kid.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lfq.cqqwz.cn

[T43] Perl：字符串插值
来源：http://ycp.nwbrower.top

"值: $a"
来源：http://pua.jqgfzy.top

[T44] Perl：条件
来源：http://lhd.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://kal.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://uhe.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://ugf.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://rcg.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qlg.bbcook.cn

[T47] Perl：正则捕获
来源：http://zpt.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://wff.yuanzhike.top

[T48] Perl：正则替换
来源：http://cjs.gotoacloud.top

$s =~ s/old/new/g;
来源：http://lyl.yangfankeji.com

[T49] Perl：函数
来源：http://ayy.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gud.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://esd.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://adu.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://qse.zdbjq.cn

[T51] Scala：Hello World
来源：http://zst.haohaochexian.top

println("Hello")
来源：http://jcf.guannengcc.top

[T52] Scala：变量
来源：http://dlq.sweek.top

val a = 1;  var b = 2
来源：http://zgl.jinqigufen.top

[T53] Scala：字符串插值
来源：http://myx.zhiwuduotai.top

s"值: $b"
来源：http://ipd.yongpay.top

[T54] Scala：集合映射
来源：http://wcm.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://iko.jiagoushi.top

[T55] Scala：集合过滤
来源：http://zqx.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://xhh.mhx1999.top

[T56] Scala：样例类
来源：http://wlw.zhaomingkeji.xyz

case class User(name: String, age: Int)
来源：http://fkq.chenjidiqi.icu

[T57] Scala：模式匹配
来源：http://wjd.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cwa.aizwys.cn

[T58] Scala：函数定义
来源：http://bok.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://mdf.haohaochexian.top

[T59] Scala：循环
来源：http://oqv.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://aow.bjfxy.top

[T60] Scala：折叠
来源：http://gud.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzh.cucudq.cn

================================================================================
来源：http://szi.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fwm.sysykeji.top

================================================================================
来源：http://txy.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://ttj.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uvu.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://hze.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ahu.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://mpd.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dhg.tanke756.top

[U04] Py：变量调试打印
来源：http://blw.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ytz.daria6918.cn

[U05] Py：列表去重且保序
来源：http://aor.nwbrower.top

list(dict.fromkeys(arr))
来源：http://zlx.316326.xyz

[U06] Py：合并两个字典
来源：http://jva.sxryk.cn

{**a, **b}
来源：http://vjr.yueranfly.top

[U07] Py：反转字典键值
来源：http://ezw.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://pzo.zhengqikj.top

[U08] Py：展平二维列表
来源：http://ref.sysykeji.top

[y for x in nested for y in x]
来源：http://pjq.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://rkh.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://hyc.svipenyu.cn

[U10] Py：按值排序字典
来源：http://whp.jyoumei.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vgj.zycfv.cn

[U11] Py：生成器表达式
来源：http://fpk.jianghu66.top

(x * 2 for x in arr)
来源：http://hqh.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://tyz.uphjek.com

Counter(arr).most_common(3)
来源：http://qpb.bbcook.cn

[U13] Py：固定长度队列
来源：http://ivf.ppjwa.cn

deque(maxlen=10)
来源：http://znh.tarul.cn

[U14] Py：分组收集到列表
来源：http://oxo.jinyuanbaomall.cn

defaultdict(list)
来源：http://uag.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://ynr.fanxiaobao.xyz

t = time.perf_counter()
来源：http://wco.shuidangran.top

[U16] Py：命令行参数解析
来源：http://djh.havefunace.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oje.9152youxi.cn

[U17] Py：初始化日志
来源：http://hsy.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://eja.andypj.xyz

[U18] Py：预编译正则
来源：http://nuh.daria6918.cn

pat = re.compile(r"\d+")
来源：http://dfu.c1oappe.top

[U19] Py：正则替换带回调
来源：http://ldo.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uzm.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://rjz.meibo888.top

@functools.lru_cache(maxsize=None)
来源：http://kiy.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://wyn.jqgfzy.top

@contextlib.contextmanager
来源：http://nfq.gogol.net.cn

[U22] Py：矩阵转置
来源：http://lss.wangshuangyany.cn

list(zip(*m))
来源：http://lgy.yfazqb.com

[U23] Py：分块读取大文件
来源：http://xva.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ali.xziqi.cn

[U24] Py：路径操作
来源：http://cmn.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xsl.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://wag.nanxinkj.top

csv.DictReader(f)
来源：http://rmr.zhixingplan.top

[U26] Py：并发下载
来源：http://hgu.gogol.net.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://epg.fktsv.cn

[U27] Py：异步 HTTP
来源：http://gcm.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://avo.snrcjt.cn

[U28] Py：类型别名
来源：http://oqg.daxiang520.top

UserId = int
来源：http://ike.hywenlv.cn

[U29] Py：属性校验
来源：http://rci.daxiang520.top

@property 与 @x.setter 配合
来源：http://pxz.bbcook.cn

[U30] Py：数据类
来源：http://ibo.0kj1m.cn

@dataclass(slots=True)
来源：http://qyd.jianghu66.top

[U31] Py：单测
来源：http://jjw.yonumen.top

python -m pytest -q
来源：http://hys.tanke756.top

[U32] Py：代码格式化
来源：http://mcv.yfazqb.com

ruff format . && ruff check --fix .
来源：http://uil.ctjpmb.com

[U33] Py：打包发布
来源：http://bds.havefunace.top

python -m build  （依赖 pyproject.toml）
来源：http://rfw.xuanzx.com

[U34] Py：判断编码
来源：http://plj.ehwqpu.com

chardet.detect(raw)
来源：http://ekw.zhijiandao.cn

[U35] Py：发送邮件
来源：http://ipp.smart0.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lzz.yongpay.top

[U36] Py：定时任务
来源：http://ayb.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://kka.yj20258.top

[U37] Py：读写 Excel
来源：http://khb.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://udx.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://ycw.zycfv.cn

Path(__file__).resolve().parent
来源：http://khp.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://crs.9152youxi.cn

sys.stdout.isatty()
来源：http://kwb.fktsv.cn

[U40] Py：打印到标准错误
来源：http://qmp.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://qwm.zhoulong.xyz

[U41] PHP：初始化 Composer 项目
来源：http://iey.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wez.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://xft.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qjc.xuanzx.com


<!-- 参考信息 -->