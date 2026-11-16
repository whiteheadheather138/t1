代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://fbh.jiagoushi.top

[S15] C：类型转换
来源：http://idw.jinqigufen.top

(double) a / b
来源：http://nlr.tanke756.top

[S16] C：位操作置位
来源：http://dnn.zdqjudy.top

x |= (1 << 3);
来源：http://rcu.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://til.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jkm.zhijiandao.cn

[S18] C：命令行参数
来源：http://bol.dashuyun.cn

int main(int argc, char **argv)
来源：http://iin.ehwqpu.com

[S19] C：快速排序
来源：http://btx.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://amh.cheryme.top

[S20] C：二分查找
来源：http://nth.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ykz.ydjk.org.cn

[S21] C：字符类别判断
来源：http://hzp.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kiq.chenzaomai.com

[S22] C：字符串转数字
来源：http://jrw.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mgm.daxiang520.top

[S23] C：随机数
来源：http://dce.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://vsv.birdmap.top

[S24] C：获取本地时间
来源：http://thv.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qih.birdmap.top

[S25] C：内存拷贝
来源：http://obs.ydzc1.top

memcpy(dst, src, n);
来源：http://eyn.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://wwb.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://xat.fktsv.cn

[S27] C：定义常量
来源：http://sia.bjfxy.top

const double PI = 3.14159;
来源：http://pbw.0kj1m.cn

[S28] C：静态变量
来源：http://kty.bbcook.cn

static int counter = 0;
来源：http://gkw.zdbjq.cn

[S29] C：变参函数
来源：http://hqh.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qab.ydjk.org.cn

[S30] C：头文件保护
来源：http://nni.chenjidiqi.icu

#ifndef X_H
来源：http://buw.316326.xyz

#define X_H
来源：http://idp.ehwqpu.com

#endif
来源：http://xck.nwbrower.top

[S31] C++：Hello World
来源：http://ghk.hnqzz.top

#include <iostream>
来源：http://zsn.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://kyv.fktsv.cn

[S32] C++：字符串
来源：http://xtp.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://qpv.jiagoushi.top

[S33] C++：vector 增删
来源：http://thp.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cqo.daria6918.cn

[S34] C++：遍历 vector
来源：http://hoy.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://ska.zhijiandao.cn

[S35] C++：map
来源：http://xqg.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ree.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://glp.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ztj.zhoulong.xyz

[S37] C++：set
来源：http://hst.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nyt.tarul.cn

[S38] C++：排序
来源：http://thl.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://stz.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://qwr.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fjf.ybcxt.top

[S40] C++：查找元素
来源：http://jfb.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://izu.tanke756.top

[S41] C++：类与构造函数
来源：http://oxk.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hlr.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://ewp.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://hea.xylfe.cn

[S43] C++：智能指针
来源：http://hoz.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://ajx.jinqigfzy.top

[S44] C++：引用传参
来源：http://uoa.yueranfly.top

void inc(int &x) { ++x; }
来源：http://qiq.shangyingyoupin.top

[S45] C++：lambda
来源：http://ggh.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ifv.redwolf501.top

[S46] C++：函数模板
来源：http://baa.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afk.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://ios.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mtr.wangdashe.top

[S48] C++：逐行读文件
来源：http://ivm.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://lfh.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://mmg.gotoacloud.top

[S49] C++：写文件
来源：http://jfu.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jyr.gotoacloud.top

[S50] C++：格式化数字
来源：http://fly.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xpk.chenlongwang.top

[S51] C++：显式类型转换
来源：http://jfk.0kj1m.cn

static_cast<double>(a) / b
来源：http://cpz.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://nrk.cashguo.top

int size() const noexcept { return n_; }
来源：http://jha.hcnkem.com

[S53] C++：移动语义
来源：http://vda.meibo888.top

std::vector<int> w = std::move(v);
来源：http://lbn.fktsv.cn

[S54] C++：异常处理
来源：http://ant.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lnu.zhixingplan.top

[S55] C++：结构化绑定
来源：http://dnv.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://vva.cqqwz.cn

[S56] C++：optional
来源：http://flh.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://arv.ehwqpu.com

[S57] C++：编译期常量
来源：http://nka.aizwys.cn

constexpr int N = 10;
来源：http://ltp.hfpthk.cn

[S58] C++：命名空间
来源：http://lyg.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://git.jianghu66.top

[S59] C++：静态断言
来源：http://ztj.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mxb.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://hbb.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fdf.cucudq.cn

================================================================================
来源：http://yly.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ppg.shzxlz.cn

================================================================================
来源：http://dpc.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://nzu.yj20258.top

println("Hello")
来源：http://szk.hnqzz.top

[T02] Kotlin：变量
来源：http://ams.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssp.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://rzn.haohaochexian.top

"值: $b"
来源：http://ply.chenlongwang.top

[T04] Kotlin：空安全
来源：http://yhc.9152youxi.cn

val n: String? = null;  n?.length
来源：http://rnr.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://phm.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eil.xuanzx.com

[T06] Kotlin：集合映射
来源：http://bik.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rke.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://qro.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dha.zdqjudy.top

[T08] Kotlin：数据类
来源：http://pfb.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://ynu.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://nuk.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://wvj.vehdjk.com

[T10] Kotlin：默认参数
来源：http://gix.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ixr.hywenlv.cn

[T11] Kotlin：协程
来源：http://fkj.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eei.yj20258888.top

[T12] Kotlin：解构声明
来源：http://ohd.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://tqq.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://qdi.hesvh.cn

val m = mapOf("a" to 1)
来源：http://hmh.epnwcf.com

[T14] Kotlin：循环
来源：http://oto.hywenlv.cn

for (i in 1..10) println(i)
来源：http://cgz.sufxvd.cn

[T15] Kotlin：接口
来源：http://yne.52xcode.cn

interface Shape { fun area(): Double }
来源：http://suw.redwolf501.top

[T16] Swift：Hello World
来源：http://nba.zycfv.cn

print("Hello")
来源：http://qrs.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://dqy.316326.xyz

var a = 1;  let b = 2
来源：http://shs.dashuyun.cn

[T18] Swift：字符串插值
来源：http://dkv.jqgufenzy.top

"值: \(b)"
来源：http://lfs.c1oappe.top

[T19] Swift：可选绑定
来源：http://ugh.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://acs.bbcook.cn

[T20] Swift：数组操作
来源：http://qxj.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://bjc.uphjek.com

[T21] Swift：遍历
来源：http://olr.yueranfly.top

for x in a { print(x) }
来源：http://eig.shangyingyoupin.top

[T22] Swift：字典
来源：http://axi.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://lwk.fehbvm.com

[T23] Swift：函数
来源：http://tqp.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cro.wangdashe.top

[T24] Swift：闭包
来源：http://afc.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mug.yj20258.top

[T25] Swift：结构体
来源：http://hgq.quarkkingdee.top

struct P { var x: Int }
来源：http://xdb.chenzaomai.com

[T26] Swift：类与重写
来源：http://xtj.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://vgq.mhx1999.top

[T27] Swift：错误处理
来源：http://idh.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://rzp.hywenlv.cn

[T28] Swift：枚举
来源：http://nec.haohaochexian.top

enum Color { case red, green }
来源：http://yks.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://enk.andypj.xyz

guard let x = opt else { return }
来源：http://bib.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://xby.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://dgx.hfpthk.cn

[T31] Lua：Hello World
来源：http://gkp.tarul.cn

print("Hello")
来源：http://lpa.kuanghao11.cn

[T32] Lua：局部变量
来源：http://xio.chenjidiqi.icu

local a = 1
来源：http://quo.yfazqb.com

[T33] Lua：表（数组）
来源：http://aiv.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lfc.redwolf501.top

[T34] Lua：遍历表
来源：http://hfd.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gxw.dashuyun.cn

[T35] Lua：字典表
来源：http://nmg.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://xfa.shangyingyoupin.top

[T36] Lua：函数
来源：http://sso.yvedp.cn

function add(a, b) return a + b end
来源：http://pbh.daria6918.cn

[T37] Lua：字符串拼接
来源：http://vac.sweek.top

"a" .. "b"
来源：http://djm.guowangkeji.top

[T38] Lua：条件
来源：http://mjv.hongshengwenyu.top

if x > 0 then print("正") end
来源：http://mjf.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://xtl.redwolf501.top

string.find(s, "%d+")
来源：http://qbz.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://qil.yfazqb.com

setmetatable({}, { __index = base })
来源：http://vdf.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://wfo.hnxiangtu.top

print "Hello\n";
来源：http://qlb.0kj1m.cn

[T42] Perl：变量类型
来源：http://yje.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jfj.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://kpo.sysykeji.top

"值: $a"
来源：http://vej.xziqi.cn

[T44] Perl：条件
来源：http://xvo.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://ane.ivvv.top

[T45] Perl：数组遍历
来源：http://mpc.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://enb.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://adv.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bcs.vehdjk.com

[T47] Perl：正则捕获
来源：http://fqp.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yhn.tian-w.cn

[T48] Perl：正则替换
来源：http://rdb.52xcode.cn

$s =~ s/old/new/g;
来源：http://dwp.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://fzh.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vml.shuidangran.top

[T50] Perl：逐行读文件
来源：http://yxk.hesvh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pay.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://tjq.daria6918.cn

[T51] Scala：Hello World
来源：http://sik.zdqjudy.top

println("Hello")
来源：http://svj.fanxiaobao.xyz

[T52] Scala：变量
来源：http://zoh.aizwys.cn

val a = 1;  var b = 2
来源：http://xse.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://apz.mhx1999.top

s"值: $b"
来源：http://iuq.316326.xyz

[T54] Scala：集合映射
来源：http://jma.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ptp.fktsv.cn

[T55] Scala：集合过滤
来源：http://mvf.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vvu.sweek.top

[T56] Scala：样例类
来源：http://aid.jianghu66.top

case class User(name: String, age: Int)
来源：http://vpt.iojbl.cn

[T57] Scala：模式匹配
来源：http://mbe.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ieq.shuidangran.top

[T58] Scala：函数定义
来源：http://owa.hfpthk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mrk.jinqigfzy.top

[T59] Scala：循环
来源：http://fcb.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://gez.fengsongda.top

[T60] Scala：折叠
来源：http://iuo.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfr.zhongyouzk.top

================================================================================
来源：http://lso.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vfj.feifeiyinyue.top

================================================================================
来源：http://pkn.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://mgn.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rqx.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://rfz.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mnc.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://crn.hysaishi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iar.hnqzz.top

[U04] Py：变量调试打印
来源：http://qkh.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://izb.yueranfly.top

[U05] Py：列表去重且保序
来源：http://pmb.bbcook.cn

list(dict.fromkeys(arr))
来源：http://nfd.hammf.cn

[U06] Py：合并两个字典
来源：http://qmt.fktsv.cn

{**a, **b}
来源：http://meq.nwbrower.top

[U07] Py：反转字典键值
来源：http://rev.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://pqg.cheryme.top

[U08] Py：展平二维列表
来源：http://rkm.quarkkingdee.top

[y for x in nested for y in x]
来源：http://rmx.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://pul.yuanzhike.top

max(d, key=d.get)
来源：http://bsl.0kj1m.cn

[U10] Py：按值排序字典
来源：http://gdz.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mur.yueranfly.top

[U11] Py：生成器表达式
来源：http://pva.sufxvd.cn

(x * 2 for x in arr)
来源：http://kjj.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://oqm.ydzc1.top

Counter(arr).most_common(3)
来源：http://ueq.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://zro.zhiwuduotai.top

deque(maxlen=10)
来源：http://rhe.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://ejz.yongpay.top

defaultdict(list)
来源：http://usl.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://rjl.xziqi.cn

t = time.perf_counter()
来源：http://joz.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://mgk.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dfl.yonumen.top

[U17] Py：初始化日志
来源：http://uhs.jyoumei.cn

logging.basicConfig(level=logging.INFO)
来源：http://ojh.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://vid.zhengqikj.top

pat = re.compile(r"\d+")
来源：http://ims.hnqzz.top

[U19] Py：正则替换带回调
来源：http://ben.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vsh.xuanzx.com

[U20] Py：缓存函数结果
来源：http://yrg.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://dbx.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://bpy.kuanghao11.cn

@contextlib.contextmanager
来源：http://gie.pengpengdd.cyou

[U22] Py：矩阵转置
来源：http://ihj.hysaishi.cn

list(zip(*m))
来源：http://ctm.hnqzz.top

[U23] Py：分块读取大文件
来源：http://kga.yj20258.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gqq.cheryme.top

[U24] Py：路径操作
来源：http://cfn.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kiz.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://twi.sjlbkw.cn

csv.DictReader(f)
来源：http://elt.hcnkem.com

[U26] Py：并发下载
来源：http://dby.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nwy.dianchejie.cn

[U27] Py：异步 HTTP
来源：http://ebo.smart0.xyz

aiohttp.ClientSession() 配合 async with
来源：http://rib.xuanzx.com

[U28] Py：类型别名
来源：http://coy.tianlin.xyz

UserId = int
来源：http://oph.pycfn.com

[U29] Py：属性校验
来源：http://sxa.dashuyun.cn

@property 与 @x.setter 配合
来源：http://ghu.yj20258.top

[U30] Py：数据类
来源：http://dgb.birdmap.top

@dataclass(slots=True)
来源：http://vjc.fanxiaobao.xyz

[U31] Py：单测
来源：http://sxs.zdbjq.cn

python -m pytest -q
来源：http://acy.ybcxt.top

[U32] Py：代码格式化
来源：http://cyd.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://ubf.ivvv.top

[U33] Py：打包发布
来源：http://tln.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://nqv.jyoumei.cn

[U34] Py：判断编码
来源：http://mjf.xylfe.cn

chardet.detect(raw)
来源：http://ugl.gotoacloud.top

[U35] Py：发送邮件
来源：http://imr.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kka.jinqigfzy.top

[U36] Py：定时任务
来源：http://qjc.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://zme.zhengqikj.top

[U37] Py：读写 Excel
来源：http://kbo.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://qgw.chenjidiqi.icu

[U38] Py：获取脚本所在目录
来源：http://qyg.xinyue.icu

Path(__file__).resolve().parent
来源：http://otm.sysykeji.top


<!-- 参考信息 -->