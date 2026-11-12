代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vxq.hongshengwenyu.top

[S13] C：宏定义
来源：http://yyk.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pal.c1oappe.top

[S14] C：枚举
来源：http://juh.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://iqr.xuanzx.com

[S15] C：类型转换
来源：http://qyf.pengpengdd.cyou

(double) a / b
来源：http://fcb.yonumen.top

[S16] C：位操作置位
来源：http://nzk.hysaishi.cn

x |= (1 << 3);
来源：http://pwa.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://bkn.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://brl.ppjwa.cn

[S18] C：命令行参数
来源：http://sxv.jqgfzy.top

int main(int argc, char **argv)
来源：http://rkd.bbcook.cn

[S19] C：快速排序
来源：http://kyf.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eus.aizwys.cn

[S20] C：二分查找
来源：http://ezo.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ndq.cdnleiting.top

[S21] C：字符类别判断
来源：http://kle.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxq.bjfxy.top

[S22] C：字符串转数字
来源：http://cwg.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rvy.havefunace.top

[S23] C：随机数
来源：http://psf.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aud.nwbrower.top

[S24] C：获取本地时间
来源：http://zmg.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cor.gotoacloud.top

[S25] C：内存拷贝
来源：http://pgh.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://vrr.chenzaomai.com

[S26] C：内存清零
来源：http://ofy.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://tyn.feifeiyinyue.top

[S27] C：定义常量
来源：http://imm.gaohongyu789.top

const double PI = 3.14159;
来源：http://rnl.ybcxt.top

[S28] C：静态变量
来源：http://tbm.guowangkeji.top

static int counter = 0;
来源：http://qxj.hywenlv.cn

[S29] C：变参函数
来源：http://xkk.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jwa.sxryk.cn

[S30] C：头文件保护
来源：http://twb.hcnkem.com

#ifndef X_H
来源：http://wdj.bjfxy.top

#define X_H
来源：http://vgj.yvedp.cn

#endif
来源：http://yob.jinqigfzy.top

[S31] C++：Hello World
来源：http://cgt.nanxuanxn.top

#include <iostream>
来源：http://vpk.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://gwe.quarkkingdee.top

[S32] C++：字符串
来源：http://chv.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://xej.tianlin.xyz

[S33] C++：vector 增删
来源：http://deu.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qvt.hywenlv.cn

[S34] C++：遍历 vector
来源：http://jse.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://tao.xuanzx.com

[S35] C++：map
来源：http://khl.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sja.aibaodan.cn

[S36] C++：unordered_map
来源：http://wzf.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bli.wangshuangyany.cn

[S37] C++：set
来源：http://yjt.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohh.vqdsnc.cn

[S38] C++：排序
来源：http://ykr.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://elw.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://nzk.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qju.chenjidiqi.icu

[S40] C++：查找元素
来源：http://lri.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yji.52xcode.cn

[S41] C++：类与构造函数
来源：http://nzl.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jng.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://tyc.yanxiufei.cn

class B : public Base { public: void f() override {} };
来源：http://czc.yonumen.top

[S43] C++：智能指针
来源：http://cbl.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://mbg.zdqjudy.top

[S44] C++：引用传参
来源：http://fyp.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://jcp.redwolf501.top

[S45] C++：lambda
来源：http://wcj.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://wfe.feifeiyinyue.top

[S46] C++：函数模板
来源：http://pzj.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kxk.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://xak.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mxd.mhx1999.top

[S48] C++：逐行读文件
来源：http://mpc.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://mxp.fzhhl.top

while (std::getline(in, line)) { }
来源：http://lqj.hcnkem.com

[S49] C++：写文件
来源：http://qud.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lov.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://ait.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yne.sysykeji.top

[S51] C++：显式类型转换
来源：http://ynl.smart0.xyz

static_cast<double>(a) / b
来源：http://rep.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://mnp.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://cbj.ybcxt.top

[S53] C++：移动语义
来源：http://zgd.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://mrr.vqdsnc.cn

[S54] C++：异常处理
来源：http://gnv.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jui.pycfn.com

[S55] C++：结构化绑定
来源：http://pki.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vgq.kuanghao11.cn

[S56] C++：optional
来源：http://pfr.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bcg.quarkkingdee.top

[S57] C++：编译期常量
来源：http://xtw.jqgufenzy.top

constexpr int N = 10;
来源：http://hes.xylfe.cn

[S58] C++：命名空间
来源：http://dts.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://rds.jqgufenzy.top

[S59] C++：静态断言
来源：http://ams.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lkt.birdmap.top

[S60] C++：遍历并删除元素
来源：http://kuc.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gph.fengsongda.top

================================================================================
来源：http://wvy.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymm.hongshengwenyu.top

================================================================================
来源：http://nzk.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://iyn.tarul.cn

println("Hello")
来源：http://fvd.nwbrower.top

[T02] Kotlin：变量
来源：http://yvn.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ujy.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://yoy.chenjidiqi.icu

"值: $b"
来源：http://dju.sufxvd.cn

[T04] Kotlin：空安全
来源：http://dal.svipenyu.cn

val n: String? = null;  n?.length
来源：http://aqp.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://jtx.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dtp.ydzc1.top

[T06] Kotlin：集合映射
来源：http://mka.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eku.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://qaj.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xrv.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://xmp.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://lrt.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://rzb.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://fex.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://scw.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wxs.cheryme.top

[T11] Kotlin：协程
来源：http://fpr.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://sfk.smart0.xyz

[T12] Kotlin：解构声明
来源：http://bzq.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://hxe.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://elh.hnqzz.top

val m = mapOf("a" to 1)
来源：http://gzp.gzhubu.top

[T14] Kotlin：循环
来源：http://jru.smart0.xyz

for (i in 1..10) println(i)
来源：http://mes.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://qwn.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://jop.yangfankeji.com

[T16] Swift：Hello World
来源：http://rdt.tian-w.cn

print("Hello")
来源：http://cdg.cheryme.top

[T17] Swift：变量与常量
来源：http://vun.cashguo.top

var a = 1;  let b = 2
来源：http://cwp.gzhubu.top

[T18] Swift：字符串插值
来源：http://vgz.tarul.cn

"值: \(b)"
来源：http://mfd.andypj.xyz

[T19] Swift：可选绑定
来源：http://bns.dashuyun.cn

if let n = opt { print(n) }
来源：http://jlh.sweek.top

[T20] Swift：数组操作
来源：http://keh.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://qot.fengsongda.top

[T21] Swift：遍历
来源：http://isl.nanxuanxn.top

for x in a { print(x) }
来源：http://tqi.cucudq.cn

[T22] Swift：字典
来源：http://jtj.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://qtr.smart0.xyz

[T23] Swift：函数
来源：http://wct.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bqb.gzhubu.top

[T24] Swift：闭包
来源：http://lov.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://muw.fengsongda.top

[T25] Swift：结构体
来源：http://kfp.xuanzx.com

struct P { var x: Int }
来源：http://qlb.jiagoushi.top

[T26] Swift：类与重写
来源：http://wsc.yvedp.cn

class A: Base { override func f() {} }
来源：http://upa.gaohongyu789.top

[T27] Swift：错误处理
来源：http://lud.wangdashe.top

do { try f() } catch { print(error) }
来源：http://jsl.yvedp.cn

[T28] Swift：枚举
来源：http://pcr.9152youxi.cn

enum Color { case red, green }
来源：http://inw.tarul.cn

[T29] Swift：guard 提前返回
来源：http://pgu.gzhubu.top

guard let x = opt else { return }
来源：http://fpc.tianlin.xyz

[T30] Swift：协议
来源：http://ass.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://opq.ivvv.top

[T31] Lua：Hello World
来源：http://zan.birdmap.top

print("Hello")
来源：http://adc.ctjpmb.com

[T32] Lua：局部变量
来源：http://hwt.shangyingyoupin.top

local a = 1
来源：http://cue.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://kvs.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://muq.bbcook.cn

[T34] Lua：遍历表
来源：http://otc.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xkc.yj202588.top

[T35] Lua：字典表
来源：http://kwg.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://dya.chenjidiqi.icu

[T36] Lua：函数
来源：http://trr.hnqzz.top

function add(a, b) return a + b end
来源：http://inj.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://dff.yfazqb.com

"a" .. "b"
来源：http://yif.havefunace.top

[T38] Lua：条件
来源：http://gjh.redwolf501.top

if x > 0 then print("正") end
来源：http://abn.uphjek.com

[T39] Lua：模式匹配
来源：http://csw.zycfv.cn

string.find(s, "%d+")
来源：http://nrd.sufxvd.cn

[T40] Lua：元表
来源：http://hmi.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://kpu.jianghu66.top

[T41] Perl：Hello World
来源：http://wgh.zhiwuduotai.top

print "Hello\n";
来源：http://amp.yongpay.top

[T42] Perl：变量类型
来源：http://bsy.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eoj.yj202588.top

[T43] Perl：字符串插值
来源：http://qyl.hcnkem.com

"值: $a"
来源：http://idt.sufxvd.cn

[T44] Perl：条件
来源：http://ohr.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://mms.gogol.net.cn

[T45] Perl：数组遍历
来源：http://cwd.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://lxa.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://iby.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dfo.hnqzz.top

[T47] Perl：正则捕获
来源：http://ahs.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://yun.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://tkp.jyoumei.cn

$s =~ s/old/new/g;
来源：http://tdl.birdmap.top

[T49] Perl：函数
来源：http://iby.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rye.yueranfly.top

[T50] Perl：逐行读文件
来源：http://icy.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zni.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://bwz.9152youxi.cn

[T51] Scala：Hello World
来源：http://zya.yvedp.cn

println("Hello")
来源：http://eoq.yj20258888.top

[T52] Scala：变量
来源：http://gzh.mhx1999.top

val a = 1;  var b = 2
来源：http://kuz.bjfxy.top

[T53] Scala：字符串插值
来源：http://flr.jqgfzy.top

s"值: $b"
来源：http://ius.cheryme.top

[T54] Scala：集合映射
来源：http://xdx.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://aql.pycfn.com

[T55] Scala：集合过滤
来源：http://pzc.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://bqn.hfpthk.cn

[T56] Scala：样例类
来源：http://rxg.nanxinkj.top

case class User(name: String, age: Int)
来源：http://naf.zhengqikj.top

[T57] Scala：模式匹配
来源：http://lzr.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://lzm.smart0.xyz

[T58] Scala：函数定义
来源：http://nuu.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vov.xuetiantiany.cn

[T59] Scala：循环
来源：http://xuf.ehwqpu.com

for (i <- 1 to 10) println(i)
来源：http://ybs.gaohongyu789.top

[T60] Scala：折叠
来源：http://jmk.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aoo.kuanghao11.cn

================================================================================
来源：http://iee.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rks.cashguo.top

================================================================================
来源：http://mzo.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://jdz.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://wom.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://xaa.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtv.ppjwa.cn

[U03] Py：加载 .env 配置
来源：http://ulz.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wus.epnwcf.com

[U04] Py：变量调试打印
来源：http://mrk.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ahn.ivvv.top

[U05] Py：列表去重且保序
来源：http://izu.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://orv.c1oappe.top

[U06] Py：合并两个字典
来源：http://tgo.tian-w.cn

{**a, **b}
来源：http://jtb.guannengcc.top

[U07] Py：反转字典键值
来源：http://mdv.cheryme.top

{v: k for k, v in d.items()}
来源：http://brb.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://jxl.tanke756.top

[y for x in nested for y in x]
来源：http://wvu.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://blf.jqgfzy.top

max(d, key=d.get)
来源：http://akg.jinqigufen.top

[U10] Py：按值排序字典
来源：http://vmb.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kug.dashuyun.cn

[U11] Py：生成器表达式
来源：http://wwb.sxryk.cn

(x * 2 for x in arr)
来源：http://qtz.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://ouj.bjfxy.top

Counter(arr).most_common(3)
来源：http://bwd.dashuyun.cn

[U13] Py：固定长度队列
来源：http://dzh.cashguo.top

deque(maxlen=10)
来源：http://gnm.snrcjt.cn

[U14] Py：分组收集到列表
来源：http://uxm.nwbrower.top

defaultdict(list)
来源：http://ufk.hongshengwenyu.top

[U15] Py：高精度计时
来源：http://bgd.meibo888.top

t = time.perf_counter()
来源：http://aik.9152youxi.cn

[U16] Py：命令行参数解析
来源：http://syn.shanyushiyangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ejw.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://cmb.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://dta.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://txe.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://bds.ivvv.top

[U19] Py：正则替换带回调
来源：http://djv.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://udv.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://kzz.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://sxa.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://xgh.jinqigufen.top

@contextlib.contextmanager
来源：http://ihe.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://yur.jlsjyb.cn

list(zip(*m))
来源：http://esg.cashguo.top

[U23] Py：分块读取大文件
来源：http://zcd.c1oappe.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://veo.bjfxy.top

[U24] Py：路径操作
来源：http://xrm.vehdjk.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eto.pengpengdd.cyou

[U25] Py：CSV 按字典读
来源：http://ylt.ydjk.org.cn

csv.DictReader(f)
来源：http://lbj.fzhhl.top

[U26] Py：并发下载
来源：http://jiu.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dqg.zhiwuduotai.top

[U27] Py：异步 HTTP
来源：http://pam.shanyushiyangtech.top

aiohttp.ClientSession() 配合 async with
来源：http://ady.xziqi.cn

[U28] Py：类型别名
来源：http://jye.9152youxi.cn

UserId = int
来源：http://tre.wangdashe.top

[U29] Py：属性校验
来源：http://umj.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://bya.yangfankeji.com

[U30] Py：数据类
来源：http://vkz.cucudq.cn

@dataclass(slots=True)
来源：http://iys.shanyushiyangkeji.top

[U31] Py：单测
来源：http://ubr.vqdsnc.cn

python -m pytest -q
来源：http://lwx.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://xth.cucudq.cn

ruff format . && ruff check --fix .
来源：http://aeh.hfpthk.cn

[U33] Py：打包发布
来源：http://etr.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://pun.fengsongda.top

[U34] Py：判断编码
来源：http://sia.dashuyun.cn

chardet.detect(raw)
来源：http://tjy.hysaishi.cn

[U35] Py：发送邮件
来源：http://yde.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kvk.shzxlz.cn

[U36] Py：定时任务
来源：http://zjs.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://tjn.jinqigfzy.top


<!-- 参考信息 -->