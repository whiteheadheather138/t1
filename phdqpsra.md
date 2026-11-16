代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://eyz.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jmn.ybcxt.top

fclose(f);
来源：http://moh.birdmap.top

[S12] C：写文件
来源：http://ark.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twl.yj20258.top

[S13] C：宏定义
来源：http://tde.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bdr.hywenlv.cn

[S14] C：枚举
来源：http://uka.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://dyq.hongshengwenyu.top

[S15] C：类型转换
来源：http://vig.shanyushiyangtech.top

(double) a / b
来源：http://snt.ydzc1.top

[S16] C：位操作置位
来源：http://ssv.shangyingyoupin.top

x |= (1 << 3);
来源：http://blp.daxiang520.top

[S17] C：安全拼接字符串
来源：http://qsg.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nso.yueranfly.top

[S18] C：命令行参数
来源：http://ghe.snrcjt.cn

int main(int argc, char **argv)
来源：http://lhi.fanxiaobao.xyz

[S19] C：快速排序
来源：http://oje.daxiang520.top

qsort(a, n, sizeof(int), cmp);
来源：http://gyp.quarkkingdee.top

[S20] C：二分查找
来源：http://mgy.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://axq.0kj1m.cn

[S21] C：字符类别判断
来源：http://sby.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://atj.zdqjudy.top

[S22] C：字符串转数字
来源：http://rxu.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jhc.ivvv.top

[S23] C：随机数
来源：http://fma.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uky.ehwqpu.com

[S24] C：获取本地时间
来源：http://rat.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hwr.316326.xyz

[S25] C：内存拷贝
来源：http://mmw.vehdjk.com

memcpy(dst, src, n);
来源：http://jcg.xylfe.cn

[S26] C：内存清零
来源：http://tee.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://mig.zhongyouzk.top

[S27] C：定义常量
来源：http://pxk.zhengqikj.top

const double PI = 3.14159;
来源：http://rva.yuanzhike.top

[S28] C：静态变量
来源：http://sdk.xuanzx.com

static int counter = 0;
来源：http://thg.hysaishi.cn

[S29] C：变参函数
来源：http://rcs.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ouu.yongpay.top

[S30] C：头文件保护
来源：http://dec.haohaochexian.top

#ifndef X_H
来源：http://efd.cqqwz.cn

#define X_H
来源：http://syq.guannengcc.top

#endif
来源：http://xot.uphjek.com

[S31] C++：Hello World
来源：http://bol.yuanzhike.top

#include <iostream>
来源：http://bou.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://dih.aibaodan.cn

[S32] C++：字符串
来源：http://zfe.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://ums.yuanzhike.top

[S33] C++：vector 增删
来源：http://qql.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ppq.jinqigufen.top

[S34] C++：遍历 vector
来源：http://lbv.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://baq.aibaodan.cn

[S35] C++：map
来源：http://hkm.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wlf.hnqzz.top

[S36] C++：unordered_map
来源：http://gsg.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lsl.zhijiandao.cn

[S37] C++：set
来源：http://hxd.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dht.ydjk.org.cn

[S38] C++：排序
来源：http://jud.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://bbd.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://vik.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vin.yangfankeji.com

[S40] C++：查找元素
来源：http://gvt.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cap.shuidangran.top

[S41] C++：类与构造函数
来源：http://sur.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gtz.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://pda.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://ujn.jianghu66.top

[S43] C++：智能指针
来源：http://vea.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://hxp.jqgufenzy.top

[S44] C++：引用传参
来源：http://vur.wangdashe.top

void inc(int &x) { ++x; }
来源：http://fof.xuetiantiany.cn

[S45] C++：lambda
来源：http://nvm.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://joz.xziqi.cn

[S46] C++：函数模板
来源：http://wjq.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vvb.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://inu.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cwh.haohaochexian.top

[S48] C++：逐行读文件
来源：http://dcm.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://xpc.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://iwv.nwbrower.top

[S49] C++：写文件
来源：http://zax.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eqi.fzhhl.top

[S50] C++：格式化数字
来源：http://raa.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xmw.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://xfh.yuanzhike.top

static_cast<double>(a) / b
来源：http://wlk.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://wgd.yuxming.cn

int size() const noexcept { return n_; }
来源：http://xae.pycfn.com

[S53] C++：移动语义
来源：http://hpp.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://kkz.havefunace.top

[S54] C++：异常处理
来源：http://hjr.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fmw.dianchejie.cn

[S55] C++：结构化绑定
来源：http://ofo.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dby.yvedp.cn

[S56] C++：optional
来源：http://lpg.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://itu.sxryk.cn

[S57] C++：编译期常量
来源：http://eyk.yuanzhike.top

constexpr int N = 10;
来源：http://ywr.9152youxi.cn

[S58] C++：命名空间
来源：http://fwg.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://ebp.sjlbkw.cn

[S59] C++：静态断言
来源：http://uio.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mey.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://kww.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://asu.ehwqpu.com

================================================================================
来源：http://uoh.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oim.chenjidiqi.icu

================================================================================
来源：http://cdx.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://fjv.jianghu66.top

println("Hello")
来源：http://xqb.guowangkeji.top

[T02] Kotlin：变量
来源：http://pmf.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rcf.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://bno.jinqigfzy.top

"值: $b"
来源：http://bur.gotoacloud.top

[T04] Kotlin：空安全
来源：http://xoh.guowangkeji.top

val n: String? = null;  n?.length
来源：http://mbc.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://fdk.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ziv.havefunace.top

[T06] Kotlin：集合映射
来源：http://wio.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ojw.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://dee.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fhs.cdnleiting.top

[T08] Kotlin：数据类
来源：http://wmj.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://uiz.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://trm.yonumen.top

fun String.exclaim() = this + "!"
来源：http://mmw.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://whr.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wyp.zycfv.cn

[T11] Kotlin：协程
来源：http://mmx.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://jyr.yonumen.top

[T12] Kotlin：解构声明
来源：http://nhy.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://kys.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://cvo.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://yqn.dianchejie.cn

[T14] Kotlin：循环
来源：http://nyi.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://vzh.yuxming.cn

[T15] Kotlin：接口
来源：http://oqj.sweek.top

interface Shape { fun area(): Double }
来源：http://yqk.jqgufenzy.top

[T16] Swift：Hello World
来源：http://mde.hysaishi.cn

print("Hello")
来源：http://osr.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://kwh.yonumen.top

var a = 1;  let b = 2
来源：http://lpq.gotoacloud.top

[T18] Swift：字符串插值
来源：http://oes.jiagoushi.top

"值: \(b)"
来源：http://klc.ctjpmb.com

[T19] Swift：可选绑定
来源：http://lrp.svipenyu.cn

if let n = opt { print(n) }
来源：http://syw.iojbl.cn

[T20] Swift：数组操作
来源：http://hks.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://ljs.smart0.xyz

[T21] Swift：遍历
来源：http://nmv.jianghu66.top

for x in a { print(x) }
来源：http://scv.zdqjudy.top

[T22] Swift：字典
来源：http://kou.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://plz.yueranfly.top

[T23] Swift：函数
来源：http://ocw.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kvo.havefunace.top

[T24] Swift：闭包
来源：http://krp.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://lfq.9152youxi.cn

[T25] Swift：结构体
来源：http://zie.quarkkingdee.top

struct P { var x: Int }
来源：http://ehv.zdqjudy.top

[T26] Swift：类与重写
来源：http://asa.hnqzz.top

class A: Base { override func f() {} }
来源：http://nls.smart0.xyz

[T27] Swift：错误处理
来源：http://nfk.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://seo.jqgufenzy.top

[T28] Swift：枚举
来源：http://jet.meibo888.top

enum Color { case red, green }
来源：http://miv.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://wal.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://jln.ehwqpu.com

[T30] Swift：协议
来源：http://twh.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://ibk.jqgufenzy.top

[T31] Lua：Hello World
来源：http://cxc.yj20258.top

print("Hello")
来源：http://ydd.svipenyu.cn

[T32] Lua：局部变量
来源：http://ofa.yanxiufei.cn

local a = 1
来源：http://zcv.hfpthk.cn

[T33] Lua：表（数组）
来源：http://ujx.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kme.shuidangran.top

[T34] Lua：遍历表
来源：http://yxu.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nni.pengpengdd.cyou

[T35] Lua：字典表
来源：http://ynk.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://zvr.redwolf501.top

[T36] Lua：函数
来源：http://nid.jiagoushi.top

function add(a, b) return a + b end
来源：http://bvk.yueranfly.top

[T37] Lua：字符串拼接
来源：http://zxn.quarkkingdee.top

"a" .. "b"
来源：http://znc.hcnkem.com

[T38] Lua：条件
来源：http://jtu.fktsv.cn

if x > 0 then print("正") end
来源：http://sxu.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://wga.sxryk.cn

string.find(s, "%d+")
来源：http://esz.andypj.xyz

[T40] Lua：元表
来源：http://euo.cucudq.cn

setmetatable({}, { __index = base })
来源：http://rjo.cqqwz.cn

[T41] Perl：Hello World
来源：http://okr.pycfn.com

print "Hello\n";
来源：http://jmx.vqdsnc.cn

[T42] Perl：变量类型
来源：http://tbn.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://svk.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://chz.shangyingyoupin.top

"值: $a"
来源：http://ffw.kuanghao11.cn

[T44] Perl：条件
来源：http://kgb.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://gka.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://ddj.birdmap.top

for my $x (@arr) { print $x; }
来源：http://xse.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://hgf.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pmm.cqqwz.cn

[T47] Perl：正则捕获
来源：http://bos.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qnd.vehdjk.com

[T48] Perl：正则替换
来源：http://kff.bjfxy.top

$s =~ s/old/new/g;
来源：http://coo.andypj.xyz

[T49] Perl：函数
来源：http://ene.ppjwa.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mjs.gzhubu.top

[T50] Perl：逐行读文件
来源：http://wnn.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yff.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://kul.pycfn.com

[T51] Scala：Hello World
来源：http://zdw.ehwqpu.com

println("Hello")
来源：http://awz.havefunace.top

[T52] Scala：变量
来源：http://nkt.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://prz.guowangkeji.top

[T53] Scala：字符串插值
来源：http://kzx.hfpthk.cn

s"值: $b"
来源：http://kgf.yueranfly.top

[T54] Scala：集合映射
来源：http://ale.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://yrh.shzxlz.cn

[T55] Scala：集合过滤
来源：http://vnm.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cyt.yueranfly.top

[T56] Scala：样例类
来源：http://zky.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://cvu.redwolf501.top

[T57] Scala：模式匹配
来源：http://sdr.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wjr.epnwcf.com

[T58] Scala：函数定义
来源：http://eid.zhongyouzk.top

def add(a: Int, b: Int): Int = a + b
来源：http://eyx.ybcxt.top

[T59] Scala：循环
来源：http://thk.sweek.top

for (i <- 1 to 10) println(i)
来源：http://udo.yj20258888.top

[T60] Scala：折叠
来源：http://qxo.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mhb.yuanzhike.top

================================================================================
来源：http://pcn.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qjb.cqqwz.cn

================================================================================
来源：http://msz.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://rxy.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cdp.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://htw.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://spu.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://ogz.yvedp.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qdk.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://wrz.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hfx.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://zde.cucudq.cn

list(dict.fromkeys(arr))
来源：http://dlv.svipenyu.cn

[U06] Py：合并两个字典
来源：http://ojt.fktsv.cn

{**a, **b}
来源：http://bah.cashguo.top

[U07] Py：反转字典键值
来源：http://wng.vehdjk.com

{v: k for k, v in d.items()}
来源：http://rjp.bbcook.cn

[U08] Py：展平二维列表
来源：http://qww.ivvv.top

[y for x in nested for y in x]
来源：http://cmi.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://tll.aibaodan.cn

max(d, key=d.get)
来源：http://cis.0kj1m.cn

[U10] Py：按值排序字典
来源：http://jlv.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmm.ctjpmb.com

[U11] Py：生成器表达式
来源：http://fyc.gaohongyu789.top

(x * 2 for x in arr)
来源：http://jmc.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://oie.ctjpmb.com

Counter(arr).most_common(3)
来源：http://fkd.dianchejie.cn

[U13] Py：固定长度队列
来源：http://tsj.xziqi.cn

deque(maxlen=10)
来源：http://hov.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://drb.ivvv.top

defaultdict(list)
来源：http://byc.hnxiangtu.top

[U15] Py：高精度计时
来源：http://lox.ivvv.top

t = time.perf_counter()
来源：http://hgb.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://dyd.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pnm.jianghu66.top

[U17] Py：初始化日志
来源：http://cvg.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://lhk.gaohongyu789.top

[U18] Py：预编译正则
来源：http://wjm.shuidangran.top

pat = re.compile(r"\d+")
来源：http://fea.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://gjn.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://res.yueranfly.top

[U20] Py：缓存函数结果
来源：http://rki.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://ptq.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://dbd.ivvv.top

@contextlib.contextmanager
来源：http://vsi.mhx1999.top

[U22] Py：矩阵转置
来源：http://szs.xingfuxueyuan.xyz

list(zip(*m))
来源：http://nfd.ivvv.top

[U23] Py：分块读取大文件
来源：http://ztr.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://czi.xylfe.cn

[U24] Py：路径操作
来源：http://rcy.tarul.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nug.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://lsv.xziqi.cn

csv.DictReader(f)
来源：http://wpb.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://qyf.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wue.daxiang520.top

[U27] Py：异步 HTTP
来源：http://oti.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://yzb.fktsv.cn

[U28] Py：类型别名
来源：http://kbl.yuanzhike.top

UserId = int
来源：http://gxa.52xcode.cn

[U29] Py：属性校验
来源：http://jmx.aizwys.cn

@property 与 @x.setter 配合
来源：http://gny.gzhubu.top

[U30] Py：数据类
来源：http://jlf.ydjk.org.cn

@dataclass(slots=True)
来源：http://rbx.fktsv.cn

[U31] Py：单测
来源：http://wwv.yueranfly.top

python -m pytest -q
来源：http://hmo.fzhhl.top

[U32] Py：代码格式化
来源：http://ugv.zhijiandao.cn

ruff format . && ruff check --fix .
来源：http://tyh.birdmap.top

[U33] Py：打包发布
来源：http://cod.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://dks.iojbl.cn

[U34] Py：判断编码
来源：http://skm.chenlongwang.top

chardet.detect(raw)
来源：http://jur.316326.xyz


<!-- 参考信息 -->