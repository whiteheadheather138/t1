代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://eyb.yonumen.top

[S15] C：类型转换
来源：http://zmc.jqgufenzy.top

(double) a / b
来源：http://ujk.yj20258888.top

[S16] C：位操作置位
来源：http://zxf.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://llr.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://dvg.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vml.tianlin.xyz

[S18] C：命令行参数
来源：http://tsl.c1oappe.top

int main(int argc, char **argv)
来源：http://hme.zhiwuduotai.top

[S19] C：快速排序
来源：http://aai.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://dnq.sxryk.cn

[S20] C：二分查找
来源：http://ddv.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dxs.xylfe.cn

[S21] C：字符类别判断
来源：http://mle.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzp.yanxiufei.cn

[S22] C：字符串转数字
来源：http://nyl.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://kez.yuanzhike.top

[S23] C：随机数
来源：http://vqv.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://odc.smart0.xyz

[S24] C：获取本地时间
来源：http://qwt.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://byk.hysaishi.cn

[S25] C：内存拷贝
来源：http://gcn.quarkkingdee.top

memcpy(dst, src, n);
来源：http://url.jianghu66.top

[S26] C：内存清零
来源：http://uij.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://zan.haohaochexian.top

[S27] C：定义常量
来源：http://nmz.aizwys.cn

const double PI = 3.14159;
来源：http://lrm.ydjk.org.cn

[S28] C：静态变量
来源：http://ofc.daxiang520.top

static int counter = 0;
来源：http://itk.pycfn.com

[S29] C：变参函数
来源：http://oho.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xid.jqgfzy.top

[S30] C：头文件保护
来源：http://rfj.yj20258.top

#ifndef X_H
来源：http://cif.xinyue.icu

#define X_H
来源：http://mwu.0kj1m.cn

#endif
来源：http://fmb.tianlin.xyz

[S31] C++：Hello World
来源：http://mcw.ivvv.top

#include <iostream>
来源：http://gze.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://dpo.aizwys.cn

[S32] C++：字符串
来源：http://zzo.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://emk.fengsongda.top

[S33] C++：vector 增删
来源：http://pbe.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ciu.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://gwv.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://bkf.gaohongyu789.top

[S35] C++：map
来源：http://fdl.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ryl.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://nuc.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oxf.xingfuxueyuan.xyz

[S37] C++：set
来源：http://bds.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbn.snrcjt.cn

[S38] C++：排序
来源：http://nqr.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://iic.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://cdq.cdnleiting.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://suw.zhijiandao.cn

[S40] C++：查找元素
来源：http://xyw.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jbu.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://bfn.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tno.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://bdr.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://pcq.jiagoushi.top

[S43] C++：智能指针
来源：http://fng.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://tpa.jyoumei.cn

[S44] C++：引用传参
来源：http://fix.mhx1999.top

void inc(int &x) { ++x; }
来源：http://bny.dashuyun.cn

[S45] C++：lambda
来源：http://pdf.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://nqn.hnqzz.top

[S46] C++：函数模板
来源：http://pyw.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ihz.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://scc.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://woz.zdbjq.cn

[S48] C++：逐行读文件
来源：http://oci.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jjo.uphjek.com

while (std::getline(in, line)) { }
来源：http://nxk.yanxiufei.cn

[S49] C++：写文件
来源：http://bpy.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aaa.tarul.cn

[S50] C++：格式化数字
来源：http://gdl.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oby.yfazqb.com

[S51] C++：显式类型转换
来源：http://dbp.xinyue.icu

static_cast<double>(a) / b
来源：http://xnv.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://eyw.cucudq.cn

int size() const noexcept { return n_; }
来源：http://ctt.daxiang520.top

[S53] C++：移动语义
来源：http://eak.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://ldc.0kj1m.cn

[S54] C++：异常处理
来源：http://qct.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hwf.hysaishi.cn

[S55] C++：结构化绑定
来源：http://bcg.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xvh.aibaodan.cn

[S56] C++：optional
来源：http://nkm.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xbe.gaohongyu789.top

[S57] C++：编译期常量
来源：http://ajh.fktsv.cn

constexpr int N = 10;
来源：http://jmz.jqgfzy.top

[S58] C++：命名空间
来源：http://hbo.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://hyh.ctjpmb.com

[S59] C++：静态断言
来源：http://ulm.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://msm.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://rfu.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://icx.hfpthk.cn

================================================================================
来源：http://zvo.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ajo.guowangkeji.top

================================================================================
来源：http://spa.ybcxt.top

[T01] Kotlin：Hello World
来源：http://rml.zhongyouzk.top

println("Hello")
来源：http://lci.daxiang520.top

[T02] Kotlin：变量
来源：http://koi.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jvf.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://mon.nwbrower.top

"值: $b"
来源：http://mby.yvedp.cn

[T04] Kotlin：空安全
来源：http://rbl.jyoumei.cn

val n: String? = null;  n?.length
来源：http://nle.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://fdn.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://spt.52xcode.cn

[T06] Kotlin：集合映射
来源：http://gbj.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dvl.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://ymo.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oei.yfazqb.com

[T08] Kotlin：数据类
来源：http://fvj.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://psi.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://dkd.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://fxu.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://lre.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://dom.zdbjq.cn

[T11] Kotlin：协程
来源：http://qbq.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://fho.birdmap.top

[T12] Kotlin：解构声明
来源：http://skw.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://bdx.yj202588.top

[T13] Kotlin：只读 Map
来源：http://fyj.fehbvm.com

val m = mapOf("a" to 1)
来源：http://ohl.hammf.cn

[T14] Kotlin：循环
来源：http://zjy.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://irf.xziqi.cn

[T15] Kotlin：接口
来源：http://rcy.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://ftu.52xcode.cn

[T16] Swift：Hello World
来源：http://zxc.xylfe.cn

print("Hello")
来源：http://jew.pycfn.com

[T17] Swift：变量与常量
来源：http://xok.jqgfzy.top

var a = 1;  let b = 2
来源：http://pdf.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://nyb.sweek.top

"值: \(b)"
来源：http://xqw.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://wax.52xcode.cn

if let n = opt { print(n) }
来源：http://vdi.shuidangran.top

[T20] Swift：数组操作
来源：http://pmd.nanxuanxn.top

var a = [1, 2, 3];  a.append(4)
来源：http://kaw.quarkkingdee.top

[T21] Swift：遍历
来源：http://sao.shangyingyoupin.top

for x in a { print(x) }
来源：http://qvq.zdbjq.cn

[T22] Swift：字典
来源：http://txh.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://hyw.aibaodan.cn

[T23] Swift：函数
来源：http://xuj.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uvv.fengsongda.top

[T24] Swift：闭包
来源：http://isc.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kjj.feifeiyinyue.top

[T25] Swift：结构体
来源：http://pqv.jqgufenzy.top

struct P { var x: Int }
来源：http://wjf.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://vyq.snrcjt.cn

class A: Base { override func f() {} }
来源：http://yew.jiagoushi.top

[T27] Swift：错误处理
来源：http://vcb.yvedp.cn

do { try f() } catch { print(error) }
来源：http://uuq.daxiang520.top

[T28] Swift：枚举
来源：http://xzt.meibo888.top

enum Color { case red, green }
来源：http://umd.yonumen.top

[T29] Swift：guard 提前返回
来源：http://hrs.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://rok.havefunace.top

[T30] Swift：协议
来源：http://lja.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://gqc.jiagoushi.top

[T31] Lua：Hello World
来源：http://gli.mhx1999.top

print("Hello")
来源：http://oho.nwbrower.top

[T32] Lua：局部变量
来源：http://rxo.shanyushiyangkeji.top

local a = 1
来源：http://lmz.ivvv.top

[T33] Lua：表（数组）
来源：http://xco.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nuh.cucudq.cn

[T34] Lua：遍历表
来源：http://ywa.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xbr.pycfn.com

[T35] Lua：字典表
来源：http://tnc.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://ukt.jianghu66.top

[T36] Lua：函数
来源：http://pop.svipenyu.cn

function add(a, b) return a + b end
来源：http://pmk.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://exm.jlsjyb.cn

"a" .. "b"
来源：http://uaf.shzxlz.cn

[T38] Lua：条件
来源：http://fud.316326.xyz

if x > 0 then print("正") end
来源：http://nmt.vehdjk.com

[T39] Lua：模式匹配
来源：http://zuw.sysykeji.top

string.find(s, "%d+")
来源：http://tbk.jlsjyb.cn

[T40] Lua：元表
来源：http://uyt.yongpay.top

setmetatable({}, { __index = base })
来源：http://jru.hysaishi.cn

[T41] Perl：Hello World
来源：http://utm.xuetiantiany.cn

print "Hello\n";
来源：http://bim.kuanghao11.cn

[T42] Perl：变量类型
来源：http://bev.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eiq.cheryme.top

[T43] Perl：字符串插值
来源：http://ehh.zhixingplan.top

"值: $a"
来源：http://tzy.dashuyun.cn

[T44] Perl：条件
来源：http://eyq.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://lbo.tianlin.xyz

[T45] Perl：数组遍历
来源：http://dce.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://ups.ppjwa.cn

[T46] Perl：哈希操作
来源：http://uak.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fid.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://rkj.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fzs.52xcode.cn

[T48] Perl：正则替换
来源：http://yrm.fktsv.cn

$s =~ s/old/new/g;
来源：http://bgy.tanke756.top

[T49] Perl：函数
来源：http://vns.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jjq.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://fir.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gzi.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://fzk.dashuyun.cn

[T51] Scala：Hello World
来源：http://hbu.zhiwuduotai.top

println("Hello")
来源：http://ywy.fktsv.cn

[T52] Scala：变量
来源：http://izs.hammf.cn

val a = 1;  var b = 2
来源：http://whn.gzhubu.top

[T53] Scala：字符串插值
来源：http://bra.sysykeji.top

s"值: $b"
来源：http://gsg.yj20258888.top

[T54] Scala：集合映射
来源：http://opd.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://jmo.ybcxt.top

[T55] Scala：集合过滤
来源：http://ebm.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://vas.hysaishi.cn

[T56] Scala：样例类
来源：http://wop.hesvh.cn

case class User(name: String, age: Int)
来源：http://vbm.zhixingplan.top

[T57] Scala：模式匹配
来源：http://odv.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gpj.ppjwa.cn

[T58] Scala：函数定义
来源：http://ofd.jinqigufen.top

def add(a: Int, b: Int): Int = a + b
来源：http://wwm.hysaishi.cn

[T59] Scala：循环
来源：http://bqq.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://omy.c1oappe.top

[T60] Scala：折叠
来源：http://dfx.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gdh.fengsongda.top

================================================================================
来源：http://bnk.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jdi.uphjek.com

================================================================================
来源：http://ynk.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://ziw.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wok.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://wcg.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wjb.ivvv.top

[U03] Py：加载 .env 配置
来源：http://hci.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iep.daria6918.cn

[U04] Py：变量调试打印
来源：http://bvg.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzs.hesvh.cn

[U05] Py：列表去重且保序
来源：http://gww.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://qjc.nanxinkj.top

[U06] Py：合并两个字典
来源：http://uab.aizwys.cn

{**a, **b}
来源：http://wzm.havefunace.top

[U07] Py：反转字典键值
来源：http://gwm.cucudq.cn

{v: k for k, v in d.items()}
来源：http://cng.aibaodan.cn

[U08] Py：展平二维列表
来源：http://zkx.redwolf501.top

[y for x in nested for y in x]
来源：http://hcs.ivvv.top

[U09] Py：字典取最大值的键
来源：http://pvq.meibo888.top

max(d, key=d.get)
来源：http://ynb.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://jel.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://aag.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://vkb.c1oappe.top

(x * 2 for x in arr)
来源：http://qga.hcnkem.com

[U12] Py：取出现最多的 3 个元素
来源：http://jdz.ivvv.top

Counter(arr).most_common(3)
来源：http://vgr.iojbl.cn

[U13] Py：固定长度队列
来源：http://kvx.0kj1m.cn

deque(maxlen=10)
来源：http://ufn.ydzc1.top

[U14] Py：分组收集到列表
来源：http://fci.yvedp.cn

defaultdict(list)
来源：http://ryg.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://pqk.hywenlv.cn

t = time.perf_counter()
来源：http://avy.jinghuilouyu.cn

[U16] Py：命令行参数解析
来源：http://uvq.hesvh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rzf.shzxlz.cn

[U17] Py：初始化日志
来源：http://emp.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://xmg.zdqjudy.top

[U18] Py：预编译正则
来源：http://opb.tarul.cn

pat = re.compile(r"\d+")
来源：http://wvo.xuetiantiany.cn

[U19] Py：正则替换带回调
来源：http://qem.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jqr.wangdashe.top

[U20] Py：缓存函数结果
来源：http://koh.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://ghk.smart0.xyz

[U21] Py：自定义上下文管理器
来源：http://zug.jinqigufen.top

@contextlib.contextmanager
来源：http://tdk.316326.xyz

[U22] Py：矩阵转置
来源：http://qex.zhixingplan.top

list(zip(*m))
来源：http://njf.havefunace.top

[U23] Py：分块读取大文件
来源：http://fqv.sjlbkw.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ghb.zhoulong.xyz

[U24] Py：路径操作
来源：http://hzp.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dmt.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://fde.yongpay.top

csv.DictReader(f)
来源：http://wky.hnqzz.top

[U26] Py：并发下载
来源：http://bfa.kuanghao11.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vvd.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://kyg.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://zkc.shangyingyoupin.top

[U28] Py：类型别名
来源：http://ikv.sysykeji.top

UserId = int
来源：http://yyh.zhoulong.xyz

[U29] Py：属性校验
来源：http://ecg.52xcode.cn

@property 与 @x.setter 配合
来源：http://edc.yuanzhike.top

[U30] Py：数据类
来源：http://ctj.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://cdi.svipenyu.cn

[U31] Py：单测
来源：http://lql.quarkkingdee.top

python -m pytest -q
来源：http://rel.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://sgb.c1oappe.top

ruff format . && ruff check --fix .
来源：http://rqb.xziqi.cn

[U33] Py：打包发布
来源：http://ods.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://nax.gogol.net.cn

[U34] Py：判断编码
来源：http://whv.nanxuanxn.top

chardet.detect(raw)
来源：http://smy.havefunace.top

[U35] Py：发送邮件
来源：http://itn.yj20258888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eda.ehwqpu.com

[U36] Py：定时任务
来源：http://bdw.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://nmp.gotoacloud.top

[U37] Py：读写 Excel
来源：http://qus.iojbl.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cst.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://xzv.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://lyp.chenzaomai.com


<!-- 参考信息 -->