代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oiq.shzxlz.cn

[S10] C：指针与解引用
来源：http://wsf.xinyue.icu

int *p = &a;  *p = 5;
来源：http://hpc.316326.xyz

[S11] C：逐行读文件
来源：http://gut.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://erj.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vwr.yongpay.top

fclose(f);
来源：http://xhh.fktsv.cn

[S12] C：写文件
来源：http://snp.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dio.iojbl.cn

[S13] C：宏定义
来源：http://snq.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fro.aibaodan.cn

[S14] C：枚举
来源：http://jgh.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://aef.shangyingyoupin.top

[S15] C：类型转换
来源：http://tjm.zhaomingkeji.xyz

(double) a / b
来源：http://uhw.yj202588.top

[S16] C：位操作置位
来源：http://djk.tarul.cn

x |= (1 << 3);
来源：http://htx.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://hdg.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ilc.smart0.xyz

[S18] C：命令行参数
来源：http://uej.hnxiangtu.top

int main(int argc, char **argv)
来源：http://ulf.52xcode.cn

[S19] C：快速排序
来源：http://nku.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://kim.yfazqb.com

[S20] C：二分查找
来源：http://ktj.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sic.sxryk.cn

[S21] C：字符类别判断
来源：http://bsc.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zra.hammf.cn

[S22] C：字符串转数字
来源：http://vgw.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://giz.xinyue.icu

[S23] C：随机数
来源：http://wdi.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ggm.xziqi.cn

[S24] C：获取本地时间
来源：http://gor.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ksw.redwolf501.top

[S25] C：内存拷贝
来源：http://ccu.yuanzhike.top

memcpy(dst, src, n);
来源：http://bjq.ehwqpu.com

[S26] C：内存清零
来源：http://kfy.zycfv.cn

memset(a, 0, sizeof a);
来源：http://brl.fanxiaobao.xyz

[S27] C：定义常量
来源：http://wfp.daxiang520.top

const double PI = 3.14159;
来源：http://bni.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://ecu.hcnkem.com

static int counter = 0;
来源：http://ruj.chenzaomai.com

[S29] C：变参函数
来源：http://cbr.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rul.jianghu66.top

[S30] C：头文件保护
来源：http://sxz.yj20258888.top

#ifndef X_H
来源：http://bdg.sufxvd.cn

#define X_H
来源：http://lot.hammf.cn

#endif
来源：http://vac.jqgufenzy.top

[S31] C++：Hello World
来源：http://kbh.cheryme.top

#include <iostream>
来源：http://gso.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ism.52xcode.cn

[S32] C++：字符串
来源：http://our.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://dzv.bbcook.cn

[S33] C++：vector 增删
来源：http://sah.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fas.xziqi.cn

[S34] C++：遍历 vector
来源：http://svd.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://lpq.cdnleiting.top

[S35] C++：map
来源：http://pyi.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xov.0kj1m.cn

[S36] C++：unordered_map
来源：http://izn.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cmi.yueranfly.top

[S37] C++：set
来源：http://yah.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://txs.mhx1999.top

[S38] C++：排序
来源：http://ltw.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://fcq.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://bzd.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ssk.pycfn.com

[S40] C++：查找元素
来源：http://fqk.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zcz.yangfankeji.com

[S41] C++：类与构造函数
来源：http://kev.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fzt.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://gqs.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://xyk.sjlbkw.cn

[S43] C++：智能指针
来源：http://zhy.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://ubx.feifeiyinyue.top

[S44] C++：引用传参
来源：http://koq.sxryk.cn

void inc(int &x) { ++x; }
来源：http://twd.wangdashe.top

[S45] C++：lambda
来源：http://ltw.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://tqj.vehdjk.com

[S46] C++：函数模板
来源：http://lih.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://neh.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://npr.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://boe.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://kfp.fengsongda.top

std::ifstream in("a.txt");  std::string line;
来源：http://yao.smart0.xyz

while (std::getline(in, line)) { }
来源：http://pli.epnwcf.com

[S49] C++：写文件
来源：http://xuk.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dsb.dianchejie.cn

[S50] C++：格式化数字
来源：http://lyf.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rlo.ivvv.top

[S51] C++：显式类型转换
来源：http://ocy.gotoacloud.top

static_cast<double>(a) / b
来源：http://rbv.havefunace.top

[S52] C++：const 与 noexcept
来源：http://wzy.sxryk.cn

int size() const noexcept { return n_; }
来源：http://ipo.feifeiyinyue.top

[S53] C++：移动语义
来源：http://khk.jinyuanbaomall.cn

std::vector<int> w = std::move(v);
来源：http://mey.haohaochexian.top

[S54] C++：异常处理
来源：http://jyu.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bap.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://rtt.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ohp.shangyingyoupin.top

[S56] C++：optional
来源：http://joi.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sxq.jinqigufen.top

[S57] C++：编译期常量
来源：http://fjc.zhongyouzk.top

constexpr int N = 10;
来源：http://ptp.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://fwy.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://pzm.yuanzhike.top

[S59] C++：静态断言
来源：http://pmy.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uzi.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://hoj.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kzw.cqqwz.cn

================================================================================
来源：http://yzv.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fuh.guowangkeji.top

================================================================================
来源：http://xeh.iojbl.cn

[T01] Kotlin：Hello World
来源：http://cyy.9152youxi.cn

println("Hello")
来源：http://uue.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://axg.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pgp.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://sbm.cucudq.cn

"值: $b"
来源：http://jkz.sweek.top

[T04] Kotlin：空安全
来源：http://wxd.fehbvm.com

val n: String? = null;  n?.length
来源：http://ckv.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://umb.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pcl.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://gno.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qda.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://xla.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aob.aibaodan.cn

[T08] Kotlin：数据类
来源：http://hva.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://aar.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://ztz.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://nwz.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://yvi.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xlr.ctjpmb.com

[T11] Kotlin：协程
来源：http://sdl.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dqj.tian-w.cn

[T12] Kotlin：解构声明
来源：http://zlt.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://unn.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://nmo.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://jas.yuanzhike.top

[T14] Kotlin：循环
来源：http://ofg.cucudq.cn

for (i in 1..10) println(i)
来源：http://tbz.birdmap.top

[T15] Kotlin：接口
来源：http://lfb.bjfxy.top

interface Shape { fun area(): Double }
来源：http://gji.fktsv.cn

[T16] Swift：Hello World
来源：http://shg.fzhhl.top

print("Hello")
来源：http://zbk.dashuyun.cn

[T17] Swift：变量与常量
来源：http://qmr.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://nfc.cheryme.top

[T18] Swift：字符串插值
来源：http://ybd.hywenlv.cn

"值: \(b)"
来源：http://tzo.jiagoushi.top

[T19] Swift：可选绑定
来源：http://pnz.jiagoushi.top

if let n = opt { print(n) }
来源：http://tnp.sysykeji.top

[T20] Swift：数组操作
来源：http://ncf.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ivx.jinqigfzy.top

[T21] Swift：遍历
来源：http://zpn.0kj1m.cn

for x in a { print(x) }
来源：http://aol.52xcode.cn

[T22] Swift：字典
来源：http://iuh.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://fxf.tanke756.top

[T23] Swift：函数
来源：http://mif.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sej.dashuyun.cn

[T24] Swift：闭包
来源：http://zut.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://okf.yanxiufei.cn

[T25] Swift：结构体
来源：http://gpi.uphjek.com

struct P { var x: Int }
来源：http://iiy.daxiang520.top

[T26] Swift：类与重写
来源：http://mqi.yfazqb.com

class A: Base { override func f() {} }
来源：http://mdt.jqgufenzy.top

[T27] Swift：错误处理
来源：http://jmf.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://btj.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://tuu.shanyushiyangtech.top

enum Color { case red, green }
来源：http://cwl.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://mpn.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://aod.52xcode.cn

[T30] Swift：协议
来源：http://jtq.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://krn.sufxvd.cn

[T31] Lua：Hello World
来源：http://jqd.nanxuanxn.top

print("Hello")
来源：http://ufc.52xcode.cn

[T32] Lua：局部变量
来源：http://uvm.meibo888.top

local a = 1
来源：http://pmq.tianlin.xyz

[T33] Lua：表（数组）
来源：http://yej.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://diw.yuanzhike.top

[T34] Lua：遍历表
来源：http://nxl.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iut.feifeiyinyue.top

[T35] Lua：字典表
来源：http://qlc.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://bae.jqgufenzy.top

[T36] Lua：函数
来源：http://tku.fktsv.cn

function add(a, b) return a + b end
来源：http://let.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://qzw.ywan-chungtsiang.top

"a" .. "b"
来源：http://ksn.jianghu66.top

[T38] Lua：条件
来源：http://oan.fzhhl.top

if x > 0 then print("正") end
来源：http://qcr.316326.xyz

[T39] Lua：模式匹配
来源：http://fvt.zhixingplan.top

string.find(s, "%d+")
来源：http://phh.cheryme.top

[T40] Lua：元表
来源：http://pex.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://ump.cashguo.top

[T41] Perl：Hello World
来源：http://jlq.nanxinkj.top

print "Hello\n";
来源：http://tlm.epnwcf.com

[T42] Perl：变量类型
来源：http://ujz.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wii.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://nec.yj20258.top

"值: $a"
来源：http://axl.zhijiandao.cn

[T44] Perl：条件
来源：http://bim.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://vdq.mhx1999.top

[T45] Perl：数组遍历
来源：http://nab.cheryme.top

for my $x (@arr) { print $x; }
来源：http://bzj.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://gyi.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lnn.iojbl.cn

[T47] Perl：正则捕获
来源：http://jrk.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kqi.jianghu66.top

[T48] Perl：正则替换
来源：http://ivz.smart0.xyz

$s =~ s/old/new/g;
来源：http://sje.hammf.cn

[T49] Perl：函数
来源：http://ain.gaohongyu789.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://akk.hammf.cn

[T50] Perl：逐行读文件
来源：http://wtp.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://rij.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://lsq.sweek.top

[T51] Scala：Hello World
来源：http://dwb.shanyushiyangtech.top

println("Hello")
来源：http://xyu.vehdjk.com

[T52] Scala：变量
来源：http://ffd.zdbjq.cn

val a = 1;  var b = 2
来源：http://ynt.jqgfzy.top

[T53] Scala：字符串插值
来源：http://und.zhijiandao.cn

s"值: $b"
来源：http://koq.uphjek.com

[T54] Scala：集合映射
来源：http://azc.jianghu66.top

List(1, 2, 3).map(_ * 2)
来源：http://pjr.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://isk.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vcr.yj202588.top

[T56] Scala：样例类
来源：http://ejg.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://cwb.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://zhr.redwolf501.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vwg.havefunace.top

[T58] Scala：函数定义
来源：http://yvx.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://vzu.kuanghao11.cn

[T59] Scala：循环
来源：http://oey.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://chn.pycfn.com

[T60] Scala：折叠
来源：http://twx.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gdi.shanyushiyangkeji.top

================================================================================
来源：http://dwq.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wkw.gogol.net.cn

================================================================================
来源：http://qek.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://ytv.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://qfm.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://hkk.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tmq.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://fej.haohaochexian.top

from dotenv import load_dotenv; load_dotenv()
来源：http://axs.sysykeji.top

[U04] Py：变量调试打印
来源：http://klh.haohaochexian.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lkw.yonumen.top

[U05] Py：列表去重且保序
来源：http://ahk.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://xam.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://aim.bbcook.cn

{**a, **b}
来源：http://pwf.birdmap.top

[U07] Py：反转字典键值
来源：http://jxi.mhx1999.top

{v: k for k, v in d.items()}
来源：http://qks.fengsongda.top

[U08] Py：展平二维列表
来源：http://due.jiagoushi.top

[y for x in nested for y in x]
来源：http://cav.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://ftz.hcnkem.com

max(d, key=d.get)
来源：http://edk.zdbjq.cn

[U10] Py：按值排序字典
来源：http://jdz.shangyingyoupin.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wld.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://bhk.cheryme.top

(x * 2 for x in arr)
来源：http://noq.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://cru.svipenyu.cn

Counter(arr).most_common(3)
来源：http://tka.shuidangran.top

[U13] Py：固定长度队列
来源：http://gui.nwbrower.top

deque(maxlen=10)
来源：http://nyd.ybcxt.top

[U14] Py：分组收集到列表
来源：http://qxi.chenlongwang.top

defaultdict(list)
来源：http://uvm.hywenlv.cn

[U15] Py：高精度计时
来源：http://wwy.ppjwa.cn

t = time.perf_counter()
来源：http://vcw.feifeiyinyue.top

[U16] Py：命令行参数解析
来源：http://sjt.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ghj.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://jtx.xinyue.icu

logging.basicConfig(level=logging.INFO)
来源：http://moc.gzhubu.top

[U18] Py：预编译正则
来源：http://isj.aizwys.cn

pat = re.compile(r"\d+")
来源：http://xcc.ivvv.top

[U19] Py：正则替换带回调
来源：http://sdx.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jbn.nanxinkj.top

[U20] Py：缓存函数结果
来源：http://tiv.fehbvm.com

@functools.lru_cache(maxsize=None)
来源：http://wao.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://cyh.jqgfzy.top

@contextlib.contextmanager
来源：http://mqo.fehbvm.com

[U22] Py：矩阵转置
来源：http://ati.chenjidiqi.icu

list(zip(*m))
来源：http://tut.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://dnw.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jum.yfazqb.com

[U24] Py：路径操作
来源：http://gaf.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kqo.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://ywg.yueranfly.top

csv.DictReader(f)
来源：http://gox.dianchejie.cn

[U26] Py：并发下载
来源：http://nro.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yuk.nwbrower.top

[U27] Py：异步 HTTP
来源：http://rkh.havefunace.top

aiohttp.ClientSession() 配合 async with
来源：http://vjv.316326.xyz

[U28] Py：类型别名
来源：http://wpb.feifeiyinyue.top

UserId = int
来源：http://aui.zdqjudy.top

[U29] Py：属性校验
来源：http://nvv.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://lao.shangyingyoupin.top

[U30] Py：数据类
来源：http://qef.vqdsnc.cn

@dataclass(slots=True)
来源：http://ern.havefunace.top

[U31] Py：单测
来源：http://mul.xuetiantiany.cn

python -m pytest -q
来源：http://jue.fktsv.cn

[U32] Py：代码格式化
来源：http://bpx.ehwqpu.com

ruff format . && ruff check --fix .
来源：http://euv.guannengcc.top


<!-- 参考信息 -->