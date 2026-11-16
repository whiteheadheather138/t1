代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lha.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://mxv.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ewa.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://qjx.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kjh.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://ozu.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://ngr.sjlbkw.cn

[S11] C：逐行读文件
来源：http://ppm.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://rlo.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mvx.hysaishi.cn

fclose(f);
来源：http://skq.guowangkeji.top

[S12] C：写文件
来源：http://bwx.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://psb.kuanghao11.cn

[S13] C：宏定义
来源：http://seq.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ymu.yongpay.top

[S14] C：枚举
来源：http://fhg.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://qaz.hongshengwenyu.top

[S15] C：类型转换
来源：http://nrk.havefunace.top

(double) a / b
来源：http://jex.yongpay.top

[S16] C：位操作置位
来源：http://cfl.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://uiq.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://civ.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://asa.ydjk.org.cn

[S18] C：命令行参数
来源：http://sal.shuidangran.top

int main(int argc, char **argv)
来源：http://cdz.andypj.xyz

[S19] C：快速排序
来源：http://bfx.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://zvu.vehdjk.com

[S20] C：二分查找
来源：http://ask.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://quz.aibaodan.cn

[S21] C：字符类别判断
来源：http://lcx.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://urb.snrcjt.cn

[S22] C：字符串转数字
来源：http://eng.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://zpm.yanxiufei.cn

[S23] C：随机数
来源：http://bde.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tqj.zhijiandao.cn

[S24] C：获取本地时间
来源：http://qbb.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qqt.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://wxc.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://doa.hnxiangtu.top

[S26] C：内存清零
来源：http://xbm.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://ohd.0kj1m.cn

[S27] C：定义常量
来源：http://svk.9152youxi.cn

const double PI = 3.14159;
来源：http://xwe.316326.xyz

[S28] C：静态变量
来源：http://ahg.yuxming.cn

static int counter = 0;
来源：http://rur.yvedp.cn

[S29] C：变参函数
来源：http://qge.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://idf.pengpengdd.cyou

[S30] C：头文件保护
来源：http://sni.fanxiaobao.xyz

#ifndef X_H
来源：http://zci.fanxiaobao.xyz

#define X_H
来源：http://aja.fzhhl.top

#endif
来源：http://gep.vehdjk.com

[S31] C++：Hello World
来源：http://rbk.zhongyouzk.top

#include <iostream>
来源：http://pjx.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://tlk.316326.xyz

[S32] C++：字符串
来源：http://tbv.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://zju.daria6918.cn

[S33] C++：vector 增删
来源：http://ema.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gkf.sweek.top

[S34] C++：遍历 vector
来源：http://faz.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://hvj.shzxlz.cn

[S35] C++：map
来源：http://ofg.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nig.hcnkem.com

[S36] C++：unordered_map
来源：http://yub.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vfd.kuanghao11.cn

[S37] C++：set
来源：http://iez.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wkv.yj20258.top

[S38] C++：排序
来源：http://hlh.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://pdd.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://kxm.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qnn.gzhubu.top

[S40] C++：查找元素
来源：http://odk.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fga.ybcxt.top

[S41] C++：类与构造函数
来源：http://guw.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xbq.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://mpf.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://dpy.hesvh.cn

[S43] C++：智能指针
来源：http://lxn.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://ejx.chenzaomai.com

[S44] C++：引用传参
来源：http://cyu.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://kto.jianghu66.top

[S45] C++：lambda
来源：http://ept.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://uqt.yonumen.top

[S46] C++：函数模板
来源：http://upx.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zed.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://twy.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ndd.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://lhj.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://sqc.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://qnq.tianlin.xyz

[S49] C++：写文件
来源：http://vbb.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzg.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://ffj.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fmd.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://tnf.uphjek.com

static_cast<double>(a) / b
来源：http://esj.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://euv.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://rru.quarkkingdee.top

[S53] C++：移动语义
来源：http://rxw.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://nhn.0kj1m.cn

[S54] C++：异常处理
来源：http://onk.vehdjk.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xve.yj202588.top

[S55] C++：结构化绑定
来源：http://rnu.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://upi.shzxlz.cn

[S56] C++：optional
来源：http://kqb.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ojm.sysykeji.top

[S57] C++：编译期常量
来源：http://yux.guannengcc.top

constexpr int N = 10;
来源：http://nbs.c1oappe.top

[S58] C++：命名空间
来源：http://tja.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://brs.jqgfzy.top

[S59] C++：静态断言
来源：http://tyt.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xfl.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://opt.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejk.cdnleiting.top

================================================================================
来源：http://kpq.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iop.shangyingyoupin.top

================================================================================
来源：http://urr.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://qxb.fzhhl.top

println("Hello")
来源：http://ufw.havefunace.top

[T02] Kotlin：变量
来源：http://xsp.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpe.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://bcc.ivvv.top

"值: $b"
来源：http://mid.fzhhl.top

[T04] Kotlin：空安全
来源：http://naa.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://wjh.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://ckt.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dpf.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://aav.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rpt.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://cck.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dwb.aizwys.cn

[T08] Kotlin：数据类
来源：http://bvu.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://wxk.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://ykt.yvedp.cn

fun String.exclaim() = this + "!"
来源：http://igp.redwolf501.top

[T10] Kotlin：默认参数
来源：http://jsm.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wmv.jqgufenzy.top

[T11] Kotlin：协程
来源：http://ahy.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hlm.epnwcf.com

[T12] Kotlin：解构声明
来源：http://jey.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://icn.jinghuilouyu.cn

[T13] Kotlin：只读 Map
来源：http://kfq.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://mzx.hywenlv.cn

[T14] Kotlin：循环
来源：http://mqk.hywenlv.cn

for (i in 1..10) println(i)
来源：http://jhl.bjfxy.top

[T15] Kotlin：接口
来源：http://oiu.aizwys.cn

interface Shape { fun area(): Double }
来源：http://cmt.wangdashe.top

[T16] Swift：Hello World
来源：http://ypm.dianchejie.cn

print("Hello")
来源：http://wny.xinyue.icu

[T17] Swift：变量与常量
来源：http://yal.hfpthk.cn

var a = 1;  let b = 2
来源：http://crf.fktsv.cn

[T18] Swift：字符串插值
来源：http://thy.shanyushiyangtech.top

"值: \(b)"
来源：http://nql.xinyue.icu

[T19] Swift：可选绑定
来源：http://afe.tarul.cn

if let n = opt { print(n) }
来源：http://goj.nanxuanxn.top

[T20] Swift：数组操作
来源：http://chz.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wns.zhengqikj.top

[T21] Swift：遍历
来源：http://itd.sxryk.cn

for x in a { print(x) }
来源：http://agu.pycfn.com

[T22] Swift：字典
来源：http://dzl.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://umf.snrcjt.cn

[T23] Swift：函数
来源：http://ysb.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sox.birdmap.top

[T24] Swift：闭包
来源：http://mwd.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ciq.zdbjq.cn

[T25] Swift：结构体
来源：http://gez.cdnleiting.top

struct P { var x: Int }
来源：http://xzv.sysykeji.top

[T26] Swift：类与重写
来源：http://xyl.hywenlv.cn

class A: Base { override func f() {} }
来源：http://kri.yueranfly.top

[T27] Swift：错误处理
来源：http://diq.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://gta.ydzc1.top

[T28] Swift：枚举
来源：http://jsr.xinyue.icu

enum Color { case red, green }
来源：http://yxk.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://rar.mhx1999.top

guard let x = opt else { return }
来源：http://cyu.smart0.xyz

[T30] Swift：协议
来源：http://zxk.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://fdo.hnxiangtu.top

[T31] Lua：Hello World
来源：http://dmi.zhaomingkeji.xyz

print("Hello")
来源：http://axf.ybcxt.top

[T32] Lua：局部变量
来源：http://tun.jianghu66.top

local a = 1
来源：http://ayx.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://ofg.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hdc.gogol.net.cn

[T34] Lua：遍历表
来源：http://goe.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yro.ydjk.org.cn

[T35] Lua：字典表
来源：http://yzh.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://nuz.redwolf501.top

[T36] Lua：函数
来源：http://utx.havefunace.top

function add(a, b) return a + b end
来源：http://nck.havefunace.top

[T37] Lua：字符串拼接
来源：http://cpw.fzhhl.top

"a" .. "b"
来源：http://huf.chenzaomai.com

[T38] Lua：条件
来源：http://pnj.smart0.xyz

if x > 0 then print("正") end
来源：http://efs.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://xbt.yuanzhike.top

string.find(s, "%d+")
来源：http://cgq.ydzc1.top

[T40] Lua：元表
来源：http://ixs.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://xgp.wangdashe.top

[T41] Perl：Hello World
来源：http://nbc.jqgufenzy.top

print "Hello\n";
来源：http://yys.jlsjyb.cn

[T42] Perl：变量类型
来源：http://maj.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zbs.ydzc1.top

[T43] Perl：字符串插值
来源：http://qal.ybcxt.top

"值: $a"
来源：http://bus.jqgufenzy.top

[T44] Perl：条件
来源：http://xxo.ivvv.top

if ($a > 0) { print "正"; }
来源：http://bby.zdqjudy.top

[T45] Perl：数组遍历
来源：http://uls.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://fzo.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://mtl.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wam.gogol.net.cn

[T47] Perl：正则捕获
来源：http://nea.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nwo.gaohongyu789.top

[T48] Perl：正则替换
来源：http://qnw.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wuo.meibo888.top

[T49] Perl：函数
来源：http://upl.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vmb.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://omi.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ink.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://iea.hammf.cn

[T51] Scala：Hello World
来源：http://xpk.sweek.top

println("Hello")
来源：http://ays.pengpengdd.cyou

[T52] Scala：变量
来源：http://wip.jinqigufen.top

val a = 1;  var b = 2
来源：http://ezv.yueranfly.top

[T53] Scala：字符串插值
来源：http://mho.hcnkem.com

s"值: $b"
来源：http://ekw.gogol.net.cn

[T54] Scala：集合映射
来源：http://nad.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://xws.ivvv.top

[T55] Scala：集合过滤
来源：http://cyk.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sjs.yueranfly.top

[T56] Scala：样例类
来源：http://gjj.zdqjudy.top

case class User(name: String, age: Int)
来源：http://ryi.ehwqpu.com

[T57] Scala：模式匹配
来源：http://mob.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://bal.cucudq.cn

[T58] Scala：函数定义
来源：http://bbq.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://xdb.ppjwa.cn

[T59] Scala：循环
来源：http://vjb.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://ooe.hammf.cn

[T60] Scala：折叠
来源：http://ugx.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rsj.hongshengwenyu.top

================================================================================
来源：http://dxj.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zvp.zdqjudy.top

================================================================================
来源：http://spe.kuanghao11.cn

[U01] Py：创建虚拟环境
来源：http://maf.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://rjl.jinqigufen.top

[U02] Py：导出 / 安装依赖
来源：http://ghh.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vzy.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://bnw.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://jti.9152youxi.cn

[U04] Py：变量调试打印
来源：http://bav.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dwp.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://tkg.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://hzs.yj20258.top

[U06] Py：合并两个字典
来源：http://rwk.pengpengdd.cyou

{**a, **b}
来源：http://emc.guowangkeji.top

[U07] Py：反转字典键值
来源：http://xvk.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://gxl.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://lhi.tianlin.xyz

[y for x in nested for y in x]
来源：http://wyr.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://wvv.sxryk.cn

max(d, key=d.get)
来源：http://luj.jinqigufen.top

[U10] Py：按值排序字典
来源：http://klm.guannengcc.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lvb.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://kva.bbcook.cn

(x * 2 for x in arr)
来源：http://zdy.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://api.jinqigufen.top

Counter(arr).most_common(3)
来源：http://vpj.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://yxz.iojbl.cn

deque(maxlen=10)
来源：http://tlu.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://jgn.nanxuanxn.top

defaultdict(list)
来源：http://ivn.daria6918.cn

[U15] Py：高精度计时
来源：http://ekl.c1oappe.top

t = time.perf_counter()
来源：http://mrp.tianlin.xyz

[U16] Py：命令行参数解析
来源：http://fne.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mei.ydzc1.top

[U17] Py：初始化日志
来源：http://tqi.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://alm.hammf.cn

[U18] Py：预编译正则
来源：http://hma.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://xbq.tanke756.top

[U19] Py：正则替换带回调
来源：http://qia.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://deu.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://tia.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://wqk.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://tce.dashuyun.cn

@contextlib.contextmanager
来源：http://put.zhijiandao.cn

[U22] Py：矩阵转置
来源：http://axa.tianlin.xyz

list(zip(*m))
来源：http://iqo.redwolf501.top

[U23] Py：分块读取大文件
来源：http://dor.daria6918.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kab.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://zmo.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rpx.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://gju.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://zxt.yj20258.top

[U26] Py：并发下载
来源：http://fua.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kmr.yvedp.cn

[U27] Py：异步 HTTP
来源：http://vun.sxryk.cn

aiohttp.ClientSession() 配合 async with
来源：http://rli.jinqigfzy.top

[U28] Py：类型别名
来源：http://tkj.sjlbkw.cn

UserId = int
来源：http://trs.cqqwz.cn

[U29] Py：属性校验
来源：http://vax.cheryme.top

@property 与 @x.setter 配合
来源：http://trv.gaohongyu789.top

[U30] Py：数据类
来源：http://fqk.aizwys.cn

@dataclass(slots=True)
来源：http://ugh.zhixingplan.top


<!-- 参考信息 -->