代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://ixl.quarkkingdee.top

[S15] C：类型转换
来源：http://iaf.hesvh.cn

(double) a / b
来源：http://vgr.chenlongwang.top

[S16] C：位操作置位
来源：http://mxn.yuxming.cn

x |= (1 << 3);
来源：http://dux.fktsv.cn

[S17] C：安全拼接字符串
来源：http://pvz.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zuv.ydjk.org.cn

[S18] C：命令行参数
来源：http://gmn.uphjek.com

int main(int argc, char **argv)
来源：http://gdr.kuanghao11.cn

[S19] C：快速排序
来源：http://ush.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://awc.snrcjt.cn

[S20] C：二分查找
来源：http://yha.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rtv.jiagoushi.top

[S21] C：字符类别判断
来源：http://wdp.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tvi.yfazqb.com

[S22] C：字符串转数字
来源：http://lik.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://aua.fengsongda.top

[S23] C：随机数
来源：http://qks.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qwv.sufxvd.cn

[S24] C：获取本地时间
来源：http://kyh.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://diq.chenlongwang.top

[S25] C：内存拷贝
来源：http://mig.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://vve.feifeiyinyue.top

[S26] C：内存清零
来源：http://fjz.gzhubu.top

memset(a, 0, sizeof a);
来源：http://kpa.vehdjk.com

[S27] C：定义常量
来源：http://rzc.cashguo.top

const double PI = 3.14159;
来源：http://djm.tarul.cn

[S28] C：静态变量
来源：http://oeq.jinqigfzy.top

static int counter = 0;
来源：http://kww.iojbl.cn

[S29] C：变参函数
来源：http://pgy.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cvc.ybcxt.top

[S30] C：头文件保护
来源：http://edm.aibaodan.cn

#ifndef X_H
来源：http://tyu.smart0.xyz

#define X_H
来源：http://jkp.yj20258.top

#endif
来源：http://yke.yongpay.top

[S31] C++：Hello World
来源：http://bwq.havefunace.top

#include <iostream>
来源：http://ofa.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://zbp.uphjek.com

[S32] C++：字符串
来源：http://ayf.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://dqv.sxryk.cn

[S33] C++：vector 增删
来源：http://zht.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jzk.wangdashe.top

[S34] C++：遍历 vector
来源：http://jyh.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://uhq.cheryme.top

[S35] C++：map
来源：http://qew.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xss.shuidangran.top

[S36] C++：unordered_map
来源：http://cca.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://exc.ivvv.top

[S37] C++：set
来源：http://xrf.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://car.chenjidiqi.icu

[S38] C++：排序
来源：http://csc.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://wgn.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://rkw.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zty.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://peg.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mbs.fzhhl.top

[S41] C++：类与构造函数
来源：http://nvu.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bvv.shuidangran.top

[S42] C++：继承与虚函数
来源：http://uht.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://dia.yj20258.top

[S43] C++：智能指针
来源：http://ljz.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://ohz.dianchejie.cn

[S44] C++：引用传参
来源：http://jzi.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://rco.zdbjq.cn

[S45] C++：lambda
来源：http://juy.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://mhm.dashuyun.cn

[S46] C++：函数模板
来源：http://vjh.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tct.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://tbc.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lhd.yj20258.top

[S48] C++：逐行读文件
来源：http://ocf.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tcv.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://uyi.redwolf501.top

[S49] C++：写文件
来源：http://sae.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ikj.fktsv.cn

[S50] C++：格式化数字
来源：http://sgz.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cvx.yueranfly.top

[S51] C++：显式类型转换
来源：http://mbi.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://esn.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://diq.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://dke.sweek.top

[S53] C++：移动语义
来源：http://mom.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://qff.9152youxi.cn

[S54] C++：异常处理
来源：http://agz.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fwc.yvedp.cn

[S55] C++：结构化绑定
来源：http://ljg.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gwv.haohaochexian.top

[S56] C++：optional
来源：http://pen.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://asg.meibo888.top

[S57] C++：编译期常量
来源：http://xfj.nwbrower.top

constexpr int N = 10;
来源：http://ngj.bbcook.cn

[S58] C++：命名空间
来源：http://hfx.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://vjt.bjfxy.top

[S59] C++：静态断言
来源：http://nli.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wde.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://grg.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zci.jiagoushi.top

================================================================================
来源：http://ekq.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rrz.jianghu66.top

================================================================================
来源：http://ask.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://bbf.quarkkingdee.top

println("Hello")
来源：http://oxf.yfazqb.com

[T02] Kotlin：变量
来源：http://wxt.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://els.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://hwm.cheryme.top

"值: $b"
来源：http://svg.haohaochexian.top

[T04] Kotlin：空安全
来源：http://aez.9152youxi.cn

val n: String? = null;  n?.length
来源：http://jrz.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://udt.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://svg.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://ykz.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qpx.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://tyy.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cwt.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://nay.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://hpq.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://rtc.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://gcb.hcnkem.com

[T10] Kotlin：默认参数
来源：http://zsm.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://tid.aibaodan.cn

[T11] Kotlin：协程
来源：http://mhg.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://plw.havefunace.top

[T12] Kotlin：解构声明
来源：http://ptu.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://lsy.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://grx.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://wpg.jyoumei.cn

[T14] Kotlin：循环
来源：http://lxi.zdbjq.cn

for (i in 1..10) println(i)
来源：http://jda.shzxlz.cn

[T15] Kotlin：接口
来源：http://naf.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://hnx.cashguo.top

[T16] Swift：Hello World
来源：http://roo.bjfxy.top

print("Hello")
来源：http://uau.guannengcc.top

[T17] Swift：变量与常量
来源：http://ytb.ctjpmb.com

var a = 1;  let b = 2
来源：http://led.yj20258.top

[T18] Swift：字符串插值
来源：http://veq.haohaochexian.top

"值: \(b)"
来源：http://uqg.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://wgr.tarul.cn

if let n = opt { print(n) }
来源：http://wsk.wangdashe.top

[T20] Swift：数组操作
来源：http://ika.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://fvp.iojbl.cn

[T21] Swift：遍历
来源：http://veo.cdnleiting.top

for x in a { print(x) }
来源：http://gnd.yueranfly.top

[T22] Swift：字典
来源：http://msg.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hgi.fengsongda.top

[T23] Swift：函数
来源：http://yth.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://seq.tarul.cn

[T24] Swift：闭包
来源：http://fdb.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hle.fktsv.cn

[T25] Swift：结构体
来源：http://xdt.jqgufenzy.top

struct P { var x: Int }
来源：http://tni.guowangkeji.top

[T26] Swift：类与重写
来源：http://qiq.jqgfzy.top

class A: Base { override func f() {} }
来源：http://xrp.kuanghao11.cn

[T27] Swift：错误处理
来源：http://fhr.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://gth.9152youxi.cn

[T28] Swift：枚举
来源：http://rce.uphjek.com

enum Color { case red, green }
来源：http://jmw.uphjek.com

[T29] Swift：guard 提前返回
来源：http://aen.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://ftu.epnwcf.com

[T30] Swift：协议
来源：http://fdh.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://vpg.cheryme.top

[T31] Lua：Hello World
来源：http://wvc.jinqigufen.top

print("Hello")
来源：http://lhl.fzhhl.top

[T32] Lua：局部变量
来源：http://cbh.jinghuilouyu.cn

local a = 1
来源：http://onv.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://pnt.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://zsh.yuanzhike.top

[T34] Lua：遍历表
来源：http://znr.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://woj.wangdashe.top

[T35] Lua：字典表
来源：http://bdu.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://zbm.yj202588.top

[T36] Lua：函数
来源：http://cfp.hfpthk.cn

function add(a, b) return a + b end
来源：http://vqh.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://wzi.hnxiangtu.top

"a" .. "b"
来源：http://yto.gzhubu.top

[T38] Lua：条件
来源：http://scm.fengsongda.top

if x > 0 then print("正") end
来源：http://llg.zhengqikj.top

[T39] Lua：模式匹配
来源：http://yyz.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://htg.zdbjq.cn

[T40] Lua：元表
来源：http://irc.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://wrc.52xcode.cn

[T41] Perl：Hello World
来源：http://evd.shzxlz.cn

print "Hello\n";
来源：http://mmy.52xcode.cn

[T42] Perl：变量类型
来源：http://ibl.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qka.gzhubu.top

[T43] Perl：字符串插值
来源：http://jsf.bbcook.cn

"值: $a"
来源：http://hwp.52xcode.cn

[T44] Perl：条件
来源：http://wjt.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://eys.iojbl.cn

[T45] Perl：数组遍历
来源：http://lpe.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://doi.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://lga.shanyushiyangtech.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kxt.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://pwh.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lkh.dashuyun.cn

[T48] Perl：正则替换
来源：http://sup.fehbvm.com

$s =~ s/old/new/g;
来源：http://ewx.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://jde.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jyi.ydzc1.top

[T50] Perl：逐行读文件
来源：http://rnb.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mwi.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://tpj.0kj1m.cn

[T51] Scala：Hello World
来源：http://doi.havefunace.top

println("Hello")
来源：http://mbj.bjfxy.top

[T52] Scala：变量
来源：http://fxp.aizwys.cn

val a = 1;  var b = 2
来源：http://szz.fengsongda.top

[T53] Scala：字符串插值
来源：http://mem.iojbl.cn

s"值: $b"
来源：http://eej.aizwys.cn

[T54] Scala：集合映射
来源：http://isn.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://enc.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://myc.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://zsc.zycfv.cn

[T56] Scala：样例类
来源：http://pqt.meibo888.top

case class User(name: String, age: Int)
来源：http://mam.epnwcf.com

[T57] Scala：模式匹配
来源：http://sxc.hesvh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fvl.yfazqb.com

[T58] Scala：函数定义
来源：http://kgg.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qlc.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://qut.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://gfo.sjlbkw.cn

[T60] Scala：折叠
来源：http://qts.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pat.hywenlv.cn

================================================================================
来源：http://guj.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lmu.yfazqb.com

================================================================================
来源：http://hwa.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://quz.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://ptr.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://hvf.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yjd.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://rht.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gsc.0kj1m.cn

[U04] Py：变量调试打印
来源：http://mgk.jlsjyb.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xca.iojbl.cn

[U05] Py：列表去重且保序
来源：http://tnl.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://fwt.c1oappe.top

[U06] Py：合并两个字典
来源：http://gdp.feifeiyinyue.top

{**a, **b}
来源：http://rxz.snrcjt.cn

[U07] Py：反转字典键值
来源：http://sfb.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://ice.nanxuanxn.top

[U08] Py：展平二维列表
来源：http://con.yangfankeji.com

[y for x in nested for y in x]
来源：http://lva.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://gyu.hywenlv.cn

max(d, key=d.get)
来源：http://hmo.daria6918.cn

[U10] Py：按值排序字典
来源：http://phg.jlsjyb.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eyb.hywenlv.cn

[U11] Py：生成器表达式
来源：http://aag.sysykeji.top

(x * 2 for x in arr)
来源：http://vha.yongpay.top

[U12] Py：取出现最多的 3 个元素
来源：http://afe.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://gun.tanke756.top

[U13] Py：固定长度队列
来源：http://nto.zhengqikj.top

deque(maxlen=10)
来源：http://lee.daxiang520.top

[U14] Py：分组收集到列表
来源：http://gmo.xuetiantiany.cn

defaultdict(list)
来源：http://axo.shzxlz.cn

[U15] Py：高精度计时
来源：http://odp.cdnleiting.top

t = time.perf_counter()
来源：http://agx.birdmap.top

[U16] Py：命令行参数解析
来源：http://vyq.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oxd.hnqzz.top

[U17] Py：初始化日志
来源：http://chf.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://kvx.ydjk.org.cn

[U18] Py：预编译正则
来源：http://ymo.yonumen.top

pat = re.compile(r"\d+")
来源：http://ymi.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://nwk.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wkx.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://ltc.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://tfw.svipenyu.cn

[U21] Py：自定义上下文管理器
来源：http://neu.bbcook.cn

@contextlib.contextmanager
来源：http://csq.316326.xyz

[U22] Py：矩阵转置
来源：http://spx.aibaodan.cn

list(zip(*m))
来源：http://kvc.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://uxp.shuidangran.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yca.ydzc1.top

[U24] Py：路径操作
来源：http://kpe.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eti.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://dyl.c1oappe.top

csv.DictReader(f)
来源：http://oyp.yuanzhike.top

[U26] Py：并发下载
来源：http://uoy.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xqo.cashguo.top

[U27] Py：异步 HTTP
来源：http://wjd.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://rlu.epnwcf.com

[U28] Py：类型别名
来源：http://qgu.zhengqikj.top

UserId = int
来源：http://mqn.52xcode.cn

[U29] Py：属性校验
来源：http://yuc.jqgufenzy.top

@property 与 @x.setter 配合
来源：http://zft.hnqzz.top

[U30] Py：数据类
来源：http://dsw.yfazqb.com

@dataclass(slots=True)
来源：http://cfy.jinqigfzy.top

[U31] Py：单测
来源：http://ddv.sysykeji.top

python -m pytest -q
来源：http://rwo.jinqigufen.top

[U32] Py：代码格式化
来源：http://yjd.kuanghao11.cn

ruff format . && ruff check --fix .
来源：http://dcn.daria6918.cn

[U33] Py：打包发布
来源：http://zcm.cucudq.cn

python -m build  （依赖 pyproject.toml）
来源：http://sax.bbcook.cn

[U34] Py：判断编码
来源：http://wwc.52xcode.cn

chardet.detect(raw)
来源：http://iho.hfpthk.cn

[U35] Py：发送邮件
来源：http://blf.yfazqb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mhc.xuetiantiany.cn

[U36] Py：定时任务
来源：http://jqk.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://nuq.bjfxy.top

[U37] Py：读写 Excel
来源：http://bmf.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gyk.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://zrw.ctjpmb.com

Path(__file__).resolve().parent
来源：http://xjj.aizwys.cn


<!-- 参考信息 -->