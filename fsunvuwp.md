代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://jeb.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fkz.316326.xyz

fclose(f);
来源：http://lwr.pycfn.com

[S12] C：写文件
来源：http://qso.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pxw.mhx1999.top

[S13] C：宏定义
来源：http://edi.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ijx.quarkkingdee.top

[S14] C：枚举
来源：http://mws.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://jnl.aibaodan.cn

[S15] C：类型转换
来源：http://wqy.daria6918.cn

(double) a / b
来源：http://wib.hnxiangtu.top

[S16] C：位操作置位
来源：http://jwe.chenjidiqi.icu

x |= (1 << 3);
来源：http://wzz.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://stg.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wqx.hcnkem.com

[S18] C：命令行参数
来源：http://xqg.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://gml.zdqjudy.top

[S19] C：快速排序
来源：http://nam.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tls.havefunace.top

[S20] C：二分查找
来源：http://lyc.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vvn.snrcjt.cn

[S21] C：字符类别判断
来源：http://bid.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wgw.ehwqpu.com

[S22] C：字符串转数字
来源：http://wfe.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://vnw.shzxlz.cn

[S23] C：随机数
来源：http://owj.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yhk.fzhhl.top

[S24] C：获取本地时间
来源：http://cqw.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://guc.nwbrower.top

[S25] C：内存拷贝
来源：http://pen.jqgufenzy.top

memcpy(dst, src, n);
来源：http://zkl.jqgfzy.top

[S26] C：内存清零
来源：http://eek.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://fip.fktsv.cn

[S27] C：定义常量
来源：http://jze.sxryk.cn

const double PI = 3.14159;
来源：http://xjp.guowangkeji.top

[S28] C：静态变量
来源：http://add.gogol.net.cn

static int counter = 0;
来源：http://dgi.sysykeji.top

[S29] C：变参函数
来源：http://ubn.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://opq.haohaochexian.top

[S30] C：头文件保护
来源：http://uyg.xylfe.cn

#ifndef X_H
来源：http://pvb.iojbl.cn

#define X_H
来源：http://kxa.jinghuilouyu.cn

#endif
来源：http://kau.redwolf501.top

[S31] C++：Hello World
来源：http://otb.sxryk.cn

#include <iostream>
来源：http://hcz.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://vyp.hongshengwenyu.top

[S32] C++：字符串
来源：http://uor.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://srs.shuidangran.top

[S33] C++：vector 增删
来源：http://sij.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://arx.aibaodan.cn

[S34] C++：遍历 vector
来源：http://jxw.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://ssl.zhengqikj.top

[S35] C++：map
来源：http://ayd.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yly.jyoumei.cn

[S36] C++：unordered_map
来源：http://eqd.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ksk.yangfankeji.com

[S37] C++：set
来源：http://amd.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://glb.iojbl.cn

[S38] C++：排序
来源：http://yvw.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://diq.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://mrh.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://upw.hongshengwenyu.top

[S40] C++：查找元素
来源：http://fgs.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mip.xziqi.cn

[S41] C++：类与构造函数
来源：http://cup.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cuj.yj20258.top

[S42] C++：继承与虚函数
来源：http://dsu.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://yog.vehdjk.com

[S43] C++：智能指针
来源：http://aun.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://fvz.pycfn.com

[S44] C++：引用传参
来源：http://nyj.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://ukf.jqgufenzy.top

[S45] C++：lambda
来源：http://ese.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://zao.yonumen.top

[S46] C++：函数模板
来源：http://wgh.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://svz.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://zcu.guannengcc.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uoj.yonumen.top

[S48] C++：逐行读文件
来源：http://nde.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dfx.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://ypa.sufxvd.cn

[S49] C++：写文件
来源：http://thq.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hng.hywenlv.cn

[S50] C++：格式化数字
来源：http://uhh.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fkb.ybcxt.top

[S51] C++：显式类型转换
来源：http://lud.sjlbkw.cn

static_cast<double>(a) / b
来源：http://fng.cashguo.top

[S52] C++：const 与 noexcept
来源：http://qtf.fengsongda.top

int size() const noexcept { return n_; }
来源：http://vqa.sysykeji.top

[S53] C++：移动语义
来源：http://wcn.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://dop.snrcjt.cn

[S54] C++：异常处理
来源：http://zhl.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://unl.xinyue.icu

[S55] C++：结构化绑定
来源：http://duf.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dpx.jinqigfzy.top

[S56] C++：optional
来源：http://cmk.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xag.gogol.net.cn

[S57] C++：编译期常量
来源：http://ziq.sweek.top

constexpr int N = 10;
来源：http://css.zdbjq.cn

[S58] C++：命名空间
来源：http://jyl.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://zys.guowangkeji.top

[S59] C++：静态断言
来源：http://ftp.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ses.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://pxg.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ojq.hfpthk.cn

================================================================================
来源：http://ikt.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybz.cashguo.top

================================================================================
来源：http://rcx.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://spi.hfpthk.cn

println("Hello")
来源：http://udp.kuanghao11.cn

[T02] Kotlin：变量
来源：http://hkr.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kka.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://ylk.gotoacloud.top

"值: $b"
来源：http://acl.zhixingplan.top

[T04] Kotlin：空安全
来源：http://gld.hnqzz.top

val n: String? = null;  n?.length
来源：http://loy.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://gqq.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qaw.zycfv.cn

[T06] Kotlin：集合映射
来源：http://erm.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xed.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://far.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://snn.0kj1m.cn

[T08] Kotlin：数据类
来源：http://saf.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://vsz.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://rug.ivvv.top

fun String.exclaim() = this + "!"
来源：http://vur.sxryk.cn

[T10] Kotlin：默认参数
来源：http://ndl.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hqb.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://spd.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eto.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://mgc.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://xmx.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://ajt.jianghu66.top

val m = mapOf("a" to 1)
来源：http://zaf.andypj.xyz

[T14] Kotlin：循环
来源：http://srt.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://ume.vehdjk.com

[T15] Kotlin：接口
来源：http://vcd.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://jyz.nanxinkj.top

[T16] Swift：Hello World
来源：http://dyh.meibo888.top

print("Hello")
来源：http://sja.bbcook.cn

[T17] Swift：变量与常量
来源：http://qoe.meibo888.top

var a = 1;  let b = 2
来源：http://mvc.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://uag.xingfuxueyuan.xyz

"值: \(b)"
来源：http://wch.chenlongwang.top

[T19] Swift：可选绑定
来源：http://jhu.redwolf501.top

if let n = opt { print(n) }
来源：http://tuj.xuanzx.com

[T20] Swift：数组操作
来源：http://jzx.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://big.pengpengdd.cyou

[T21] Swift：遍历
来源：http://dey.zhijiandao.cn

for x in a { print(x) }
来源：http://gzr.nanxuanxn.top

[T22] Swift：字典
来源：http://vll.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rvj.vehdjk.com

[T23] Swift：函数
来源：http://ivt.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kst.hesvh.cn

[T24] Swift：闭包
来源：http://kpk.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jjp.cqqwz.cn

[T25] Swift：结构体
来源：http://dpm.zhixingplan.top

struct P { var x: Int }
来源：http://gjy.tian-w.cn

[T26] Swift：类与重写
来源：http://zzc.daxiang520.top

class A: Base { override func f() {} }
来源：http://ecy.yangfankeji.com

[T27] Swift：错误处理
来源：http://hhd.andypj.xyz

do { try f() } catch { print(error) }
来源：http://vph.sxryk.cn

[T28] Swift：枚举
来源：http://rkd.hesvh.cn

enum Color { case red, green }
来源：http://rgm.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://wce.gaohongyu789.top

guard let x = opt else { return }
来源：http://qxg.yangfankeji.com

[T30] Swift：协议
来源：http://lek.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://uab.fzhhl.top

[T31] Lua：Hello World
来源：http://tme.feifeiyinyue.top

print("Hello")
来源：http://qtk.hesvh.cn

[T32] Lua：局部变量
来源：http://znv.havefunace.top

local a = 1
来源：http://rfd.zdbjq.cn

[T33] Lua：表（数组）
来源：http://flh.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://rpx.fengsongda.top

[T34] Lua：遍历表
来源：http://ofc.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ann.vehdjk.com

[T35] Lua：字典表
来源：http://wkx.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://xva.vehdjk.com

[T36] Lua：函数
来源：http://ukz.hnqzz.top

function add(a, b) return a + b end
来源：http://bct.fzhhl.top

[T37] Lua：字符串拼接
来源：http://ccd.iojbl.cn

"a" .. "b"
来源：http://xpu.zdbjq.cn

[T38] Lua：条件
来源：http://cyb.kuanghao11.cn

if x > 0 then print("正") end
来源：http://tzj.hesvh.cn

[T39] Lua：模式匹配
来源：http://atg.havefunace.top

string.find(s, "%d+")
来源：http://zph.fktsv.cn

[T40] Lua：元表
来源：http://jsv.yvedp.cn

setmetatable({}, { __index = base })
来源：http://rum.sysykeji.top

[T41] Perl：Hello World
来源：http://rpc.cashguo.top

print "Hello\n";
来源：http://iqb.hnqzz.top

[T42] Perl：变量类型
来源：http://wnh.bbcook.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ttu.fktsv.cn

[T43] Perl：字符串插值
来源：http://sca.vqdsnc.cn

"值: $a"
来源：http://ezv.zhijiandao.cn

[T44] Perl：条件
来源：http://kqb.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://yuo.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://djj.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://okg.chenzaomai.com

[T46] Perl：哈希操作
来源：http://byu.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://atb.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://qjh.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://xmj.tarul.cn

[T48] Perl：正则替换
来源：http://fuw.redwolf501.top

$s =~ s/old/new/g;
来源：http://aeo.jiagoushi.top

[T49] Perl：函数
来源：http://usa.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jje.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://lre.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hxk.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://txx.zdbjq.cn

[T51] Scala：Hello World
来源：http://rte.316326.xyz

println("Hello")
来源：http://dpp.gotoacloud.top

[T52] Scala：变量
来源：http://bcr.tanke756.top

val a = 1;  var b = 2
来源：http://nmw.yonumen.top

[T53] Scala：字符串插值
来源：http://uyj.sysykeji.top

s"值: $b"
来源：http://hbu.316326.xyz

[T54] Scala：集合映射
来源：http://neo.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://bpt.wangdashe.top

[T55] Scala：集合过滤
来源：http://zox.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://tat.smart0.xyz

[T56] Scala：样例类
来源：http://ohf.hywenlv.cn

case class User(name: String, age: Int)
来源：http://djf.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://han.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://drp.jyoumei.cn

[T58] Scala：函数定义
来源：http://hxt.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zxj.epnwcf.com

[T59] Scala：循环
来源：http://rei.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://sph.meibo888.top

[T60] Scala：折叠
来源：http://uir.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pso.yongpay.top

================================================================================
来源：http://zyc.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xps.0kj1m.cn

================================================================================
来源：http://fpr.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://zwn.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dxj.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://bsc.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yet.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://vvo.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qsa.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://atd.jiagoushi.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rfs.yongpay.top

[U05] Py：列表去重且保序
来源：http://yyi.nwbrower.top

list(dict.fromkeys(arr))
来源：http://mhr.xziqi.cn

[U06] Py：合并两个字典
来源：http://fhr.yueranfly.top

{**a, **b}
来源：http://dkj.cdnleiting.top

[U07] Py：反转字典键值
来源：http://bll.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://orz.yfazqb.com

[U08] Py：展平二维列表
来源：http://tjo.kuanghao11.cn

[y for x in nested for y in x]
来源：http://zla.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://ofk.jinqigfzy.top

max(d, key=d.get)
来源：http://exj.chenlongwang.top

[U10] Py：按值排序字典
来源：http://wlx.chenlongwang.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ybo.shuidangran.top

[U11] Py：生成器表达式
来源：http://vfw.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://kfo.chenzaomai.com

[U12] Py：取出现最多的 3 个元素
来源：http://ulw.feifeiyinyue.top

Counter(arr).most_common(3)
来源：http://syu.yuanzhike.top

[U13] Py：固定长度队列
来源：http://ipl.yuanzhike.top

deque(maxlen=10)
来源：http://waq.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://azu.yueranfly.top

defaultdict(list)
来源：http://tlq.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://uuf.pycfn.com

t = time.perf_counter()
来源：http://qqw.daria6918.cn

[U16] Py：命令行参数解析
来源：http://fii.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jzs.kuanghao11.cn

[U17] Py：初始化日志
来源：http://cmb.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://huo.cucudq.cn

[U18] Py：预编译正则
来源：http://cuo.shuidangran.top

pat = re.compile(r"\d+")
来源：http://uic.zycfv.cn

[U19] Py：正则替换带回调
来源：http://qiz.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ryo.ydzc1.top

[U20] Py：缓存函数结果
来源：http://uqt.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://jxs.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://tym.zhiwuduotai.top

@contextlib.contextmanager
来源：http://wiv.gaohongyu789.top

[U22] Py：矩阵转置
来源：http://kla.jianghu66.top

list(zip(*m))
来源：http://bmw.52xcode.cn

[U23] Py：分块读取大文件
来源：http://kbv.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://udj.jinqigfzy.top

[U24] Py：路径操作
来源：http://ukl.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zmc.316326.xyz

[U25] Py：CSV 按字典读
来源：http://ufb.chenjidiqi.icu

csv.DictReader(f)
来源：http://rad.zdbjq.cn

[U26] Py：并发下载
来源：http://djf.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mgi.tarul.cn

[U27] Py：异步 HTTP
来源：http://wle.hfpthk.cn

aiohttp.ClientSession() 配合 async with
来源：http://uct.iojbl.cn

[U28] Py：类型别名
来源：http://cmk.wangdashe.top

UserId = int
来源：http://tki.hysaishi.cn

[U29] Py：属性校验
来源：http://yhm.sxryk.cn

@property 与 @x.setter 配合
来源：http://ius.snrcjt.cn

[U30] Py：数据类
来源：http://phh.nwbrower.top

@dataclass(slots=True)
来源：http://max.shuidangran.top

[U31] Py：单测
来源：http://ytk.jqgufenzy.top

python -m pytest -q
来源：http://edz.havefunace.top

[U32] Py：代码格式化
来源：http://xkj.hcnkem.com

ruff format . && ruff check --fix .
来源：http://rlu.chenlongwang.top

[U33] Py：打包发布
来源：http://rrs.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://erw.guannengcc.top

[U34] Py：判断编码
来源：http://qxr.0kj1m.cn

chardet.detect(raw)
来源：http://ewp.ehwqpu.com


<!-- 参考信息 -->