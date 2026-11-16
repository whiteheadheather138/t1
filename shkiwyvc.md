代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nvf.gogol.net.cn

[S13] C：宏定义
来源：http://dos.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mlo.yfazqb.com

[S14] C：枚举
来源：http://rgj.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://kep.shuidangran.top

[S15] C：类型转换
来源：http://kkn.yanxiufei.cn

(double) a / b
来源：http://qkl.sysykeji.top

[S16] C：位操作置位
来源：http://wux.ydzc1.top

x |= (1 << 3);
来源：http://qof.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://ghc.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jlj.gzhubu.top

[S18] C：命令行参数
来源：http://xlg.zhengqikj.top

int main(int argc, char **argv)
来源：http://cae.cheryme.top

[S19] C：快速排序
来源：http://kqt.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://soe.cqqwz.cn

[S20] C：二分查找
来源：http://jic.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ysg.yongpay.top

[S21] C：字符类别判断
来源：http://pcj.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://msh.hesvh.cn

[S22] C：字符串转数字
来源：http://hak.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://bnx.shzxlz.cn

[S23] C：随机数
来源：http://amx.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ffu.zhixingplan.top

[S24] C：获取本地时间
来源：http://tfx.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mui.daxiang520.top

[S25] C：内存拷贝
来源：http://xvk.sweek.top

memcpy(dst, src, n);
来源：http://ocz.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://tjx.gzhubu.top

memset(a, 0, sizeof a);
来源：http://kzw.wangdashe.top

[S27] C：定义常量
来源：http://nlh.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://sba.bjfxy.top

[S28] C：静态变量
来源：http://jbc.cucudq.cn

static int counter = 0;
来源：http://grw.fanxiaobao.xyz

[S29] C：变参函数
来源：http://xdq.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eyh.guowangkeji.top

[S30] C：头文件保护
来源：http://njj.yj20258.top

#ifndef X_H
来源：http://qdk.yangfankeji.com

#define X_H
来源：http://bhe.fehbvm.com

#endif
来源：http://tpw.9152youxi.cn

[S31] C++：Hello World
来源：http://ddv.sweek.top

#include <iostream>
来源：http://ije.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://lat.ctjpmb.com

[S32] C++：字符串
来源：http://lir.meibo888.top

std::string s = "hi";  s += "!";
来源：http://pda.epnwcf.com

[S33] C++：vector 增删
来源：http://fei.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nvm.cqqwz.cn

[S34] C++：遍历 vector
来源：http://xba.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://uhb.zhixingplan.top

[S35] C++：map
来源：http://hzx.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bil.zhixingplan.top

[S36] C++：unordered_map
来源：http://qpo.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyx.chenjidiqi.icu

[S37] C++：set
来源：http://wis.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dqc.yonumen.top

[S38] C++：排序
来源：http://lcm.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://gfv.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://gcg.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hsf.ydzc1.top

[S40] C++：查找元素
来源：http://nzd.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lve.gotoacloud.top

[S41] C++：类与构造函数
来源：http://zgk.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bev.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://tdf.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://hxz.jqgufenzy.top

[S43] C++：智能指针
来源：http://rzn.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://hwb.uphjek.com

[S44] C++：引用传参
来源：http://rlo.uphjek.com

void inc(int &x) { ++x; }
来源：http://uqy.cdnleiting.top

[S45] C++：lambda
来源：http://qxa.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ltg.mhx1999.top

[S46] C++：函数模板
来源：http://qyp.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://khr.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://unh.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdm.yfazqb.com

[S48] C++：逐行读文件
来源：http://djp.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mts.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://ier.quarkkingdee.top

[S49] C++：写文件
来源：http://zhn.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://izx.yongpay.top

[S50] C++：格式化数字
来源：http://ieg.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vnb.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://hoi.ctjpmb.com

static_cast<double>(a) / b
来源：http://fpn.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://wrl.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://yfk.sweek.top

[S53] C++：移动语义
来源：http://nkz.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://vyq.gotoacloud.top

[S54] C++：异常处理
来源：http://pkw.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdo.gzhubu.top

[S55] C++：结构化绑定
来源：http://yfj.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aat.zhixingplan.top

[S56] C++：optional
来源：http://ldf.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vqp.jinqigufen.top

[S57] C++：编译期常量
来源：http://mas.nwbrower.top

constexpr int N = 10;
来源：http://pib.hcnkem.com

[S58] C++：命名空间
来源：http://hxy.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://wnc.shzxlz.cn

[S59] C++：静态断言
来源：http://mia.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://svv.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://ihn.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ken.jiagoushi.top

================================================================================
来源：http://jmd.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pvr.52xcode.cn

================================================================================
来源：http://wij.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://vbb.svipenyu.cn

println("Hello")
来源：http://ids.fengsongda.top

[T02] Kotlin：变量
来源：http://vwh.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vss.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://wuv.uphjek.com

"值: $b"
来源：http://brm.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://ktz.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://ttc.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://fmp.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hif.wangdashe.top

[T06] Kotlin：集合映射
来源：http://fis.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://uvp.yonumen.top

[T07] Kotlin：集合过滤
来源：http://xza.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qsh.redwolf501.top

[T08] Kotlin：数据类
来源：http://dih.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://vyz.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://rmb.316326.xyz

fun String.exclaim() = this + "!"
来源：http://tbr.yonumen.top

[T10] Kotlin：默认参数
来源：http://dmt.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wdd.ybcxt.top

[T11] Kotlin：协程
来源：http://cvq.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vxi.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://ctg.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://nkv.cheryme.top

[T13] Kotlin：只读 Map
来源：http://zti.xziqi.cn

val m = mapOf("a" to 1)
来源：http://qqg.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://qro.tarul.cn

for (i in 1..10) println(i)
来源：http://tqd.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://jjt.yongpay.top

interface Shape { fun area(): Double }
来源：http://trh.jinqigfzy.top

[T16] Swift：Hello World
来源：http://qkg.tian-w.cn

print("Hello")
来源：http://mpa.0kj1m.cn

[T17] Swift：变量与常量
来源：http://eqp.hfpthk.cn

var a = 1;  let b = 2
来源：http://cba.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://odz.aizwys.cn

"值: \(b)"
来源：http://oaa.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://wxd.vehdjk.com

if let n = opt { print(n) }
来源：http://fir.zhongyouzk.top

[T20] Swift：数组操作
来源：http://njc.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://tzs.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://ytq.yfazqb.com

for x in a { print(x) }
来源：http://kde.yvedp.cn

[T22] Swift：字典
来源：http://qtm.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://maa.gaohongyu789.top

[T23] Swift：函数
来源：http://qtz.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://grl.yvedp.cn

[T24] Swift：闭包
来源：http://wte.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rep.zhoulong.xyz

[T25] Swift：结构体
来源：http://hxz.shangyingyoupin.top

struct P { var x: Int }
来源：http://tbo.jiagoushi.top

[T26] Swift：类与重写
来源：http://vri.fzhhl.top

class A: Base { override func f() {} }
来源：http://ode.xylfe.cn

[T27] Swift：错误处理
来源：http://yuf.316326.xyz

do { try f() } catch { print(error) }
来源：http://gme.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://xsq.hywenlv.cn

enum Color { case red, green }
来源：http://ytp.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://rdq.zhijiandao.cn

guard let x = opt else { return }
来源：http://ipl.daxiang520.top

[T30] Swift：协议
来源：http://npy.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://roy.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://jkb.zhaomingkeji.xyz

print("Hello")
来源：http://ofl.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://kwr.xuetiantiany.cn

local a = 1
来源：http://qch.daxiang520.top

[T33] Lua：表（数组）
来源：http://xly.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ddl.sysykeji.top

[T34] Lua：遍历表
来源：http://aqa.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ydl.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://mrw.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://dwl.sufxvd.cn

[T36] Lua：函数
来源：http://fmj.ivvv.top

function add(a, b) return a + b end
来源：http://gix.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://erl.jyoumei.cn

"a" .. "b"
来源：http://cbo.sxryk.cn

[T38] Lua：条件
来源：http://ohk.yueranfly.top

if x > 0 then print("正") end
来源：http://ved.guannengcc.top

[T39] Lua：模式匹配
来源：http://lzo.xziqi.cn

string.find(s, "%d+")
来源：http://gtx.chenzaomai.com

[T40] Lua：元表
来源：http://snh.birdmap.top

setmetatable({}, { __index = base })
来源：http://gem.jqgfzy.top

[T41] Perl：Hello World
来源：http://hng.birdmap.top

print "Hello\n";
来源：http://ddd.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://xjb.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ydu.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://ecj.jqgfzy.top

"值: $a"
来源：http://wmv.svipenyu.cn

[T44] Perl：条件
来源：http://otd.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://gkp.zhengqikj.top

[T45] Perl：数组遍历
来源：http://hkg.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://mik.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://vix.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jvg.nanxinkj.top

[T47] Perl：正则捕获
来源：http://gsf.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://igh.zdbjq.cn

[T48] Perl：正则替换
来源：http://uvs.hywenlv.cn

$s =~ s/old/new/g;
来源：http://kdr.sxryk.cn

[T49] Perl：函数
来源：http://rob.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gpy.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://xto.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://woi.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://lhd.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://edn.feifeiyinyue.top

println("Hello")
来源：http://lfc.sufxvd.cn

[T52] Scala：变量
来源：http://axi.yj20258.top

val a = 1;  var b = 2
来源：http://mcp.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://vux.yj20258888.top

s"值: $b"
来源：http://dbq.0kj1m.cn

[T54] Scala：集合映射
来源：http://dtf.jyoumei.cn

List(1, 2, 3).map(_ * 2)
来源：http://sbj.fengsongda.top

[T55] Scala：集合过滤
来源：http://uuy.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://far.shzxlz.cn

[T56] Scala：样例类
来源：http://eez.sweek.top

case class User(name: String, age: Int)
来源：http://rhe.aizwys.cn

[T57] Scala：模式匹配
来源：http://oek.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mni.cashguo.top

[T58] Scala：函数定义
来源：http://hka.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://zds.haohaochexian.top

[T59] Scala：循环
来源：http://bzw.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://jmd.zhoulong.xyz

[T60] Scala：折叠
来源：http://ozh.zhijiandao.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cac.bbcook.cn

================================================================================
来源：http://arg.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iqz.jqgfzy.top

================================================================================
来源：http://jkx.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://aqm.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kgk.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://gdu.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zxs.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://kdt.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kuy.uphjek.com

[U04] Py：变量调试打印
来源：http://txy.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fkg.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://jug.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://ftt.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://umz.ivvv.top

{**a, **b}
来源：http://yvf.fehbvm.com

[U07] Py：反转字典键值
来源：http://fpy.ydzc1.top

{v: k for k, v in d.items()}
来源：http://xrr.xinyue.icu

[U08] Py：展平二维列表
来源：http://lsl.chenzaomai.com

[y for x in nested for y in x]
来源：http://uai.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://bza.xylfe.cn

max(d, key=d.get)
来源：http://aby.gzhubu.top

[U10] Py：按值排序字典
来源：http://ahn.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yug.aibaodan.cn

[U11] Py：生成器表达式
来源：http://fxf.gogol.net.cn

(x * 2 for x in arr)
来源：http://xfc.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://pvu.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://gws.wangshuangyany.cn

[U13] Py：固定长度队列
来源：http://ctj.guowangkeji.top

deque(maxlen=10)
来源：http://mve.hnqzz.top

[U14] Py：分组收集到列表
来源：http://ehd.jqgfzy.top

defaultdict(list)
来源：http://vcm.aibaodan.cn

[U15] Py：高精度计时
来源：http://qoi.9152youxi.cn

t = time.perf_counter()
来源：http://tas.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://bss.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mut.ppjwa.cn

[U17] Py：初始化日志
来源：http://hfa.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://zwk.sxryk.cn

[U18] Py：预编译正则
来源：http://tch.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://agb.shuidangran.top

[U19] Py：正则替换带回调
来源：http://rba.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gga.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://edi.xziqi.cn

@functools.lru_cache(maxsize=None)
来源：http://pgu.hnxiangtu.top

[U21] Py：自定义上下文管理器
来源：http://gth.sxryk.cn

@contextlib.contextmanager
来源：http://jdh.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://fsc.jyoumei.cn

list(zip(*m))
来源：http://bqz.hammf.cn

[U23] Py：分块读取大文件
来源：http://ypg.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wme.yueranfly.top

[U24] Py：路径操作
来源：http://xuh.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gnp.cucudq.cn

[U25] Py：CSV 按字典读
来源：http://kkh.vehdjk.com

csv.DictReader(f)
来源：http://upq.316326.xyz

[U26] Py：并发下载
来源：http://dtg.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nzg.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://mgx.cheryme.top

aiohttp.ClientSession() 配合 async with
来源：http://bmf.ctjpmb.com

[U28] Py：类型别名
来源：http://fnz.vehdjk.com

UserId = int
来源：http://atc.zhixingplan.top

[U29] Py：属性校验
来源：http://pne.yonumen.top

@property 与 @x.setter 配合
来源：http://mhg.uphjek.com

[U30] Py：数据类
来源：http://kzm.jlsjyb.cn

@dataclass(slots=True)
来源：http://frn.gaohongyu789.top

[U31] Py：单测
来源：http://sjr.jinqigfzy.top

python -m pytest -q
来源：http://yjr.shzxlz.cn

[U32] Py：代码格式化
来源：http://xzr.yongpay.top

ruff format . && ruff check --fix .
来源：http://zbe.hammf.cn

[U33] Py：打包发布
来源：http://reg.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://nvs.xziqi.cn

[U34] Py：判断编码
来源：http://fwl.jinqigufen.top

chardet.detect(raw)
来源：http://pve.jianghu66.top

[U35] Py：发送邮件
来源：http://dox.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://djd.zhiwuduotai.top

[U36] Py：定时任务
来源：http://lok.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://kgi.jiagoushi.top


<!-- 参考信息 -->