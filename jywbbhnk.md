代发 wailian999

x |= (1 << 3);
来源：http://hug.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://vnx.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csv.9152youxi.cn

[S18] C：命令行参数
来源：http://ymk.shuidangran.top

int main(int argc, char **argv)
来源：http://xox.tianlin.xyz

[S19] C：快速排序
来源：http://ddj.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://cnu.redwolf501.top

[S20] C：二分查找
来源：http://cbz.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bom.andypj.xyz

[S21] C：字符类别判断
来源：http://clk.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ash.sufxvd.cn

[S22] C：字符串转数字
来源：http://red.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://rgq.xinyue.icu

[S23] C：随机数
来源：http://ydv.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uzt.shuidangran.top

[S24] C：获取本地时间
来源：http://lyw.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yip.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://mjy.zhijiandao.cn

memcpy(dst, src, n);
来源：http://gog.quarkkingdee.top

[S26] C：内存清零
来源：http://ebd.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://dlw.9152youxi.cn

[S27] C：定义常量
来源：http://vpo.feifeiyinyue.top

const double PI = 3.14159;
来源：http://stg.hnqzz.top

[S28] C：静态变量
来源：http://phj.zhengqikj.top

static int counter = 0;
来源：http://mvy.zhixingplan.top

[S29] C：变参函数
来源：http://dpz.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rak.yfazqb.com

[S30] C：头文件保护
来源：http://zsb.zhaomingkeji.xyz

#ifndef X_H
来源：http://oda.nanxinkj.top

#define X_H
来源：http://wbl.xinyue.icu

#endif
来源：http://fhy.pycfn.com

[S31] C++：Hello World
来源：http://xnq.meibo888.top

#include <iostream>
来源：http://skl.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://xcu.ppjwa.cn

[S32] C++：字符串
来源：http://oas.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://sem.dianchejie.cn

[S33] C++：vector 增删
来源：http://qzi.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://usv.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://bcd.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://iir.bbcook.cn

[S35] C++：map
来源：http://coi.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wxi.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://usn.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwd.zdqjudy.top

[S37] C++：set
来源：http://ncg.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jsb.nwbrower.top

[S38] C++：排序
来源：http://ycp.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://huf.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://dpw.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ibh.tianlin.xyz

[S40] C++：查找元素
来源：http://spf.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dld.xinyue.icu

[S41] C++：类与构造函数
来源：http://cdc.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://emn.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://stc.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://xod.yanxiufei.cn

[S43] C++：智能指针
来源：http://alo.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://ipl.chenjidiqi.icu

[S44] C++：引用传参
来源：http://hxx.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://hlx.jinqigufen.top

[S45] C++：lambda
来源：http://zvi.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://mbw.haohaochexian.top

[S46] C++：函数模板
来源：http://rfn.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zdb.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://wzv.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jno.vehdjk.com

[S48] C++：逐行读文件
来源：http://bug.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://emr.ivvv.top

while (std::getline(in, line)) { }
来源：http://nrr.hammf.cn

[S49] C++：写文件
来源：http://qqb.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pce.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://ujo.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://djx.sweek.top

[S51] C++：显式类型转换
来源：http://axr.aizwys.cn

static_cast<double>(a) / b
来源：http://cds.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://qrn.yonumen.top

int size() const noexcept { return n_; }
来源：http://pho.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://bbu.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://gov.iojbl.cn

[S54] C++：异常处理
来源：http://ffm.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eek.andypj.xyz

[S55] C++：结构化绑定
来源：http://wfw.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cql.bbcook.cn

[S56] C++：optional
来源：http://soi.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jmz.fzhhl.top

[S57] C++：编译期常量
来源：http://ykl.sweek.top

constexpr int N = 10;
来源：http://lzz.ybcxt.top

[S58] C++：命名空间
来源：http://fdj.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://adt.hywenlv.cn

[S59] C++：静态断言
来源：http://ptp.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vmj.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://ejc.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lnb.xuetiantiany.cn

================================================================================
来源：http://imi.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ail.gotoacloud.top

================================================================================
来源：http://cmn.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://voq.gotoacloud.top

println("Hello")
来源：http://vsq.daria6918.cn

[T02] Kotlin：变量
来源：http://slu.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qqn.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://dsa.cheryme.top

"值: $b"
来源：http://bpt.zdbjq.cn

[T04] Kotlin：空安全
来源：http://sra.shuidangran.top

val n: String? = null;  n?.length
来源：http://gle.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ila.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bgw.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://qxg.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://swm.sweek.top

[T07] Kotlin：集合过滤
来源：http://rjt.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bqi.cucudq.cn

[T08] Kotlin：数据类
来源：http://fgc.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://hmz.ivvv.top

[T09] Kotlin：扩展函数
来源：http://lxw.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://ljo.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://kev.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wmx.hywenlv.cn

[T11] Kotlin：协程
来源：http://mbq.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xov.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://pia.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://lyp.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://sen.yj202588.top

val m = mapOf("a" to 1)
来源：http://uzj.tanke756.top

[T14] Kotlin：循环
来源：http://vao.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://cww.uphjek.com

[T15] Kotlin：接口
来源：http://doo.yj20258888.top

interface Shape { fun area(): Double }
来源：http://ypp.yueranfly.top

[T16] Swift：Hello World
来源：http://hzq.gaohongyu789.top

print("Hello")
来源：http://uss.yuanzhike.top

[T17] Swift：变量与常量
来源：http://bjf.jyoumei.cn

var a = 1;  let b = 2
来源：http://jcg.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://elw.smart0.xyz

"值: \(b)"
来源：http://tmy.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://nmo.hnxiangtu.top

if let n = opt { print(n) }
来源：http://dis.yj20258.top

[T20] Swift：数组操作
来源：http://ppc.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://oru.meibo888.top

[T21] Swift：遍历
来源：http://bfi.guannengcc.top

for x in a { print(x) }
来源：http://def.gaohongyu789.top

[T22] Swift：字典
来源：http://dkd.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mco.xuanzx.com

[T23] Swift：函数
来源：http://rcx.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://civ.nanxinkj.top

[T24] Swift：闭包
来源：http://iln.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ctv.hesvh.cn

[T25] Swift：结构体
来源：http://bhj.gzhubu.top

struct P { var x: Int }
来源：http://emp.yfazqb.com

[T26] Swift：类与重写
来源：http://tve.snrcjt.cn

class A: Base { override func f() {} }
来源：http://ilj.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://spk.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://mty.yuanzhike.top

[T28] Swift：枚举
来源：http://rct.ydzc1.top

enum Color { case red, green }
来源：http://qku.pycfn.com

[T29] Swift：guard 提前返回
来源：http://ens.zhiwuduotai.top

guard let x = opt else { return }
来源：http://ajv.0kj1m.cn

[T30] Swift：协议
来源：http://omi.sweek.top

protocol Shape { func area() -> Double }
来源：http://wwc.svipenyu.cn

[T31] Lua：Hello World
来源：http://gzd.zhaomingkeji.xyz

print("Hello")
来源：http://xdg.shzxlz.cn

[T32] Lua：局部变量
来源：http://oix.zdqjudy.top

local a = 1
来源：http://ayz.dianchejie.cn

[T33] Lua：表（数组）
来源：http://gys.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dbu.yongpay.top

[T34] Lua：遍历表
来源：http://leh.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yee.zycfv.cn

[T35] Lua：字典表
来源：http://bcu.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://eee.daxiang520.top

[T36] Lua：函数
来源：http://puk.redwolf501.top

function add(a, b) return a + b end
来源：http://zfc.fzhhl.top

[T37] Lua：字符串拼接
来源：http://nxn.chenlongwang.top

"a" .. "b"
来源：http://stj.yfazqb.com

[T38] Lua：条件
来源：http://guo.yonumen.top

if x > 0 then print("正") end
来源：http://ece.sufxvd.cn

[T39] Lua：模式匹配
来源：http://nss.sysykeji.top

string.find(s, "%d+")
来源：http://okj.ydjk.org.cn

[T40] Lua：元表
来源：http://qln.gzhubu.top

setmetatable({}, { __index = base })
来源：http://hea.zhongyouzk.top

[T41] Perl：Hello World
来源：http://gkd.gogol.net.cn

print "Hello\n";
来源：http://tbk.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://doy.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rzi.jiagoushi.top

[T43] Perl：字符串插值
来源：http://dqp.52xcode.cn

"值: $a"
来源：http://sbj.guowangkeji.top

[T44] Perl：条件
来源：http://nvx.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://ozk.jyoumei.cn

[T45] Perl：数组遍历
来源：http://mlo.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://dxa.xinyue.icu

[T46] Perl：哈希操作
来源：http://glo.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zru.yvedp.cn

[T47] Perl：正则捕获
来源：http://kjk.hongshengwenyu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xwx.hesvh.cn

[T48] Perl：正则替换
来源：http://guk.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://jlz.fzhhl.top

[T49] Perl：函数
来源：http://jlh.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tcf.yvedp.cn

[T50] Perl：逐行读文件
来源：http://don.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://djq.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://olh.316326.xyz

[T51] Scala：Hello World
来源：http://aid.ehwqpu.com

println("Hello")
来源：http://czr.jinqigufen.top

[T52] Scala：变量
来源：http://wdp.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://tpi.jqgfzy.top

[T53] Scala：字符串插值
来源：http://emj.nwbrower.top

s"值: $b"
来源：http://tti.zhijiandao.cn

[T54] Scala：集合映射
来源：http://zgg.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://mvi.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://exr.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dgx.fzhhl.top

[T56] Scala：样例类
来源：http://tbg.sufxvd.cn

case class User(name: String, age: Int)
来源：http://afn.yuanzhike.top

[T57] Scala：模式匹配
来源：http://zsy.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jbr.havefunace.top

[T58] Scala：函数定义
来源：http://wgp.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://mkj.tanke756.top

[T59] Scala：循环
来源：http://etq.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://rng.quarkkingdee.top

[T60] Scala：折叠
来源：http://nct.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xnz.0kj1m.cn

================================================================================
来源：http://bzm.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xex.gzhubu.top

================================================================================
来源：http://hua.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://sgy.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xov.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://tat.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://deq.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://qin.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://ayg.sysykeji.top

[U04] Py：变量调试打印
来源：http://vby.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pqq.cheryme.top

[U05] Py：列表去重且保序
来源：http://fxs.epnwcf.com

list(dict.fromkeys(arr))
来源：http://oyq.jiagoushi.top

[U06] Py：合并两个字典
来源：http://ykq.zhixingplan.top

{**a, **b}
来源：http://kqe.aibaodan.cn

[U07] Py：反转字典键值
来源：http://ofg.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://tqh.zhengqikj.top

[U08] Py：展平二维列表
来源：http://wcf.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://xgr.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://jos.yanxiufei.cn

max(d, key=d.get)
来源：http://fhj.dashuyun.cn

[U10] Py：按值排序字典
来源：http://sph.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syo.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://hgw.uphjek.com

(x * 2 for x in arr)
来源：http://qby.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://kww.hammf.cn

Counter(arr).most_common(3)
来源：http://qpm.andypj.xyz

[U13] Py：固定长度队列
来源：http://kzq.gogol.net.cn

deque(maxlen=10)
来源：http://oiy.yj20258.top

[U14] Py：分组收集到列表
来源：http://cbt.shanyushiyangkeji.top

defaultdict(list)
来源：http://zge.vehdjk.com

[U15] Py：高精度计时
来源：http://ukb.havefunace.top

t = time.perf_counter()
来源：http://xtx.yonumen.top

[U16] Py：命令行参数解析
来源：http://jof.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://del.hesvh.cn

[U17] Py：初始化日志
来源：http://kln.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://vxh.hcnkem.com

[U18] Py：预编译正则
来源：http://ktb.bbcook.cn

pat = re.compile(r"\d+")
来源：http://vqz.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://ugg.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tmz.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://mmn.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://cni.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://gys.tianlin.xyz

@contextlib.contextmanager
来源：http://yne.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://lxb.yonumen.top

list(zip(*m))
来源：http://txu.hammf.cn

[U23] Py：分块读取大文件
来源：http://fjp.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://atb.xuanzx.com

[U24] Py：路径操作
来源：http://otm.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qol.tanke756.top

[U25] Py：CSV 按字典读
来源：http://xgh.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://kjg.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://dsq.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tvf.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://zhz.gzhubu.top

aiohttp.ClientSession() 配合 async with
来源：http://ohj.yj202588.top

[U28] Py：类型别名
来源：http://gor.jqgufenzy.top

UserId = int
来源：http://ami.xinyue.icu

[U29] Py：属性校验
来源：http://nfw.chenzaomai.com

@property 与 @x.setter 配合
来源：http://rjb.redwolf501.top

[U30] Py：数据类
来源：http://srh.tianlin.xyz

@dataclass(slots=True)
来源：http://ehr.iojbl.cn

[U31] Py：单测
来源：http://qjg.zhixingplan.top

python -m pytest -q
来源：http://uqx.vehdjk.com

[U32] Py：代码格式化
来源：http://myy.bbcook.cn

ruff format . && ruff check --fix .
来源：http://gto.hfpthk.cn

[U33] Py：打包发布
来源：http://fiy.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://nhy.cheryme.top

[U34] Py：判断编码
来源：http://uhy.feifeiyinyue.top

chardet.detect(raw)
来源：http://twu.tarul.cn

[U35] Py：发送邮件
来源：http://vyi.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fyf.zycfv.cn

[U36] Py：定时任务
来源：http://qsh.shangyingyoupin.top

schedule.every(10).minutes.do(job)
来源：http://cxi.snrcjt.cn

[U37] Py：读写 Excel
来源：http://reb.0kj1m.cn

pandas.read_excel / DataFrame.to_excel
来源：http://goe.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://fvn.sysykeji.top

Path(__file__).resolve().parent
来源：http://wos.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://qzt.yonumen.top

sys.stdout.isatty()
来源：http://sdx.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://urz.shuidangran.top

print("err", file=sys.stderr)
来源：http://ktu.bbcook.cn


<!-- 参考信息 -->