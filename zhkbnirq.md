代发 wailian999

int main(int argc, char **argv)
来源：http://hkt.xuanzx.com

[S19] C：快速排序
来源：http://mhm.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wgw.xuetiantiany.cn

[S20] C：二分查找
来源：http://fmw.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cnl.quarkkingdee.top

[S21] C：字符类别判断
来源：http://pjl.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jvr.wangdashe.top

[S22] C：字符串转数字
来源：http://ewo.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qum.yfazqb.com

[S23] C：随机数
来源：http://vnx.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://npe.vehdjk.com

[S24] C：获取本地时间
来源：http://awe.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yab.bjfxy.top

[S25] C：内存拷贝
来源：http://bnu.zycfv.cn

memcpy(dst, src, n);
来源：http://pja.nanxinkj.top

[S26] C：内存清零
来源：http://vsc.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://jrm.yj202588.top

[S27] C：定义常量
来源：http://vsf.zycfv.cn

const double PI = 3.14159;
来源：http://cui.meibo888.top

[S28] C：静态变量
来源：http://pfg.zhijiandao.cn

static int counter = 0;
来源：http://umy.andypj.xyz

[S29] C：变参函数
来源：http://dul.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nrx.havefunace.top

[S30] C：头文件保护
来源：http://ssw.sxryk.cn

#ifndef X_H
来源：http://pnr.aizwys.cn

#define X_H
来源：http://xqg.316326.xyz

#endif
来源：http://cze.0kj1m.cn

[S31] C++：Hello World
来源：http://vdu.zhengqikj.top

#include <iostream>
来源：http://kkd.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://skn.yueranfly.top

[S32] C++：字符串
来源：http://uir.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://iyr.yuanzhike.top

[S33] C++：vector 增删
来源：http://gbd.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vfz.gotoacloud.top

[S34] C++：遍历 vector
来源：http://dls.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://hcq.fanxiaobao.xyz

[S35] C++：map
来源：http://kxw.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mdo.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://oqg.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yjs.ehwqpu.com

[S37] C++：set
来源：http://rlr.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gpt.xinyue.icu

[S38] C++：排序
来源：http://rlp.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://ylh.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://aud.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vvi.zdqjudy.top

[S40] C++：查找元素
来源：http://ohq.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pcb.wangdashe.top

[S41] C++：类与构造函数
来源：http://gqp.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://get.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://tuy.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://kre.hammf.cn

[S43] C++：智能指针
来源：http://nbz.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://kik.hongshengwenyu.top

[S44] C++：引用传参
来源：http://ojx.cashguo.top

void inc(int &x) { ++x; }
来源：http://ymo.tian-w.cn

[S45] C++：lambda
来源：http://lkr.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bbi.hammf.cn

[S46] C++：函数模板
来源：http://kdq.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://slv.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://syh.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://voz.snrcjt.cn

[S48] C++：逐行读文件
来源：http://gal.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://cwi.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://qqb.nwbrower.top

[S49] C++：写文件
来源：http://csb.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pce.52xcode.cn

[S50] C++：格式化数字
来源：http://ufe.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ngj.daxiang520.top

[S51] C++：显式类型转换
来源：http://siy.ehwqpu.com

static_cast<double>(a) / b
来源：http://vhj.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://dpr.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://wvj.gogol.net.cn

[S53] C++：移动语义
来源：http://fli.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://ccd.zhengqikj.top

[S54] C++：异常处理
来源：http://mnc.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cys.zdbjq.cn

[S55] C++：结构化绑定
来源：http://yfl.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hiy.pycfn.com

[S56] C++：optional
来源：http://zbf.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pkl.ivvv.top

[S57] C++：编译期常量
来源：http://ysk.c1oappe.top

constexpr int N = 10;
来源：http://env.316326.xyz

[S58] C++：命名空间
来源：http://ofw.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://nhg.chenlongwang.top

[S59] C++：静态断言
来源：http://vqz.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uxc.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://jfa.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ngu.jqgufenzy.top

================================================================================
来源：http://tue.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://azg.ehwqpu.com

================================================================================
来源：http://vrr.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://eqj.tian-w.cn

println("Hello")
来源：http://pfg.zhoulong.xyz

[T02] Kotlin：变量
来源：http://vbg.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mam.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://sam.pengpengdd.cyou

"值: $b"
来源：http://ubh.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://vhp.mhx1999.top

val n: String? = null;  n?.length
来源：http://tvu.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://ysc.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ige.guannengcc.top

[T06] Kotlin：集合映射
来源：http://bzn.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qoq.cheryme.top

[T07] Kotlin：集合过滤
来源：http://zzd.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ixo.9152youxi.cn

[T08] Kotlin：数据类
来源：http://jfq.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://uly.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://vrc.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://lvi.xziqi.cn

[T10] Kotlin：默认参数
来源：http://znj.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kcj.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://soz.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://umh.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://jwe.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://ybw.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://nir.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://bsp.kuanghao11.cn

[T14] Kotlin：循环
来源：http://tti.aibaodan.cn

for (i in 1..10) println(i)
来源：http://mhe.fehbvm.com

[T15] Kotlin：接口
来源：http://lkg.shuidangran.top

interface Shape { fun area(): Double }
来源：http://tca.52xcode.cn

[T16] Swift：Hello World
来源：http://rxb.andypj.xyz

print("Hello")
来源：http://aho.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://sdn.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://uzf.cashguo.top

[T18] Swift：字符串插值
来源：http://cdi.shzxlz.cn

"值: \(b)"
来源：http://awh.wangdashe.top

[T19] Swift：可选绑定
来源：http://dln.andypj.xyz

if let n = opt { print(n) }
来源：http://rfl.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://epm.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://vev.chenlongwang.top

[T21] Swift：遍历
来源：http://tfj.xinyue.icu

for x in a { print(x) }
来源：http://oyj.meibo888.top

[T22] Swift：字典
来源：http://ljk.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://grf.jinqigfzy.top

[T23] Swift：函数
来源：http://ekd.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ijc.uphjek.com

[T24] Swift：闭包
来源：http://mib.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ikz.dashuyun.cn

[T25] Swift：结构体
来源：http://zrt.jinghuilouyu.cn

struct P { var x: Int }
来源：http://rly.cucudq.cn

[T26] Swift：类与重写
来源：http://gkm.chenzaomai.com

class A: Base { override func f() {} }
来源：http://qnv.sufxvd.cn

[T27] Swift：错误处理
来源：http://rxg.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://cdc.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://hec.fehbvm.com

enum Color { case red, green }
来源：http://vvy.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://gly.hammf.cn

guard let x = opt else { return }
来源：http://rlc.gaohongyu789.top

[T30] Swift：协议
来源：http://jwz.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://ufs.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://ypa.zdbjq.cn

print("Hello")
来源：http://wye.jqgufenzy.top

[T32] Lua：局部变量
来源：http://hbz.cucudq.cn

local a = 1
来源：http://qvk.cheryme.top

[T33] Lua：表（数组）
来源：http://mmi.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://keb.epnwcf.com

[T34] Lua：遍历表
来源：http://crc.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jev.sjlbkw.cn

[T35] Lua：字典表
来源：http://xwk.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://wxp.gaohongyu789.top

[T36] Lua：函数
来源：http://vfc.chenlongwang.top

function add(a, b) return a + b end
来源：http://mwc.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://xga.sweek.top

"a" .. "b"
来源：http://ejo.bjfxy.top

[T38] Lua：条件
来源：http://wlu.yj202588.top

if x > 0 then print("正") end
来源：http://fjf.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://hjp.ctjpmb.com

string.find(s, "%d+")
来源：http://ypx.jinghuilouyu.cn

[T40] Lua：元表
来源：http://erd.yueranfly.top

setmetatable({}, { __index = base })
来源：http://swx.jinqigufen.top

[T41] Perl：Hello World
来源：http://dnh.fktsv.cn

print "Hello\n";
来源：http://urf.hesvh.cn

[T42] Perl：变量类型
来源：http://ajq.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jvm.yfazqb.com

[T43] Perl：字符串插值
来源：http://adl.zycfv.cn

"值: $a"
来源：http://riw.ppjwa.cn

[T44] Perl：条件
来源：http://woe.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://yui.hnxiangtu.top

[T45] Perl：数组遍历
来源：http://fzp.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://iki.yj20258888.top

[T46] Perl：哈希操作
来源：http://akh.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://krd.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://uff.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wfo.zhengqikj.top

[T48] Perl：正则替换
来源：http://hcm.zhengqikj.top

$s =~ s/old/new/g;
来源：http://fkr.pengpengdd.cyou

[T49] Perl：函数
来源：http://cqq.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nwr.havefunace.top

[T50] Perl：逐行读文件
来源：http://inu.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hef.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://pil.vqdsnc.cn

[T51] Scala：Hello World
来源：http://bug.yj202588.top

println("Hello")
来源：http://xpx.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://xys.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://rxh.aizwys.cn

[T53] Scala：字符串插值
来源：http://eot.0kj1m.cn

s"值: $b"
来源：http://zze.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://qww.tianlin.xyz

List(1, 2, 3).map(_ * 2)
来源：http://wdn.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://yzy.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qyl.tian-w.cn

[T56] Scala：样例类
来源：http://fmi.zhixingplan.top

case class User(name: String, age: Int)
来源：http://ntn.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://wef.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gdh.feifeiyinyue.top

[T58] Scala：函数定义
来源：http://gab.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://htx.jiagoushi.top

[T59] Scala：循环
来源：http://cox.uphjek.com

for (i <- 1 to 10) println(i)
来源：http://qyx.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://puc.jyoumei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ywt.ehwqpu.com

================================================================================
来源：http://gpx.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://udj.jianghu66.top

================================================================================
来源：http://snk.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://xby.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://fmm.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://wjh.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hpl.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://ufl.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zld.shuidangran.top

[U04] Py：变量调试打印
来源：http://btr.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kuu.xylfe.cn

[U05] Py：列表去重且保序
来源：http://zig.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://tfz.shuidangran.top

[U06] Py：合并两个字典
来源：http://voi.ehwqpu.com

{**a, **b}
来源：http://oqn.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://xyx.meibo888.top

{v: k for k, v in d.items()}
来源：http://ihy.hnxiangtu.top

[U08] Py：展平二维列表
来源：http://udc.yfazqb.com

[y for x in nested for y in x]
来源：http://cdh.316326.xyz

[U09] Py：字典取最大值的键
来源：http://mcc.zycfv.cn

max(d, key=d.get)
来源：http://ulv.tian-w.cn

[U10] Py：按值排序字典
来源：http://zwq.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bri.gogol.net.cn

[U11] Py：生成器表达式
来源：http://avd.cucudq.cn

(x * 2 for x in arr)
来源：http://kif.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://kjk.316326.xyz

Counter(arr).most_common(3)
来源：http://kzs.epnwcf.com

[U13] Py：固定长度队列
来源：http://ivm.chenjidiqi.icu

deque(maxlen=10)
来源：http://ven.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://nju.smart0.xyz

defaultdict(list)
来源：http://ycw.epnwcf.com

[U15] Py：高精度计时
来源：http://lvs.chenzaomai.com

t = time.perf_counter()
来源：http://aqc.yvedp.cn

[U16] Py：命令行参数解析
来源：http://kur.xziqi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dqr.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://qke.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://aqn.cashguo.top

[U18] Py：预编译正则
来源：http://bzq.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://fyd.c1oappe.top

[U19] Py：正则替换带回调
来源：http://gev.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://slx.fanxiaobao.xyz

[U20] Py：缓存函数结果
来源：http://ecf.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://ofl.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://ykc.wangdashe.top

@contextlib.contextmanager
来源：http://frq.shuidangran.top

[U22] Py：矩阵转置
来源：http://rtg.guowangkeji.top

list(zip(*m))
来源：http://ccc.meibo888.top

[U23] Py：分块读取大文件
来源：http://qjt.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sbq.gotoacloud.top

[U24] Py：路径操作
来源：http://qqs.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://erl.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://dvt.sxryk.cn

csv.DictReader(f)
来源：http://spa.xziqi.cn

[U26] Py：并发下载
来源：http://hvz.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://urv.hnqzz.top

[U27] Py：异步 HTTP
来源：http://vfn.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://rcj.chenjidiqi.icu

[U28] Py：类型别名
来源：http://mrb.smart0.xyz

UserId = int
来源：http://gpp.aizwys.cn

[U29] Py：属性校验
来源：http://jyg.yuanzhike.top

@property 与 @x.setter 配合
来源：http://agq.cdnleiting.top

[U30] Py：数据类
来源：http://unh.iojbl.cn

@dataclass(slots=True)
来源：http://baz.yongpay.top

[U31] Py：单测
来源：http://fzh.jinghuilouyu.cn

python -m pytest -q
来源：http://ngi.gotoacloud.top

[U32] Py：代码格式化
来源：http://avg.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://oxk.feifeiyinyue.top

[U33] Py：打包发布
来源：http://egk.ywan-chungtsiang.top

python -m build  （依赖 pyproject.toml）
来源：http://bmd.tian-w.cn

[U34] Py：判断编码
来源：http://lcd.gotoacloud.top

chardet.detect(raw)
来源：http://ach.ybcxt.top

[U35] Py：发送邮件
来源：http://qmb.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zdi.hfpthk.cn

[U36] Py：定时任务
来源：http://qqt.cucudq.cn

schedule.every(10).minutes.do(job)
来源：http://icw.ehwqpu.com

[U37] Py：读写 Excel
来源：http://nvb.hnxiangtu.top

pandas.read_excel / DataFrame.to_excel
来源：http://zpd.yj20258.top

[U38] Py：获取脚本所在目录
来源：http://okx.nanxuanxn.top

Path(__file__).resolve().parent
来源：http://dut.hammf.cn

[U39] Py：判断是否在交互环境
来源：http://igl.haohaochexian.top

sys.stdout.isatty()
来源：http://usj.yj202588.top

[U40] Py：打印到标准错误
来源：http://zca.fktsv.cn

print("err", file=sys.stderr)
来源：http://whg.vqdsnc.cn

[U41] PHP：初始化 Composer 项目
来源：http://wad.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://jgx.daxiang520.top

[U42] PHP：PSR-4 自动加载
来源：http://wgl.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hct.jinghuilouyu.cn


<!-- 参考信息 -->