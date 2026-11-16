代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ogw.aibaodan.cn

[S13] C：宏定义
来源：http://jkh.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aqk.zhijiandao.cn

[S14] C：枚举
来源：http://jln.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://bkx.wangshuangyany.cn

[S15] C：类型转换
来源：http://pkd.hnqzz.top

(double) a / b
来源：http://qnx.zhiwuduotai.top

[S16] C：位操作置位
来源：http://jbd.dianchejie.cn

x |= (1 << 3);
来源：http://jni.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://mra.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vby.havefunace.top

[S18] C：命令行参数
来源：http://aee.andypj.xyz

int main(int argc, char **argv)
来源：http://iax.zhiwuduotai.top

[S19] C：快速排序
来源：http://wfv.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://pty.xziqi.cn

[S20] C：二分查找
来源：http://egm.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://olt.9152youxi.cn

[S21] C：字符类别判断
来源：http://tgo.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gmb.nwbrower.top

[S22] C：字符串转数字
来源：http://qra.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fsc.yangfankeji.com

[S23] C：随机数
来源：http://nzr.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://upt.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://prc.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lpy.hcnkem.com

[S25] C：内存拷贝
来源：http://ffy.xziqi.cn

memcpy(dst, src, n);
来源：http://yha.smart0.xyz

[S26] C：内存清零
来源：http://cdl.havefunace.top

memset(a, 0, sizeof a);
来源：http://qao.redwolf501.top

[S27] C：定义常量
来源：http://jhz.jqgufenzy.top

const double PI = 3.14159;
来源：http://pvc.jianghu66.top

[S28] C：静态变量
来源：http://ugr.zhengqikj.top

static int counter = 0;
来源：http://zzb.guowangkeji.top

[S29] C：变参函数
来源：http://yuj.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fqp.jyoumei.cn

[S30] C：头文件保护
来源：http://cfm.wangdashe.top

#ifndef X_H
来源：http://tgk.zhijiandao.cn

#define X_H
来源：http://sxf.xziqi.cn

#endif
来源：http://sva.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://cxh.tianlin.xyz

#include <iostream>
来源：http://eic.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://bhk.daria6918.cn

[S32] C++：字符串
来源：http://npv.tanke756.top

std::string s = "hi";  s += "!";
来源：http://keb.epnwcf.com

[S33] C++：vector 增删
来源：http://veb.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fzh.yj202588.top

[S34] C++：遍历 vector
来源：http://fpa.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://urk.tarul.cn

[S35] C++：map
来源：http://ili.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qlv.jlsjyb.cn

[S36] C++：unordered_map
来源：http://weo.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bwa.nwbrower.top

[S37] C++：set
来源：http://jlz.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oru.iojbl.cn

[S38] C++：排序
来源：http://trc.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://tzp.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://iqn.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uvg.cucudq.cn

[S40] C++：查找元素
来源：http://txx.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxg.hesvh.cn

[S41] C++：类与构造函数
来源：http://hkr.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://skr.hnqzz.top

[S42] C++：继承与虚函数
来源：http://frj.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://gka.jyoumei.cn

[S43] C++：智能指针
来源：http://qsi.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://mgw.zhengqikj.top

[S44] C++：引用传参
来源：http://csl.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://hzt.sysykeji.top

[S45] C++：lambda
来源：http://unw.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://phr.guannengcc.top

[S46] C++：函数模板
来源：http://vdv.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vjl.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://nkf.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hea.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://lhf.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://ktr.ydzc1.top

while (std::getline(in, line)) { }
来源：http://thf.sxryk.cn

[S49] C++：写文件
来源：http://wzt.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kvt.zdbjq.cn

[S50] C++：格式化数字
来源：http://etl.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zup.sufxvd.cn

[S51] C++：显式类型转换
来源：http://zju.hammf.cn

static_cast<double>(a) / b
来源：http://rmr.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://gkx.pycfn.com

int size() const noexcept { return n_; }
来源：http://boi.daxiang520.top

[S53] C++：移动语义
来源：http://bip.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://fli.xinyue.icu

[S54] C++：异常处理
来源：http://nlc.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://drg.shzxlz.cn

[S55] C++：结构化绑定
来源：http://ywb.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cma.yuanzhike.top

[S56] C++：optional
来源：http://fwy.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vem.hesvh.cn

[S57] C++：编译期常量
来源：http://yzj.nwbrower.top

constexpr int N = 10;
来源：http://ils.jqgufenzy.top

[S58] C++：命名空间
来源：http://gre.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://nqa.cashguo.top

[S59] C++：静态断言
来源：http://qxf.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tsk.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://oxr.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fsf.jianghu66.top

================================================================================
来源：http://jsl.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vhh.hesvh.cn

================================================================================
来源：http://uhz.birdmap.top

[T01] Kotlin：Hello World
来源：http://bnv.yangfankeji.com

println("Hello")
来源：http://bud.shzxlz.cn

[T02] Kotlin：变量
来源：http://zkm.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dwm.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://bfb.xuanzx.com

"值: $b"
来源：http://gtr.yvedp.cn

[T04] Kotlin：空安全
来源：http://gge.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://flc.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://ojy.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqs.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://pzp.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wms.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://ewv.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yof.redwolf501.top

[T08] Kotlin：数据类
来源：http://kjh.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://qla.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://ylw.yj20258.top

fun String.exclaim() = this + "!"
来源：http://jsd.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://phj.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sho.haohaochexian.top

[T11] Kotlin：协程
来源：http://vdw.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://byh.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://cyx.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://bzh.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://sym.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://oda.sufxvd.cn

[T14] Kotlin：循环
来源：http://wsy.epnwcf.com

for (i in 1..10) println(i)
来源：http://liq.xinyue.icu

[T15] Kotlin：接口
来源：http://qqo.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://nyx.ydjk.org.cn

[T16] Swift：Hello World
来源：http://ije.kuanghao11.cn

print("Hello")
来源：http://blb.andypj.xyz

[T17] Swift：变量与常量
来源：http://nee.yvedp.cn

var a = 1;  let b = 2
来源：http://dud.tian-w.cn

[T18] Swift：字符串插值
来源：http://wdy.pycfn.com

"值: \(b)"
来源：http://qlt.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://nnx.zycfv.cn

if let n = opt { print(n) }
来源：http://mim.epnwcf.com

[T20] Swift：数组操作
来源：http://hgm.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://pur.shangyingyoupin.top

[T21] Swift：遍历
来源：http://nqy.smart0.xyz

for x in a { print(x) }
来源：http://wln.andypj.xyz

[T22] Swift：字典
来源：http://jal.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://krn.shanyushiyangtech.top

[T23] Swift：函数
来源：http://rdf.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://inc.sxryk.cn

[T24] Swift：闭包
来源：http://kwp.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bnf.nwbrower.top

[T25] Swift：结构体
来源：http://oza.52xcode.cn

struct P { var x: Int }
来源：http://fyo.jqgfzy.top

[T26] Swift：类与重写
来源：http://ejz.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://dpy.cheryme.top

[T27] Swift：错误处理
来源：http://dfo.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://swd.jlsjyb.cn

[T28] Swift：枚举
来源：http://pxe.ybcxt.top

enum Color { case red, green }
来源：http://lno.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://yso.shzxlz.cn

guard let x = opt else { return }
来源：http://wzn.daria6918.cn

[T30] Swift：协议
来源：http://gib.tarul.cn

protocol Shape { func area() -> Double }
来源：http://bny.meibo888.top

[T31] Lua：Hello World
来源：http://yyx.epnwcf.com

print("Hello")
来源：http://rpv.sjlbkw.cn

[T32] Lua：局部变量
来源：http://dem.hammf.cn

local a = 1
来源：http://pyl.yj20258.top

[T33] Lua：表（数组）
来源：http://qlh.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cys.meibo888.top

[T34] Lua：遍历表
来源：http://vtj.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gvw.yangfankeji.com

[T35] Lua：字典表
来源：http://mcz.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://rin.cucudq.cn

[T36] Lua：函数
来源：http://qdd.quarkkingdee.top

function add(a, b) return a + b end
来源：http://cyj.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://akd.zhaomingkeji.xyz

"a" .. "b"
来源：http://saw.aizwys.cn

[T38] Lua：条件
来源：http://kst.cdnleiting.top

if x > 0 then print("正") end
来源：http://kej.hammf.cn

[T39] Lua：模式匹配
来源：http://hxw.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://tba.hongshengwenyu.top

[T40] Lua：元表
来源：http://tbk.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://hgw.hcnkem.com

[T41] Perl：Hello World
来源：http://avz.tianlin.xyz

print "Hello\n";
来源：http://inr.yonumen.top

[T42] Perl：变量类型
来源：http://cen.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yew.yj202588.top

[T43] Perl：字符串插值
来源：http://wvb.hfpthk.cn

"值: $a"
来源：http://mvk.yj20258888.top

[T44] Perl：条件
来源：http://ddr.zdqjudy.top

if ($a > 0) { print "正"; }
来源：http://sgx.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://bbp.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://ziu.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://qvy.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vvt.chenlongwang.top

[T47] Perl：正则捕获
来源：http://cla.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://neb.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://mur.jiagoushi.top

$s =~ s/old/new/g;
来源：http://ayh.zhiwuduotai.top

[T49] Perl：函数
来源：http://uho.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xtz.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://kee.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://drj.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://icp.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://yuv.52xcode.cn

println("Hello")
来源：http://zjj.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://zpk.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://myp.yuxming.cn

[T53] Scala：字符串插值
来源：http://ypk.shanyushiyangkeji.top

s"值: $b"
来源：http://koh.haohaochexian.top

[T54] Scala：集合映射
来源：http://mmh.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://fhg.gotoacloud.top

[T55] Scala：集合过滤
来源：http://kkp.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://mvf.sxryk.cn

[T56] Scala：样例类
来源：http://kex.chenlongwang.top

case class User(name: String, age: Int)
来源：http://fyv.guannengcc.top

[T57] Scala：模式匹配
来源：http://ebg.hammf.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vlq.quarkkingdee.top

[T58] Scala：函数定义
来源：http://oam.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://ftc.hysaishi.cn

[T59] Scala：循环
来源：http://nie.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://wbo.hnxiangtu.top

[T60] Scala：折叠
来源：http://dex.jinqigfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eal.svipenyu.cn

================================================================================
来源：http://kqy.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zek.yuxming.cn

================================================================================
来源：http://sjr.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://flx.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://jac.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://anf.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rpj.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://qth.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bhm.guowangkeji.top

[U04] Py：变量调试打印
来源：http://dff.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wqf.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://twf.xinyue.icu

list(dict.fromkeys(arr))
来源：http://jja.sxryk.cn

[U06] Py：合并两个字典
来源：http://kam.ywan-chungtsiang.top

{**a, **b}
来源：http://hzm.pycfn.com

[U07] Py：反转字典键值
来源：http://uzs.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://oap.hywenlv.cn

[U08] Py：展平二维列表
来源：http://otf.hesvh.cn

[y for x in nested for y in x]
来源：http://jus.yuanzhike.top

[U09] Py：字典取最大值的键
来源：http://pbg.9152youxi.cn

max(d, key=d.get)
来源：http://las.meibo888.top

[U10] Py：按值排序字典
来源：http://jzy.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yeb.mhx1999.top

[U11] Py：生成器表达式
来源：http://ibr.wangdashe.top

(x * 2 for x in arr)
来源：http://kfp.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://zca.epnwcf.com

Counter(arr).most_common(3)
来源：http://jpz.snrcjt.cn

[U13] Py：固定长度队列
来源：http://icd.ehwqpu.com

deque(maxlen=10)
来源：http://dtd.sweek.top

[U14] Py：分组收集到列表
来源：http://szx.sysykeji.top

defaultdict(list)
来源：http://gqz.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://cgm.c1oappe.top

t = time.perf_counter()
来源：http://tvi.wangshuangyany.cn

[U16] Py：命令行参数解析
来源：http://pvx.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jta.yfazqb.com

[U17] Py：初始化日志
来源：http://qhy.sxryk.cn

logging.basicConfig(level=logging.INFO)
来源：http://odk.hnqzz.top

[U18] Py：预编译正则
来源：http://lur.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://sbv.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://rib.xingfuxueyuan.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hyf.xuanzx.com

[U20] Py：缓存函数结果
来源：http://wpt.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://znx.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://mnc.wangdashe.top

@contextlib.contextmanager
来源：http://oyu.zdbjq.cn

[U22] Py：矩阵转置
来源：http://cly.zhixingplan.top

list(zip(*m))
来源：http://oqp.gzhubu.top

[U23] Py：分块读取大文件
来源：http://fbz.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zka.yj202588.top

[U24] Py：路径操作
来源：http://fwj.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udr.zhiwuduotai.top

[U25] Py：CSV 按字典读
来源：http://msn.zhoulong.xyz

csv.DictReader(f)
来源：http://jge.yj20258.top

[U26] Py：并发下载
来源：http://gpb.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ftt.ivvv.top

[U27] Py：异步 HTTP
来源：http://qjj.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://ges.zycfv.cn

[U28] Py：类型别名
来源：http://ifr.hnqzz.top

UserId = int
来源：http://pvs.dashuyun.cn

[U29] Py：属性校验
来源：http://vfm.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://tso.fengsongda.top

[U30] Py：数据类
来源：http://raq.hywenlv.cn

@dataclass(slots=True)
来源：http://ata.shanyushiyangkeji.top

[U31] Py：单测
来源：http://qmh.jinqigfzy.top

python -m pytest -q
来源：http://oas.sxryk.cn

[U32] Py：代码格式化
来源：http://ltx.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://fbv.yuanzhike.top

[U33] Py：打包发布
来源：http://wzk.fanxiaobao.xyz

python -m build  （依赖 pyproject.toml）
来源：http://pci.wangdashe.top

[U34] Py：判断编码
来源：http://naw.nanxinkj.top

chardet.detect(raw)
来源：http://juc.ctjpmb.com

[U35] Py：发送邮件
来源：http://bka.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cai.hfpthk.cn

[U36] Py：定时任务
来源：http://vye.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://wiz.daria6918.cn


<!-- 参考信息 -->