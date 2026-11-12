代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kso.yuanzhike.top

[S13] C：宏定义
来源：http://ckg.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yog.chenzaomai.com

[S14] C：枚举
来源：http://ril.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://jaj.hysaishi.cn

[S15] C：类型转换
来源：http://xlt.yangfankeji.com

(double) a / b
来源：http://kqi.xinyue.icu

[S16] C：位操作置位
来源：http://brr.hfpthk.cn

x |= (1 << 3);
来源：http://ydd.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://ema.dashuyun.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gjo.jqgufenzy.top

[S18] C：命令行参数
来源：http://ysr.yanxiufei.cn

int main(int argc, char **argv)
来源：http://pin.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://zeg.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://xct.shangyingyoupin.top

[S20] C：二分查找
来源：http://prs.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbq.smart0.xyz

[S21] C：字符类别判断
来源：http://yyh.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rsi.yvedp.cn

[S22] C：字符串转数字
来源：http://gby.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ccn.chenlongwang.top

[S23] C：随机数
来源：http://hsb.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://emm.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://dhn.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dpg.havefunace.top

[S25] C：内存拷贝
来源：http://osh.guowangkeji.top

memcpy(dst, src, n);
来源：http://hcn.cheryme.top

[S26] C：内存清零
来源：http://yjv.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://rlx.guannengcc.top

[S27] C：定义常量
来源：http://tpl.shuidangran.top

const double PI = 3.14159;
来源：http://zpq.vehdjk.com

[S28] C：静态变量
来源：http://epu.mhx1999.top

static int counter = 0;
来源：http://vms.shangyingyoupin.top

[S29] C：变参函数
来源：http://ldb.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jhp.smart0.xyz

[S30] C：头文件保护
来源：http://gwe.cdnleiting.top

#ifndef X_H
来源：http://gti.shanyushiyangtech.top

#define X_H
来源：http://bfi.jlsjyb.cn

#endif
来源：http://fhl.shuidangran.top

[S31] C++：Hello World
来源：http://nrq.andypj.xyz

#include <iostream>
来源：http://ikg.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://yld.52xcode.cn

[S32] C++：字符串
来源：http://ves.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://cqp.sjlbkw.cn

[S33] C++：vector 增删
来源：http://fhz.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qin.svipenyu.cn

[S34] C++：遍历 vector
来源：http://vhz.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://zcv.yfazqb.com

[S35] C++：map
来源：http://ftl.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cla.yj20258888.top

[S36] C++：unordered_map
来源：http://kpq.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dkt.hesvh.cn

[S37] C++：set
来源：http://rpx.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rcc.xuetiantiany.cn

[S38] C++：排序
来源：http://qeg.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://lhq.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://evc.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hgx.aizwys.cn

[S40] C++：查找元素
来源：http://hvh.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wom.tarul.cn

[S41] C++：类与构造函数
来源：http://lvm.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rbk.tanke756.top

[S42] C++：继承与虚函数
来源：http://uqy.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://diu.cdnleiting.top

[S43] C++：智能指针
来源：http://fgc.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://tzd.dashuyun.cn

[S44] C++：引用传参
来源：http://znp.316326.xyz

void inc(int &x) { ++x; }
来源：http://xpl.chenzaomai.com

[S45] C++：lambda
来源：http://lqj.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://vii.zhoulong.xyz

[S46] C++：函数模板
来源：http://bqe.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wyo.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://iac.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qrs.tianlin.xyz

[S48] C++：逐行读文件
来源：http://izo.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://krq.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://zej.andypj.xyz

[S49] C++：写文件
来源：http://apf.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zcf.guowangkeji.top

[S50] C++：格式化数字
来源：http://rgi.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://smr.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://tey.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://lku.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://yys.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://sth.xinyue.icu

[S53] C++：移动语义
来源：http://kle.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://hxf.svipenyu.cn

[S54] C++：异常处理
来源：http://erx.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://idf.yueranfly.top

[S55] C++：结构化绑定
来源：http://bnh.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pki.havefunace.top

[S56] C++：optional
来源：http://wlc.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xdn.c1oappe.top

[S57] C++：编译期常量
来源：http://bgk.nanxinkj.top

constexpr int N = 10;
来源：http://uaw.hywenlv.cn

[S58] C++：命名空间
来源：http://bfg.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://yoy.bbcook.cn

[S59] C++：静态断言
来源：http://foj.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ipr.sweek.top

[S60] C++：遍历并删除元素
来源：http://zxm.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ruo.wangshuangyany.cn

================================================================================
来源：http://cfs.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rxa.yonumen.top

================================================================================
来源：http://asx.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://itg.zdbjq.cn

println("Hello")
来源：http://gje.yanxiufei.cn

[T02] Kotlin：变量
来源：http://jsf.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lvi.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://sse.yvedp.cn

"值: $b"
来源：http://fdt.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://ops.svipenyu.cn

val n: String? = null;  n?.length
来源：http://vxm.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://njr.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://npr.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://nqw.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://upj.ivvv.top

[T07] Kotlin：集合过滤
来源：http://hva.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://czx.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://kfq.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://ict.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://lve.hammf.cn

fun String.exclaim() = this + "!"
来源：http://kaa.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://wro.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mqp.gotoacloud.top

[T11] Kotlin：协程
来源：http://cdg.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ydz.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://nkq.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://fvy.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://orh.epnwcf.com

val m = mapOf("a" to 1)
来源：http://gjv.jyoumei.cn

[T14] Kotlin：循环
来源：http://hmb.xylfe.cn

for (i in 1..10) println(i)
来源：http://pbx.hammf.cn

[T15] Kotlin：接口
来源：http://qol.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://mal.cqqwz.cn

[T16] Swift：Hello World
来源：http://cuv.zhengqikj.top

print("Hello")
来源：http://djs.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://vhk.xylfe.cn

var a = 1;  let b = 2
来源：http://ouh.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://ftt.snrcjt.cn

"值: \(b)"
来源：http://wjd.haohaochexian.top

[T19] Swift：可选绑定
来源：http://lql.ppjwa.cn

if let n = opt { print(n) }
来源：http://uzp.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://dvr.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aun.hnxiangtu.top

[T21] Swift：遍历
来源：http://hmo.hnqzz.top

for x in a { print(x) }
来源：http://ljv.shuidangran.top

[T22] Swift：字典
来源：http://boh.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://buh.yj202588.top

[T23] Swift：函数
来源：http://rst.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nxg.aibaodan.cn

[T24] Swift：闭包
来源：http://ngp.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://idd.chenzaomai.com

[T25] Swift：结构体
来源：http://mva.gzhubu.top

struct P { var x: Int }
来源：http://mlj.xinyue.icu

[T26] Swift：类与重写
来源：http://aft.yuxming.cn

class A: Base { override func f() {} }
来源：http://gnt.chenlongwang.top

[T27] Swift：错误处理
来源：http://ygy.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://kcb.zhoulong.xyz

[T28] Swift：枚举
来源：http://bpu.jyoumei.cn

enum Color { case red, green }
来源：http://osn.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://akr.316326.xyz

guard let x = opt else { return }
来源：http://uzs.chenjidiqi.icu

[T30] Swift：协议
来源：http://qra.uphjek.com

protocol Shape { func area() -> Double }
来源：http://onq.xuanzx.com

[T31] Lua：Hello World
来源：http://oka.dashuyun.cn

print("Hello")
来源：http://mzs.sweek.top

[T32] Lua：局部变量
来源：http://tsp.yanxiufei.cn

local a = 1
来源：http://fcx.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://rhd.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uva.ydzc1.top

[T34] Lua：遍历表
来源：http://ezw.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fxb.sufxvd.cn

[T35] Lua：字典表
来源：http://xsh.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://ozf.hesvh.cn

[T36] Lua：函数
来源：http://zsk.chenzaomai.com

function add(a, b) return a + b end
来源：http://zff.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://lkb.daria6918.cn

"a" .. "b"
来源：http://qko.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://isw.xuanzx.com

if x > 0 then print("正") end
来源：http://zlx.jianghu66.top

[T39] Lua：模式匹配
来源：http://zrc.yonumen.top

string.find(s, "%d+")
来源：http://cif.yj202588.top

[T40] Lua：元表
来源：http://svi.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://ljo.tianlin.xyz

[T41] Perl：Hello World
来源：http://lzv.9152youxi.cn

print "Hello\n";
来源：http://ccl.ppjwa.cn

[T42] Perl：变量类型
来源：http://xhc.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hxa.smart0.xyz

[T43] Perl：字符串插值
来源：http://dhg.bjfxy.top

"值: $a"
来源：http://fsf.dashuyun.cn

[T44] Perl：条件
来源：http://mux.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://jao.fengsongda.top

[T45] Perl：数组遍历
来源：http://mam.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://lhp.ivvv.top

[T46] Perl：哈希操作
来源：http://ijl.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://obu.cashguo.top

[T47] Perl：正则捕获
来源：http://wib.vqdsnc.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ain.kuanghao11.cn

[T48] Perl：正则替换
来源：http://hoc.chenlongwang.top

$s =~ s/old/new/g;
来源：http://uzr.dashuyun.cn

[T49] Perl：函数
来源：http://hfw.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wry.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://tfx.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://llb.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://pdj.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://nqq.quarkkingdee.top

println("Hello")
来源：http://wxo.zhijiandao.cn

[T52] Scala：变量
来源：http://nia.hfpthk.cn

val a = 1;  var b = 2
来源：http://smv.haohaochexian.top

[T53] Scala：字符串插值
来源：http://yvb.ctjpmb.com

s"值: $b"
来源：http://jbj.pycfn.com

[T54] Scala：集合映射
来源：http://ysj.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://ypo.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://rol.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bhn.yanxiufei.cn

[T56] Scala：样例类
来源：http://xtw.jinqigfzy.top

case class User(name: String, age: Int)
来源：http://dvl.feifeiyinyue.top

[T57] Scala：模式匹配
来源：http://ubl.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iie.ppjwa.cn

[T58] Scala：函数定义
来源：http://aef.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://txm.jinghuilouyu.cn

[T59] Scala：循环
来源：http://yka.yanxiufei.cn

for (i <- 1 to 10) println(i)
来源：http://blq.svipenyu.cn

[T60] Scala：折叠
来源：http://pcy.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lok.quarkkingdee.top

================================================================================
来源：http://blv.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wrx.yfazqb.com

================================================================================
来源：http://gti.bbcook.cn

[U01] Py：创建虚拟环境
来源：http://nbj.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://qeq.kuanghao11.cn

[U02] Py：导出 / 安装依赖
来源：http://wrs.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vem.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://ctn.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qpp.shzxlz.cn

[U04] Py：变量调试打印
来源：http://uue.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eqd.jianghu66.top

[U05] Py：列表去重且保序
来源：http://mkd.yonumen.top

list(dict.fromkeys(arr))
来源：http://kfu.cdnleiting.top

[U06] Py：合并两个字典
来源：http://xqw.yj20258.top

{**a, **b}
来源：http://qhy.aibaodan.cn

[U07] Py：反转字典键值
来源：http://pcc.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://kzl.daria6918.cn

[U08] Py：展平二维列表
来源：http://zhs.xylfe.cn

[y for x in nested for y in x]
来源：http://rom.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://aik.vehdjk.com

max(d, key=d.get)
来源：http://rip.yfazqb.com

[U10] Py：按值排序字典
来源：http://oif.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lmv.jyoumei.cn

[U11] Py：生成器表达式
来源：http://bwe.hywenlv.cn

(x * 2 for x in arr)
来源：http://hnv.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wrw.fehbvm.com

Counter(arr).most_common(3)
来源：http://dis.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://qlv.vehdjk.com

deque(maxlen=10)
来源：http://uzn.zhiwuduotai.top

[U14] Py：分组收集到列表
来源：http://zfr.shangyingyoupin.top

defaultdict(list)
来源：http://lwv.yfazqb.com

[U15] Py：高精度计时
来源：http://ukl.yj202588.top

t = time.perf_counter()
来源：http://fqm.daria6918.cn

[U16] Py：命令行参数解析
来源：http://qdj.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gfv.sjlbkw.cn

[U17] Py：初始化日志
来源：http://yoi.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://bqx.chenlongwang.top

[U18] Py：预编译正则
来源：http://jkt.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://dky.xinyue.icu

[U19] Py：正则替换带回调
来源：http://yst.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zkf.yfazqb.com

[U20] Py：缓存函数结果
来源：http://nvy.aibaodan.cn

@functools.lru_cache(maxsize=None)
来源：http://bnd.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://hui.hongshengwenyu.top

@contextlib.contextmanager
来源：http://rqt.chenlongwang.top

[U22] Py：矩阵转置
来源：http://iih.yueranfly.top

list(zip(*m))
来源：http://dnb.zdbjq.cn

[U23] Py：分块读取大文件
来源：http://hbo.ehwqpu.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fds.shzxlz.cn

[U24] Py：路径操作
来源：http://asb.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ssf.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://gdk.hesvh.cn

csv.DictReader(f)
来源：http://ttu.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://sqk.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oaq.aizwys.cn

[U27] Py：异步 HTTP
来源：http://kcb.xziqi.cn

aiohttp.ClientSession() 配合 async with
来源：http://nhr.andypj.xyz

[U28] Py：类型别名
来源：http://xlp.jinyuanbaomall.cn

UserId = int
来源：http://lfl.epnwcf.com

[U29] Py：属性校验
来源：http://vzp.snrcjt.cn

@property 与 @x.setter 配合
来源：http://kjw.hfpthk.cn

[U30] Py：数据类
来源：http://jqz.tanke756.top

@dataclass(slots=True)
来源：http://nbz.aizwys.cn

[U31] Py：单测
来源：http://wix.sysykeji.top

python -m pytest -q
来源：http://nso.hysaishi.cn

[U32] Py：代码格式化
来源：http://lcb.xuetiantiany.cn

ruff format . && ruff check --fix .
来源：http://qnp.jyoumei.cn

[U33] Py：打包发布
来源：http://zzm.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://vye.jianghu66.top

[U34] Py：判断编码
来源：http://ojo.tanke756.top

chardet.detect(raw)
来源：http://bmn.nanxuanxn.top

[U35] Py：发送邮件
来源：http://btw.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://crz.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://bhv.xuetiantiany.cn

schedule.every(10).minutes.do(job)
来源：http://szh.fanxiaobao.xyz


<!-- 参考信息 -->