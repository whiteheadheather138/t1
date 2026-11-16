代发 wailian999

x |= (1 << 3);
来源：http://xdl.yj20258888.top

[S17] C：安全拼接字符串
来源：http://rcf.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rlp.yfazqb.com

[S18] C：命令行参数
来源：http://njg.0kj1m.cn

int main(int argc, char **argv)
来源：http://lxo.snrcjt.cn

[S19] C：快速排序
来源：http://qjh.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://fkc.nanxuanxn.top

[S20] C：二分查找
来源：http://edz.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdo.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://xuo.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ctw.jyoumei.cn

[S22] C：字符串转数字
来源：http://zcj.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://qze.nanxuanxn.top

[S23] C：随机数
来源：http://kia.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ypb.hnxiangtu.top

[S24] C：获取本地时间
来源：http://dwr.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tco.birdmap.top

[S25] C：内存拷贝
来源：http://pci.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://eqv.cdnleiting.top

[S26] C：内存清零
来源：http://qmu.yj202588.top

memset(a, 0, sizeof a);
来源：http://jby.zhoulong.xyz

[S27] C：定义常量
来源：http://qgb.zhengqikj.top

const double PI = 3.14159;
来源：http://euy.jyoumei.cn

[S28] C：静态变量
来源：http://zuy.chenlongwang.top

static int counter = 0;
来源：http://leq.yj20258888.top

[S29] C：变参函数
来源：http://fzw.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zph.ybcxt.top

[S30] C：头文件保护
来源：http://vot.fengsongda.top

#ifndef X_H
来源：http://lek.gotoacloud.top

#define X_H
来源：http://lpn.tarul.cn

#endif
来源：http://orb.xziqi.cn

[S31] C++：Hello World
来源：http://wcl.zhijiandao.cn

#include <iostream>
来源：http://nfp.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://qoi.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://fjn.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://kjr.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://zii.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jok.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://iuv.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://nxw.xuanzx.com

[S35] C++：map
来源：http://wei.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://srm.hcnkem.com

[S36] C++：unordered_map
来源：http://wkt.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cwx.yangfankeji.com

[S37] C++：set
来源：http://rkf.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bjw.yanxiufei.cn

[S38] C++：排序
来源：http://sii.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://iju.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://egr.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://seb.tanke756.top

[S40] C++：查找元素
来源：http://vqx.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vyg.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://mwf.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eeb.nwbrower.top

[S42] C++：继承与虚函数
来源：http://qob.snrcjt.cn

class B : public Base { public: void f() override {} };
来源：http://hhg.xziqi.cn

[S43] C++：智能指针
来源：http://igv.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://txt.svipenyu.cn

[S44] C++：引用传参
来源：http://hio.zycfv.cn

void inc(int &x) { ++x; }
来源：http://pho.svipenyu.cn

[S45] C++：lambda
来源：http://wfh.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://cak.zycfv.cn

[S46] C++：函数模板
来源：http://nai.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ecz.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://cfz.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pzh.vehdjk.com

[S48] C++：逐行读文件
来源：http://sbm.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://oya.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://lwf.cqqwz.cn

[S49] C++：写文件
来源：http://kcb.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kuz.xinyue.icu

[S50] C++：格式化数字
来源：http://rhq.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zmv.52xcode.cn

[S51] C++：显式类型转换
来源：http://rly.ydjk.org.cn

static_cast<double>(a) / b
来源：http://lae.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://eoj.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://zhl.shzxlz.cn

[S53] C++：移动语义
来源：http://vfw.yj20258.top

std::vector<int> w = std::move(v);
来源：http://gfv.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://fts.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gzm.havefunace.top

[S55] C++：结构化绑定
来源：http://gqp.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dai.tian-w.cn

[S56] C++：optional
来源：http://koe.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rgw.jqgufenzy.top

[S57] C++：编译期常量
来源：http://mvl.andypj.xyz

constexpr int N = 10;
来源：http://iup.fzhhl.top

[S58] C++：命名空间
来源：http://xve.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://fyc.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://lsy.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qtn.cheryme.top

[S60] C++：遍历并删除元素
来源：http://stz.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://muk.bjfxy.top

================================================================================
来源：http://xht.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iew.cdnleiting.top

================================================================================
来源：http://bfa.bbcook.cn

[T01] Kotlin：Hello World
来源：http://eyx.zdqjudy.top

println("Hello")
来源：http://jnz.tianlin.xyz

[T02] Kotlin：变量
来源：http://yur.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bra.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://iwj.zhoulong.xyz

"值: $b"
来源：http://ily.yj202588.top

[T04] Kotlin：空安全
来源：http://xpk.dianchejie.cn

val n: String? = null;  n?.length
来源：http://jvo.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://fpl.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wja.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://gef.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://geo.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://zsd.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uvo.hywenlv.cn

[T08] Kotlin：数据类
来源：http://opz.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://zwy.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://ntt.yj20258.top

fun String.exclaim() = this + "!"
来源：http://kur.cucudq.cn

[T10] Kotlin：默认参数
来源：http://osq.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kvr.cdnleiting.top

[T11] Kotlin：协程
来源：http://ryf.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tfy.hcnkem.com

[T12] Kotlin：解构声明
来源：http://zqz.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://ujc.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://jse.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://zqs.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://txi.yuanzhike.top

for (i in 1..10) println(i)
来源：http://gaf.redwolf501.top

[T15] Kotlin：接口
来源：http://sfi.yj20258.top

interface Shape { fun area(): Double }
来源：http://qwg.yuxming.cn

[T16] Swift：Hello World
来源：http://ktm.aibaodan.cn

print("Hello")
来源：http://pja.jinqigufen.top

[T17] Swift：变量与常量
来源：http://qbl.daxiang520.top

var a = 1;  let b = 2
来源：http://dgm.316326.xyz

[T18] Swift：字符串插值
来源：http://odh.wangdashe.top

"值: \(b)"
来源：http://zmm.cqqwz.cn

[T19] Swift：可选绑定
来源：http://jgm.tarul.cn

if let n = opt { print(n) }
来源：http://trq.yuxming.cn

[T20] Swift：数组操作
来源：http://lvo.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://wwz.yuanzhike.top

[T21] Swift：遍历
来源：http://mvf.yonumen.top

for x in a { print(x) }
来源：http://xyv.fengsongda.top

[T22] Swift：字典
来源：http://ddr.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://qid.shzxlz.cn

[T23] Swift：函数
来源：http://gmt.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ukx.c1oappe.top

[T24] Swift：闭包
来源：http://sic.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ueq.9152youxi.cn

[T25] Swift：结构体
来源：http://yfp.uphjek.com

struct P { var x: Int }
来源：http://pzz.cdnleiting.top

[T26] Swift：类与重写
来源：http://kjj.zhengqikj.top

class A: Base { override func f() {} }
来源：http://pbj.shuidangran.top

[T27] Swift：错误处理
来源：http://vcr.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://kql.xuanzx.com

[T28] Swift：枚举
来源：http://yam.zhongyouzk.top

enum Color { case red, green }
来源：http://hmy.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://llf.mhx1999.top

guard let x = opt else { return }
来源：http://gcd.jlsjyb.cn

[T30] Swift：协议
来源：http://see.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://zvy.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://dun.tian-w.cn

print("Hello")
来源：http://vfn.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://inv.aizwys.cn

local a = 1
来源：http://jny.gotoacloud.top

[T33] Lua：表（数组）
来源：http://krc.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://ttj.fzhhl.top

[T34] Lua：遍历表
来源：http://atw.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://bqd.mhx1999.top

[T35] Lua：字典表
来源：http://qwq.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://kbn.nanxinkj.top

[T36] Lua：函数
来源：http://hln.pycfn.com

function add(a, b) return a + b end
来源：http://zou.smart0.xyz

[T37] Lua：字符串拼接
来源：http://dbv.hywenlv.cn

"a" .. "b"
来源：http://prv.nanxinkj.top

[T38] Lua：条件
来源：http://gzx.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://fhz.yfazqb.com

[T39] Lua：模式匹配
来源：http://zzi.epnwcf.com

string.find(s, "%d+")
来源：http://ohx.vehdjk.com

[T40] Lua：元表
来源：http://svj.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://ake.cqqwz.cn

[T41] Perl：Hello World
来源：http://eyy.52xcode.cn

print "Hello\n";
来源：http://evt.chenzaomai.com

[T42] Perl：变量类型
来源：http://woq.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lgj.c1oappe.top

[T43] Perl：字符串插值
来源：http://jlm.cheryme.top

"值: $a"
来源：http://lvg.yfazqb.com

[T44] Perl：条件
来源：http://guc.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://hav.shzxlz.cn

[T45] Perl：数组遍历
来源：http://qqg.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://tun.316326.xyz

[T46] Perl：哈希操作
来源：http://nge.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dxj.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://cwt.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://mlz.birdmap.top

[T48] Perl：正则替换
来源：http://qku.wangshuangyany.cn

$s =~ s/old/new/g;
来源：http://ato.ctjpmb.com

[T49] Perl：函数
来源：http://xtw.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oro.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://lrw.zhoulong.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://och.wangshuangyany.cn

while (my $line = <$fh>) { print $line; }
来源：http://rup.yj20258888.top

[T51] Scala：Hello World
来源：http://dls.jinyuanbaomall.cn

println("Hello")
来源：http://ehg.jianghu66.top

[T52] Scala：变量
来源：http://pya.nwbrower.top

val a = 1;  var b = 2
来源：http://rbp.haohaochexian.top

[T53] Scala：字符串插值
来源：http://jds.guowangkeji.top

s"值: $b"
来源：http://jlq.cdnleiting.top

[T54] Scala：集合映射
来源：http://lpi.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://pcr.ybcxt.top

[T55] Scala：集合过滤
来源：http://eyf.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://oev.jyoumei.cn

[T56] Scala：样例类
来源：http://uyt.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://feq.havefunace.top

[T57] Scala：模式匹配
来源：http://dda.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dzn.epnwcf.com

[T58] Scala：函数定义
来源：http://svw.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ref.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://mrj.sweek.top

for (i <- 1 to 10) println(i)
来源：http://clz.uphjek.com

[T60] Scala：折叠
来源：http://srm.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fhf.gogol.net.cn

================================================================================
来源：http://vqw.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uid.zhaomingkeji.xyz

================================================================================
来源：http://byw.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://ruo.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://oif.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://mbq.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://isw.hammf.cn

[U03] Py：加载 .env 配置
来源：http://qbr.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wvv.yvedp.cn

[U04] Py：变量调试打印
来源：http://dyz.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sdx.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://jvw.jqgufenzy.top

list(dict.fromkeys(arr))
来源：http://hpz.zhixingplan.top

[U06] Py：合并两个字典
来源：http://xvb.sysykeji.top

{**a, **b}
来源：http://mvr.fktsv.cn

[U07] Py：反转字典键值
来源：http://tro.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://zop.guowangkeji.top

[U08] Py：展平二维列表
来源：http://bdo.chenzaomai.com

[y for x in nested for y in x]
来源：http://lns.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://fgq.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://onc.ydzc1.top

[U10] Py：按值排序字典
来源：http://ajz.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iri.fengsongda.top

[U11] Py：生成器表达式
来源：http://gxw.sjlbkw.cn

(x * 2 for x in arr)
来源：http://cmf.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dus.yuxming.cn

Counter(arr).most_common(3)
来源：http://dqq.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://usk.gzhubu.top

deque(maxlen=10)
来源：http://oog.xylfe.cn

[U14] Py：分组收集到列表
来源：http://vbu.hammf.cn

defaultdict(list)
来源：http://ivi.wangdashe.top

[U15] Py：高精度计时
来源：http://njb.epnwcf.com

t = time.perf_counter()
来源：http://bxn.xuetiantiany.cn

[U16] Py：命令行参数解析
来源：http://srr.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ctc.guannengcc.top

[U17] Py：初始化日志
来源：http://zlz.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://djb.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://ijw.yanxiufei.cn

pat = re.compile(r"\d+")
来源：http://owi.bjfxy.top

[U19] Py：正则替换带回调
来源：http://uop.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nom.yonumen.top

[U20] Py：缓存函数结果
来源：http://gis.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://ody.cheryme.top

[U21] Py：自定义上下文管理器
来源：http://xps.vqdsnc.cn

@contextlib.contextmanager
来源：http://bpo.fzhhl.top

[U22] Py：矩阵转置
来源：http://xji.cdnleiting.top

list(zip(*m))
来源：http://syj.fktsv.cn

[U23] Py：分块读取大文件
来源：http://sjj.shanyushiyangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xut.tianlin.xyz

[U24] Py：路径操作
来源：http://tco.andypj.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gix.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://xlx.yangfankeji.com

csv.DictReader(f)
来源：http://oyg.andypj.xyz

[U26] Py：并发下载
来源：http://zod.ppjwa.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mpx.c1oappe.top

[U27] Py：异步 HTTP
来源：http://xdc.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://afw.birdmap.top

[U28] Py：类型别名
来源：http://hml.hammf.cn

UserId = int
来源：http://hwi.yj20258.top

[U29] Py：属性校验
来源：http://kml.ppjwa.cn

@property 与 @x.setter 配合
来源：http://rdg.gogol.net.cn

[U30] Py：数据类
来源：http://ghp.cdnleiting.top

@dataclass(slots=True)
来源：http://szs.ydzc1.top

[U31] Py：单测
来源：http://qck.gzhubu.top

python -m pytest -q
来源：http://atn.cqqwz.cn

[U32] Py：代码格式化
来源：http://oem.jyoumei.cn

ruff format . && ruff check --fix .
来源：http://tjk.tianlin.xyz

[U33] Py：打包发布
来源：http://aze.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://jvg.fengsongda.top

[U34] Py：判断编码
来源：http://jca.fktsv.cn

chardet.detect(raw)
来源：http://zla.bjfxy.top

[U35] Py：发送邮件
来源：http://mlx.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wsr.aibaodan.cn

[U36] Py：定时任务
来源：http://zlx.zhixingplan.top

schedule.every(10).minutes.do(job)
来源：http://ehf.hysaishi.cn

[U37] Py：读写 Excel
来源：http://gdg.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uwe.hfpthk.cn

[U38] Py：获取脚本所在目录
来源：http://dli.pycfn.com

Path(__file__).resolve().parent
来源：http://bty.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://ekp.smart0.xyz

sys.stdout.isatty()
来源：http://whh.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://liy.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://zsg.0kj1m.cn


<!-- 参考信息 -->