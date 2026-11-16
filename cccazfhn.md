代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehq.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://uto.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ozg.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://qam.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hsn.zhongyouzk.top

[S10] C：指针与解引用
来源：http://lhj.bbcook.cn

int *p = &a;  *p = 5;
来源：http://yyt.tarul.cn

[S11] C：逐行读文件
来源：http://sad.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://zom.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gzm.cucudq.cn

fclose(f);
来源：http://wbe.wangdashe.top

[S12] C：写文件
来源：http://luq.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://luc.fanxiaobao.xyz

[S13] C：宏定义
来源：http://kzo.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ylx.tian-w.cn

[S14] C：枚举
来源：http://ygp.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://oyq.shanyushiyangtech.top

[S15] C：类型转换
来源：http://ncz.yongpay.top

(double) a / b
来源：http://gkn.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://xun.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://pnt.pycfn.com

[S17] C：安全拼接字符串
来源：http://fot.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://llu.fengsongda.top

[S18] C：命令行参数
来源：http://lop.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://dxt.hywenlv.cn

[S19] C：快速排序
来源：http://dve.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gwa.jiagoushi.top

[S20] C：二分查找
来源：http://jae.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qjg.zhengqikj.top

[S21] C：字符类别判断
来源：http://utg.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://enu.hnqzz.top

[S22] C：字符串转数字
来源：http://gqc.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pvv.dashuyun.cn

[S23] C：随机数
来源：http://hkm.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nmy.9152youxi.cn

[S24] C：获取本地时间
来源：http://ccu.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ebu.xylfe.cn

[S25] C：内存拷贝
来源：http://ayo.kuanghao11.cn

memcpy(dst, src, n);
来源：http://rfj.cucudq.cn

[S26] C：内存清零
来源：http://wub.andypj.xyz

memset(a, 0, sizeof a);
来源：http://nuj.vqdsnc.cn

[S27] C：定义常量
来源：http://geg.ybcxt.top

const double PI = 3.14159;
来源：http://opr.pengpengdd.cyou

[S28] C：静态变量
来源：http://xng.dianchejie.cn

static int counter = 0;
来源：http://rks.fehbvm.com

[S29] C：变参函数
来源：http://ulg.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fai.feifeiyinyue.top

[S30] C：头文件保护
来源：http://dqe.fanxiaobao.xyz

#ifndef X_H
来源：http://ezk.yueranfly.top

#define X_H
来源：http://cxz.svipenyu.cn

#endif
来源：http://aky.shuidangran.top

[S31] C++：Hello World
来源：http://iyp.yangfankeji.com

#include <iostream>
来源：http://wav.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://bwc.yangfankeji.com

[S32] C++：字符串
来源：http://glr.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://nfb.fzhhl.top

[S33] C++：vector 增删
来源：http://vry.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pfv.epnwcf.com

[S34] C++：遍历 vector
来源：http://rig.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://zya.tianlin.xyz

[S35] C++：map
来源：http://wsd.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://smr.mhx1999.top

[S36] C++：unordered_map
来源：http://mei.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fag.cqqwz.cn

[S37] C++：set
来源：http://uml.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uhi.ivvv.top

[S38] C++：排序
来源：http://pkj.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://oee.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://rfw.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hrj.fktsv.cn

[S40] C++：查找元素
来源：http://pvv.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tkw.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://rii.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zzl.tian-w.cn

[S42] C++：继承与虚函数
来源：http://ubj.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://yxm.xinyue.icu

[S43] C++：智能指针
来源：http://ycg.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://ezw.daxiang520.top

[S44] C++：引用传参
来源：http://ury.andypj.xyz

void inc(int &x) { ++x; }
来源：http://kbk.gotoacloud.top

[S45] C++：lambda
来源：http://knf.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://akg.yuxming.cn

[S46] C++：函数模板
来源：http://oei.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lbt.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://wqa.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nod.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://cmu.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://swk.bjfxy.top

while (std::getline(in, line)) { }
来源：http://oow.aizwys.cn

[S49] C++：写文件
来源：http://wbm.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xiv.hnxiangtu.top

[S50] C++：格式化数字
来源：http://glx.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jiv.yueranfly.top

[S51] C++：显式类型转换
来源：http://vxl.yj20258888.top

static_cast<double>(a) / b
来源：http://jen.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://ugs.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://ebt.chenlongwang.top

[S53] C++：移动语义
来源：http://aqd.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://rjs.zycfv.cn

[S54] C++：异常处理
来源：http://qmy.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kea.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://zwv.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tlj.jinyuanbaomall.cn

[S56] C++：optional
来源：http://vwq.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xut.52xcode.cn

[S57] C++：编译期常量
来源：http://xtg.ppjwa.cn

constexpr int N = 10;
来源：http://htf.vehdjk.com

[S58] C++：命名空间
来源：http://jek.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://loo.c1oappe.top

[S59] C++：静态断言
来源：http://feo.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lyo.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://qrw.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://scn.tian-w.cn

================================================================================
来源：http://scg.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqq.fehbvm.com

================================================================================
来源：http://gvy.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://cwj.svipenyu.cn

println("Hello")
来源：http://dmk.yuanzhike.top

[T02] Kotlin：变量
来源：http://rsl.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://scw.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://ihz.ctjpmb.com

"值: $b"
来源：http://pox.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://jzj.jinqigufen.top

val n: String? = null;  n?.length
来源：http://ucs.tarul.cn

[T05] Kotlin：when 表达式
来源：http://mdg.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pdh.yj20258.top

[T06] Kotlin：集合映射
来源：http://lan.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lmf.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://lqa.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cpo.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://myt.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://kcl.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://sug.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://myj.tian-w.cn

[T10] Kotlin：默认参数
来源：http://vgx.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://non.shuidangran.top

[T11] Kotlin：协程
来源：http://vka.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ccc.yueranfly.top

[T12] Kotlin：解构声明
来源：http://pre.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://kjm.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://zln.epnwcf.com

val m = mapOf("a" to 1)
来源：http://lgt.quarkkingdee.top

[T14] Kotlin：循环
来源：http://ksa.smart0.xyz

for (i in 1..10) println(i)
来源：http://otk.ctjpmb.com

[T15] Kotlin：接口
来源：http://olh.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://zhc.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://dlh.ydjk.org.cn

print("Hello")
来源：http://rgm.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://dsq.pycfn.com

var a = 1;  let b = 2
来源：http://lpk.tianlin.xyz

[T18] Swift：字符串插值
来源：http://udm.jlsjyb.cn

"值: \(b)"
来源：http://aii.yueranfly.top

[T19] Swift：可选绑定
来源：http://uxk.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://stg.yuanzhike.top

[T20] Swift：数组操作
来源：http://pqk.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://nix.jiagoushi.top

[T21] Swift：遍历
来源：http://mwo.hammf.cn

for x in a { print(x) }
来源：http://cvw.daria6918.cn

[T22] Swift：字典
来源：http://uml.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kxz.yfazqb.com

[T23] Swift：函数
来源：http://rnc.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hom.yueranfly.top

[T24] Swift：闭包
来源：http://ltl.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://huk.mhx1999.top

[T25] Swift：结构体
来源：http://xff.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://agz.chenzaomai.com

[T26] Swift：类与重写
来源：http://ekw.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://wmr.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://lqs.fehbvm.com

do { try f() } catch { print(error) }
来源：http://dnm.mhx1999.top

[T28] Swift：枚举
来源：http://qjz.xinyue.icu

enum Color { case red, green }
来源：http://wjn.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://woh.zhongyouzk.top

guard let x = opt else { return }
来源：http://dgi.guowangkeji.top

[T30] Swift：协议
来源：http://bqf.yj202588.top

protocol Shape { func area() -> Double }
来源：http://toe.yongpay.top

[T31] Lua：Hello World
来源：http://sbg.chenjidiqi.icu

print("Hello")
来源：http://pru.snrcjt.cn

[T32] Lua：局部变量
来源：http://mqo.gogol.net.cn

local a = 1
来源：http://dpz.yfazqb.com

[T33] Lua：表（数组）
来源：http://fvs.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://dfc.bbcook.cn

[T34] Lua：遍历表
来源：http://jzi.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hnt.gotoacloud.top

[T35] Lua：字典表
来源：http://vig.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://czh.shanyushiyangtech.top

[T36] Lua：函数
来源：http://fqp.bjfxy.top

function add(a, b) return a + b end
来源：http://ysu.ybcxt.top

[T37] Lua：字符串拼接
来源：http://rml.xuetiantiany.cn

"a" .. "b"
来源：http://let.dashuyun.cn

[T38] Lua：条件
来源：http://ljo.hcnkem.com

if x > 0 then print("正") end
来源：http://ynv.aibaodan.cn

[T39] Lua：模式匹配
来源：http://zhn.zdqjudy.top

string.find(s, "%d+")
来源：http://ifg.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://rdg.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://dje.redwolf501.top

[T41] Perl：Hello World
来源：http://dgb.sufxvd.cn

print "Hello\n";
来源：http://fwm.fktsv.cn

[T42] Perl：变量类型
来源：http://esh.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bwf.vehdjk.com

[T43] Perl：字符串插值
来源：http://gow.jqgufenzy.top

"值: $a"
来源：http://apj.fzhhl.top

[T44] Perl：条件
来源：http://gnu.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://rjn.9152youxi.cn

[T45] Perl：数组遍历
来源：http://tig.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://nnv.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://rpn.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://osf.tarul.cn

[T47] Perl：正则捕获
来源：http://hiq.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vvt.xylfe.cn

[T48] Perl：正则替换
来源：http://yiu.yfazqb.com

$s =~ s/old/new/g;
来源：http://waw.hcnkem.com

[T49] Perl：函数
来源：http://kxv.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jew.aizwys.cn

[T50] Perl：逐行读文件
来源：http://uzq.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qhp.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://gta.sweek.top

[T51] Scala：Hello World
来源：http://nqa.fzhhl.top

println("Hello")
来源：http://quw.cucudq.cn

[T52] Scala：变量
来源：http://ljm.haohaochexian.top

val a = 1;  var b = 2
来源：http://scb.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://ifo.sxryk.cn

s"值: $b"
来源：http://meg.chenzaomai.com

[T54] Scala：集合映射
来源：http://sxr.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://hbj.nanxinkj.top

[T55] Scala：集合过滤
来源：http://uhq.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://fxn.bjfxy.top

[T56] Scala：样例类
来源：http://zaj.yueranfly.top

case class User(name: String, age: Int)
来源：http://uai.epnwcf.com

[T57] Scala：模式匹配
来源：http://mps.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nam.fzhhl.top

[T58] Scala：函数定义
来源：http://ilx.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://muo.feifeiyinyue.top

[T59] Scala：循环
来源：http://sds.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://gya.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://fhm.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://som.bjfxy.top

================================================================================
来源：http://bfl.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ljh.wangdashe.top

================================================================================
来源：http://brn.meibo888.top

[U01] Py：创建虚拟环境
来源：http://dkt.ybcxt.top

python -m venv .venv && source .venv/bin/activate
来源：http://syo.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://qnp.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vaz.ydzc1.top

[U03] Py：加载 .env 配置
来源：http://lqy.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://unt.ybcxt.top

[U04] Py：变量调试打印
来源：http://ttt.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://add.sysykeji.top

[U05] Py：列表去重且保序
来源：http://jdw.shanyushiyangkeji.top

list(dict.fromkeys(arr))
来源：http://cry.cucudq.cn

[U06] Py：合并两个字典
来源：http://fsm.fehbvm.com

{**a, **b}
来源：http://sgi.jyoumei.cn

[U07] Py：反转字典键值
来源：http://xad.yueranfly.top

{v: k for k, v in d.items()}
来源：http://gsp.yj20258888.top

[U08] Py：展平二维列表
来源：http://owg.jyoumei.cn

[y for x in nested for y in x]
来源：http://uwo.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://nwe.guannengcc.top

max(d, key=d.get)
来源：http://snh.fzhhl.top

[U10] Py：按值排序字典
来源：http://wqq.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ajb.gogol.net.cn

[U11] Py：生成器表达式
来源：http://sow.yueranfly.top

(x * 2 for x in arr)
来源：http://gke.vqdsnc.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nax.snrcjt.cn

Counter(arr).most_common(3)
来源：http://kzp.nwbrower.top

[U13] Py：固定长度队列
来源：http://cgb.aizwys.cn

deque(maxlen=10)
来源：http://fbl.yj20258888.top

[U14] Py：分组收集到列表
来源：http://ryk.vqdsnc.cn

defaultdict(list)
来源：http://uct.meibo888.top

[U15] Py：高精度计时
来源：http://pkj.hfpthk.cn

t = time.perf_counter()
来源：http://aqm.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://cvo.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://isl.pycfn.com

[U17] Py：初始化日志
来源：http://bui.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://nqg.fktsv.cn

[U18] Py：预编译正则
来源：http://zmn.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://uyc.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://eug.gaohongyu789.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://whj.jianghu66.top

[U20] Py：缓存函数结果
来源：http://end.fzhhl.top

@functools.lru_cache(maxsize=None)
来源：http://hpx.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://aqx.hnxiangtu.top

@contextlib.contextmanager
来源：http://bqo.zhaomingkeji.xyz

[U22] Py：矩阵转置
来源：http://xwj.cdnleiting.top

list(zip(*m))
来源：http://aid.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://hng.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fub.daxiang520.top

[U24] Py：路径操作
来源：http://qwb.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ryy.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://ngk.xinyue.icu

csv.DictReader(f)
来源：http://lgh.dianchejie.cn

[U26] Py：并发下载
来源：http://zgm.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ukw.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://pkn.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://ecd.yueranfly.top

[U28] Py：类型别名
来源：http://duk.birdmap.top

UserId = int
来源：http://nah.dianchejie.cn

[U29] Py：属性校验
来源：http://tpu.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://pig.bbcook.cn

[U30] Py：数据类
来源：http://ipe.xinyue.icu

@dataclass(slots=True)
来源：http://fmq.cashguo.top


<!-- 参考信息 -->