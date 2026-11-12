代发 wailian999

x |= (1 << 3);
来源：http://yey.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://mwq.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sti.gaohongyu789.top

[S18] C：命令行参数
来源：http://lzv.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://heb.hesvh.cn

[S19] C：快速排序
来源：http://ugb.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lui.ctjpmb.com

[S20] C：二分查找
来源：http://gny.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdq.gogol.net.cn

[S21] C：字符类别判断
来源：http://oyl.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yod.zhijiandao.cn

[S22] C：字符串转数字
来源：http://piz.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vqv.yj202588.top

[S23] C：随机数
来源：http://nif.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://lnk.cucudq.cn

[S24] C：获取本地时间
来源：http://kbu.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://erj.mhx1999.top

[S25] C：内存拷贝
来源：http://cse.vehdjk.com

memcpy(dst, src, n);
来源：http://wjb.tian-w.cn

[S26] C：内存清零
来源：http://yyw.andypj.xyz

memset(a, 0, sizeof a);
来源：http://wmp.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://nqf.yfazqb.com

const double PI = 3.14159;
来源：http://knl.sjlbkw.cn

[S28] C：静态变量
来源：http://wsi.jiagoushi.top

static int counter = 0;
来源：http://ufc.xuetiantiany.cn

[S29] C：变参函数
来源：http://lkc.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cpn.kuanghao11.cn

[S30] C：头文件保护
来源：http://igw.zhoulong.xyz

#ifndef X_H
来源：http://tpg.yj20258888.top

#define X_H
来源：http://sai.jqgufenzy.top

#endif
来源：http://zhg.pycfn.com

[S31] C++：Hello World
来源：http://non.tarul.cn

#include <iostream>
来源：http://vij.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://uit.wangshuangyany.cn

[S32] C++：字符串
来源：http://myt.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://rms.hywenlv.cn

[S33] C++：vector 增删
来源：http://ffd.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fhy.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://lac.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://mdz.tianlin.xyz

[S35] C++：map
来源：http://arr.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ksi.yj202588.top

[S36] C++：unordered_map
来源：http://sln.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rpg.feifeiyinyue.top

[S37] C++：set
来源：http://rfm.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://otm.yangfankeji.com

[S38] C++：排序
来源：http://bfd.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://wqt.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://fsj.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pxn.zdqjudy.top

[S40] C++：查找元素
来源：http://qvy.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cvf.haohaochexian.top

[S41] C++：类与构造函数
来源：http://crn.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qop.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://rii.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://avi.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://esl.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://ssx.yvedp.cn

[S44] C++：引用传参
来源：http://ayh.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://hjf.hnqzz.top

[S45] C++：lambda
来源：http://jxt.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uti.sxryk.cn

[S46] C++：函数模板
来源：http://vcb.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uin.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://jbb.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oyu.c1oappe.top

[S48] C++：逐行读文件
来源：http://swh.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wiu.sxryk.cn

while (std::getline(in, line)) { }
来源：http://xtq.jyoumei.cn

[S49] C++：写文件
来源：http://gru.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oci.gaohongyu789.top

[S50] C++：格式化数字
来源：http://xpf.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uvg.jyoumei.cn

[S51] C++：显式类型转换
来源：http://szn.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://lbl.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://zia.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://auj.haohaochexian.top

[S53] C++：移动语义
来源：http://vdg.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://hhw.vehdjk.com

[S54] C++：异常处理
来源：http://rgm.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hmq.xziqi.cn

[S55] C++：结构化绑定
来源：http://sxt.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ufq.hywenlv.cn

[S56] C++：optional
来源：http://iel.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hvd.redwolf501.top

[S57] C++：编译期常量
来源：http://laf.gaohongyu789.top

constexpr int N = 10;
来源：http://miv.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://nny.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://wtb.shangyingyoupin.top

[S59] C++：静态断言
来源：http://rqv.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vwa.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://kgw.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://peu.dashuyun.cn

================================================================================
来源：http://sxf.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ais.yj20258888.top

================================================================================
来源：http://fta.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://ipj.epnwcf.com

println("Hello")
来源：http://aaa.vqdsnc.cn

[T02] Kotlin：变量
来源：http://tfq.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tvt.ivvv.top

[T03] Kotlin：字符串模板
来源：http://uvc.xylfe.cn

"值: $b"
来源：http://mbh.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://eyq.nwbrower.top

val n: String? = null;  n?.length
来源：http://asi.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://uyk.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://klh.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://trw.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uzi.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://cbb.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jpt.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://wfn.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://gum.meibo888.top

[T09] Kotlin：扩展函数
来源：http://rmb.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://tny.nwbrower.top

[T10] Kotlin：默认参数
来源：http://ofg.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xbr.zhixingplan.top

[T11] Kotlin：协程
来源：http://guw.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hpo.daria6918.cn

[T12] Kotlin：解构声明
来源：http://xgp.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://wlx.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://ppb.52xcode.cn

val m = mapOf("a" to 1)
来源：http://pql.tianlin.xyz

[T14] Kotlin：循环
来源：http://sdn.gzhubu.top

for (i in 1..10) println(i)
来源：http://ebf.vqdsnc.cn

[T15] Kotlin：接口
来源：http://kaw.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://yud.zhijiandao.cn

[T16] Swift：Hello World
来源：http://nbi.snrcjt.cn

print("Hello")
来源：http://xwa.ybcxt.top

[T17] Swift：变量与常量
来源：http://yut.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://bdp.hfpthk.cn

[T18] Swift：字符串插值
来源：http://psc.guowangkeji.top

"值: \(b)"
来源：http://hoc.daxiang520.top

[T19] Swift：可选绑定
来源：http://mgq.zhongyouzk.top

if let n = opt { print(n) }
来源：http://ifn.zycfv.cn

[T20] Swift：数组操作
来源：http://gym.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://dai.fktsv.cn

[T21] Swift：遍历
来源：http://oxq.ehwqpu.com

for x in a { print(x) }
来源：http://iom.cdnleiting.top

[T22] Swift：字典
来源：http://vzw.chenzaomai.com

var d = ["a": 1];  d["b"] = 2
来源：http://mcr.guowangkeji.top

[T23] Swift：函数
来源：http://pol.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xsh.aibaodan.cn

[T24] Swift：闭包
来源：http://iaj.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wjq.gotoacloud.top

[T25] Swift：结构体
来源：http://cpi.iojbl.cn

struct P { var x: Int }
来源：http://oih.haohaochexian.top

[T26] Swift：类与重写
来源：http://ggr.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://jpq.shzxlz.cn

[T27] Swift：错误处理
来源：http://yza.bbcook.cn

do { try f() } catch { print(error) }
来源：http://pya.tanke756.top

[T28] Swift：枚举
来源：http://tut.ehwqpu.com

enum Color { case red, green }
来源：http://idr.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://inv.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://zyj.snrcjt.cn

[T30] Swift：协议
来源：http://aku.yj20258.top

protocol Shape { func area() -> Double }
来源：http://sbh.hammf.cn

[T31] Lua：Hello World
来源：http://gqf.ppjwa.cn

print("Hello")
来源：http://cuk.tarul.cn

[T32] Lua：局部变量
来源：http://okx.sweek.top

local a = 1
来源：http://cmh.hywenlv.cn

[T33] Lua：表（数组）
来源：http://bzx.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wln.svipenyu.cn

[T34] Lua：遍历表
来源：http://hmp.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cfl.chenlongwang.top

[T35] Lua：字典表
来源：http://vnr.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://xms.hfpthk.cn

[T36] Lua：函数
来源：http://oui.chenzaomai.com

function add(a, b) return a + b end
来源：http://hdl.mhx1999.top

[T37] Lua：字符串拼接
来源：http://ngn.fehbvm.com

"a" .. "b"
来源：http://gnt.svipenyu.cn

[T38] Lua：条件
来源：http://hab.9152youxi.cn

if x > 0 then print("正") end
来源：http://jsm.cqqwz.cn

[T39] Lua：模式匹配
来源：http://fja.yuxming.cn

string.find(s, "%d+")
来源：http://rkw.yfazqb.com

[T40] Lua：元表
来源：http://fdb.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://oik.fengsongda.top

[T41] Perl：Hello World
来源：http://avz.jinqigfzy.top

print "Hello\n";
来源：http://fhu.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://rit.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yiz.zhengqikj.top

[T43] Perl：字符串插值
来源：http://cpt.ppjwa.cn

"值: $a"
来源：http://ooq.fzhhl.top

[T44] Perl：条件
来源：http://rlx.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://eis.dashuyun.cn

[T45] Perl：数组遍历
来源：http://lvn.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://ahw.gogol.net.cn

[T46] Perl：哈希操作
来源：http://dsw.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qio.shanyushiyangkeji.top

[T47] Perl：正则捕获
来源：http://yuw.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hkd.zhixingplan.top

[T48] Perl：正则替换
来源：http://usg.yuanzhike.top

$s =~ s/old/new/g;
来源：http://yib.daria6918.cn

[T49] Perl：函数
来源：http://kvh.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://obz.ivvv.top

[T50] Perl：逐行读文件
来源：http://szf.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://joo.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://sfk.yuanzhike.top

[T51] Scala：Hello World
来源：http://zlu.gogol.net.cn

println("Hello")
来源：http://qor.gogol.net.cn

[T52] Scala：变量
来源：http://ieh.gzhubu.top

val a = 1;  var b = 2
来源：http://gme.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://bcu.tianlin.xyz

s"值: $b"
来源：http://hpk.haohaochexian.top

[T54] Scala：集合映射
来源：http://bin.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://itr.sxryk.cn

[T55] Scala：集合过滤
来源：http://hat.zycfv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kjt.fktsv.cn

[T56] Scala：样例类
来源：http://nbp.tianlin.xyz

case class User(name: String, age: Int)
来源：http://bbe.vehdjk.com

[T57] Scala：模式匹配
来源：http://yvf.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mzv.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://dgc.jinyuanbaomall.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pbs.hongshengwenyu.top

[T59] Scala：循环
来源：http://jda.sweek.top

for (i <- 1 to 10) println(i)
来源：http://lqe.ctjpmb.com

[T60] Scala：折叠
来源：http://vdn.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://upu.sweek.top

================================================================================
来源：http://stg.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fsj.sxryk.cn

================================================================================
来源：http://vjy.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://dlc.vqdsnc.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aqy.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://aux.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kmq.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://aae.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jca.jqgfzy.top

[U04] Py：变量调试打印
来源：http://vxu.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzg.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://ops.shuidangran.top

list(dict.fromkeys(arr))
来源：http://okj.epnwcf.com

[U06] Py：合并两个字典
来源：http://olj.ctjpmb.com

{**a, **b}
来源：http://xtn.shzxlz.cn

[U07] Py：反转字典键值
来源：http://zxd.c1oappe.top

{v: k for k, v in d.items()}
来源：http://vbh.guannengcc.top

[U08] Py：展平二维列表
来源：http://rta.hesvh.cn

[y for x in nested for y in x]
来源：http://kbi.yongpay.top

[U09] Py：字典取最大值的键
来源：http://ijd.9152youxi.cn

max(d, key=d.get)
来源：http://fqy.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://oqt.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://alr.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://kwx.ydzc1.top

(x * 2 for x in arr)
来源：http://dre.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qux.jyoumei.cn

Counter(arr).most_common(3)
来源：http://bsf.snrcjt.cn

[U13] Py：固定长度队列
来源：http://paj.pengpengdd.cyou

deque(maxlen=10)
来源：http://aup.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://xcf.hfpthk.cn

defaultdict(list)
来源：http://pok.tarul.cn

[U15] Py：高精度计时
来源：http://eqe.bjfxy.top

t = time.perf_counter()
来源：http://ifa.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://axq.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://emk.cheryme.top

[U17] Py：初始化日志
来源：http://dwz.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://ojr.iojbl.cn

[U18] Py：预编译正则
来源：http://rkr.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://qfn.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://fcw.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ryn.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://bxu.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://zim.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://qhg.iojbl.cn

@contextlib.contextmanager
来源：http://rxd.zhengqikj.top

[U22] Py：矩阵转置
来源：http://caa.birdmap.top

list(zip(*m))
来源：http://ztu.bjfxy.top

[U23] Py：分块读取大文件
来源：http://jsq.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tnd.dashuyun.cn

[U24] Py：路径操作
来源：http://rnk.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xzs.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://ndt.zdbjq.cn

csv.DictReader(f)
来源：http://cxg.shzxlz.cn

[U26] Py：并发下载
来源：http://qul.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nno.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://bgr.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://bzo.xziqi.cn

[U28] Py：类型别名
来源：http://jdp.zdqjudy.top

UserId = int
来源：http://xev.jqgfzy.top

[U29] Py：属性校验
来源：http://wga.ybcxt.top

@property 与 @x.setter 配合
来源：http://wzw.tanke756.top

[U30] Py：数据类
来源：http://qip.cheryme.top

@dataclass(slots=True)
来源：http://waj.hywenlv.cn

[U31] Py：单测
来源：http://fyp.quarkkingdee.top

python -m pytest -q
来源：http://jtk.zhiwuduotai.top

[U32] Py：代码格式化
来源：http://asr.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://swo.hysaishi.cn

[U33] Py：打包发布
来源：http://nzj.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://gzy.nanxinkj.top

[U34] Py：判断编码
来源：http://cgt.chenzaomai.com

chardet.detect(raw)
来源：http://twu.redwolf501.top

[U35] Py：发送邮件
来源：http://kce.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rle.zycfv.cn

[U36] Py：定时任务
来源：http://rmc.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ygx.cqqwz.cn

[U37] Py：读写 Excel
来源：http://mli.yvedp.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qoa.jlsjyb.cn

[U38] Py：获取脚本所在目录
来源：http://mhi.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://ein.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://djr.tian-w.cn

sys.stdout.isatty()
来源：http://hsz.fengsongda.top

[U40] Py：打印到标准错误
来源：http://tgy.zhixingplan.top

print("err", file=sys.stderr)
来源：http://zcw.hywenlv.cn


<!-- 参考信息 -->