代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ibd.zdbjq.cn

[S13] C：宏定义
来源：http://hub.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xmi.ydjk.org.cn

[S14] C：枚举
来源：http://rby.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://dfh.vqdsnc.cn

[S15] C：类型转换
来源：http://ddj.jiagoushi.top

(double) a / b
来源：http://kou.nanxinkj.top

[S16] C：位操作置位
来源：http://bsk.cucudq.cn

x |= (1 << 3);
来源：http://vic.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://lnp.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fda.jinqigfzy.top

[S18] C：命令行参数
来源：http://ewr.cdnleiting.top

int main(int argc, char **argv)
来源：http://jxu.yuanzhike.top

[S19] C：快速排序
来源：http://pec.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://cuv.dianchejie.cn

[S20] C：二分查找
来源：http://ukp.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ood.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://xes.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ysv.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://dbr.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nia.havefunace.top

[S23] C：随机数
来源：http://nvc.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://dmk.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://gep.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oku.sufxvd.cn

[S25] C：内存拷贝
来源：http://fmf.ctjpmb.com

memcpy(dst, src, n);
来源：http://xiy.snrcjt.cn

[S26] C：内存清零
来源：http://aka.redwolf501.top

memset(a, 0, sizeof a);
来源：http://zil.xuetiantiany.cn

[S27] C：定义常量
来源：http://yxc.zdqjudy.top

const double PI = 3.14159;
来源：http://luz.aizwys.cn

[S28] C：静态变量
来源：http://pkj.hfpthk.cn

static int counter = 0;
来源：http://iax.andypj.xyz

[S29] C：变参函数
来源：http://fko.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hoz.cheryme.top

[S30] C：头文件保护
来源：http://xlj.andypj.xyz

#ifndef X_H
来源：http://cbj.cashguo.top

#define X_H
来源：http://oid.yueranfly.top

#endif
来源：http://nef.hnqzz.top

[S31] C++：Hello World
来源：http://hwd.ybcxt.top

#include <iostream>
来源：http://hxu.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://vzy.sufxvd.cn

[S32] C++：字符串
来源：http://nya.yonumen.top

std::string s = "hi";  s += "!";
来源：http://yjh.bbcook.cn

[S33] C++：vector 增删
来源：http://bmv.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dcl.andypj.xyz

[S34] C++：遍历 vector
来源：http://skk.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://prv.yueranfly.top

[S35] C++：map
来源：http://lqn.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dmg.xylfe.cn

[S36] C++：unordered_map
来源：http://jzj.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://erl.birdmap.top

[S37] C++：set
来源：http://rma.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qay.chenlongwang.top

[S38] C++：排序
来源：http://cpq.cashguo.top

std::sort(v.begin(), v.end());
来源：http://inn.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://lol.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhd.52xcode.cn

[S40] C++：查找元素
来源：http://mbz.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sso.birdmap.top

[S41] C++：类与构造函数
来源：http://srd.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oqy.yvedp.cn

[S42] C++：继承与虚函数
来源：http://cqr.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://dfy.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://guc.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://nzz.316326.xyz

[S44] C++：引用传参
来源：http://yky.pycfn.com

void inc(int &x) { ++x; }
来源：http://atb.ydzc1.top

[S45] C++：lambda
来源：http://guz.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://amw.uphjek.com

[S46] C++：函数模板
来源：http://znk.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cyb.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://dku.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sjn.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://pzg.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zve.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://hnp.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://hxj.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ykq.gotoacloud.top

[S50] C++：格式化数字
来源：http://fsc.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pmh.52xcode.cn

[S51] C++：显式类型转换
来源：http://umk.hfpthk.cn

static_cast<double>(a) / b
来源：http://bhl.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://why.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://oov.ehwqpu.com

[S53] C++：移动语义
来源：http://lgl.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://npv.andypj.xyz

[S54] C++：异常处理
来源：http://aqj.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fme.hnqzz.top

[S55] C++：结构化绑定
来源：http://sqb.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://yrj.xinyue.icu

[S56] C++：optional
来源：http://cjh.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://laz.redwolf501.top

[S57] C++：编译期常量
来源：http://jjn.mhx1999.top

constexpr int N = 10;
来源：http://ieg.zycfv.cn

[S58] C++：命名空间
来源：http://zrj.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://wrb.ydjk.org.cn

[S59] C++：静态断言
来源：http://ccg.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eww.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://sjq.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oiw.nanxinkj.top

================================================================================
来源：http://zvt.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yfw.feifeiyinyue.top

================================================================================
来源：http://pjf.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://ymt.zycfv.cn

println("Hello")
来源：http://ear.cdnleiting.top

[T02] Kotlin：变量
来源：http://ldx.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pbe.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://tqq.mhx1999.top

"值: $b"
来源：http://ewz.nanxinkj.top

[T04] Kotlin：空安全
来源：http://cln.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://kty.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://kdw.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ntk.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://mtg.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tzw.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://nlm.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lvd.uphjek.com

[T08] Kotlin：数据类
来源：http://niz.tarul.cn

data class User(val name: String, val age: Int)
来源：http://whv.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://uxx.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://lip.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://fln.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://quq.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://mgh.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hsg.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://rdl.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://opp.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://ncu.yongpay.top

val m = mapOf("a" to 1)
来源：http://tms.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://gaa.yonumen.top

for (i in 1..10) println(i)
来源：http://lds.jqgufenzy.top

[T15] Kotlin：接口
来源：http://yox.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://jjt.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://sse.shanyushiyangtech.top

print("Hello")
来源：http://rbk.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://myu.0kj1m.cn

var a = 1;  let b = 2
来源：http://eid.aibaodan.cn

[T18] Swift：字符串插值
来源：http://tej.dianchejie.cn

"值: \(b)"
来源：http://xey.jyoumei.cn

[T19] Swift：可选绑定
来源：http://slp.xuanzx.com

if let n = opt { print(n) }
来源：http://gcq.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://wqs.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://vab.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://voj.hesvh.cn

for x in a { print(x) }
来源：http://wys.redwolf501.top

[T22] Swift：字典
来源：http://jut.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xqh.gotoacloud.top

[T23] Swift：函数
来源：http://ony.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wjy.pycfn.com

[T24] Swift：闭包
来源：http://vrs.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cdn.hywenlv.cn

[T25] Swift：结构体
来源：http://lmy.ehwqpu.com

struct P { var x: Int }
来源：http://olv.tanke756.top

[T26] Swift：类与重写
来源：http://koc.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://nsd.havefunace.top

[T27] Swift：错误处理
来源：http://nop.bbcook.cn

do { try f() } catch { print(error) }
来源：http://fbl.sxryk.cn

[T28] Swift：枚举
来源：http://end.epnwcf.com

enum Color { case red, green }
来源：http://hce.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://oci.hfpthk.cn

guard let x = opt else { return }
来源：http://arm.cdnleiting.top

[T30] Swift：协议
来源：http://lod.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://zhk.guowangkeji.top

[T31] Lua：Hello World
来源：http://skr.hammf.cn

print("Hello")
来源：http://lnh.cashguo.top

[T32] Lua：局部变量
来源：http://jll.tarul.cn

local a = 1
来源：http://szt.snrcjt.cn

[T33] Lua：表（数组）
来源：http://xzq.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wtp.aizwys.cn

[T34] Lua：遍历表
来源：http://xml.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zif.hnqzz.top

[T35] Lua：字典表
来源：http://ruc.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://ovl.feifeiyinyue.top

[T36] Lua：函数
来源：http://zhg.pycfn.com

function add(a, b) return a + b end
来源：http://yyx.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://ltn.yfazqb.com

"a" .. "b"
来源：http://kpy.hnxiangtu.top

[T38] Lua：条件
来源：http://oae.hnxiangtu.top

if x > 0 then print("正") end
来源：http://agf.snrcjt.cn

[T39] Lua：模式匹配
来源：http://iyk.zhijiandao.cn

string.find(s, "%d+")
来源：http://jyi.vehdjk.com

[T40] Lua：元表
来源：http://gcz.yj20258.top

setmetatable({}, { __index = base })
来源：http://zft.fzhhl.top

[T41] Perl：Hello World
来源：http://xfh.hammf.cn

print "Hello\n";
来源：http://juq.52xcode.cn

[T42] Perl：变量类型
来源：http://wrl.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vll.zycfv.cn

[T43] Perl：字符串插值
来源：http://vrs.nwbrower.top

"值: $a"
来源：http://pus.hammf.cn

[T44] Perl：条件
来源：http://yrl.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://dld.yangfankeji.com

[T45] Perl：数组遍历
来源：http://bxa.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://lhl.yj20258888.top

[T46] Perl：哈希操作
来源：http://htp.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://waq.chenzaomai.com

[T47] Perl：正则捕获
来源：http://xps.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://efw.gogol.net.cn

[T48] Perl：正则替换
来源：http://hfn.aibaodan.cn

$s =~ s/old/new/g;
来源：http://tcu.cashguo.top

[T49] Perl：函数
来源：http://eew.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mqv.52xcode.cn

[T50] Perl：逐行读文件
来源：http://uad.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mea.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://ubx.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://kjy.nanxinkj.top

println("Hello")
来源：http://eto.mhx1999.top

[T52] Scala：变量
来源：http://wcl.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://gyh.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://opn.xuanzx.com

s"值: $b"
来源：http://umj.zhijiandao.cn

[T54] Scala：集合映射
来源：http://zgu.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://nff.jyoumei.cn

[T55] Scala：集合过滤
来源：http://zrh.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://qem.cdnleiting.top

[T56] Scala：样例类
来源：http://ysc.jinghuilouyu.cn

case class User(name: String, age: Int)
来源：http://qav.ydjk.org.cn

[T57] Scala：模式匹配
来源：http://vjd.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rac.zhengqikj.top

[T58] Scala：函数定义
来源：http://qky.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ctv.hesvh.cn

[T59] Scala：循环
来源：http://mlu.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://ays.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://svr.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qiw.yj20258.top

================================================================================
来源：http://aco.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mos.cheryme.top

================================================================================
来源：http://ucv.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://icn.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://wzz.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://prk.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hit.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://uid.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://okw.jinghuilouyu.cn

[U04] Py：变量调试打印
来源：http://ngw.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mit.nwbrower.top

[U05] Py：列表去重且保序
来源：http://khx.sweek.top

list(dict.fromkeys(arr))
来源：http://vmx.sufxvd.cn

[U06] Py：合并两个字典
来源：http://wpq.gaohongyu789.top

{**a, **b}
来源：http://pcu.jinqigufen.top

[U07] Py：反转字典键值
来源：http://mlh.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://iqy.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://yaz.hnxiangtu.top

[y for x in nested for y in x]
来源：http://uli.bbcook.cn

[U09] Py：字典取最大值的键
来源：http://mbv.zdbjq.cn

max(d, key=d.get)
来源：http://jah.xinyue.icu

[U10] Py：按值排序字典
来源：http://oao.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cag.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://ylt.zhengqikj.top

(x * 2 for x in arr)
来源：http://tnb.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://dtx.c1oappe.top

Counter(arr).most_common(3)
来源：http://uga.jinyuanbaomall.cn

[U13] Py：固定长度队列
来源：http://qdu.hammf.cn

deque(maxlen=10)
来源：http://egz.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://lgx.guowangkeji.top

defaultdict(list)
来源：http://hrh.jlsjyb.cn

[U15] Py：高精度计时
来源：http://tog.chenlongwang.top

t = time.perf_counter()
来源：http://lmd.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://bja.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lba.hcnkem.com

[U17] Py：初始化日志
来源：http://vcv.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://rpr.aizwys.cn

[U18] Py：预编译正则
来源：http://jpy.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://dxf.fengsongda.top

[U19] Py：正则替换带回调
来源：http://qjh.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sbm.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://qte.shzxlz.cn

@functools.lru_cache(maxsize=None)
来源：http://tfv.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://ujk.feifeiyinyue.top

@contextlib.contextmanager
来源：http://ytx.zhixingplan.top

[U22] Py：矩阵转置
来源：http://ndu.xziqi.cn

list(zip(*m))
来源：http://xgu.gzhubu.top

[U23] Py：分块读取大文件
来源：http://hya.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://krs.zhijiandao.cn

[U24] Py：路径操作
来源：http://mcf.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rwu.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://kyb.tanke756.top

csv.DictReader(f)
来源：http://eje.cqqwz.cn

[U26] Py：并发下载
来源：http://euh.xziqi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ren.jianghu66.top

[U27] Py：异步 HTTP
来源：http://wjv.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://feq.yangfankeji.com

[U28] Py：类型别名
来源：http://zsk.chenzaomai.com

UserId = int
来源：http://rbc.zhongyouzk.top

[U29] Py：属性校验
来源：http://kxv.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://mdd.aibaodan.cn

[U30] Py：数据类
来源：http://dav.cheryme.top

@dataclass(slots=True)
来源：http://snm.hnxiangtu.top

[U31] Py：单测
来源：http://oul.jlsjyb.cn

python -m pytest -q
来源：http://ttq.aizwys.cn

[U32] Py：代码格式化
来源：http://wkx.tarul.cn

ruff format . && ruff check --fix .
来源：http://wov.52xcode.cn

[U33] Py：打包发布
来源：http://bhn.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://yhv.fzhhl.top

[U34] Py：判断编码
来源：http://uuw.sxryk.cn

chardet.detect(raw)
来源：http://wro.yanxiufei.cn

[U35] Py：发送邮件
来源：http://acr.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://drl.gogol.net.cn

[U36] Py：定时任务
来源：http://qbj.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://zog.hammf.cn


<!-- 参考信息 -->