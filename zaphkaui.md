代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbn.uphjek.com

[S08] C：动态内存分配与释放
来源：http://qtx.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rfc.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://eyg.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mkt.tianlin.xyz

[S10] C：指针与解引用
来源：http://dek.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://zqm.dashuyun.cn

[S11] C：逐行读文件
来源：http://bzw.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://hys.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hno.hysaishi.cn

fclose(f);
来源：http://jkg.ctjpmb.com

[S12] C：写文件
来源：http://bqx.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnr.gaohongyu789.top

[S13] C：宏定义
来源：http://wiv.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vlz.aibaodan.cn

[S14] C：枚举
来源：http://pji.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://wki.snrcjt.cn

[S15] C：类型转换
来源：http://fel.pycfn.com

(double) a / b
来源：http://pmp.iojbl.cn

[S16] C：位操作置位
来源：http://mbq.ctjpmb.com

x |= (1 << 3);
来源：http://gus.sxryk.cn

[S17] C：安全拼接字符串
来源：http://dov.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zcf.andypj.xyz

[S18] C：命令行参数
来源：http://kcv.cucudq.cn

int main(int argc, char **argv)
来源：http://pka.iojbl.cn

[S19] C：快速排序
来源：http://gjq.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://uli.zdqjudy.top

[S20] C：二分查找
来源：http://gum.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bzz.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://csd.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ibn.316326.xyz

[S22] C：字符串转数字
来源：http://noo.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pcd.vehdjk.com

[S23] C：随机数
来源：http://iyy.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fbz.yfazqb.com

[S24] C：获取本地时间
来源：http://iwg.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zsn.pycfn.com

[S25] C：内存拷贝
来源：http://spv.havefunace.top

memcpy(dst, src, n);
来源：http://ulz.hammf.cn

[S26] C：内存清零
来源：http://ymn.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://qpw.mhx1999.top

[S27] C：定义常量
来源：http://iro.ivvv.top

const double PI = 3.14159;
来源：http://mvb.shangyingyoupin.top

[S28] C：静态变量
来源：http://pue.haohaochexian.top

static int counter = 0;
来源：http://ijd.birdmap.top

[S29] C：变参函数
来源：http://xxq.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybr.epnwcf.com

[S30] C：头文件保护
来源：http://ijj.ydjk.org.cn

#ifndef X_H
来源：http://vuh.tarul.cn

#define X_H
来源：http://lgu.wangdashe.top

#endif
来源：http://dsx.zycfv.cn

[S31] C++：Hello World
来源：http://uys.hnqzz.top

#include <iostream>
来源：http://omo.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://zcv.jyoumei.cn

[S32] C++：字符串
来源：http://gyv.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://hug.ctjpmb.com

[S33] C++：vector 增删
来源：http://vlf.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://swc.yvedp.cn

[S34] C++：遍历 vector
来源：http://ppi.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://vst.zhaomingkeji.xyz

[S35] C++：map
来源：http://fft.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iez.sjlbkw.cn

[S36] C++：unordered_map
来源：http://dzj.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gze.nanxuanxn.top

[S37] C++：set
来源：http://sfj.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://brk.fanxiaobao.xyz

[S38] C++：排序
来源：http://web.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://eth.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://gno.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://czd.jinqigfzy.top

[S40] C++：查找元素
来源：http://tny.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hcl.uphjek.com

[S41] C++：类与构造函数
来源：http://njk.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://thm.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://sfp.9152youxi.cn

class B : public Base { public: void f() override {} };
来源：http://myy.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://nhy.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://ipr.zhongyouzk.top

[S44] C++：引用传参
来源：http://qlf.smart0.xyz

void inc(int &x) { ++x; }
来源：http://mrw.nwbrower.top

[S45] C++：lambda
来源：http://jom.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://efn.xuetiantiany.cn

[S46] C++：函数模板
来源：http://bnv.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kid.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://lyu.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://npl.ydzc1.top

[S48] C++：逐行读文件
来源：http://yxu.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://fyl.tarul.cn

while (std::getline(in, line)) { }
来源：http://zyy.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://kan.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jdz.bjfxy.top

[S50] C++：格式化数字
来源：http://gxj.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mqq.aizwys.cn

[S51] C++：显式类型转换
来源：http://jja.fengsongda.top

static_cast<double>(a) / b
来源：http://cmt.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://kzn.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://llf.snrcjt.cn

[S53] C++：移动语义
来源：http://pnc.yj20258.top

std::vector<int> w = std::move(v);
来源：http://ulx.svipenyu.cn

[S54] C++：异常处理
来源：http://gyy.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gnk.ehwqpu.com

[S55] C++：结构化绑定
来源：http://dsk.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ozp.jqgufenzy.top

[S56] C++：optional
来源：http://pmt.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aak.jinqigfzy.top

[S57] C++：编译期常量
来源：http://kyo.9152youxi.cn

constexpr int N = 10;
来源：http://tgk.dashuyun.cn

[S58] C++：命名空间
来源：http://okl.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://kmp.ppjwa.cn

[S59] C++：静态断言
来源：http://zos.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ypq.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://rir.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://juu.yj20258.top

================================================================================
来源：http://eou.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gar.zdbjq.cn

================================================================================
来源：http://isu.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://xpm.wangshuangyany.cn

println("Hello")
来源：http://kgi.vqdsnc.cn

[T02] Kotlin：变量
来源：http://doz.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dew.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://ojd.yongpay.top

"值: $b"
来源：http://wti.0kj1m.cn

[T04] Kotlin：空安全
来源：http://pse.shzxlz.cn

val n: String? = null;  n?.length
来源：http://val.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://cuo.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cxt.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://xon.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zow.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://adb.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ejo.dianchejie.cn

[T08] Kotlin：数据类
来源：http://hui.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://jcz.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://igm.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://qyi.nwbrower.top

[T10] Kotlin：默认参数
来源：http://tad.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aiq.jinqigufen.top

[T11] Kotlin：协程
来源：http://kzr.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lox.yueranfly.top

[T12] Kotlin：解构声明
来源：http://qna.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://pxr.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://rhd.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://nyg.ppjwa.cn

[T14] Kotlin：循环
来源：http://xzx.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://ain.shuidangran.top

[T15] Kotlin：接口
来源：http://apv.ydzc1.top

interface Shape { fun area(): Double }
来源：http://wly.jinqigufen.top

[T16] Swift：Hello World
来源：http://eck.guannengcc.top

print("Hello")
来源：http://jep.chenzaomai.com

[T17] Swift：变量与常量
来源：http://hwy.hnqzz.top

var a = 1;  let b = 2
来源：http://kco.ehwqpu.com

[T18] Swift：字符串插值
来源：http://xyq.zhongyouzk.top

"值: \(b)"
来源：http://hnz.hesvh.cn

[T19] Swift：可选绑定
来源：http://quf.jqgufenzy.top

if let n = opt { print(n) }
来源：http://zvh.yonumen.top

[T20] Swift：数组操作
来源：http://euc.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://xkn.guannengcc.top

[T21] Swift：遍历
来源：http://hfe.dianchejie.cn

for x in a { print(x) }
来源：http://qui.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://sfu.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://rnc.yangfankeji.com

[T23] Swift：函数
来源：http://yba.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://byo.ydzc1.top

[T24] Swift：闭包
来源：http://axg.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mdg.chenjidiqi.icu

[T25] Swift：结构体
来源：http://ruu.feifeiyinyue.top

struct P { var x: Int }
来源：http://luu.jyoumei.cn

[T26] Swift：类与重写
来源：http://pav.ybcxt.top

class A: Base { override func f() {} }
来源：http://iqp.zhixingplan.top

[T27] Swift：错误处理
来源：http://ysa.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://bcf.chenlongwang.top

[T28] Swift：枚举
来源：http://tuh.yfazqb.com

enum Color { case red, green }
来源：http://lsq.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://ucn.guannengcc.top

guard let x = opt else { return }
来源：http://iqm.0kj1m.cn

[T30] Swift：协议
来源：http://unc.havefunace.top

protocol Shape { func area() -> Double }
来源：http://sih.yj20258888.top

[T31] Lua：Hello World
来源：http://aji.ppjwa.cn

print("Hello")
来源：http://pfi.jiagoushi.top

[T32] Lua：局部变量
来源：http://ngi.jyoumei.cn

local a = 1
来源：http://cgc.zdqjudy.top

[T33] Lua：表（数组）
来源：http://ozy.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qik.jianghu66.top

[T34] Lua：遍历表
来源：http://wjw.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pwy.uphjek.com

[T35] Lua：字典表
来源：http://asc.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://env.iojbl.cn

[T36] Lua：函数
来源：http://pag.andypj.xyz

function add(a, b) return a + b end
来源：http://iuv.uphjek.com

[T37] Lua：字符串拼接
来源：http://dom.yonumen.top

"a" .. "b"
来源：http://srg.aibaodan.cn

[T38] Lua：条件
来源：http://jam.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://kph.ehwqpu.com

[T39] Lua：模式匹配
来源：http://xjz.vehdjk.com

string.find(s, "%d+")
来源：http://ieo.hfpthk.cn

[T40] Lua：元表
来源：http://uvx.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://xwp.yuxming.cn

[T41] Perl：Hello World
来源：http://rpv.pycfn.com

print "Hello\n";
来源：http://cpr.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://csq.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xpk.guowangkeji.top

[T43] Perl：字符串插值
来源：http://gwk.cheryme.top

"值: $a"
来源：http://xfm.shanyushiyangtech.top

[T44] Perl：条件
来源：http://brd.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://jnv.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://lix.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://ycl.hywenlv.cn

[T46] Perl：哈希操作
来源：http://xbv.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nuj.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://qob.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://haz.havefunace.top

[T48] Perl：正则替换
来源：http://lnf.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://zjd.9152youxi.cn

[T49] Perl：函数
来源：http://oge.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xcb.jlsjyb.cn

[T50] Perl：逐行读文件
来源：http://ixp.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://iqq.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://mwq.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://rxd.ydjk.org.cn

println("Hello")
来源：http://zsb.0kj1m.cn

[T52] Scala：变量
来源：http://jcy.sweek.top

val a = 1;  var b = 2
来源：http://hop.yj20258.top

[T53] Scala：字符串插值
来源：http://kht.zhoulong.xyz

s"值: $b"
来源：http://yer.vehdjk.com

[T54] Scala：集合映射
来源：http://juo.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://dzt.0kj1m.cn

[T55] Scala：集合过滤
来源：http://lnt.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://gjh.fzhhl.top

[T56] Scala：样例类
来源：http://qwo.andypj.xyz

case class User(name: String, age: Int)
来源：http://zsk.yuanzhike.top

[T57] Scala：模式匹配
来源：http://xfk.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://ivd.xuanzx.com

[T58] Scala：函数定义
来源：http://fwa.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uuz.jqgufenzy.top

[T59] Scala：循环
来源：http://bwl.ydjk.org.cn

for (i <- 1 to 10) println(i)
来源：http://uvt.vqdsnc.cn

[T60] Scala：折叠
来源：http://qih.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mpm.hammf.cn

================================================================================
来源：http://xuf.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://exj.yueranfly.top

================================================================================
来源：http://fae.0kj1m.cn

[U01] Py：创建虚拟环境
来源：http://iyv.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://efa.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://ruf.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://apn.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://omd.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vcx.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://drj.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zyn.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://vct.aizwys.cn

list(dict.fromkeys(arr))
来源：http://pxb.jinqigufen.top

[U06] Py：合并两个字典
来源：http://kym.shanyushiyangtech.top

{**a, **b}
来源：http://her.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://sot.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://ypg.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://bkd.nwbrower.top

[y for x in nested for y in x]
来源：http://bfe.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://cpd.fehbvm.com

max(d, key=d.get)
来源：http://qzp.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://mvt.shzxlz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wvf.nanxuanxn.top

[U11] Py：生成器表达式
来源：http://bni.gogol.net.cn

(x * 2 for x in arr)
来源：http://aqd.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://sla.shzxlz.cn

Counter(arr).most_common(3)
来源：http://hhv.sxryk.cn

[U13] Py：固定长度队列
来源：http://clk.fanxiaobao.xyz

deque(maxlen=10)
来源：http://wfi.xingfuxueyuan.xyz

[U14] Py：分组收集到列表
来源：http://vux.9152youxi.cn

defaultdict(list)
来源：http://wcn.gaohongyu789.top

[U15] Py：高精度计时
来源：http://imy.haohaochexian.top

t = time.perf_counter()
来源：http://xed.wangdashe.top

[U16] Py：命令行参数解析
来源：http://ouh.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kek.cashguo.top

[U17] Py：初始化日志
来源：http://trt.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://njr.yj20258.top

[U18] Py：预编译正则
来源：http://ndl.chenlongwang.top

pat = re.compile(r"\d+")
来源：http://tuj.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://sww.haohaochexian.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nxf.zycfv.cn

[U20] Py：缓存函数结果
来源：http://sve.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://bmr.xinyue.icu

[U21] Py：自定义上下文管理器
来源：http://mpq.pycfn.com

@contextlib.contextmanager
来源：http://wye.gotoacloud.top

[U22] Py：矩阵转置
来源：http://dtd.ehwqpu.com

list(zip(*m))
来源：http://bby.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://vjx.gaohongyu789.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eag.kuanghao11.cn

[U24] Py：路径操作
来源：http://vhu.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dsp.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://ixf.fengsongda.top

csv.DictReader(f)
来源：http://isa.bjfxy.top

[U26] Py：并发下载
来源：http://dzk.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aso.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://ryd.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://gok.snrcjt.cn

[U28] Py：类型别名
来源：http://ozz.jlsjyb.cn

UserId = int
来源：http://iwa.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://nyw.hnqzz.top

@property 与 @x.setter 配合
来源：http://pkn.jlsjyb.cn

[U30] Py：数据类
来源：http://dpu.wangshuangyany.cn

@dataclass(slots=True)
来源：http://ghv.shangyingyoupin.top


<!-- 参考信息 -->