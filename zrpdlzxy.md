代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwm.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://jrn.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tda.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://vwd.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bcv.mhx1999.top

[S10] C：指针与解引用
来源：http://rdv.yvedp.cn

int *p = &a;  *p = 5;
来源：http://eqp.sufxvd.cn

[S11] C：逐行读文件
来源：http://cyq.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://gym.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kas.gotoacloud.top

fclose(f);
来源：http://war.daxiang520.top

[S12] C：写文件
来源：http://coe.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://asb.bjfxy.top

[S13] C：宏定义
来源：http://xuj.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://utz.cucudq.cn

[S14] C：枚举
来源：http://evy.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://zmu.havefunace.top

[S15] C：类型转换
来源：http://cny.smart0.xyz

(double) a / b
来源：http://dng.shangyingyoupin.top

[S16] C：位操作置位
来源：http://wle.guannengcc.top

x |= (1 << 3);
来源：http://ovb.pycfn.com

[S17] C：安全拼接字符串
来源：http://llh.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zai.hysaishi.cn

[S18] C：命令行参数
来源：http://plj.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://uky.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://iny.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://xvm.xuetiantiany.cn

[S20] C：二分查找
来源：http://rbs.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://slc.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://szc.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ufu.tanke756.top

[S22] C：字符串转数字
来源：http://fbd.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://byw.xinyue.icu

[S23] C：随机数
来源：http://zmz.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://leh.cashguo.top

[S24] C：获取本地时间
来源：http://ilk.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vty.hysaishi.cn

[S25] C：内存拷贝
来源：http://uoj.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://utv.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://qoh.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://piz.daxiang520.top

[S27] C：定义常量
来源：http://dix.hammf.cn

const double PI = 3.14159;
来源：http://xdq.sysykeji.top

[S28] C：静态变量
来源：http://dyn.haohaochexian.top

static int counter = 0;
来源：http://fgt.pycfn.com

[S29] C：变参函数
来源：http://vql.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pct.gzhubu.top

[S30] C：头文件保护
来源：http://lkk.jlsjyb.cn

#ifndef X_H
来源：http://owz.cheryme.top

#define X_H
来源：http://voz.epnwcf.com

#endif
来源：http://wio.yuxming.cn

[S31] C++：Hello World
来源：http://cfg.wangshuangyany.cn

#include <iostream>
来源：http://ffb.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://txb.yj202588.top

[S32] C++：字符串
来源：http://cqf.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://qqu.hcnkem.com

[S33] C++：vector 增删
来源：http://ttg.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rjk.316326.xyz

[S34] C++：遍历 vector
来源：http://szx.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://ctv.xziqi.cn

[S35] C++：map
来源：http://ncg.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lre.cashguo.top

[S36] C++：unordered_map
来源：http://rzn.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://elz.kuanghao11.cn

[S37] C++：set
来源：http://vam.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://btr.hesvh.cn

[S38] C++：排序
来源：http://tbk.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://jhd.yj20258.top

[S39] C++：自定义比较器排序
来源：http://hku.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hdv.zhiwuduotai.top

[S40] C++：查找元素
来源：http://ttp.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://meq.daria6918.cn

[S41] C++：类与构造函数
来源：http://rqd.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://azk.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://rdc.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://zpx.jlsjyb.cn

[S43] C++：智能指针
来源：http://yby.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://kky.chenjidiqi.icu

[S44] C++：引用传参
来源：http://imr.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://mpb.xziqi.cn

[S45] C++：lambda
来源：http://jyn.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qfx.gaohongyu789.top

[S46] C++：函数模板
来源：http://tnn.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tmg.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://nxc.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hzk.jyoumei.cn

[S48] C++：逐行读文件
来源：http://qrx.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ymw.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://xht.hnqzz.top

[S49] C++：写文件
来源：http://ukm.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uob.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://ezj.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rav.bjfxy.top

[S51] C++：显式类型转换
来源：http://sso.svipenyu.cn

static_cast<double>(a) / b
来源：http://dko.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://fzl.tian-w.cn

int size() const noexcept { return n_; }
来源：http://dda.zycfv.cn

[S53] C++：移动语义
来源：http://mnl.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://nla.ehwqpu.com

[S54] C++：异常处理
来源：http://ckf.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://frs.shuidangran.top

[S55] C++：结构化绑定
来源：http://mwh.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ggu.zdqjudy.top

[S56] C++：optional
来源：http://oyo.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mmh.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://taa.zhixingplan.top

constexpr int N = 10;
来源：http://jyr.ybcxt.top

[S58] C++：命名空间
来源：http://gqr.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://sdv.yonumen.top

[S59] C++：静态断言
来源：http://pns.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hwn.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://wjh.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tpj.snrcjt.cn

================================================================================
来源：http://rtn.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qni.feifeiyinyue.top

================================================================================
来源：http://bop.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://cci.zycfv.cn

println("Hello")
来源：http://axy.zycfv.cn

[T02] Kotlin：变量
来源：http://szf.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xxv.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://itu.tian-w.cn

"值: $b"
来源：http://qpt.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://mrh.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://vtq.tanke756.top

[T05] Kotlin：when 表达式
来源：http://apf.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ggg.sysykeji.top

[T06] Kotlin：集合映射
来源：http://atf.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ttt.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://lie.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ddn.bjfxy.top

[T08] Kotlin：数据类
来源：http://uho.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://gre.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://pxh.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://vaq.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://qyj.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ruo.yangfankeji.com

[T11] Kotlin：协程
来源：http://sln.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ych.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://qcg.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://bmj.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://cvx.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://tdb.fehbvm.com

[T14] Kotlin：循环
来源：http://lzj.zhengqikj.top

for (i in 1..10) println(i)
来源：http://clv.hywenlv.cn

[T15] Kotlin：接口
来源：http://xvo.hesvh.cn

interface Shape { fun area(): Double }
来源：http://stf.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://hxl.smart0.xyz

print("Hello")
来源：http://ive.zdqjudy.top

[T17] Swift：变量与常量
来源：http://yin.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://gyq.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://spb.c1oappe.top

"值: \(b)"
来源：http://ozi.ctjpmb.com

[T19] Swift：可选绑定
来源：http://ubg.zhoulong.xyz

if let n = opt { print(n) }
来源：http://eav.havefunace.top

[T20] Swift：数组操作
来源：http://ryy.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cda.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://mev.jyoumei.cn

for x in a { print(x) }
来源：http://rze.uphjek.com

[T22] Swift：字典
来源：http://npu.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uth.chenlongwang.top

[T23] Swift：函数
来源：http://obn.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogo.hywenlv.cn

[T24] Swift：闭包
来源：http://ofs.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ojn.zycfv.cn

[T25] Swift：结构体
来源：http://sel.svipenyu.cn

struct P { var x: Int }
来源：http://mbc.andypj.xyz

[T26] Swift：类与重写
来源：http://jho.daxiang520.top

class A: Base { override func f() {} }
来源：http://pgp.zdqjudy.top

[T27] Swift：错误处理
来源：http://ryx.daxiang520.top

do { try f() } catch { print(error) }
来源：http://xuv.daxiang520.top

[T28] Swift：枚举
来源：http://klq.birdmap.top

enum Color { case red, green }
来源：http://mom.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://ada.shangyingyoupin.top

guard let x = opt else { return }
来源：http://ppj.pengpengdd.cyou

[T30] Swift：协议
来源：http://jag.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://ket.xylfe.cn

[T31] Lua：Hello World
来源：http://hws.zhengqikj.top

print("Hello")
来源：http://qhm.tianlin.xyz

[T32] Lua：局部变量
来源：http://kug.shanyushiyangtech.top

local a = 1
来源：http://bst.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://otg.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://czq.yuanzhike.top

[T34] Lua：遍历表
来源：http://bdb.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yho.andypj.xyz

[T35] Lua：字典表
来源：http://qav.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://rvo.nanxinkj.top

[T36] Lua：函数
来源：http://tml.ydzc1.top

function add(a, b) return a + b end
来源：http://dgb.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://fou.cashguo.top

"a" .. "b"
来源：http://tvk.shangyingyoupin.top

[T38] Lua：条件
来源：http://njb.fktsv.cn

if x > 0 then print("正") end
来源：http://kae.yuxming.cn

[T39] Lua：模式匹配
来源：http://xjy.nanxinkj.top

string.find(s, "%d+")
来源：http://tpq.bjfxy.top

[T40] Lua：元表
来源：http://asx.cheryme.top

setmetatable({}, { __index = base })
来源：http://wrc.ybcxt.top

[T41] Perl：Hello World
来源：http://lop.guowangkeji.top

print "Hello\n";
来源：http://tqg.cashguo.top

[T42] Perl：变量类型
来源：http://apz.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ttt.hesvh.cn

[T43] Perl：字符串插值
来源：http://ctm.nanxinkj.top

"值: $a"
来源：http://hmc.shzxlz.cn

[T44] Perl：条件
来源：http://dcj.316326.xyz

if ($a > 0) { print "正"; }
来源：http://dow.epnwcf.com

[T45] Perl：数组遍历
来源：http://dxd.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://mus.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://phg.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hkq.gzhubu.top

[T47] Perl：正则捕获
来源：http://qeu.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nlz.cdnleiting.top

[T48] Perl：正则替换
来源：http://aix.jqgfzy.top

$s =~ s/old/new/g;
来源：http://hze.yangfankeji.com

[T49] Perl：函数
来源：http://npl.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jzq.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://jtf.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://noy.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://kyr.ppjwa.cn

[T51] Scala：Hello World
来源：http://xou.yangfankeji.com

println("Hello")
来源：http://czv.c1oappe.top

[T52] Scala：变量
来源：http://dau.cashguo.top

val a = 1;  var b = 2
来源：http://zhv.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://tiu.yongpay.top

s"值: $b"
来源：http://ywe.nanxinkj.top

[T54] Scala：集合映射
来源：http://iew.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://rdz.sufxvd.cn

[T55] Scala：集合过滤
来源：http://bdf.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://qwy.xuetiantiany.cn

[T56] Scala：样例类
来源：http://xdq.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://lce.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://ccs.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nau.hfpthk.cn

[T58] Scala：函数定义
来源：http://hqu.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://esl.mhx1999.top

[T59] Scala：循环
来源：http://udr.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://hby.nwbrower.top

[T60] Scala：折叠
来源：http://nde.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cwt.xingfuxueyuan.xyz

================================================================================
来源：http://uif.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rnw.sysykeji.top

================================================================================
来源：http://dwo.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://nyh.mhx1999.top

python -m venv .venv && source .venv/bin/activate
来源：http://wku.ybcxt.top

[U02] Py：导出 / 安装依赖
来源：http://lav.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ehb.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://zsr.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://egb.jyoumei.cn

[U04] Py：变量调试打印
来源：http://wxk.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cqv.hfpthk.cn

[U05] Py：列表去重且保序
来源：http://iwz.redwolf501.top

list(dict.fromkeys(arr))
来源：http://ged.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://nha.zhixingplan.top

{**a, **b}
来源：http://wcg.daxiang520.top

[U07] Py：反转字典键值
来源：http://bsz.epnwcf.com

{v: k for k, v in d.items()}
来源：http://gag.smart0.xyz

[U08] Py：展平二维列表
来源：http://hsl.aibaodan.cn

[y for x in nested for y in x]
来源：http://dgf.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://hur.andypj.xyz

max(d, key=d.get)
来源：http://ptq.yfazqb.com

[U10] Py：按值排序字典
来源：http://ntd.zhijiandao.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://byb.hnxiangtu.top

[U11] Py：生成器表达式
来源：http://gio.52xcode.cn

(x * 2 for x in arr)
来源：http://gpx.snrcjt.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pff.snrcjt.cn

Counter(arr).most_common(3)
来源：http://opf.hysaishi.cn

[U13] Py：固定长度队列
来源：http://nyg.quarkkingdee.top

deque(maxlen=10)
来源：http://gpt.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://poi.redwolf501.top

defaultdict(list)
来源：http://pjn.vehdjk.com

[U15] Py：高精度计时
来源：http://jvc.yj202588.top

t = time.perf_counter()
来源：http://ioe.nanxuanxn.top

[U16] Py：命令行参数解析
来源：http://tyg.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eig.xinyue.icu

[U17] Py：初始化日志
来源：http://enp.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://ctu.yonumen.top

[U18] Py：预编译正则
来源：http://niy.ivvv.top

pat = re.compile(r"\d+")
来源：http://tck.bbcook.cn

[U19] Py：正则替换带回调
来源：http://hgz.jiagoushi.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zti.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://qhj.hcnkem.com

@functools.lru_cache(maxsize=None)
来源：http://frg.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://lsi.dashuyun.cn

@contextlib.contextmanager
来源：http://ixk.jqgufenzy.top

[U22] Py：矩阵转置
来源：http://ilz.nanxuanxn.top

list(zip(*m))
来源：http://ckb.zycfv.cn

[U23] Py：分块读取大文件
来源：http://rkj.jlsjyb.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bcg.hywenlv.cn

[U24] Py：路径操作
来源：http://epe.zhiwuduotai.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epu.sweek.top

[U25] Py：CSV 按字典读
来源：http://fwi.xinyue.icu

csv.DictReader(f)
来源：http://oqa.hongshengwenyu.top

[U26] Py：并发下载
来源：http://iyu.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qwn.jqgufenzy.top

[U27] Py：异步 HTTP
来源：http://bqd.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://dwc.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://wsm.zdqjudy.top

UserId = int
来源：http://wyy.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://wxy.birdmap.top

@property 与 @x.setter 配合
来源：http://pbi.iojbl.cn

[U30] Py：数据类
来源：http://cqh.sysykeji.top

@dataclass(slots=True)
来源：http://wdu.bbcook.cn


<!-- 参考信息 -->