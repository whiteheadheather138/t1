代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ttq.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://thv.dashuyun.cn

fclose(f);
来源：http://luk.fengsongda.top

[S12] C：写文件
来源：http://tmv.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jwd.daxiang520.top

[S13] C：宏定义
来源：http://rfg.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eon.chenjidiqi.icu

[S14] C：枚举
来源：http://jnn.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://iic.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://mts.yueranfly.top

(double) a / b
来源：http://iwc.hesvh.cn

[S16] C：位操作置位
来源：http://ntk.jyoumei.cn

x |= (1 << 3);
来源：http://wdg.pycfn.com

[S17] C：安全拼接字符串
来源：http://qwj.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hld.xuanzx.com

[S18] C：命令行参数
来源：http://ipa.hywenlv.cn

int main(int argc, char **argv)
来源：http://num.yonumen.top

[S19] C：快速排序
来源：http://lhn.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://dwx.fehbvm.com

[S20] C：二分查找
来源：http://ruq.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tat.gotoacloud.top

[S21] C：字符类别判断
来源：http://puq.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gjp.mhx1999.top

[S22] C：字符串转数字
来源：http://obg.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://xsu.ppjwa.cn

[S23] C：随机数
来源：http://rzy.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dmt.yfazqb.com

[S24] C：获取本地时间
来源：http://nls.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://prx.smart0.xyz

[S25] C：内存拷贝
来源：http://tdn.jiagoushi.top

memcpy(dst, src, n);
来源：http://mzy.haohaochexian.top

[S26] C：内存清零
来源：http://buq.jqgfzy.top

memset(a, 0, sizeof a);
来源：http://kjz.zhongyouzk.top

[S27] C：定义常量
来源：http://kls.chenzaomai.com

const double PI = 3.14159;
来源：http://qar.dashuyun.cn

[S28] C：静态变量
来源：http://vgv.yj20258.top

static int counter = 0;
来源：http://hbv.cashguo.top

[S29] C：变参函数
来源：http://ggc.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xch.cashguo.top

[S30] C：头文件保护
来源：http://wrc.hcnkem.com

#ifndef X_H
来源：http://yfd.fengsongda.top

#define X_H
来源：http://tai.birdmap.top

#endif
来源：http://han.dashuyun.cn

[S31] C++：Hello World
来源：http://ynz.snrcjt.cn

#include <iostream>
来源：http://tkm.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://gxh.0kj1m.cn

[S32] C++：字符串
来源：http://bge.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://fqb.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://sxl.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tto.cqqwz.cn

[S34] C++：遍历 vector
来源：http://hae.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://qin.bjfxy.top

[S35] C++：map
来源：http://jhn.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hqn.bjfxy.top

[S36] C++：unordered_map
来源：http://jeq.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kfa.ctjpmb.com

[S37] C++：set
来源：http://ywb.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://htp.guannengcc.top

[S38] C++：排序
来源：http://wwb.sweek.top

std::sort(v.begin(), v.end());
来源：http://mzo.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://jsq.yj20258.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lel.hnxiangtu.top

[S40] C++：查找元素
来源：http://lxq.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://knk.xuanzx.com

[S41] C++：类与构造函数
来源：http://apr.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zmd.ybcxt.top

[S42] C++：继承与虚函数
来源：http://lds.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://fqs.316326.xyz

[S43] C++：智能指针
来源：http://tfj.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://zwf.zdqjudy.top

[S44] C++：引用传参
来源：http://ptp.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://wjf.quarkkingdee.top

[S45] C++：lambda
来源：http://lta.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://phk.yuanzhike.top

[S46] C++：函数模板
来源：http://wyq.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jma.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://nbv.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iyr.snrcjt.cn

[S48] C++：逐行读文件
来源：http://orp.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://jmf.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://nky.yvedp.cn

[S49] C++：写文件
来源：http://uyb.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rio.chenlongwang.top

[S50] C++：格式化数字
来源：http://wut.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://akt.9152youxi.cn

[S51] C++：显式类型转换
来源：http://iaa.hywenlv.cn

static_cast<double>(a) / b
来源：http://nvj.meibo888.top

[S52] C++：const 与 noexcept
来源：http://ptm.uphjek.com

int size() const noexcept { return n_; }
来源：http://sef.chenlongwang.top

[S53] C++：移动语义
来源：http://wzx.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://hwv.xylfe.cn

[S54] C++：异常处理
来源：http://cti.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bse.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://srl.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zco.shzxlz.cn

[S56] C++：optional
来源：http://xua.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fql.dashuyun.cn

[S57] C++：编译期常量
来源：http://oby.gaohongyu789.top

constexpr int N = 10;
来源：http://lkl.aizwys.cn

[S58] C++：命名空间
来源：http://shz.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://xzl.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://gmy.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nln.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://gmt.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ujd.fzhhl.top

================================================================================
来源：http://lip.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uiy.tanke756.top

================================================================================
来源：http://ldd.52xcode.cn

[T01] Kotlin：Hello World
来源：http://hsc.uphjek.com

println("Hello")
来源：http://wth.cheryme.top

[T02] Kotlin：变量
来源：http://aki.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ysq.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://das.cashguo.top

"值: $b"
来源：http://hvm.gogol.net.cn

[T04] Kotlin：空安全
来源：http://ifb.jqgfzy.top

val n: String? = null;  n?.length
来源：http://szd.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://rpk.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yef.sysykeji.top

[T06] Kotlin：集合映射
来源：http://swe.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://drt.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://nqg.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zel.9152youxi.cn

[T08] Kotlin：数据类
来源：http://hjf.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://izt.havefunace.top

[T09] Kotlin：扩展函数
来源：http://kdd.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://euo.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://bjj.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nbx.zycfv.cn

[T11] Kotlin：协程
来源：http://uam.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://btt.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://hos.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://gcy.uphjek.com

[T13] Kotlin：只读 Map
来源：http://gdq.yonumen.top

val m = mapOf("a" to 1)
来源：http://ext.sjlbkw.cn

[T14] Kotlin：循环
来源：http://ehf.xuanzx.com

for (i in 1..10) println(i)
来源：http://jpg.sysykeji.top

[T15] Kotlin：接口
来源：http://sbn.shuidangran.top

interface Shape { fun area(): Double }
来源：http://mht.yj202588.top

[T16] Swift：Hello World
来源：http://wye.shanyushiyangkeji.top

print("Hello")
来源：http://yaz.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://yws.fzhhl.top

var a = 1;  let b = 2
来源：http://ytw.cqqwz.cn

[T18] Swift：字符串插值
来源：http://aeh.xuanzx.com

"值: \(b)"
来源：http://mkl.jiagoushi.top

[T19] Swift：可选绑定
来源：http://xjf.zhixingplan.top

if let n = opt { print(n) }
来源：http://xat.iojbl.cn

[T20] Swift：数组操作
来源：http://cst.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://olb.zhongyouzk.top

[T21] Swift：遍历
来源：http://lsf.epnwcf.com

for x in a { print(x) }
来源：http://dbm.hesvh.cn

[T22] Swift：字典
来源：http://kuw.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vue.ehwqpu.com

[T23] Swift：函数
来源：http://qww.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://byz.fehbvm.com

[T24] Swift：闭包
来源：http://tvj.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://brd.daria6918.cn

[T25] Swift：结构体
来源：http://ykq.smart0.xyz

struct P { var x: Int }
来源：http://qax.andypj.xyz

[T26] Swift：类与重写
来源：http://epi.andypj.xyz

class A: Base { override func f() {} }
来源：http://wup.yuanzhike.top

[T27] Swift：错误处理
来源：http://cdv.yuxming.cn

do { try f() } catch { print(error) }
来源：http://gpy.yongpay.top

[T28] Swift：枚举
来源：http://uux.yj20258.top

enum Color { case red, green }
来源：http://yok.yongpay.top

[T29] Swift：guard 提前返回
来源：http://kdw.yanxiufei.cn

guard let x = opt else { return }
来源：http://fqi.yueranfly.top

[T30] Swift：协议
来源：http://klc.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://lxz.haohaochexian.top

[T31] Lua：Hello World
来源：http://ivv.jqgufenzy.top

print("Hello")
来源：http://gin.shzxlz.cn

[T32] Lua：局部变量
来源：http://iax.zycfv.cn

local a = 1
来源：http://xbp.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://otx.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yul.hywenlv.cn

[T34] Lua：遍历表
来源：http://mya.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://npm.gotoacloud.top

[T35] Lua：字典表
来源：http://ppv.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://qwf.quarkkingdee.top

[T36] Lua：函数
来源：http://owg.zhixingplan.top

function add(a, b) return a + b end
来源：http://apo.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://cbh.zhixingplan.top

"a" .. "b"
来源：http://yho.yangfankeji.com

[T38] Lua：条件
来源：http://aaf.xylfe.cn

if x > 0 then print("正") end
来源：http://iep.cucudq.cn

[T39] Lua：模式匹配
来源：http://dwh.yanxiufei.cn

string.find(s, "%d+")
来源：http://wty.chenlongwang.top

[T40] Lua：元表
来源：http://bkq.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://hbw.yuxming.cn

[T41] Perl：Hello World
来源：http://nsd.ywan-chungtsiang.top

print "Hello\n";
来源：http://his.pycfn.com

[T42] Perl：变量类型
来源：http://fwe.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vyu.jiagoushi.top

[T43] Perl：字符串插值
来源：http://cce.ydzc1.top

"值: $a"
来源：http://dqw.shzxlz.cn

[T44] Perl：条件
来源：http://iya.c1oappe.top

if ($a > 0) { print "正"; }
来源：http://hrm.dianchejie.cn

[T45] Perl：数组遍历
来源：http://nnk.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://zrx.jqgfzy.top

[T46] Perl：哈希操作
来源：http://epp.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xeo.yj202588.top

[T47] Perl：正则捕获
来源：http://vob.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hqw.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://uux.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://kfo.0kj1m.cn

[T49] Perl：函数
来源：http://ibu.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oej.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://puh.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://duk.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://qxz.ydjk.org.cn

[T51] Scala：Hello World
来源：http://arq.yvedp.cn

println("Hello")
来源：http://ess.sysykeji.top

[T52] Scala：变量
来源：http://fvq.cheryme.top

val a = 1;  var b = 2
来源：http://pny.yueranfly.top

[T53] Scala：字符串插值
来源：http://xlo.nwbrower.top

s"值: $b"
来源：http://ryl.c1oappe.top

[T54] Scala：集合映射
来源：http://auz.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://kxa.yuanzhike.top

[T55] Scala：集合过滤
来源：http://kbj.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://fvp.hongshengwenyu.top

[T56] Scala：样例类
来源：http://seb.snrcjt.cn

case class User(name: String, age: Int)
来源：http://ysb.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://wtk.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qtr.guannengcc.top

[T58] Scala：函数定义
来源：http://lkw.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://uhb.zhiwuduotai.top

[T59] Scala：循环
来源：http://uta.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://nil.ydjk.org.cn

[T60] Scala：折叠
来源：http://qcu.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tco.hesvh.cn

================================================================================
来源：http://pue.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nqz.sweek.top

================================================================================
来源：http://prc.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://qwq.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://cbv.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://weo.fktsv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://efx.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://mxo.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://von.xziqi.cn

[U04] Py：变量调试打印
来源：http://mrd.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ake.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://jct.yonumen.top

list(dict.fromkeys(arr))
来源：http://pgg.pycfn.com

[U06] Py：合并两个字典
来源：http://sfc.shuidangran.top

{**a, **b}
来源：http://epc.tian-w.cn

[U07] Py：反转字典键值
来源：http://rlj.tanke756.top

{v: k for k, v in d.items()}
来源：http://ter.sufxvd.cn

[U08] Py：展平二维列表
来源：http://fwu.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://ztq.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://bti.shangyingyoupin.top

max(d, key=d.get)
来源：http://ifp.ivvv.top

[U10] Py：按值排序字典
来源：http://qxk.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vyz.andypj.xyz

[U11] Py：生成器表达式
来源：http://woj.uphjek.com

(x * 2 for x in arr)
来源：http://utz.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://rsz.yj202588.top

Counter(arr).most_common(3)
来源：http://gss.yfazqb.com

[U13] Py：固定长度队列
来源：http://ayg.jlsjyb.cn

deque(maxlen=10)
来源：http://nen.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://fau.aizwys.cn

defaultdict(list)
来源：http://nfz.cqqwz.cn

[U15] Py：高精度计时
来源：http://ghw.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://isb.guannengcc.top

[U16] Py：命令行参数解析
来源：http://aqd.hnxiangtu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ywg.nwbrower.top

[U17] Py：初始化日志
来源：http://jdp.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://cca.316326.xyz

[U18] Py：预编译正则
来源：http://hyt.mhx1999.top

pat = re.compile(r"\d+")
来源：http://eoz.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://gps.shangyingyoupin.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://prw.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://onz.fanxiaobao.xyz

@functools.lru_cache(maxsize=None)
来源：http://hrh.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://uak.gaohongyu789.top

@contextlib.contextmanager
来源：http://wpb.ydzc1.top

[U22] Py：矩阵转置
来源：http://dtu.daxiang520.top

list(zip(*m))
来源：http://rys.havefunace.top

[U23] Py：分块读取大文件
来源：http://yzu.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fmo.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://rim.tanke756.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ret.zhixingplan.top

[U25] Py：CSV 按字典读
来源：http://cgx.fehbvm.com

csv.DictReader(f)
来源：http://bpf.sxryk.cn

[U26] Py：并发下载
来源：http://nxv.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://odn.yangfankeji.com

[U27] Py：异步 HTTP
来源：http://trd.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://vxx.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://lrr.chenjidiqi.icu

UserId = int
来源：http://tzi.fktsv.cn

[U29] Py：属性校验
来源：http://fbx.guannengcc.top

@property 与 @x.setter 配合
来源：http://anc.hongshengwenyu.top

[U30] Py：数据类
来源：http://orz.zhongyouzk.top

@dataclass(slots=True)
来源：http://fqo.smart0.xyz

[U31] Py：单测
来源：http://psy.iojbl.cn

python -m pytest -q
来源：http://ewh.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://weg.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://rth.fengsongda.top

[U33] Py：打包发布
来源：http://xix.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://wsm.yongpay.top

[U34] Py：判断编码
来源：http://zle.yangfankeji.com

chardet.detect(raw)
来源：http://bgm.chenlongwang.top


<!-- 参考信息 -->