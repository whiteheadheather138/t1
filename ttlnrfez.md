代发 wailian999

int main(int argc, char **argv)
来源：http://jmg.hfpthk.cn

[S19] C：快速排序
来源：http://yaf.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vgq.cheryme.top

[S20] C：二分查找
来源：http://aqc.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://irb.yonumen.top

[S21] C：字符类别判断
来源：http://dyw.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pwf.sxryk.cn

[S22] C：字符串转数字
来源：http://cql.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://gnw.yfazqb.com

[S23] C：随机数
来源：http://sev.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rgk.ivvv.top

[S24] C：获取本地时间
来源：http://nva.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zly.jqgufenzy.top

[S25] C：内存拷贝
来源：http://yra.chenlongwang.top

memcpy(dst, src, n);
来源：http://ems.jqgfzy.top

[S26] C：内存清零
来源：http://bbn.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://cqr.ybcxt.top

[S27] C：定义常量
来源：http://udn.jinqigfzy.top

const double PI = 3.14159;
来源：http://bqv.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://mmg.fanxiaobao.xyz

static int counter = 0;
来源：http://adr.hysaishi.cn

[S29] C：变参函数
来源：http://iwf.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hae.zdqjudy.top

[S30] C：头文件保护
来源：http://jwi.zhengqikj.top

#ifndef X_H
来源：http://zrd.gotoacloud.top

#define X_H
来源：http://rro.52xcode.cn

#endif
来源：http://kck.fehbvm.com

[S31] C++：Hello World
来源：http://qry.jqgfzy.top

#include <iostream>
来源：http://lwd.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://wla.zdqjudy.top

[S32] C++：字符串
来源：http://hzj.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://two.zdqjudy.top

[S33] C++：vector 增删
来源：http://ddx.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pmr.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://ato.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://bcq.daria6918.cn

[S35] C++：map
来源：http://fox.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qtq.yj20258888.top

[S36] C++：unordered_map
来源：http://ssd.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cpj.yonumen.top

[S37] C++：set
来源：http://hol.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vwy.mhx1999.top

[S38] C++：排序
来源：http://shm.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://yfd.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://sim.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ccm.jyoumei.cn

[S40] C++：查找元素
来源：http://her.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oyf.cashguo.top

[S41] C++：类与构造函数
来源：http://zmi.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nql.xylfe.cn

[S42] C++：继承与虚函数
来源：http://vjw.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://eph.hnxiangtu.top

[S43] C++：智能指针
来源：http://bov.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://cye.jianghu66.top

[S44] C++：引用传参
来源：http://lra.guannengcc.top

void inc(int &x) { ++x; }
来源：http://vqw.hnxiangtu.top

[S45] C++：lambda
来源：http://woy.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://tgy.xinyue.icu

[S46] C++：函数模板
来源：http://avd.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ace.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://mjc.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fxs.gogol.net.cn

[S48] C++：逐行读文件
来源：http://wwk.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://kmy.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://gjl.yfazqb.com

[S49] C++：写文件
来源：http://uli.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qyg.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://vkk.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://siz.52xcode.cn

[S51] C++：显式类型转换
来源：http://mrf.snrcjt.cn

static_cast<double>(a) / b
来源：http://ljp.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://kvh.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://whh.daxiang520.top

[S53] C++：移动语义
来源：http://sej.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://cyo.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://jqa.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxk.bjfxy.top

[S55] C++：结构化绑定
来源：http://skc.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nac.chenjidiqi.icu

[S56] C++：optional
来源：http://bjh.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szn.bbcook.cn

[S57] C++：编译期常量
来源：http://tnk.hongshengwenyu.top

constexpr int N = 10;
来源：http://lgu.gogol.net.cn

[S58] C++：命名空间
来源：http://heo.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://vsb.xuanzx.com

[S59] C++：静态断言
来源：http://jjr.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zyd.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://fjx.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxd.shanyushiyangkeji.top

================================================================================
来源：http://rki.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iqw.cqqwz.cn

================================================================================
来源：http://tfg.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://rjv.chenlongwang.top

println("Hello")
来源：http://zee.c1oappe.top

[T02] Kotlin：变量
来源：http://osg.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gpu.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://drk.cheryme.top

"值: $b"
来源：http://mgx.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://bju.daxiang520.top

val n: String? = null;  n?.length
来源：http://yxm.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://ahp.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsq.xziqi.cn

[T06] Kotlin：集合映射
来源：http://gsf.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://brm.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://esj.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oug.9152youxi.cn

[T08] Kotlin：数据类
来源：http://rtu.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://lnj.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://ola.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://hfa.daxiang520.top

[T10] Kotlin：默认参数
来源：http://eoc.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://bmf.sjlbkw.cn

[T11] Kotlin：协程
来源：http://uzr.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gli.guannengcc.top

[T12] Kotlin：解构声明
来源：http://xga.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://opa.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://sqp.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://kyn.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://jtf.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://msi.sysykeji.top

[T15] Kotlin：接口
来源：http://qvc.hcnkem.com

interface Shape { fun area(): Double }
来源：http://ofa.ydzc1.top

[T16] Swift：Hello World
来源：http://ovz.ivvv.top

print("Hello")
来源：http://cmx.cucudq.cn

[T17] Swift：变量与常量
来源：http://lab.jinqigufen.top

var a = 1;  let b = 2
来源：http://jqb.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://kwk.316326.xyz

"值: \(b)"
来源：http://ffl.9152youxi.cn

[T19] Swift：可选绑定
来源：http://ygz.jinqigufen.top

if let n = opt { print(n) }
来源：http://hyv.vqdsnc.cn

[T20] Swift：数组操作
来源：http://sup.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://svu.wangdashe.top

[T21] Swift：遍历
来源：http://mhc.shzxlz.cn

for x in a { print(x) }
来源：http://mfw.jqgufenzy.top

[T22] Swift：字典
来源：http://kes.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://roj.nanxuanxn.top

[T23] Swift：函数
来源：http://lqa.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rqv.52xcode.cn

[T24] Swift：闭包
来源：http://xza.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://niy.aibaodan.cn

[T25] Swift：结构体
来源：http://bwc.chenlongwang.top

struct P { var x: Int }
来源：http://psv.yfazqb.com

[T26] Swift：类与重写
来源：http://hlh.hnqzz.top

class A: Base { override func f() {} }
来源：http://rnh.ydzc1.top

[T27] Swift：错误处理
来源：http://dqo.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://yic.gzhubu.top

[T28] Swift：枚举
来源：http://axw.fengsongda.top

enum Color { case red, green }
来源：http://nob.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://sge.gotoacloud.top

guard let x = opt else { return }
来源：http://jiw.hcnkem.com

[T30] Swift：协议
来源：http://akf.yongpay.top

protocol Shape { func area() -> Double }
来源：http://vzw.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://trv.zhaomingkeji.xyz

print("Hello")
来源：http://cvi.bbcook.cn

[T32] Lua：局部变量
来源：http://ixl.zhengqikj.top

local a = 1
来源：http://kve.daxiang520.top

[T33] Lua：表（数组）
来源：http://ydd.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://acp.jinqigufen.top

[T34] Lua：遍历表
来源：http://urq.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yuk.hywenlv.cn

[T35] Lua：字典表
来源：http://orh.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://azh.hysaishi.cn

[T36] Lua：函数
来源：http://ifi.guannengcc.top

function add(a, b) return a + b end
来源：http://ztr.sweek.top

[T37] Lua：字符串拼接
来源：http://vpz.tianlin.xyz

"a" .. "b"
来源：http://axp.pycfn.com

[T38] Lua：条件
来源：http://mek.gzhubu.top

if x > 0 then print("正") end
来源：http://jfb.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://agz.svipenyu.cn

string.find(s, "%d+")
来源：http://eva.pycfn.com

[T40] Lua：元表
来源：http://hel.yueranfly.top

setmetatable({}, { __index = base })
来源：http://vjk.smart0.xyz

[T41] Perl：Hello World
来源：http://iuh.guowangkeji.top

print "Hello\n";
来源：http://xwc.bbcook.cn

[T42] Perl：变量类型
来源：http://mnx.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mgn.guowangkeji.top

[T43] Perl：字符串插值
来源：http://wpa.316326.xyz

"值: $a"
来源：http://kdg.dashuyun.cn

[T44] Perl：条件
来源：http://rsg.havefunace.top

if ($a > 0) { print "正"; }
来源：http://ccu.xuanzx.com

[T45] Perl：数组遍历
来源：http://avx.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://bhk.zhixingplan.top

[T46] Perl：哈希操作
来源：http://nrl.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vhq.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://pbu.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://adm.jqgufenzy.top

[T48] Perl：正则替换
来源：http://zlf.ybcxt.top

$s =~ s/old/new/g;
来源：http://owo.dianchejie.cn

[T49] Perl：函数
来源：http://iub.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gxp.fehbvm.com

[T50] Perl：逐行读文件
来源：http://ilb.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://alm.zdqjudy.top

while (my $line = <$fh>) { print $line; }
来源：http://ydq.yj202588.top

[T51] Scala：Hello World
来源：http://dsv.ppjwa.cn

println("Hello")
来源：http://hnu.ydzc1.top

[T52] Scala：变量
来源：http://yij.xuetiantiany.cn

val a = 1;  var b = 2
来源：http://wuc.ehwqpu.com

[T53] Scala：字符串插值
来源：http://ccz.sysykeji.top

s"值: $b"
来源：http://uic.tian-w.cn

[T54] Scala：集合映射
来源：http://gia.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://eoo.yueranfly.top

[T55] Scala：集合过滤
来源：http://kts.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hnr.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://iim.jyoumei.cn

case class User(name: String, age: Int)
来源：http://qsg.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://wol.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iza.daxiang520.top

[T58] Scala：函数定义
来源：http://bto.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lnn.shzxlz.cn

[T59] Scala：循环
来源：http://nla.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://rhx.sxryk.cn

[T60] Scala：折叠
来源：http://isu.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uba.andypj.xyz

================================================================================
来源：http://kck.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ceo.pycfn.com

================================================================================
来源：http://rkv.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://pqq.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://kpm.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://gfr.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vdy.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://qjz.fktsv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ohz.yongpay.top

[U04] Py：变量调试打印
来源：http://aal.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nau.guowangkeji.top

[U05] Py：列表去重且保序
来源：http://ywc.andypj.xyz

list(dict.fromkeys(arr))
来源：http://nzw.sysykeji.top

[U06] Py：合并两个字典
来源：http://mxb.jinqigufen.top

{**a, **b}
来源：http://oty.ehwqpu.com

[U07] Py：反转字典键值
来源：http://cjq.hammf.cn

{v: k for k, v in d.items()}
来源：http://pcn.jyoumei.cn

[U08] Py：展平二维列表
来源：http://twp.chenzaomai.com

[y for x in nested for y in x]
来源：http://arz.havefunace.top

[U09] Py：字典取最大值的键
来源：http://aqg.hammf.cn

max(d, key=d.get)
来源：http://nog.vehdjk.com

[U10] Py：按值排序字典
来源：http://aoz.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tdb.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://zvx.ivvv.top

(x * 2 for x in arr)
来源：http://shx.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://tvl.yj20258.top

Counter(arr).most_common(3)
来源：http://imw.sysykeji.top

[U13] Py：固定长度队列
来源：http://ekx.jinqigufen.top

deque(maxlen=10)
来源：http://gul.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://myq.aizwys.cn

defaultdict(list)
来源：http://okk.yj202588.top

[U15] Py：高精度计时
来源：http://rlb.shanyushiyangtech.top

t = time.perf_counter()
来源：http://vhm.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://ili.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gqw.tanke756.top

[U17] Py：初始化日志
来源：http://zqc.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://myo.jinqigufen.top

[U18] Py：预编译正则
来源：http://umt.andypj.xyz

pat = re.compile(r"\d+")
来源：http://uxj.fehbvm.com

[U19] Py：正则替换带回调
来源：http://fsl.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cye.meibo888.top

[U20] Py：缓存函数结果
来源：http://iwg.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://wwv.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://ami.pengpengdd.cyou

@contextlib.contextmanager
来源：http://vvg.yj20258.top

[U22] Py：矩阵转置
来源：http://xbz.yj202588.top

list(zip(*m))
来源：http://qhp.aizwys.cn

[U23] Py：分块读取大文件
来源：http://pen.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fiu.bjfxy.top

[U24] Py：路径操作
来源：http://lup.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zhw.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://zpx.iojbl.cn

csv.DictReader(f)
来源：http://gbd.yvedp.cn

[U26] Py：并发下载
来源：http://gwt.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pgp.xziqi.cn

[U27] Py：异步 HTTP
来源：http://qub.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://ezi.aibaodan.cn

[U28] Py：类型别名
来源：http://xvz.havefunace.top

UserId = int
来源：http://mtj.guowangkeji.top

[U29] Py：属性校验
来源：http://llm.sjlbkw.cn

@property 与 @x.setter 配合
来源：http://ixp.hongshengwenyu.top

[U30] Py：数据类
来源：http://gjc.cqqwz.cn

@dataclass(slots=True)
来源：http://ljs.chenjidiqi.icu

[U31] Py：单测
来源：http://adu.52xcode.cn

python -m pytest -q
来源：http://uod.dianchejie.cn

[U32] Py：代码格式化
来源：http://zhb.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://xpd.xuetiantiany.cn

[U33] Py：打包发布
来源：http://jcs.yj20258.top

python -m build  （依赖 pyproject.toml）
来源：http://ptz.cheryme.top

[U34] Py：判断编码
来源：http://ber.316326.xyz

chardet.detect(raw)
来源：http://phf.cashguo.top

[U35] Py：发送邮件
来源：http://hvt.tian-w.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vrp.xinyue.icu

[U36] Py：定时任务
来源：http://sdr.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://mck.yvedp.cn

[U37] Py：读写 Excel
来源：http://ddk.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://ywq.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://erz.yj20258.top

Path(__file__).resolve().parent
来源：http://jyr.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://bzu.yj20258888.top

sys.stdout.isatty()
来源：http://efa.fengsongda.top

[U40] Py：打印到标准错误
来源：http://zau.fengsongda.top

print("err", file=sys.stderr)
来源：http://ppx.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://oax.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lbx.yangfankeji.com

[U42] PHP：PSR-4 自动加载
来源：http://rwx.jqgufenzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yxr.ydjk.org.cn


<!-- 参考信息 -->