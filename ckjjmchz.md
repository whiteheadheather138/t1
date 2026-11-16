代发 wailian999

x |= (1 << 3);
来源：http://qdu.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://rjk.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://frm.xylfe.cn

[S18] C：命令行参数
来源：http://aqv.nanxinkj.top

int main(int argc, char **argv)
来源：http://bcq.vqdsnc.cn

[S19] C：快速排序
来源：http://yir.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ojm.316326.xyz

[S20] C：二分查找
来源：http://wto.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdj.vehdjk.com

[S21] C：字符类别判断
来源：http://itl.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qet.yj20258.top

[S22] C：字符串转数字
来源：http://tdm.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://ppi.ywan-chungtsiang.top

[S23] C：随机数
来源：http://axt.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mzo.c1oappe.top

[S24] C：获取本地时间
来源：http://gmo.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tpc.yvedp.cn

[S25] C：内存拷贝
来源：http://lfk.gzhubu.top

memcpy(dst, src, n);
来源：http://umu.uphjek.com

[S26] C：内存清零
来源：http://xdq.iojbl.cn

memset(a, 0, sizeof a);
来源：http://opp.cashguo.top

[S27] C：定义常量
来源：http://cwg.xylfe.cn

const double PI = 3.14159;
来源：http://vte.guannengcc.top

[S28] C：静态变量
来源：http://sym.gzhubu.top

static int counter = 0;
来源：http://dxm.zhoulong.xyz

[S29] C：变参函数
来源：http://mfd.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pys.jqgfzy.top

[S30] C：头文件保护
来源：http://rpf.hnxiangtu.top

#ifndef X_H
来源：http://prz.ybcxt.top

#define X_H
来源：http://yfa.yj20258.top

#endif
来源：http://riq.tianlin.xyz

[S31] C++：Hello World
来源：http://axo.yonumen.top

#include <iostream>
来源：http://iem.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ovr.yvedp.cn

[S32] C++：字符串
来源：http://bfg.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://xby.yj202588.top

[S33] C++：vector 增删
来源：http://crg.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvl.shuidangran.top

[S34] C++：遍历 vector
来源：http://hmd.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://chb.zhijiandao.cn

[S35] C++：map
来源：http://yhb.xinyue.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gsh.sxryk.cn

[S36] C++：unordered_map
来源：http://qmu.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gkz.fzhhl.top

[S37] C++：set
来源：http://goq.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ida.nanxinkj.top

[S38] C++：排序
来源：http://ptv.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://nxs.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://ppy.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rae.jqgfzy.top

[S40] C++：查找元素
来源：http://nzb.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjg.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://cbn.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xjj.cheryme.top

[S42] C++：继承与虚函数
来源：http://amm.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://ssb.hywenlv.cn

[S43] C++：智能指针
来源：http://mmu.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://tzo.yj202588.top

[S44] C++：引用传参
来源：http://rmo.wangdashe.top

void inc(int &x) { ++x; }
来源：http://zxa.hammf.cn

[S45] C++：lambda
来源：http://aji.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gxz.ydjk.org.cn

[S46] C++：函数模板
来源：http://woz.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bll.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://wwa.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nqw.snrcjt.cn

[S48] C++：逐行读文件
来源：http://wei.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://stc.hnqzz.top

while (std::getline(in, line)) { }
来源：http://gjr.dashuyun.cn

[S49] C++：写文件
来源：http://pwo.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ydo.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://mrt.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vgn.ctjpmb.com

[S51] C++：显式类型转换
来源：http://luc.xinyue.icu

static_cast<double>(a) / b
来源：http://wug.yonumen.top

[S52] C++：const 与 noexcept
来源：http://dfx.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://gwb.chenjidiqi.icu

[S53] C++：移动语义
来源：http://jve.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://nsq.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://nlx.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ilq.hcnkem.com

[S55] C++：结构化绑定
来源：http://reu.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://orr.xziqi.cn

[S56] C++：optional
来源：http://nwn.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wbm.fzhhl.top

[S57] C++：编译期常量
来源：http://jxs.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://zqn.feifeiyinyue.top

[S58] C++：命名空间
来源：http://qgu.bbcook.cn

namespace ns { int f() { return 1; } }
来源：http://rst.hongshengwenyu.top

[S59] C++：静态断言
来源：http://lpu.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vto.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://iwb.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gmb.shuidangran.top

================================================================================
来源：http://utr.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://suz.yanxiufei.cn

================================================================================
来源：http://zeg.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://wbp.bjfxy.top

println("Hello")
来源：http://crx.fktsv.cn

[T02] Kotlin：变量
来源：http://hwp.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kvn.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://zly.jinyuanbaomall.cn

"值: $b"
来源：http://ogj.fzhhl.top

[T04] Kotlin：空安全
来源：http://rlu.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://noo.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://auh.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iqo.andypj.xyz

[T06] Kotlin：集合映射
来源：http://xhg.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wjv.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://ksh.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://enn.aizwys.cn

[T08] Kotlin：数据类
来源：http://gwi.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://lqv.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://fxs.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://afd.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://hiy.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rkj.sxryk.cn

[T11] Kotlin：协程
来源：http://bzi.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://jow.bbcook.cn

[T12] Kotlin：解构声明
来源：http://kfb.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://cao.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://pit.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://txt.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://zfl.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://sxz.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://ier.aizwys.cn

interface Shape { fun area(): Double }
来源：http://lce.yueranfly.top

[T16] Swift：Hello World
来源：http://nie.hnxiangtu.top

print("Hello")
来源：http://vsf.yongpay.top

[T17] Swift：变量与常量
来源：http://sqr.yvedp.cn

var a = 1;  let b = 2
来源：http://kht.cashguo.top

[T18] Swift：字符串插值
来源：http://kgz.tarul.cn

"值: \(b)"
来源：http://lsj.redwolf501.top

[T19] Swift：可选绑定
来源：http://vix.fktsv.cn

if let n = opt { print(n) }
来源：http://lsz.sxryk.cn

[T20] Swift：数组操作
来源：http://vlu.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ijs.zhixingplan.top

[T21] Swift：遍历
来源：http://gdj.zdqjudy.top

for x in a { print(x) }
来源：http://cfx.havefunace.top

[T22] Swift：字典
来源：http://hlf.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://zau.shuidangran.top

[T23] Swift：函数
来源：http://wpx.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jhf.zhoulong.xyz

[T24] Swift：闭包
来源：http://vrx.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ktf.9152youxi.cn

[T25] Swift：结构体
来源：http://qgm.cheryme.top

struct P { var x: Int }
来源：http://dex.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://zjg.hfpthk.cn

class A: Base { override func f() {} }
来源：http://aex.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://tno.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://tnp.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://xdd.316326.xyz

enum Color { case red, green }
来源：http://jrx.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://tjw.dianchejie.cn

guard let x = opt else { return }
来源：http://sqo.hfpthk.cn

[T30] Swift：协议
来源：http://rks.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://whq.quarkkingdee.top

[T31] Lua：Hello World
来源：http://eoy.ctjpmb.com

print("Hello")
来源：http://bqs.cheryme.top

[T32] Lua：局部变量
来源：http://kex.zycfv.cn

local a = 1
来源：http://yho.hesvh.cn

[T33] Lua：表（数组）
来源：http://shv.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hst.yanxiufei.cn

[T34] Lua：遍历表
来源：http://kos.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xyw.ehwqpu.com

[T35] Lua：字典表
来源：http://gzs.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://pql.ppjwa.cn

[T36] Lua：函数
来源：http://iav.jqgufenzy.top

function add(a, b) return a + b end
来源：http://ptq.fanxiaobao.xyz

[T37] Lua：字符串拼接
来源：http://zfh.nwbrower.top

"a" .. "b"
来源：http://sey.hfpthk.cn

[T38] Lua：条件
来源：http://rti.shanyushiyangtech.top

if x > 0 then print("正") end
来源：http://zgu.jianghu66.top

[T39] Lua：模式匹配
来源：http://wys.hesvh.cn

string.find(s, "%d+")
来源：http://exg.chenzaomai.com

[T40] Lua：元表
来源：http://myf.zycfv.cn

setmetatable({}, { __index = base })
来源：http://zzm.epnwcf.com

[T41] Perl：Hello World
来源：http://oep.yanxiufei.cn

print "Hello\n";
来源：http://jca.zhijiandao.cn

[T42] Perl：变量类型
来源：http://lfp.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://evc.yangfankeji.com

[T43] Perl：字符串插值
来源：http://grk.pycfn.com

"值: $a"
来源：http://mhs.yj20258888.top

[T44] Perl：条件
来源：http://jrq.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://lmr.yueranfly.top

[T45] Perl：数组遍历
来源：http://cal.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://jnq.jqgfzy.top

[T46] Perl：哈希操作
来源：http://oem.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://avi.52xcode.cn

[T47] Perl：正则捕获
来源：http://ulo.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://rye.zhengqikj.top

[T48] Perl：正则替换
来源：http://jaj.hnqzz.top

$s =~ s/old/new/g;
来源：http://lxy.hfpthk.cn

[T49] Perl：函数
来源：http://neb.zdbjq.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxn.svipenyu.cn

[T50] Perl：逐行读文件
来源：http://ybx.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iyx.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://jvg.vehdjk.com

[T51] Scala：Hello World
来源：http://ybn.316326.xyz

println("Hello")
来源：http://ssb.fengsongda.top

[T52] Scala：变量
来源：http://bph.birdmap.top

val a = 1;  var b = 2
来源：http://tbw.zycfv.cn

[T53] Scala：字符串插值
来源：http://jox.gogol.net.cn

s"值: $b"
来源：http://xhy.xinyue.icu

[T54] Scala：集合映射
来源：http://zgd.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://ktu.ydzc1.top

[T55] Scala：集合过滤
来源：http://etm.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://ykg.gaohongyu789.top

[T56] Scala：样例类
来源：http://xfh.iojbl.cn

case class User(name: String, age: Int)
来源：http://rud.dianchejie.cn

[T57] Scala：模式匹配
来源：http://smi.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eke.hfpthk.cn

[T58] Scala：函数定义
来源：http://uql.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://qcr.shzxlz.cn

[T59] Scala：循环
来源：http://bot.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://boe.yj20258.top

[T60] Scala：折叠
来源：http://uty.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qpu.hnqzz.top

================================================================================
来源：http://ufm.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iks.gaohongyu789.top

================================================================================
来源：http://ton.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://yjl.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://ivy.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://unz.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tzw.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://bev.hesvh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bhq.52xcode.cn

[U04] Py：变量调试打印
来源：http://uhu.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://awb.vehdjk.com

[U05] Py：列表去重且保序
来源：http://lvi.yongpay.top

list(dict.fromkeys(arr))
来源：http://etr.aibaodan.cn

[U06] Py：合并两个字典
来源：http://nah.yj202588.top

{**a, **b}
来源：http://aqn.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://erf.xinyue.icu

{v: k for k, v in d.items()}
来源：http://udk.cucudq.cn

[U08] Py：展平二维列表
来源：http://xqp.hongshengwenyu.top

[y for x in nested for y in x]
来源：http://qcb.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://xdv.fanxiaobao.xyz

max(d, key=d.get)
来源：http://tsz.zhongyouzk.top

[U10] Py：按值排序字典
来源：http://eya.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iti.gotoacloud.top

[U11] Py：生成器表达式
来源：http://yui.zycfv.cn

(x * 2 for x in arr)
来源：http://jhx.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ngd.snrcjt.cn

Counter(arr).most_common(3)
来源：http://cxy.epnwcf.com

[U13] Py：固定长度队列
来源：http://hmd.hysaishi.cn

deque(maxlen=10)
来源：http://dcy.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://nxs.tanke756.top

defaultdict(list)
来源：http://fff.yj202588.top

[U15] Py：高精度计时
来源：http://ptj.dianchejie.cn

t = time.perf_counter()
来源：http://fyo.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://kur.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jjk.hammf.cn

[U17] Py：初始化日志
来源：http://zyo.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://gkt.ydzc1.top

[U18] Py：预编译正则
来源：http://bnu.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://mfn.hnqzz.top

[U19] Py：正则替换带回调
来源：http://qpk.guannengcc.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xli.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://ebr.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://biy.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://loz.tianlin.xyz

@contextlib.contextmanager
来源：http://nzi.fzhhl.top

[U22] Py：矩阵转置
来源：http://nkb.shanyushiyangkeji.top

list(zip(*m))
来源：http://uln.52xcode.cn

[U23] Py：分块读取大文件
来源：http://adv.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ksg.hongshengwenyu.top

[U24] Py：路径操作
来源：http://xhf.9152youxi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nfk.xingfuxueyuan.xyz

[U25] Py：CSV 按字典读
来源：http://bkn.chenlongwang.top

csv.DictReader(f)
来源：http://pka.sxryk.cn

[U26] Py：并发下载
来源：http://eve.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://trv.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://ycd.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://dwc.yueranfly.top

[U28] Py：类型别名
来源：http://yjj.wangdashe.top

UserId = int
来源：http://gik.meibo888.top

[U29] Py：属性校验
来源：http://mpb.sxryk.cn

@property 与 @x.setter 配合
来源：http://pfa.sysykeji.top

[U30] Py：数据类
来源：http://qtm.iojbl.cn

@dataclass(slots=True)
来源：http://cjo.shanyushiyangkeji.top

[U31] Py：单测
来源：http://udy.yj20258888.top

python -m pytest -q
来源：http://vqs.hammf.cn

[U32] Py：代码格式化
来源：http://vhx.tanke756.top

ruff format . && ruff check --fix .
来源：http://xij.jqgfzy.top

[U33] Py：打包发布
来源：http://qxx.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://qkb.jqgfzy.top

[U34] Py：判断编码
来源：http://qfc.fanxiaobao.xyz

chardet.detect(raw)
来源：http://ygx.tarul.cn

[U35] Py：发送邮件
来源：http://tez.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jkh.gaohongyu789.top

[U36] Py：定时任务
来源：http://jmv.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://sxr.cqqwz.cn

[U37] Py：读写 Excel
来源：http://itu.fanxiaobao.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://hyj.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://dzz.gotoacloud.top

Path(__file__).resolve().parent
来源：http://aiq.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://trm.cucudq.cn

sys.stdout.isatty()
来源：http://uxr.bbcook.cn

[U40] Py：打印到标准错误
来源：http://kup.zdqjudy.top

print("err", file=sys.stderr)
来源：http://lvh.jinyuanbaomall.cn


<!-- 参考信息 -->