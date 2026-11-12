代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://avt.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nkv.zhoulong.xyz

fclose(f);
来源：http://ago.hcnkem.com

[S12] C：写文件
来源：http://kla.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://quk.sjlbkw.cn

[S13] C：宏定义
来源：http://efe.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zue.cqqwz.cn

[S14] C：枚举
来源：http://lfh.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://gwp.zhijiandao.cn

[S15] C：类型转换
来源：http://dlu.shanyushiyangkeji.top

(double) a / b
来源：http://kdx.redwolf501.top

[S16] C：位操作置位
来源：http://soe.epnwcf.com

x |= (1 << 3);
来源：http://fel.hammf.cn

[S17] C：安全拼接字符串
来源：http://qll.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqq.kuanghao11.cn

[S18] C：命令行参数
来源：http://lyf.snrcjt.cn

int main(int argc, char **argv)
来源：http://qoo.tianlin.xyz

[S19] C：快速排序
来源：http://ykj.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://eud.shangyingyoupin.top

[S20] C：二分查找
来源：http://wzi.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://scj.uphjek.com

[S21] C：字符类别判断
来源：http://ksv.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://crl.xziqi.cn

[S22] C：字符串转数字
来源：http://squ.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://szu.jinqigufen.top

[S23] C：随机数
来源：http://euc.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aqn.nwbrower.top

[S24] C：获取本地时间
来源：http://tzf.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ywk.zdbjq.cn

[S25] C：内存拷贝
来源：http://hdg.fengsongda.top

memcpy(dst, src, n);
来源：http://wpa.jyoumei.cn

[S26] C：内存清零
来源：http://ffm.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://lhg.yongpay.top

[S27] C：定义常量
来源：http://xdj.ivvv.top

const double PI = 3.14159;
来源：http://elo.hywenlv.cn

[S28] C：静态变量
来源：http://rxq.smart0.xyz

static int counter = 0;
来源：http://bqc.yj202588.top

[S29] C：变参函数
来源：http://tcn.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ihw.hcnkem.com

[S30] C：头文件保护
来源：http://zbl.jianghu66.top

#ifndef X_H
来源：http://fwt.aibaodan.cn

#define X_H
来源：http://okp.ehwqpu.com

#endif
来源：http://ucz.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://bgq.zycfv.cn

#include <iostream>
来源：http://jng.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://nep.fengsongda.top

[S32] C++：字符串
来源：http://dux.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://dmu.ehwqpu.com

[S33] C++：vector 增删
来源：http://mox.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rwk.zycfv.cn

[S34] C++：遍历 vector
来源：http://upp.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://fgo.jlsjyb.cn

[S35] C++：map
来源：http://kcc.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yye.ehwqpu.com

[S36] C++：unordered_map
来源：http://vwr.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fpd.zdbjq.cn

[S37] C++：set
来源：http://bxj.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fzr.bbcook.cn

[S38] C++：排序
来源：http://qbt.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://iiq.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://mjn.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://suy.hnqzz.top

[S40] C++：查找元素
来源：http://qok.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tvq.birdmap.top

[S41] C++：类与构造函数
来源：http://adn.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cfq.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://kgn.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://etf.havefunace.top

[S43] C++：智能指针
来源：http://joc.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://dxo.feifeiyinyue.top

[S44] C++：引用传参
来源：http://cnc.daxiang520.top

void inc(int &x) { ++x; }
来源：http://psr.xinyue.icu

[S45] C++：lambda
来源：http://pye.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://wxe.fengsongda.top

[S46] C++：函数模板
来源：http://vov.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tcp.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://rtk.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bki.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://lfa.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tuy.yj20258888.top

while (std::getline(in, line)) { }
来源：http://abl.ehwqpu.com

[S49] C++：写文件
来源：http://tvr.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://joh.zhiwuduotai.top

[S50] C++：格式化数字
来源：http://blu.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://swy.xziqi.cn

[S51] C++：显式类型转换
来源：http://hqo.andypj.xyz

static_cast<double>(a) / b
来源：http://xag.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://zvp.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://sdm.yonumen.top

[S53] C++：移动语义
来源：http://zuh.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://juo.hnqzz.top

[S54] C++：异常处理
来源：http://idr.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jxe.smart0.xyz

[S55] C++：结构化绑定
来源：http://smk.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jok.hnxiangtu.top

[S56] C++：optional
来源：http://lnd.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dqu.ppjwa.cn

[S57] C++：编译期常量
来源：http://vaz.quarkkingdee.top

constexpr int N = 10;
来源：http://myd.zhengqikj.top

[S58] C++：命名空间
来源：http://szz.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://lem.cashguo.top

[S59] C++：静态断言
来源：http://wbp.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uru.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://hab.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nts.hesvh.cn

================================================================================
来源：http://ikt.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpe.aibaodan.cn

================================================================================
来源：http://ryq.yvedp.cn

[T01] Kotlin：Hello World
来源：http://jqg.zhiwuduotai.top

println("Hello")
来源：http://nnf.vehdjk.com

[T02] Kotlin：变量
来源：http://mzs.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hbo.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://hoi.tian-w.cn

"值: $b"
来源：http://msu.vehdjk.com

[T04] Kotlin：空安全
来源：http://pyd.sufxvd.cn

val n: String? = null;  n?.length
来源：http://gws.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://cis.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qyf.wangdashe.top

[T06] Kotlin：集合映射
来源：http://bjk.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://acd.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://xjm.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://del.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://dor.hammf.cn

data class User(val name: String, val age: Int)
来源：http://qnv.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://hjk.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://vkr.cashguo.top

[T10] Kotlin：默认参数
来源：http://ptp.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rwc.yuxming.cn

[T11] Kotlin：协程
来源：http://quu.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sum.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://qbm.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://wvo.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://cbh.nwbrower.top

val m = mapOf("a" to 1)
来源：http://leg.nwbrower.top

[T14] Kotlin：循环
来源：http://xiy.tianlin.xyz

for (i in 1..10) println(i)
来源：http://wfr.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://aqb.bjfxy.top

interface Shape { fun area(): Double }
来源：http://ypu.jqgfzy.top

[T16] Swift：Hello World
来源：http://vkb.hongshengwenyu.top

print("Hello")
来源：http://xcc.hcnkem.com

[T17] Swift：变量与常量
来源：http://avh.jinghuilouyu.cn

var a = 1;  let b = 2
来源：http://dhi.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://stz.zdqjudy.top

"值: \(b)"
来源：http://tze.svipenyu.cn

[T19] Swift：可选绑定
来源：http://pup.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://chu.yuanzhike.top

[T20] Swift：数组操作
来源：http://xtf.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://owl.cheryme.top

[T21] Swift：遍历
来源：http://bwn.yonumen.top

for x in a { print(x) }
来源：http://tse.xuetiantiany.cn

[T22] Swift：字典
来源：http://wkk.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://arb.ybcxt.top

[T23] Swift：函数
来源：http://lxh.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fqs.hesvh.cn

[T24] Swift：闭包
来源：http://vah.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cac.uphjek.com

[T25] Swift：结构体
来源：http://bde.c1oappe.top

struct P { var x: Int }
来源：http://lhc.aizwys.cn

[T26] Swift：类与重写
来源：http://ghh.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://vkf.sysykeji.top

[T27] Swift：错误处理
来源：http://ncz.fehbvm.com

do { try f() } catch { print(error) }
来源：http://nek.xinyue.icu

[T28] Swift：枚举
来源：http://qzo.cheryme.top

enum Color { case red, green }
来源：http://mtn.cashguo.top

[T29] Swift：guard 提前返回
来源：http://psd.chenjidiqi.icu

guard let x = opt else { return }
来源：http://ekb.feifeiyinyue.top

[T30] Swift：协议
来源：http://gsv.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://drh.zhoulong.xyz

[T31] Lua：Hello World
来源：http://cwb.zdqjudy.top

print("Hello")
来源：http://azs.yj202588.top

[T32] Lua：局部变量
来源：http://qdf.cashguo.top

local a = 1
来源：http://gtj.zdbjq.cn

[T33] Lua：表（数组）
来源：http://wvh.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dbo.cheryme.top

[T34] Lua：遍历表
来源：http://uxb.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://znw.yj20258888.top

[T35] Lua：字典表
来源：http://csy.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://ghf.fengsongda.top

[T36] Lua：函数
来源：http://ssi.0kj1m.cn

function add(a, b) return a + b end
来源：http://uvt.zycfv.cn

[T37] Lua：字符串拼接
来源：http://qps.xuanzx.com

"a" .. "b"
来源：http://pzr.fzhhl.top

[T38] Lua：条件
来源：http://cpc.pycfn.com

if x > 0 then print("正") end
来源：http://tla.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://hlv.ydjk.org.cn

string.find(s, "%d+")
来源：http://wpn.svipenyu.cn

[T40] Lua：元表
来源：http://orz.yj20258.top

setmetatable({}, { __index = base })
来源：http://pzt.ehwqpu.com

[T41] Perl：Hello World
来源：http://iwg.jinqigufen.top

print "Hello\n";
来源：http://njd.aibaodan.cn

[T42] Perl：变量类型
来源：http://vtz.nwbrower.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uca.sysykeji.top

[T43] Perl：字符串插值
来源：http://kcl.snrcjt.cn

"值: $a"
来源：http://izx.vehdjk.com

[T44] Perl：条件
来源：http://itz.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://ilj.jqgfzy.top

[T45] Perl：数组遍历
来源：http://ezi.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://hma.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://crc.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kcw.xylfe.cn

[T47] Perl：正则捕获
来源：http://fpt.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qnd.yj202588.top

[T48] Perl：正则替换
来源：http://dcl.yj20258.top

$s =~ s/old/new/g;
来源：http://rfd.daxiang520.top

[T49] Perl：函数
来源：http://ufb.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yko.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://fzt.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ess.kuanghao11.cn

while (my $line = <$fh>) { print $line; }
来源：http://xso.316326.xyz

[T51] Scala：Hello World
来源：http://uhm.ybcxt.top

println("Hello")
来源：http://fnu.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://ltq.nwbrower.top

val a = 1;  var b = 2
来源：http://tiz.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://dxe.9152youxi.cn

s"值: $b"
来源：http://hte.c1oappe.top

[T54] Scala：集合映射
来源：http://thp.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://xjb.iojbl.cn

[T55] Scala：集合过滤
来源：http://jbg.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://smn.jinqigufen.top

[T56] Scala：样例类
来源：http://iuk.fehbvm.com

case class User(name: String, age: Int)
来源：http://oww.uphjek.com

[T57] Scala：模式匹配
来源：http://hke.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://buf.chenlongwang.top

[T58] Scala：函数定义
来源：http://odw.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://luk.pycfn.com

[T59] Scala：循环
来源：http://abb.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://idn.sjlbkw.cn

[T60] Scala：折叠
来源：http://doe.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jbd.fehbvm.com

================================================================================
来源：http://uhi.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gdc.pycfn.com

================================================================================
来源：http://uql.jinqigufen.top

[U01] Py：创建虚拟环境
来源：http://axb.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://cnk.jyoumei.cn

[U02] Py：导出 / 安装依赖
来源：http://bgf.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rdo.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://ubv.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://oik.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://qdm.gaohongyu789.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uwe.yuxming.cn

[U05] Py：列表去重且保序
来源：http://sox.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://jgk.ivvv.top

[U06] Py：合并两个字典
来源：http://xht.fehbvm.com

{**a, **b}
来源：http://yjr.cucudq.cn

[U07] Py：反转字典键值
来源：http://nky.tanke756.top

{v: k for k, v in d.items()}
来源：http://yaa.tianlin.xyz

[U08] Py：展平二维列表
来源：http://odl.ydzc1.top

[y for x in nested for y in x]
来源：http://vbz.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://gpa.yj20258.top

max(d, key=d.get)
来源：http://wog.hywenlv.cn

[U10] Py：按值排序字典
来源：http://dlz.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://agb.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://szi.chenzaomai.com

(x * 2 for x in arr)
来源：http://typ.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tvu.tarul.cn

Counter(arr).most_common(3)
来源：http://ami.chenzaomai.com

[U13] Py：固定长度队列
来源：http://dng.jlsjyb.cn

deque(maxlen=10)
来源：http://kox.jlsjyb.cn

[U14] Py：分组收集到列表
来源：http://hgd.sysykeji.top

defaultdict(list)
来源：http://gbo.pengpengdd.cyou

[U15] Py：高精度计时
来源：http://xkc.meibo888.top

t = time.perf_counter()
来源：http://bum.bbcook.cn

[U16] Py：命令行参数解析
来源：http://zcv.fanxiaobao.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yrn.sufxvd.cn

[U17] Py：初始化日志
来源：http://kvp.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wlh.sufxvd.cn

[U18] Py：预编译正则
来源：http://foj.fengsongda.top

pat = re.compile(r"\d+")
来源：http://vxa.mhx1999.top

[U19] Py：正则替换带回调
来源：http://nzy.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hun.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://gdx.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://xpm.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://gem.vqdsnc.cn

@contextlib.contextmanager
来源：http://czh.zhoulong.xyz

[U22] Py：矩阵转置
来源：http://dih.jinqigufen.top

list(zip(*m))
来源：http://btz.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://jrw.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xzw.gaohongyu789.top

[U24] Py：路径操作
来源：http://sfy.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vhr.pycfn.com

[U25] Py：CSV 按字典读
来源：http://wom.hongshengwenyu.top

csv.DictReader(f)
来源：http://wea.tarul.cn

[U26] Py：并发下载
来源：http://jau.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://crb.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://xrp.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://kmf.zhiwuduotai.top

[U28] Py：类型别名
来源：http://cdi.hfpthk.cn

UserId = int
来源：http://qgt.fehbvm.com

[U29] Py：属性校验
来源：http://erf.nwbrower.top

@property 与 @x.setter 配合
来源：http://xsj.guowangkeji.top

[U30] Py：数据类
来源：http://cct.daria6918.cn

@dataclass(slots=True)
来源：http://vgj.ehwqpu.com

[U31] Py：单测
来源：http://yzd.wangshuangyany.cn

python -m pytest -q
来源：http://xiq.fktsv.cn

[U32] Py：代码格式化
来源：http://met.guannengcc.top

ruff format . && ruff check --fix .
来源：http://isn.quarkkingdee.top

[U33] Py：打包发布
来源：http://mnu.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://cwx.vqdsnc.cn

[U34] Py：判断编码
来源：http://rto.hammf.cn

chardet.detect(raw)
来源：http://egb.hfpthk.cn


<!-- 参考信息 -->