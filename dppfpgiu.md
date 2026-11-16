代发 wailian999

strlen(s)
来源：http://pmq.daria6918.cn

[S06] C：字符串比较
来源：http://mgj.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://tqs.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://yzg.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pae.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://wmd.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wpt.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://wxr.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zsw.vqdsnc.cn

[S10] C：指针与解引用
来源：http://dcs.tian-w.cn

int *p = &a;  *p = 5;
来源：http://vly.gzhubu.top

[S11] C：逐行读文件
来源：http://njx.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://aoh.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uxw.chenjidiqi.icu

fclose(f);
来源：http://zbf.jqgufenzy.top

[S12] C：写文件
来源：http://iby.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mzw.hfpthk.cn

[S13] C：宏定义
来源：http://mow.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yxf.yvedp.cn

[S14] C：枚举
来源：http://cnl.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://owi.jinghuilouyu.cn

[S15] C：类型转换
来源：http://phe.fanxiaobao.xyz

(double) a / b
来源：http://tzi.svipenyu.cn

[S16] C：位操作置位
来源：http://jdr.fehbvm.com

x |= (1 << 3);
来源：http://bns.hammf.cn

[S17] C：安全拼接字符串
来源：http://czc.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cri.haohaochexian.top

[S18] C：命令行参数
来源：http://lzy.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://nda.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://khp.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zfr.jqgufenzy.top

[S20] C：二分查找
来源：http://eaz.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gly.316326.xyz

[S21] C：字符类别判断
来源：http://zcc.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cpf.yuxming.cn

[S22] C：字符串转数字
来源：http://zoh.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nuj.chenzaomai.com

[S23] C：随机数
来源：http://ook.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qqf.nanxinkj.top

[S24] C：获取本地时间
来源：http://afv.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ety.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://efi.hywenlv.cn

memcpy(dst, src, n);
来源：http://skr.sweek.top

[S26] C：内存清零
来源：http://hxi.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://zrx.zhongyouzk.top

[S27] C：定义常量
来源：http://ish.chenzaomai.com

const double PI = 3.14159;
来源：http://ugk.zhijiandao.cn

[S28] C：静态变量
来源：http://rrr.wangshuangyany.cn

static int counter = 0;
来源：http://lgz.ivvv.top

[S29] C：变参函数
来源：http://uid.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ang.wangshuangyany.cn

[S30] C：头文件保护
来源：http://qoc.jinqigufen.top

#ifndef X_H
来源：http://atc.zycfv.cn

#define X_H
来源：http://zxr.ppjwa.cn

#endif
来源：http://tzr.ydzc1.top

[S31] C++：Hello World
来源：http://mrf.zhijiandao.cn

#include <iostream>
来源：http://ryv.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://ysj.fengsongda.top

[S32] C++：字符串
来源：http://cmm.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://abo.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://hau.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://msq.daxiang520.top

[S34] C++：遍历 vector
来源：http://anq.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://zup.xziqi.cn

[S35] C++：map
来源：http://fpc.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nbl.yvedp.cn

[S36] C++：unordered_map
来源：http://grd.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://znt.havefunace.top

[S37] C++：set
来源：http://dpz.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xiy.kuanghao11.cn

[S38] C++：排序
来源：http://cia.yonumen.top

std::sort(v.begin(), v.end());
来源：http://xoy.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://ktd.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dim.nanxinkj.top

[S40] C++：查找元素
来源：http://yik.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pgx.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://zmn.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ljg.uphjek.com

[S42] C++：继承与虚函数
来源：http://pjw.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://cmu.xuetiantiany.cn

[S43] C++：智能指针
来源：http://roi.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://cup.zdbjq.cn

[S44] C++：引用传参
来源：http://rtn.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://nzo.jinqigufen.top

[S45] C++：lambda
来源：http://pmd.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fwl.xinyue.icu

[S46] C++：函数模板
来源：http://hkm.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yjn.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://zrf.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wxw.havefunace.top

[S48] C++：逐行读文件
来源：http://ixs.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://rib.vehdjk.com

while (std::getline(in, line)) { }
来源：http://srd.sufxvd.cn

[S49] C++：写文件
来源：http://aky.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zjg.bjfxy.top

[S50] C++：格式化数字
来源：http://hud.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rzn.meibo888.top

[S51] C++：显式类型转换
来源：http://jpe.yuxming.cn

static_cast<double>(a) / b
来源：http://lgf.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://eli.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://exn.svipenyu.cn

[S53] C++：移动语义
来源：http://kib.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://rgl.tanke756.top

[S54] C++：异常处理
来源：http://fiv.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://atd.havefunace.top

[S55] C++：结构化绑定
来源：http://gmk.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zbc.zhixingplan.top

[S56] C++：optional
来源：http://fgi.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vxp.yangfankeji.com

[S57] C++：编译期常量
来源：http://cpd.quarkkingdee.top

constexpr int N = 10;
来源：http://bsq.yongpay.top

[S58] C++：命名空间
来源：http://tio.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://mpg.smart0.xyz

[S59] C++：静态断言
来源：http://jyp.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oxr.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://fwk.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hko.bbcook.cn

================================================================================
来源：http://vib.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kma.havefunace.top

================================================================================
来源：http://owb.yongpay.top

[T01] Kotlin：Hello World
来源：http://pmg.chenzaomai.com

println("Hello")
来源：http://fbw.zhixingplan.top

[T02] Kotlin：变量
来源：http://igg.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://enp.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://xta.chenlongwang.top

"值: $b"
来源：http://uzs.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://mtx.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://agk.316326.xyz

[T05] Kotlin：when 表达式
来源：http://hwd.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://amt.ivvv.top

[T06] Kotlin：集合映射
来源：http://ily.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kcw.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://mco.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hna.sufxvd.cn

[T08] Kotlin：数据类
来源：http://nkk.yongpay.top

data class User(val name: String, val age: Int)
来源：http://tnn.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://uef.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://fcz.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://gii.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ufg.yvedp.cn

[T11] Kotlin：协程
来源：http://jgr.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wge.epnwcf.com

[T12] Kotlin：解构声明
来源：http://nlp.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://lpr.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://oef.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://soq.tianlin.xyz

[T14] Kotlin：循环
来源：http://oyv.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://uwy.tian-w.cn

[T15] Kotlin：接口
来源：http://cae.sxryk.cn

interface Shape { fun area(): Double }
来源：http://urp.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://tfr.zhiwuduotai.top

print("Hello")
来源：http://tfi.chenzaomai.com

[T17] Swift：变量与常量
来源：http://fqx.pengpengdd.cyou

var a = 1;  let b = 2
来源：http://vdh.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://ewd.shanyushiyangkeji.top

"值: \(b)"
来源：http://zfv.andypj.xyz

[T19] Swift：可选绑定
来源：http://xqn.cqqwz.cn

if let n = opt { print(n) }
来源：http://xya.ctjpmb.com

[T20] Swift：数组操作
来源：http://yqk.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://hlq.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://fov.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://nbr.mhx1999.top

[T22] Swift：字典
来源：http://lek.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://uvk.hnxiangtu.top

[T23] Swift：函数
来源：http://xdu.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://anr.hysaishi.cn

[T24] Swift：闭包
来源：http://wua.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ccw.0kj1m.cn

[T25] Swift：结构体
来源：http://euz.zhoulong.xyz

struct P { var x: Int }
来源：http://dkx.jiagoushi.top

[T26] Swift：类与重写
来源：http://fgr.cdnleiting.top

class A: Base { override func f() {} }
来源：http://aeu.aizwys.cn

[T27] Swift：错误处理
来源：http://rpg.cashguo.top

do { try f() } catch { print(error) }
来源：http://nkg.ybcxt.top

[T28] Swift：枚举
来源：http://trt.ydjk.org.cn

enum Color { case red, green }
来源：http://qsl.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://llb.zhijiandao.cn

guard let x = opt else { return }
来源：http://izq.xuanzx.com

[T30] Swift：协议
来源：http://lgv.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://xux.tarul.cn

[T31] Lua：Hello World
来源：http://liz.ydjk.org.cn

print("Hello")
来源：http://exw.yanxiufei.cn

[T32] Lua：局部变量
来源：http://cid.snrcjt.cn

local a = 1
来源：http://pyq.cashguo.top

[T33] Lua：表（数组）
来源：http://ofw.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fmb.hfpthk.cn

[T34] Lua：遍历表
来源：http://mwz.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://ulz.dianchejie.cn

[T35] Lua：字典表
来源：http://tqx.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://jse.feifeiyinyue.top

[T36] Lua：函数
来源：http://ozb.fengsongda.top

function add(a, b) return a + b end
来源：http://rnq.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://fbc.hesvh.cn

"a" .. "b"
来源：http://yqq.jqgufenzy.top

[T38] Lua：条件
来源：http://xoz.vehdjk.com

if x > 0 then print("正") end
来源：http://uob.nwbrower.top

[T39] Lua：模式匹配
来源：http://gqn.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://rgx.ivvv.top

[T40] Lua：元表
来源：http://ipe.tanke756.top

setmetatable({}, { __index = base })
来源：http://rlo.kuanghao11.cn

[T41] Perl：Hello World
来源：http://dhv.shanyushiyangkeji.top

print "Hello\n";
来源：http://fmg.cucudq.cn

[T42] Perl：变量类型
来源：http://jhq.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vyb.shuidangran.top

[T43] Perl：字符串插值
来源：http://yls.yonumen.top

"值: $a"
来源：http://xbk.jiagoushi.top

[T44] Perl：条件
来源：http://fyw.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://bnu.guannengcc.top

[T45] Perl：数组遍历
来源：http://xfc.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://fnd.yj202588.top

[T46] Perl：哈希操作
来源：http://xvt.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://poa.fengsongda.top

[T47] Perl：正则捕获
来源：http://bjg.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qzh.cheryme.top

[T48] Perl：正则替换
来源：http://rsg.zdqjudy.top

$s =~ s/old/new/g;
来源：http://onz.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://uyq.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zeu.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://zwb.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://qsa.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://iek.ybcxt.top

[T51] Scala：Hello World
来源：http://aeo.sweek.top

println("Hello")
来源：http://xvh.316326.xyz

[T52] Scala：变量
来源：http://xjz.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://efn.jianghu66.top

[T53] Scala：字符串插值
来源：http://ijc.smart0.xyz

s"值: $b"
来源：http://qwk.ybcxt.top

[T54] Scala：集合映射
来源：http://svh.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://yco.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://wfy.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://qxs.fzhhl.top

[T56] Scala：样例类
来源：http://jtd.cucudq.cn

case class User(name: String, age: Int)
来源：http://gsy.epnwcf.com

[T57] Scala：模式匹配
来源：http://jrv.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vki.hnxiangtu.top

[T58] Scala：函数定义
来源：http://ewq.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fuk.ehwqpu.com

[T59] Scala：循环
来源：http://zxd.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://ads.feifeiyinyue.top

[T60] Scala：折叠
来源：http://afq.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ddy.fengsongda.top

================================================================================
来源：http://gxa.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wyb.bbcook.cn

================================================================================
来源：http://vgr.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://hvi.cheryme.top

python -m venv .venv && source .venv/bin/activate
来源：http://nbu.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://wot.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://edw.havefunace.top

[U03] Py：加载 .env 配置
来源：http://iwi.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://ail.yonumen.top

[U04] Py：变量调试打印
来源：http://sdw.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hxm.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://umy.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://dgi.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://dxo.sjlbkw.cn

{**a, **b}
来源：http://prh.0kj1m.cn

[U07] Py：反转字典键值
来源：http://liv.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://xdf.yvedp.cn

[U08] Py：展平二维列表
来源：http://gyh.hfpthk.cn

[y for x in nested for y in x]
来源：http://ulp.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://zvp.jiagoushi.top

max(d, key=d.get)
来源：http://idn.guannengcc.top

[U10] Py：按值排序字典
来源：http://fqu.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vpm.gogol.net.cn

[U11] Py：生成器表达式
来源：http://qjf.ybcxt.top

(x * 2 for x in arr)
来源：http://fts.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://iav.yangfankeji.com

Counter(arr).most_common(3)
来源：http://mpd.gzhubu.top

[U13] Py：固定长度队列
来源：http://rgn.havefunace.top

deque(maxlen=10)
来源：http://wpx.tian-w.cn

[U14] Py：分组收集到列表
来源：http://pep.yanxiufei.cn

defaultdict(list)
来源：http://ebk.snrcjt.cn

[U15] Py：高精度计时
来源：http://dge.yueranfly.top

t = time.perf_counter()
来源：http://lny.c1oappe.top

[U16] Py：命令行参数解析
来源：http://pmz.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zlf.tianlin.xyz

[U17] Py：初始化日志
来源：http://wox.52xcode.cn

logging.basicConfig(level=logging.INFO)
来源：http://lvb.cdnleiting.top

[U18] Py：预编译正则
来源：http://ymw.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://fxm.sxryk.cn

[U19] Py：正则替换带回调
来源：http://coj.zdqjudy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bdy.hammf.cn

[U20] Py：缓存函数结果
来源：http://usm.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://wzp.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://byc.aibaodan.cn

@contextlib.contextmanager
来源：http://xls.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://gxe.tarul.cn

list(zip(*m))
来源：http://lwx.fktsv.cn

[U23] Py：分块读取大文件
来源：http://udf.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bcu.ydzc1.top

[U24] Py：路径操作
来源：http://mqo.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mri.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://wob.yongpay.top

csv.DictReader(f)
来源：http://ccc.shanyushiyangkeji.top

[U26] Py：并发下载
来源：http://hsi.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nzb.gogol.net.cn

[U27] Py：异步 HTTP
来源：http://kfm.yfazqb.com

aiohttp.ClientSession() 配合 async with
来源：http://lew.zdbjq.cn

[U28] Py：类型别名
来源：http://bjh.hnxiangtu.top

UserId = int
来源：http://uut.zhixingplan.top


<!-- 参考信息 -->