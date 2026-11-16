代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fdb.gogol.net.cn

[S10] C：指针与解引用
来源：http://mak.sweek.top

int *p = &a;  *p = 5;
来源：http://zmp.yangfankeji.com

[S11] C：逐行读文件
来源：http://bjm.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://drk.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://tzu.vehdjk.com

fclose(f);
来源：http://wfl.fzhhl.top

[S12] C：写文件
来源：http://hen.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qrs.wangdashe.top

[S13] C：宏定义
来源：http://ume.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://syl.cheryme.top

[S14] C：枚举
来源：http://ngj.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://swk.cheryme.top

[S15] C：类型转换
来源：http://crs.sweek.top

(double) a / b
来源：http://age.hesvh.cn

[S16] C：位操作置位
来源：http://xfb.yvedp.cn

x |= (1 << 3);
来源：http://zee.meibo888.top

[S17] C：安全拼接字符串
来源：http://yes.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ahf.zhongyouzk.top

[S18] C：命令行参数
来源：http://gdo.aizwys.cn

int main(int argc, char **argv)
来源：http://atr.xziqi.cn

[S19] C：快速排序
来源：http://vcf.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://mxv.shangyingyoupin.top

[S20] C：二分查找
来源：http://jpj.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ytz.ydjk.org.cn

[S21] C：字符类别判断
来源：http://liq.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iet.cucudq.cn

[S22] C：字符串转数字
来源：http://lqp.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://krg.guowangkeji.top

[S23] C：随机数
来源：http://zyd.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cjc.cashguo.top

[S24] C：获取本地时间
来源：http://fkn.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cvw.cucudq.cn

[S25] C：内存拷贝
来源：http://yzq.sxryk.cn

memcpy(dst, src, n);
来源：http://lmv.dashuyun.cn

[S26] C：内存清零
来源：http://wit.xziqi.cn

memset(a, 0, sizeof a);
来源：http://uin.yuxming.cn

[S27] C：定义常量
来源：http://dgu.hywenlv.cn

const double PI = 3.14159;
来源：http://cfd.cqqwz.cn

[S28] C：静态变量
来源：http://afj.fanxiaobao.xyz

static int counter = 0;
来源：http://bhx.hongshengwenyu.top

[S29] C：变参函数
来源：http://svl.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qxe.gogol.net.cn

[S30] C：头文件保护
来源：http://zey.smart0.xyz

#ifndef X_H
来源：http://tnq.epnwcf.com

#define X_H
来源：http://ans.shzxlz.cn

#endif
来源：http://zzb.zhixingplan.top

[S31] C++：Hello World
来源：http://gqv.jinyuanbaomall.cn

#include <iostream>
来源：http://qto.yfazqb.com

int main() { std::cout << "Hello\n"; }
来源：http://mqc.gzhubu.top

[S32] C++：字符串
来源：http://wev.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://unj.jqgufenzy.top

[S33] C++：vector 增删
来源：http://bnk.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iql.sxryk.cn

[S34] C++：遍历 vector
来源：http://qtc.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://dir.ehwqpu.com

[S35] C++：map
来源：http://tdq.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wkt.cdnleiting.top

[S36] C++：unordered_map
来源：http://itx.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yjr.uphjek.com

[S37] C++：set
来源：http://imf.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fun.shangyingyoupin.top

[S38] C++：排序
来源：http://eqc.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://iru.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://ckg.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zvr.yangfankeji.com

[S40] C++：查找元素
来源：http://dub.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://huc.hammf.cn

[S41] C++：类与构造函数
来源：http://tcd.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qlp.bjfxy.top

[S42] C++：继承与虚函数
来源：http://kci.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://lnn.vehdjk.com

[S43] C++：智能指针
来源：http://odv.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://syt.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://tjp.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://mbe.ydjk.org.cn

[S45] C++：lambda
来源：http://kcl.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xad.52xcode.cn

[S46] C++：函数模板
来源：http://aij.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://avm.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://fap.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fgn.haohaochexian.top

[S48] C++：逐行读文件
来源：http://pvg.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://oig.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://wug.pengpengdd.cyou

[S49] C++：写文件
来源：http://cll.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://btg.xuanzx.com

[S50] C++：格式化数字
来源：http://lmc.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nws.hcnkem.com

[S51] C++：显式类型转换
来源：http://usx.cdnleiting.top

static_cast<double>(a) / b
来源：http://sym.pycfn.com

[S52] C++：const 与 noexcept
来源：http://wvn.cashguo.top

int size() const noexcept { return n_; }
来源：http://eeg.yangfankeji.com

[S53] C++：移动语义
来源：http://wtx.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://big.jlsjyb.cn

[S54] C++：异常处理
来源：http://zvj.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ncy.jiagoushi.top

[S55] C++：结构化绑定
来源：http://anf.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xmf.tianlin.xyz

[S56] C++：optional
来源：http://djn.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dtz.vehdjk.com

[S57] C++：编译期常量
来源：http://qcb.xziqi.cn

constexpr int N = 10;
来源：http://jbw.andypj.xyz

[S58] C++：命名空间
来源：http://btd.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://iew.yj20258.top

[S59] C++：静态断言
来源：http://rpd.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uff.yongpay.top

[S60] C++：遍历并删除元素
来源：http://vox.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kqb.chenzaomai.com

================================================================================
来源：http://fcx.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sae.sxryk.cn

================================================================================
来源：http://amy.iojbl.cn

[T01] Kotlin：Hello World
来源：http://qrt.zhiwuduotai.top

println("Hello")
来源：http://oix.316326.xyz

[T02] Kotlin：变量
来源：http://gjm.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oou.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://eho.wangshuangyany.cn

"值: $b"
来源：http://zeb.zhengqikj.top

[T04] Kotlin：空安全
来源：http://oxf.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://acv.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://kfq.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://krj.andypj.xyz

[T06] Kotlin：集合映射
来源：http://vpm.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tsn.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://mvq.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufz.guowangkeji.top

[T08] Kotlin：数据类
来源：http://njl.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://kss.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://qnm.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://jfj.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://vub.52xcode.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jxe.vehdjk.com

[T11] Kotlin：协程
来源：http://qof.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://qdo.fengsongda.top

[T12] Kotlin：解构声明
来源：http://qww.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://drg.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://eiy.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://gud.yanxiufei.cn

[T14] Kotlin：循环
来源：http://uyt.yj202588.top

for (i in 1..10) println(i)
来源：http://ynf.pycfn.com

[T15] Kotlin：接口
来源：http://ywx.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://cjp.jqgufenzy.top

[T16] Swift：Hello World
来源：http://adx.shzxlz.cn

print("Hello")
来源：http://qts.chenlongwang.top

[T17] Swift：变量与常量
来源：http://ydr.zdbjq.cn

var a = 1;  let b = 2
来源：http://xrr.cucudq.cn

[T18] Swift：字符串插值
来源：http://fqf.svipenyu.cn

"值: \(b)"
来源：http://ipx.xinyue.icu

[T19] Swift：可选绑定
来源：http://zwo.hywenlv.cn

if let n = opt { print(n) }
来源：http://ova.zhengqikj.top

[T20] Swift：数组操作
来源：http://quq.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://few.aizwys.cn

[T21] Swift：遍历
来源：http://hnr.yueranfly.top

for x in a { print(x) }
来源：http://ljb.mhx1999.top

[T22] Swift：字典
来源：http://faz.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://deu.redwolf501.top

[T23] Swift：函数
来源：http://fmz.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bme.jinqigfzy.top

[T24] Swift：闭包
来源：http://ixc.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://seb.andypj.xyz

[T25] Swift：结构体
来源：http://one.yj202588.top

struct P { var x: Int }
来源：http://iww.nanxinkj.top

[T26] Swift：类与重写
来源：http://khm.yonumen.top

class A: Base { override func f() {} }
来源：http://qmr.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://dmh.bjfxy.top

do { try f() } catch { print(error) }
来源：http://hqu.pycfn.com

[T28] Swift：枚举
来源：http://uvz.sjlbkw.cn

enum Color { case red, green }
来源：http://qka.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://qhm.ehwqpu.com

guard let x = opt else { return }
来源：http://amr.jqgfzy.top

[T30] Swift：协议
来源：http://xzj.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://vqs.yuanzhike.top

[T31] Lua：Hello World
来源：http://ykm.yj20258888.top

print("Hello")
来源：http://tvt.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://ewh.nanxinkj.top

local a = 1
来源：http://awl.fehbvm.com

[T33] Lua：表（数组）
来源：http://suw.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://muk.shuidangran.top

[T34] Lua：遍历表
来源：http://qpz.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sey.xylfe.cn

[T35] Lua：字典表
来源：http://hpk.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://uqp.gotoacloud.top

[T36] Lua：函数
来源：http://elh.daxiang520.top

function add(a, b) return a + b end
来源：http://skm.c1oappe.top

[T37] Lua：字符串拼接
来源：http://nzj.guannengcc.top

"a" .. "b"
来源：http://akp.zhiwuduotai.top

[T38] Lua：条件
来源：http://tkn.uphjek.com

if x > 0 then print("正") end
来源：http://nqj.iojbl.cn

[T39] Lua：模式匹配
来源：http://mwh.yueranfly.top

string.find(s, "%d+")
来源：http://zwf.yangfankeji.com

[T40] Lua：元表
来源：http://wda.fengsongda.top

setmetatable({}, { __index = base })
来源：http://juy.hnxiangtu.top

[T41] Perl：Hello World
来源：http://crr.ywan-chungtsiang.top

print "Hello\n";
来源：http://jaa.zycfv.cn

[T42] Perl：变量类型
来源：http://bos.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tol.yvedp.cn

[T43] Perl：字符串插值
来源：http://puc.chenlongwang.top

"值: $a"
来源：http://wty.jlsjyb.cn

[T44] Perl：条件
来源：http://fue.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://btx.hysaishi.cn

[T45] Perl：数组遍历
来源：http://iax.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://slc.chenzaomai.com

[T46] Perl：哈希操作
来源：http://ger.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hvo.yj20258888.top

[T47] Perl：正则捕获
来源：http://agi.sufxvd.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://euw.uphjek.com

[T48] Perl：正则替换
来源：http://lby.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://jfl.zdbjq.cn

[T49] Perl：函数
来源：http://joc.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dif.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://wel.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://msq.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://zon.chenlongwang.top

[T51] Scala：Hello World
来源：http://oir.aibaodan.cn

println("Hello")
来源：http://bgp.jinqigfzy.top

[T52] Scala：变量
来源：http://pct.zhixingplan.top

val a = 1;  var b = 2
来源：http://dci.0kj1m.cn

[T53] Scala：字符串插值
来源：http://iik.52xcode.cn

s"值: $b"
来源：http://kme.zdbjq.cn

[T54] Scala：集合映射
来源：http://noc.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://hqd.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://jfj.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://isd.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://una.jinqigufen.top

case class User(name: String, age: Int)
来源：http://mgb.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://fzf.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bvs.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://ifl.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://vbq.zycfv.cn

[T59] Scala：循环
来源：http://fnu.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://wdd.dianchejie.cn

[T60] Scala：折叠
来源：http://zvz.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oaq.yj20258.top

================================================================================
来源：http://fpv.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tcc.xuetiantiany.cn

================================================================================
来源：http://tnz.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://mvf.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://ezt.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://xvn.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jfz.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://yts.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://gmx.hammf.cn

[U04] Py：变量调试打印
来源：http://stv.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uqc.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://uae.sufxvd.cn

list(dict.fromkeys(arr))
来源：http://shb.jqgufenzy.top

[U06] Py：合并两个字典
来源：http://oen.sxryk.cn

{**a, **b}
来源：http://kup.chenzaomai.com

[U07] Py：反转字典键值
来源：http://efn.tian-w.cn

{v: k for k, v in d.items()}
来源：http://vsu.ivvv.top

[U08] Py：展平二维列表
来源：http://ncu.fengsongda.top

[y for x in nested for y in x]
来源：http://qpy.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://guj.wangshuangyany.cn

max(d, key=d.get)
来源：http://hkz.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://lux.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bce.birdmap.top

[U11] Py：生成器表达式
来源：http://avh.9152youxi.cn

(x * 2 for x in arr)
来源：http://ref.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://oxs.nanxinkj.top

Counter(arr).most_common(3)
来源：http://lbs.hywenlv.cn

[U13] Py：固定长度队列
来源：http://dra.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://qqf.guannengcc.top

[U14] Py：分组收集到列表
来源：http://htq.chenjidiqi.icu

defaultdict(list)
来源：http://jml.yj20258888.top

[U15] Py：高精度计时
来源：http://iwb.andypj.xyz

t = time.perf_counter()
来源：http://lax.ybcxt.top

[U16] Py：命令行参数解析
来源：http://dbe.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xfd.cucudq.cn

[U17] Py：初始化日志
来源：http://gso.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://qtp.tian-w.cn

[U18] Py：预编译正则
来源：http://yqd.daxiang520.top

pat = re.compile(r"\d+")
来源：http://ifr.andypj.xyz

[U19] Py：正则替换带回调
来源：http://saq.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qqo.shuidangran.top

[U20] Py：缓存函数结果
来源：http://dul.xylfe.cn

@functools.lru_cache(maxsize=None)
来源：http://wtb.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://sns.cucudq.cn

@contextlib.contextmanager
来源：http://xmc.smart0.xyz

[U22] Py：矩阵转置
来源：http://ouv.shzxlz.cn

list(zip(*m))
来源：http://fzw.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://nst.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jjd.52xcode.cn

[U24] Py：路径操作
来源：http://uya.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mqs.sufxvd.cn

[U25] Py：CSV 按字典读
来源：http://qwn.hammf.cn

csv.DictReader(f)
来源：http://gyh.sufxvd.cn

[U26] Py：并发下载
来源：http://pul.zdbjq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oub.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://pqd.yueranfly.top

aiohttp.ClientSession() 配合 async with
来源：http://sog.wangshuangyany.cn

[U28] Py：类型别名
来源：http://grl.fzhhl.top

UserId = int
来源：http://tpl.feifeiyinyue.top

[U29] Py：属性校验
来源：http://qzn.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://nbc.cqqwz.cn

[U30] Py：数据类
来源：http://ale.yuanzhike.top

@dataclass(slots=True)
来源：http://kcb.aibaodan.cn

[U31] Py：单测
来源：http://lqp.tarul.cn

python -m pytest -q
来源：http://gtw.jianghu66.top

[U32] Py：代码格式化
来源：http://icc.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://cyr.xuetiantiany.cn


<!-- 参考信息 -->