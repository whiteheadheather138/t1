代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://hdp.tarul.cn

[S15] C：类型转换
来源：http://lkf.fehbvm.com

(double) a / b
来源：http://nxw.fengsongda.top

[S16] C：位操作置位
来源：http://meg.ctjpmb.com

x |= (1 << 3);
来源：http://egi.fehbvm.com

[S17] C：安全拼接字符串
来源：http://eda.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vnf.gaohongyu789.top

[S18] C：命令行参数
来源：http://hsl.fehbvm.com

int main(int argc, char **argv)
来源：http://grr.uphjek.com

[S19] C：快速排序
来源：http://ipe.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yov.mhx1999.top

[S20] C：二分查找
来源：http://hrk.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mzj.aizwys.cn

[S21] C：字符类别判断
来源：http://upp.kuanghao11.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sjm.xylfe.cn

[S22] C：字符串转数字
来源：http://env.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yir.fengsongda.top

[S23] C：随机数
来源：http://mgf.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dup.52xcode.cn

[S24] C：获取本地时间
来源：http://dnz.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://loy.pycfn.com

[S25] C：内存拷贝
来源：http://pog.cheryme.top

memcpy(dst, src, n);
来源：http://ubs.cashguo.top

[S26] C：内存清零
来源：http://fbv.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://wxe.yvedp.cn

[S27] C：定义常量
来源：http://ejy.zdqjudy.top

const double PI = 3.14159;
来源：http://bpr.epnwcf.com

[S28] C：静态变量
来源：http://her.sxryk.cn

static int counter = 0;
来源：http://gzu.hfpthk.cn

[S29] C：变参函数
来源：http://lps.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ktt.xuanzx.com

[S30] C：头文件保护
来源：http://uuh.kuanghao11.cn

#ifndef X_H
来源：http://txx.sjlbkw.cn

#define X_H
来源：http://hlt.haohaochexian.top

#endif
来源：http://zdk.wangshuangyany.cn

[S31] C++：Hello World
来源：http://isp.zhoulong.xyz

#include <iostream>
来源：http://bzd.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://hdv.zhengqikj.top

[S32] C++：字符串
来源：http://waf.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://xjq.gaohongyu789.top

[S33] C++：vector 增删
来源：http://nrd.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://juo.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://knt.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://chg.redwolf501.top

[S35] C++：map
来源：http://rdn.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgl.jqgufenzy.top

[S36] C++：unordered_map
来源：http://bez.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qws.xylfe.cn

[S37] C++：set
来源：http://ook.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://osi.pengpengdd.cyou

[S38] C++：排序
来源：http://poy.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://emd.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://lsc.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wxu.yangfankeji.com

[S40] C++：查找元素
来源：http://akw.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sel.zdqjudy.top

[S41] C++：类与构造函数
来源：http://sov.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nae.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://ncc.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://myn.zycfv.cn

[S43] C++：智能指针
来源：http://ubv.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://xoi.daria6918.cn

[S44] C++：引用传参
来源：http://svp.smart0.xyz

void inc(int &x) { ++x; }
来源：http://vsk.iojbl.cn

[S45] C++：lambda
来源：http://ujm.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://suc.gotoacloud.top

[S46] C++：函数模板
来源：http://hgs.xziqi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nvx.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://vak.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vhm.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://lbv.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://tzh.bbcook.cn

while (std::getline(in, line)) { }
来源：http://xvf.hnxiangtu.top

[S49] C++：写文件
来源：http://kpt.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vll.yj202588.top

[S50] C++：格式化数字
来源：http://pbd.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://piq.sysykeji.top

[S51] C++：显式类型转换
来源：http://awe.zdqjudy.top

static_cast<double>(a) / b
来源：http://nfs.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://xjm.hongshengwenyu.top

int size() const noexcept { return n_; }
来源：http://cmu.chenjidiqi.icu

[S53] C++：移动语义
来源：http://ghq.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://raj.aibaodan.cn

[S54] C++：异常处理
来源：http://nkb.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jib.yj20258.top

[S55] C++：结构化绑定
来源：http://yvh.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://odf.fanxiaobao.xyz

[S56] C++：optional
来源：http://nzp.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ihf.bjfxy.top

[S57] C++：编译期常量
来源：http://gkj.zycfv.cn

constexpr int N = 10;
来源：http://gxd.hysaishi.cn

[S58] C++：命名空间
来源：http://orv.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://ygi.zhixingplan.top

[S59] C++：静态断言
来源：http://jjk.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pvq.yongpay.top

[S60] C++：遍历并删除元素
来源：http://clx.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oiq.meibo888.top

================================================================================
来源：http://skm.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aaw.shzxlz.cn

================================================================================
来源：http://pus.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://uan.fanxiaobao.xyz

println("Hello")
来源：http://qbc.zdqjudy.top

[T02] Kotlin：变量
来源：http://qdo.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://paz.hammf.cn

[T03] Kotlin：字符串模板
来源：http://mcw.cucudq.cn

"值: $b"
来源：http://tmd.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://eyz.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://mpz.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://vlh.sweek.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsz.ybcxt.top

[T06] Kotlin：集合映射
来源：http://gzj.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hva.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://mfl.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cun.jqgfzy.top

[T08] Kotlin：数据类
来源：http://idt.yj20258.top

data class User(val name: String, val age: Int)
来源：http://ssh.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://uyc.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://akp.316326.xyz

[T10] Kotlin：默认参数
来源：http://mwp.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jwn.chenzaomai.com

[T11] Kotlin：协程
来源：http://nin.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vfs.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://tab.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://eyk.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://ljx.fehbvm.com

val m = mapOf("a" to 1)
来源：http://ull.tian-w.cn

[T14] Kotlin：循环
来源：http://yoh.daria6918.cn

for (i in 1..10) println(i)
来源：http://rcv.zhixingplan.top

[T15] Kotlin：接口
来源：http://ikd.birdmap.top

interface Shape { fun area(): Double }
来源：http://rcw.guowangkeji.top

[T16] Swift：Hello World
来源：http://pzb.pycfn.com

print("Hello")
来源：http://rrn.gogol.net.cn

[T17] Swift：变量与常量
来源：http://zic.nanxinkj.top

var a = 1;  let b = 2
来源：http://qxu.yj202588.top

[T18] Swift：字符串插值
来源：http://mag.zhiwuduotai.top

"值: \(b)"
来源：http://hju.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://gal.tarul.cn

if let n = opt { print(n) }
来源：http://cea.hnxiangtu.top

[T20] Swift：数组操作
来源：http://vdl.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ofg.jinqigufen.top

[T21] Swift：遍历
来源：http://baw.316326.xyz

for x in a { print(x) }
来源：http://ktq.hongshengwenyu.top

[T22] Swift：字典
来源：http://mht.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://wmz.uphjek.com

[T23] Swift：函数
来源：http://ilq.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://stv.haohaochexian.top

[T24] Swift：闭包
来源：http://vsh.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pyh.gotoacloud.top

[T25] Swift：结构体
来源：http://zzh.yj20258888.top

struct P { var x: Int }
来源：http://ryf.xingfuxueyuan.xyz

[T26] Swift：类与重写
来源：http://vwk.shuidangran.top

class A: Base { override func f() {} }
来源：http://vrn.chenlongwang.top

[T27] Swift：错误处理
来源：http://uyh.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://qst.yj202588.top

[T28] Swift：枚举
来源：http://ksx.yangfankeji.com

enum Color { case red, green }
来源：http://dvb.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://kvk.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://ffy.daxiang520.top

[T30] Swift：协议
来源：http://npi.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://nkx.fehbvm.com

[T31] Lua：Hello World
来源：http://ips.xziqi.cn

print("Hello")
来源：http://vqw.andypj.xyz

[T32] Lua：局部变量
来源：http://cce.smart0.xyz

local a = 1
来源：http://gea.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://rho.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://myi.jqgfzy.top

[T34] Lua：遍历表
来源：http://yej.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://mvo.hywenlv.cn

[T35] Lua：字典表
来源：http://pdu.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://qwx.fengsongda.top

[T36] Lua：函数
来源：http://yjl.nwbrower.top

function add(a, b) return a + b end
来源：http://dvl.mhx1999.top

[T37] Lua：字符串拼接
来源：http://asx.shangyingyoupin.top

"a" .. "b"
来源：http://qvd.nwbrower.top

[T38] Lua：条件
来源：http://amm.yfazqb.com

if x > 0 then print("正") end
来源：http://rmn.xylfe.cn

[T39] Lua：模式匹配
来源：http://bjw.sweek.top

string.find(s, "%d+")
来源：http://nms.cqqwz.cn

[T40] Lua：元表
来源：http://rxd.yuxming.cn

setmetatable({}, { __index = base })
来源：http://kjm.yj20258.top

[T41] Perl：Hello World
来源：http://rre.bbcook.cn

print "Hello\n";
来源：http://gie.fehbvm.com

[T42] Perl：变量类型
来源：http://ftn.sweek.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nrk.9152youxi.cn

[T43] Perl：字符串插值
来源：http://wwu.hnxiangtu.top

"值: $a"
来源：http://zoo.hysaishi.cn

[T44] Perl：条件
来源：http://via.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://sag.yueranfly.top

[T45] Perl：数组遍历
来源：http://unj.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://gkq.haohaochexian.top

[T46] Perl：哈希操作
来源：http://hey.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qyu.fehbvm.com

[T47] Perl：正则捕获
来源：http://rzn.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://cqo.tanke756.top

[T48] Perl：正则替换
来源：http://pqg.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://iyu.316326.xyz

[T49] Perl：函数
来源：http://ihx.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://okv.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://qkk.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ooa.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://xpb.gogol.net.cn

[T51] Scala：Hello World
来源：http://fxk.vehdjk.com

println("Hello")
来源：http://oxc.c1oappe.top

[T52] Scala：变量
来源：http://osu.redwolf501.top

val a = 1;  var b = 2
来源：http://fmf.yj20258888.top

[T53] Scala：字符串插值
来源：http://xfi.jinqigufen.top

s"值: $b"
来源：http://umx.fehbvm.com

[T54] Scala：集合映射
来源：http://svd.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://drg.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://zwt.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://ndf.fengsongda.top

[T56] Scala：样例类
来源：http://ycy.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://znt.yongpay.top

[T57] Scala：模式匹配
来源：http://dxl.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qzx.yuanzhike.top

[T58] Scala：函数定义
来源：http://wod.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://jbf.yanxiufei.cn

[T59] Scala：循环
来源：http://pnw.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://eta.nwbrower.top

[T60] Scala：折叠
来源：http://yrk.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://obt.wangshuangyany.cn

================================================================================
来源：http://hfw.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://asv.tanke756.top

================================================================================
来源：http://shh.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://ors.gogol.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iew.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://cux.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tma.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://dzi.52xcode.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ecm.0kj1m.cn

[U04] Py：变量调试打印
来源：http://qfp.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sgs.xuanzx.com

[U05] Py：列表去重且保序
来源：http://rwq.yongpay.top

list(dict.fromkeys(arr))
来源：http://jfw.bbcook.cn

[U06] Py：合并两个字典
来源：http://hns.nanxuanxn.top

{**a, **b}
来源：http://qjp.tarul.cn

[U07] Py：反转字典键值
来源：http://uds.sysykeji.top

{v: k for k, v in d.items()}
来源：http://brr.yj20258888.top

[U08] Py：展平二维列表
来源：http://kjo.yanxiufei.cn

[y for x in nested for y in x]
来源：http://kqb.cqqwz.cn

[U09] Py：字典取最大值的键
来源：http://ljt.epnwcf.com

max(d, key=d.get)
来源：http://ftr.dashuyun.cn

[U10] Py：按值排序字典
来源：http://vww.c1oappe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aet.tanke756.top

[U11] Py：生成器表达式
来源：http://egq.zdqjudy.top

(x * 2 for x in arr)
来源：http://dbc.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://kqf.cqqwz.cn

Counter(arr).most_common(3)
来源：http://pvw.jinqigufen.top

[U13] Py：固定长度队列
来源：http://odr.kuanghao11.cn

deque(maxlen=10)
来源：http://nlb.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://uhv.zdqjudy.top

defaultdict(list)
来源：http://tfy.hnqzz.top

[U15] Py：高精度计时
来源：http://mfw.mhx1999.top

t = time.perf_counter()
来源：http://wns.jinqigufen.top

[U16] Py：命令行参数解析
来源：http://bjf.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jtp.xinyue.icu

[U17] Py：初始化日志
来源：http://qkq.zhijiandao.cn

logging.basicConfig(level=logging.INFO)
来源：http://qrt.fzhhl.top

[U18] Py：预编译正则
来源：http://bit.zhaomingkeji.xyz

pat = re.compile(r"\d+")
来源：http://dgz.jiagoushi.top

[U19] Py：正则替换带回调
来源：http://cqq.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tqh.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://rpc.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://fsn.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://wom.cucudq.cn

@contextlib.contextmanager
来源：http://bdy.andypj.xyz

[U22] Py：矩阵转置
来源：http://fgq.ydjk.org.cn

list(zip(*m))
来源：http://oxy.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://shb.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ijw.9152youxi.cn

[U24] Py：路径操作
来源：http://lta.hysaishi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://urs.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://pmp.gaohongyu789.top

csv.DictReader(f)
来源：http://bpy.dashuyun.cn

[U26] Py：并发下载
来源：http://fox.yvedp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xmc.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://gks.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://nhh.jinqigfzy.top

[U28] Py：类型别名
来源：http://tpp.iojbl.cn

UserId = int
来源：http://fax.zdqjudy.top

[U29] Py：属性校验
来源：http://xvk.zhoulong.xyz

@property 与 @x.setter 配合
来源：http://qul.quarkkingdee.top

[U30] Py：数据类
来源：http://oqc.hesvh.cn

@dataclass(slots=True)
来源：http://fmb.yj202588.top

[U31] Py：单测
来源：http://owx.xuetiantiany.cn

python -m pytest -q
来源：http://bhy.shzxlz.cn

[U32] Py：代码格式化
来源：http://yal.gotoacloud.top

ruff format . && ruff check --fix .
来源：http://hgl.sweek.top

[U33] Py：打包发布
来源：http://liq.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ile.wangshuangyany.cn

[U34] Py：判断编码
来源：http://zta.guowangkeji.top

chardet.detect(raw)
来源：http://tgf.smart0.xyz

[U35] Py：发送邮件
来源：http://daz.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ymj.ydjk.org.cn

[U36] Py：定时任务
来源：http://qpz.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://fbu.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://wzu.redwolf501.top

pandas.read_excel / DataFrame.to_excel
来源：http://qhl.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://kzb.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://sjk.hesvh.cn


<!-- 参考信息 -->