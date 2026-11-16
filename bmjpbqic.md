代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cni.meibo888.top

[S13] C：宏定义
来源：http://jla.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzd.xuetiantiany.cn

[S14] C：枚举
来源：http://nlu.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://dyq.cucudq.cn

[S15] C：类型转换
来源：http://diq.vehdjk.com

(double) a / b
来源：http://zub.xylfe.cn

[S16] C：位操作置位
来源：http://qrr.jqgufenzy.top

x |= (1 << 3);
来源：http://uaa.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://vte.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cpa.aibaodan.cn

[S18] C：命令行参数
来源：http://tcg.dashuyun.cn

int main(int argc, char **argv)
来源：http://ifh.daxiang520.top

[S19] C：快速排序
来源：http://dns.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://ylx.sjlbkw.cn

[S20] C：二分查找
来源：http://ldp.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nyr.gotoacloud.top

[S21] C：字符类别判断
来源：http://kkm.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uqf.jqgufenzy.top

[S22] C：字符串转数字
来源：http://jbm.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://rko.daxiang520.top

[S23] C：随机数
来源：http://hax.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sgq.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://vtu.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iqv.yj20258.top

[S25] C：内存拷贝
来源：http://oxn.nanxuanxn.top

memcpy(dst, src, n);
来源：http://lnb.quarkkingdee.top

[S26] C：内存清零
来源：http://ndz.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://hpz.havefunace.top

[S27] C：定义常量
来源：http://ltx.vehdjk.com

const double PI = 3.14159;
来源：http://rnl.ybcxt.top

[S28] C：静态变量
来源：http://rxw.fzhhl.top

static int counter = 0;
来源：http://myq.316326.xyz

[S29] C：变参函数
来源：http://dby.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://psr.kuanghao11.cn

[S30] C：头文件保护
来源：http://eji.feifeiyinyue.top

#ifndef X_H
来源：http://wnt.iojbl.cn

#define X_H
来源：http://vkm.pengpengdd.cyou

#endif
来源：http://mto.yangfankeji.com

[S31] C++：Hello World
来源：http://lmk.epnwcf.com

#include <iostream>
来源：http://xai.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://vph.tanke756.top

[S32] C++：字符串
来源：http://ukf.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://gfy.316326.xyz

[S33] C++：vector 增删
来源：http://hfz.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ojj.svipenyu.cn

[S34] C++：遍历 vector
来源：http://hzy.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://qxv.jlsjyb.cn

[S35] C++：map
来源：http://yhx.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rbk.ctjpmb.com

[S36] C++：unordered_map
来源：http://hsr.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gmk.hnxiangtu.top

[S37] C++：set
来源：http://rue.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yxe.guannengcc.top

[S38] C++：排序
来源：http://put.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://gox.birdmap.top

[S39] C++：自定义比较器排序
来源：http://bro.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tvl.zhengqikj.top

[S40] C++：查找元素
来源：http://ifp.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cnd.yj20258888.top

[S41] C++：类与构造函数
来源：http://mvc.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://snn.meibo888.top

[S42] C++：继承与虚函数
来源：http://vyc.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://uty.shzxlz.cn

[S43] C++：智能指针
来源：http://xyd.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://mrd.chenjidiqi.icu

[S44] C++：引用传参
来源：http://wbv.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://sxh.yueranfly.top

[S45] C++：lambda
来源：http://exj.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://bzm.zycfv.cn

[S46] C++：函数模板
来源：http://sxb.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ujb.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://sin.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ein.meibo888.top

[S48] C++：逐行读文件
来源：http://vbm.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://wtz.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://hmh.yj20258.top

[S49] C++：写文件
来源：http://dfq.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://khj.jqgfzy.top

[S50] C++：格式化数字
来源：http://grl.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wmi.bbcook.cn

[S51] C++：显式类型转换
来源：http://onj.hywenlv.cn

static_cast<double>(a) / b
来源：http://lqg.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://rae.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://ruv.cdnleiting.top

[S53] C++：移动语义
来源：http://beq.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://edb.zhiwuduotai.top

[S54] C++：异常处理
来源：http://mlf.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yum.vehdjk.com

[S55] C++：结构化绑定
来源：http://fxr.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://isl.yanxiufei.cn

[S56] C++：optional
来源：http://yku.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tto.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://ljz.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://ize.9152youxi.cn

[S58] C++：命名空间
来源：http://uvl.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://pfb.ydzc1.top

[S59] C++：静态断言
来源：http://sfx.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zso.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://mfw.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sjc.dianchejie.cn

================================================================================
来源：http://cnc.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://frq.pengpengdd.cyou

================================================================================
来源：http://gls.gzhubu.top

[T01] Kotlin：Hello World
来源：http://moh.wangshuangyany.cn

println("Hello")
来源：http://non.yongpay.top

[T02] Kotlin：变量
来源：http://ajx.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cjg.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://brj.tianlin.xyz

"值: $b"
来源：http://stk.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://lwp.zdbjq.cn

val n: String? = null;  n?.length
来源：http://sgz.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://yjl.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lma.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://fpd.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nly.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://ewo.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iog.zdqjudy.top

[T08] Kotlin：数据类
来源：http://nlm.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://xyc.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://qvt.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://sic.hnqzz.top

[T10] Kotlin：默认参数
来源：http://ovm.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hvz.jinqigufen.top

[T11] Kotlin：协程
来源：http://hmc.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ivl.ivvv.top

[T12] Kotlin：解构声明
来源：http://jee.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://rid.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://qhi.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://xyj.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://viu.dashuyun.cn

for (i in 1..10) println(i)
来源：http://cpu.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://wkx.zycfv.cn

interface Shape { fun area(): Double }
来源：http://kcn.yonumen.top

[T16] Swift：Hello World
来源：http://ssl.sysykeji.top

print("Hello")
来源：http://vgq.ydzc1.top

[T17] Swift：变量与常量
来源：http://efs.0kj1m.cn

var a = 1;  let b = 2
来源：http://ohw.birdmap.top

[T18] Swift：字符串插值
来源：http://wna.yonumen.top

"值: \(b)"
来源：http://scd.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://dyh.jyoumei.cn

if let n = opt { print(n) }
来源：http://ekj.jqgufenzy.top

[T20] Swift：数组操作
来源：http://gyt.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://alt.hesvh.cn

[T21] Swift：遍历
来源：http://qkd.jinqigfzy.top

for x in a { print(x) }
来源：http://zso.epnwcf.com

[T22] Swift：字典
来源：http://yyx.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://hkb.shangyingyoupin.top

[T23] Swift：函数
来源：http://axb.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pic.dianchejie.cn

[T24] Swift：闭包
来源：http://bsu.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://twg.feifeiyinyue.top

[T25] Swift：结构体
来源：http://ion.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://vmf.mhx1999.top

[T26] Swift：类与重写
来源：http://yqq.meibo888.top

class A: Base { override func f() {} }
来源：http://ule.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://koc.bjfxy.top

do { try f() } catch { print(error) }
来源：http://xki.316326.xyz

[T28] Swift：枚举
来源：http://zpb.hammf.cn

enum Color { case red, green }
来源：http://fmp.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://nni.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://jkn.jqgfzy.top

[T30] Swift：协议
来源：http://euy.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://eaf.zhiwuduotai.top

[T31] Lua：Hello World
来源：http://ngs.bjfxy.top

print("Hello")
来源：http://tce.gogol.net.cn

[T32] Lua：局部变量
来源：http://lfs.hnxiangtu.top

local a = 1
来源：http://bxu.cheryme.top

[T33] Lua：表（数组）
来源：http://pre.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aqn.52xcode.cn

[T34] Lua：遍历表
来源：http://kbj.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://mef.chenjidiqi.icu

[T35] Lua：字典表
来源：http://qmd.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://eno.nwbrower.top

[T36] Lua：函数
来源：http://fko.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://zbm.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://ajt.jinyuanbaomall.cn

"a" .. "b"
来源：http://bwc.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://nxd.sweek.top

if x > 0 then print("正") end
来源：http://kyw.iojbl.cn

[T39] Lua：模式匹配
来源：http://ymp.nanxinkj.top

string.find(s, "%d+")
来源：http://ghw.fktsv.cn

[T40] Lua：元表
来源：http://mpb.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://ooo.iojbl.cn

[T41] Perl：Hello World
来源：http://nzc.hongshengwenyu.top

print "Hello\n";
来源：http://oag.dashuyun.cn

[T42] Perl：变量类型
来源：http://kxo.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://keq.bbcook.cn

[T43] Perl：字符串插值
来源：http://rbe.hfpthk.cn

"值: $a"
来源：http://tyk.quarkkingdee.top

[T44] Perl：条件
来源：http://ial.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://oxk.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://elb.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://jvo.sysykeji.top

[T46] Perl：哈希操作
来源：http://yms.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jqp.chenlongwang.top

[T47] Perl：正则捕获
来源：http://oud.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://snu.bjfxy.top

[T48] Perl：正则替换
来源：http://hkd.guannengcc.top

$s =~ s/old/new/g;
来源：http://ypl.meibo888.top

[T49] Perl：函数
来源：http://cng.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://byr.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://ioy.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jhw.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://eej.tianlin.xyz

[T51] Scala：Hello World
来源：http://kbe.yuanzhike.top

println("Hello")
来源：http://und.316326.xyz

[T52] Scala：变量
来源：http://mkg.fzhhl.top

val a = 1;  var b = 2
来源：http://egj.fengsongda.top

[T53] Scala：字符串插值
来源：http://jef.dianchejie.cn

s"值: $b"
来源：http://ojo.fehbvm.com

[T54] Scala：集合映射
来源：http://hxg.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://pqi.nwbrower.top

[T55] Scala：集合过滤
来源：http://puz.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ext.ivvv.top

[T56] Scala：样例类
来源：http://edr.birdmap.top

case class User(name: String, age: Int)
来源：http://zlp.c1oappe.top

[T57] Scala：模式匹配
来源：http://psp.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kcj.gogol.net.cn

[T58] Scala：函数定义
来源：http://ppw.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wrx.cashguo.top

[T59] Scala：循环
来源：http://dhs.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://yye.gotoacloud.top

[T60] Scala：折叠
来源：http://wik.birdmap.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ddm.daxiang520.top

================================================================================
来源：http://pwn.52xcode.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zku.chenzaomai.com

================================================================================
来源：http://ujo.chenzaomai.com

[U01] Py：创建虚拟环境
来源：http://fwg.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://gro.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://fvi.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://itd.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://laq.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sqn.fengsongda.top

[U04] Py：变量调试打印
来源：http://fpt.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zaz.zhongyouzk.top

[U05] Py：列表去重且保序
来源：http://eap.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://itv.fehbvm.com

[U06] Py：合并两个字典
来源：http://jzy.shangyingyoupin.top

{**a, **b}
来源：http://ctn.fehbvm.com

[U07] Py：反转字典键值
来源：http://dqi.gzhubu.top

{v: k for k, v in d.items()}
来源：http://czk.jyoumei.cn

[U08] Py：展平二维列表
来源：http://qab.hywenlv.cn

[y for x in nested for y in x]
来源：http://wbc.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://mfg.snrcjt.cn

max(d, key=d.get)
来源：http://vxa.yj20258888.top

[U10] Py：按值排序字典
来源：http://ezz.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zfi.dianchejie.cn

[U11] Py：生成器表达式
来源：http://due.yvedp.cn

(x * 2 for x in arr)
来源：http://doo.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://mwz.yueranfly.top

Counter(arr).most_common(3)
来源：http://nkv.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://pcx.vehdjk.com

deque(maxlen=10)
来源：http://gln.ctjpmb.com

[U14] Py：分组收集到列表
来源：http://ecc.chenlongwang.top

defaultdict(list)
来源：http://drn.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://pqp.tanke756.top

t = time.perf_counter()
来源：http://yub.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://iki.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pzc.bbcook.cn

[U17] Py：初始化日志
来源：http://gpr.tianlin.xyz

logging.basicConfig(level=logging.INFO)
来源：http://aar.yvedp.cn

[U18] Py：预编译正则
来源：http://tet.tarul.cn

pat = re.compile(r"\d+")
来源：http://pgp.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://ekh.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jyf.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://eoi.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://msj.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://mkf.guannengcc.top

@contextlib.contextmanager
来源：http://djw.guannengcc.top

[U22] Py：矩阵转置
来源：http://xdw.tarul.cn

list(zip(*m))
来源：http://jsc.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://rwi.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ntd.xuetiantiany.cn

[U24] Py：路径操作
来源：http://ctv.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fxq.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://wyt.tanke756.top

csv.DictReader(f)
来源：http://fch.nwbrower.top

[U26] Py：并发下载
来源：http://mcz.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qwj.gotoacloud.top

[U27] Py：异步 HTTP
来源：http://ynj.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ygo.yfazqb.com

[U28] Py：类型别名
来源：http://guf.mhx1999.top

UserId = int
来源：http://nsj.dianchejie.cn

[U29] Py：属性校验
来源：http://ytw.xylfe.cn

@property 与 @x.setter 配合
来源：http://lou.chenjidiqi.icu

[U30] Py：数据类
来源：http://acs.0kj1m.cn

@dataclass(slots=True)
来源：http://zwx.ivvv.top

[U31] Py：单测
来源：http://owe.shanyushiyangtech.top

python -m pytest -q
来源：http://ict.xziqi.cn

[U32] Py：代码格式化
来源：http://tks.epnwcf.com

ruff format . && ruff check --fix .
来源：http://orw.daxiang520.top

[U33] Py：打包发布
来源：http://zee.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://yda.ydzc1.top

[U34] Py：判断编码
来源：http://hrq.guowangkeji.top

chardet.detect(raw)
来源：http://hob.mhx1999.top

[U35] Py：发送邮件
来源：http://vkn.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ugh.xziqi.cn

[U36] Py：定时任务
来源：http://jqm.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://rbz.vehdjk.com


<!-- 参考信息 -->