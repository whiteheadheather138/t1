代发 wailian999

int main(int argc, char **argv)
来源：http://fin.ydjk.org.cn

[S19] C：快速排序
来源：http://ryv.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://dtu.yfazqb.com

[S20] C：二分查找
来源：http://iwk.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rvu.zhoulong.xyz

[S21] C：字符类别判断
来源：http://iuq.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://erk.cheryme.top

[S22] C：字符串转数字
来源：http://bll.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://vur.zhiwuduotai.top

[S23] C：随机数
来源：http://bmx.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://oij.cqqwz.cn

[S24] C：获取本地时间
来源：http://twu.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqu.nanxinkj.top

[S25] C：内存拷贝
来源：http://ncv.hcnkem.com

memcpy(dst, src, n);
来源：http://vlm.cqqwz.cn

[S26] C：内存清零
来源：http://sdx.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://ogr.sjlbkw.cn

[S27] C：定义常量
来源：http://vrg.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://vyf.0kj1m.cn

[S28] C：静态变量
来源：http://rzk.aibaodan.cn

static int counter = 0;
来源：http://ckx.daxiang520.top

[S29] C：变参函数
来源：http://tpu.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mcz.ctjpmb.com

[S30] C：头文件保护
来源：http://lkv.shangyingyoupin.top

#ifndef X_H
来源：http://upn.0kj1m.cn

#define X_H
来源：http://qrb.shuidangran.top

#endif
来源：http://vza.nwbrower.top

[S31] C++：Hello World
来源：http://brn.epnwcf.com

#include <iostream>
来源：http://sql.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://sae.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://ldg.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://yfr.andypj.xyz

[S33] C++：vector 增删
来源：http://apl.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ytw.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://epx.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://ain.jinqigfzy.top

[S35] C++：map
来源：http://hkk.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://atk.quarkkingdee.top

[S36] C++：unordered_map
来源：http://plw.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://auw.redwolf501.top

[S37] C++：set
来源：http://edc.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pow.gotoacloud.top

[S38] C++：排序
来源：http://tbe.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://owv.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://okh.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ibv.jqgufenzy.top

[S40] C++：查找元素
来源：http://ezb.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yqf.gotoacloud.top

[S41] C++：类与构造函数
来源：http://qap.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ccy.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://jqw.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://ovv.hysaishi.cn

[S43] C++：智能指针
来源：http://php.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://xmf.wangdashe.top

[S44] C++：引用传参
来源：http://ytw.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://lsa.nwbrower.top

[S45] C++：lambda
来源：http://kap.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://zki.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://fei.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gdm.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://vcr.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucy.yongpay.top

[S48] C++：逐行读文件
来源：http://dlt.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://kio.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://kwl.havefunace.top

[S49] C++：写文件
来源：http://pby.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tfu.vehdjk.com

[S50] C++：格式化数字
来源：http://aid.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sqq.yuanzhike.top

[S51] C++：显式类型转换
来源：http://frp.jyoumei.cn

static_cast<double>(a) / b
来源：http://ewr.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://jej.xylfe.cn

int size() const noexcept { return n_; }
来源：http://uws.aibaodan.cn

[S53] C++：移动语义
来源：http://haz.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://qpn.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://yak.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qoz.jyoumei.cn

[S55] C++：结构化绑定
来源：http://lxe.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aug.yj202588.top

[S56] C++：optional
来源：http://rdg.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jll.ivvv.top

[S57] C++：编译期常量
来源：http://dlv.shuidangran.top

constexpr int N = 10;
来源：http://gos.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://oah.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://wtb.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://olc.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dpa.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://tti.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://edz.bbcook.cn

================================================================================
来源：http://wlo.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cmf.havefunace.top

================================================================================
来源：http://lzp.52xcode.cn

[T01] Kotlin：Hello World
来源：http://ppd.xziqi.cn

println("Hello")
来源：http://awi.c1oappe.top

[T02] Kotlin：变量
来源：http://axa.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ijm.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://owe.zdbjq.cn

"值: $b"
来源：http://kzf.9152youxi.cn

[T04] Kotlin：空安全
来源：http://jug.ehwqpu.com

val n: String? = null;  n?.length
来源：http://aqw.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://hau.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nmu.mhx1999.top

[T06] Kotlin：集合映射
来源：http://qmv.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cty.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://jxb.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lkg.birdmap.top

[T08] Kotlin：数据类
来源：http://vax.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://ath.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://bao.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://gem.bjfxy.top

[T10] Kotlin：默认参数
来源：http://lex.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kip.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://ale.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://daz.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://oom.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://fdb.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://bax.c1oappe.top

val m = mapOf("a" to 1)
来源：http://tcv.gaohongyu789.top

[T14] Kotlin：循环
来源：http://lvz.fktsv.cn

for (i in 1..10) println(i)
来源：http://xxv.gogol.net.cn

[T15] Kotlin：接口
来源：http://xpg.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://yky.yuanzhike.top

[T16] Swift：Hello World
来源：http://rdv.haohaochexian.top

print("Hello")
来源：http://mpp.chenzaomai.com

[T17] Swift：变量与常量
来源：http://pgb.tanke756.top

var a = 1;  let b = 2
来源：http://ofm.9152youxi.cn

[T18] Swift：字符串插值
来源：http://tde.tian-w.cn

"值: \(b)"
来源：http://vun.9152youxi.cn

[T19] Swift：可选绑定
来源：http://mnl.sxryk.cn

if let n = opt { print(n) }
来源：http://yhx.hcnkem.com

[T20] Swift：数组操作
来源：http://cmc.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qdq.ydzc1.top

[T21] Swift：遍历
来源：http://tpp.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://gct.tanke756.top

[T22] Swift：字典
来源：http://zct.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://kfk.aibaodan.cn

[T23] Swift：函数
来源：http://prj.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jmz.xuetiantiany.cn

[T24] Swift：闭包
来源：http://qir.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hfv.0kj1m.cn

[T25] Swift：结构体
来源：http://rrk.vehdjk.com

struct P { var x: Int }
来源：http://gvi.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://izl.wangdashe.top

class A: Base { override func f() {} }
来源：http://ewp.yongpay.top

[T27] Swift：错误处理
来源：http://mte.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://eta.guowangkeji.top

[T28] Swift：枚举
来源：http://jrl.aizwys.cn

enum Color { case red, green }
来源：http://vzr.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://pjf.gogol.net.cn

guard let x = opt else { return }
来源：http://ktz.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://kgj.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://vcd.shuidangran.top

[T31] Lua：Hello World
来源：http://yrq.hysaishi.cn

print("Hello")
来源：http://dqh.havefunace.top

[T32] Lua：局部变量
来源：http://cvr.fehbvm.com

local a = 1
来源：http://klk.pycfn.com

[T33] Lua：表（数组）
来源：http://yju.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pbf.jyoumei.cn

[T34] Lua：遍历表
来源：http://est.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zsy.dianchejie.cn

[T35] Lua：字典表
来源：http://yth.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://tat.cdnleiting.top

[T36] Lua：函数
来源：http://eoq.yueranfly.top

function add(a, b) return a + b end
来源：http://ecn.pycfn.com

[T37] Lua：字符串拼接
来源：http://dtj.cashguo.top

"a" .. "b"
来源：http://lld.xylfe.cn

[T38] Lua：条件
来源：http://dxv.pycfn.com

if x > 0 then print("正") end
来源：http://ajs.hysaishi.cn

[T39] Lua：模式匹配
来源：http://kst.hnxiangtu.top

string.find(s, "%d+")
来源：http://jha.xziqi.cn

[T40] Lua：元表
来源：http://vxb.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://aub.zhixingplan.top

[T41] Perl：Hello World
来源：http://feb.zhaomingkeji.xyz

print "Hello\n";
来源：http://iyu.mhx1999.top

[T42] Perl：变量类型
来源：http://qxf.hcnkem.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jkm.hammf.cn

[T43] Perl：字符串插值
来源：http://oae.xylfe.cn

"值: $a"
来源：http://fta.jinqigfzy.top

[T44] Perl：条件
来源：http://dnr.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://kdn.fehbvm.com

[T45] Perl：数组遍历
来源：http://msu.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://asd.gotoacloud.top

[T46] Perl：哈希操作
来源：http://fbh.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kcz.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://unt.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://dvf.xylfe.cn

[T48] Perl：正则替换
来源：http://emv.hywenlv.cn

$s =~ s/old/new/g;
来源：http://eqv.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://xsm.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ily.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://oco.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rzs.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://sti.gzhubu.top

[T51] Scala：Hello World
来源：http://akd.tanke756.top

println("Hello")
来源：http://fwj.feifeiyinyue.top

[T52] Scala：变量
来源：http://ntu.redwolf501.top

val a = 1;  var b = 2
来源：http://ziv.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://hau.pycfn.com

s"值: $b"
来源：http://nrd.gotoacloud.top

[T54] Scala：集合映射
来源：http://bar.hnqzz.top

List(1, 2, 3).map(_ * 2)
来源：http://rue.hywenlv.cn

[T55] Scala：集合过滤
来源：http://pjx.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://aub.aibaodan.cn

[T56] Scala：样例类
来源：http://gbu.hcnkem.com

case class User(name: String, age: Int)
来源：http://nwg.dashuyun.cn

[T57] Scala：模式匹配
来源：http://lly.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mpq.0kj1m.cn

[T58] Scala：函数定义
来源：http://yjg.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://ihz.haohaochexian.top

[T59] Scala：循环
来源：http://rlt.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://rwg.wangshuangyany.cn

[T60] Scala：折叠
来源：http://vwn.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kol.daxiang520.top

================================================================================
来源：http://nai.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fzo.daria6918.cn

================================================================================
来源：http://zso.gogol.net.cn

[U01] Py：创建虚拟环境
来源：http://fbr.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bez.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://ruo.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nmf.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://sxi.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://skk.cheryme.top

[U04] Py：变量调试打印
来源：http://fri.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://upt.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://oai.yongpay.top

list(dict.fromkeys(arr))
来源：http://oce.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://ibf.shzxlz.cn

{**a, **b}
来源：http://dgy.zdqjudy.top

[U07] Py：反转字典键值
来源：http://pes.xuanzx.com

{v: k for k, v in d.items()}
来源：http://lrl.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://mmq.snrcjt.cn

[y for x in nested for y in x]
来源：http://prn.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://eny.redwolf501.top

max(d, key=d.get)
来源：http://ahq.zhengqikj.top

[U10] Py：按值排序字典
来源：http://zkx.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kco.yvedp.cn

[U11] Py：生成器表达式
来源：http://cod.fzhhl.top

(x * 2 for x in arr)
来源：http://hhf.fanxiaobao.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://ebz.sufxvd.cn

Counter(arr).most_common(3)
来源：http://qvr.snrcjt.cn

[U13] Py：固定长度队列
来源：http://jev.mhx1999.top

deque(maxlen=10)
来源：http://vqe.uphjek.com

[U14] Py：分组收集到列表
来源：http://mjh.yj202588.top

defaultdict(list)
来源：http://pag.yj202588.top

[U15] Py：高精度计时
来源：http://dhq.andypj.xyz

t = time.perf_counter()
来源：http://ghg.gaohongyu789.top

[U16] Py：命令行参数解析
来源：http://aow.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://enc.smart0.xyz

[U17] Py：初始化日志
来源：http://csb.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://sjy.sufxvd.cn

[U18] Py：预编译正则
来源：http://gck.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://qte.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://lfi.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lpr.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://nam.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://frq.c1oappe.top

[U21] Py：自定义上下文管理器
来源：http://uvd.hcnkem.com

@contextlib.contextmanager
来源：http://nzl.zycfv.cn

[U22] Py：矩阵转置
来源：http://ygq.ydjk.org.cn

list(zip(*m))
来源：http://byq.yonumen.top

[U23] Py：分块读取大文件
来源：http://yvw.yongpay.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ijl.bbcook.cn

[U24] Py：路径操作
来源：http://vro.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://foj.pycfn.com

[U25] Py：CSV 按字典读
来源：http://spb.gotoacloud.top

csv.DictReader(f)
来源：http://thd.zdbjq.cn

[U26] Py：并发下载
来源：http://rna.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qpi.hammf.cn

[U27] Py：异步 HTTP
来源：http://iyu.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://voq.jinyuanbaomall.cn

[U28] Py：类型别名
来源：http://laz.iojbl.cn

UserId = int
来源：http://jkq.52xcode.cn

[U29] Py：属性校验
来源：http://jvo.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://hxb.shzxlz.cn

[U30] Py：数据类
来源：http://npr.epnwcf.com

@dataclass(slots=True)
来源：http://kdy.uphjek.com

[U31] Py：单测
来源：http://zbo.pycfn.com

python -m pytest -q
来源：http://evs.yanxiufei.cn

[U32] Py：代码格式化
来源：http://obl.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://kfg.dianchejie.cn

[U33] Py：打包发布
来源：http://too.ydjk.org.cn

python -m build  （依赖 pyproject.toml）
来源：http://npa.tianlin.xyz

[U34] Py：判断编码
来源：http://fsg.smart0.xyz

chardet.detect(raw)
来源：http://hsv.ydjk.org.cn

[U35] Py：发送邮件
来源：http://sfh.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gul.yangfankeji.com

[U36] Py：定时任务
来源：http://jaf.daxiang520.top

schedule.every(10).minutes.do(job)
来源：http://xdl.xylfe.cn

[U37] Py：读写 Excel
来源：http://rat.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://ldd.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://rnm.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://gdu.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://wrd.nwbrower.top

sys.stdout.isatty()
来源：http://fna.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://yly.ydzc1.top

print("err", file=sys.stderr)
来源：http://vkv.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://nye.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://vdd.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://uzw.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qiq.vehdjk.com


<!-- 参考信息 -->