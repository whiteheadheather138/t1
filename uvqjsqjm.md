代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ojx.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fnp.dashuyun.cn

fclose(f);
来源：http://shi.hammf.cn

[S12] C：写文件
来源：http://uqt.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixw.xylfe.cn

[S13] C：宏定义
来源：http://fyr.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://doo.tian-w.cn

[S14] C：枚举
来源：http://dww.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://mgp.zhongyouzk.top

[S15] C：类型转换
来源：http://mhe.hysaishi.cn

(double) a / b
来源：http://ggx.snrcjt.cn

[S16] C：位操作置位
来源：http://ugx.zycfv.cn

x |= (1 << 3);
来源：http://ecu.yj20258888.top

[S17] C：安全拼接字符串
来源：http://zwp.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yrz.yj20258888.top

[S18] C：命令行参数
来源：http://gpx.hnxiangtu.top

int main(int argc, char **argv)
来源：http://dkl.bjfxy.top

[S19] C：快速排序
来源：http://pev.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://twj.zhijiandao.cn

[S20] C：二分查找
来源：http://isg.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ymq.yueranfly.top

[S21] C：字符类别判断
来源：http://jxv.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xgu.zdqjudy.top

[S22] C：字符串转数字
来源：http://bqx.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xds.guannengcc.top

[S23] C：随机数
来源：http://aew.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qxo.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://bym.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rcp.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://bzd.ehwqpu.com

memcpy(dst, src, n);
来源：http://njj.jinqigfzy.top

[S26] C：内存清零
来源：http://lzl.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://ypa.yj20258.top

[S27] C：定义常量
来源：http://grk.zdbjq.cn

const double PI = 3.14159;
来源：http://bcx.xziqi.cn

[S28] C：静态变量
来源：http://ibp.gotoacloud.top

static int counter = 0;
来源：http://ywa.haohaochexian.top

[S29] C：变参函数
来源：http://hte.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xpk.zhoulong.xyz

[S30] C：头文件保护
来源：http://szm.yanxiufei.cn

#ifndef X_H
来源：http://ohk.zhoulong.xyz

#define X_H
来源：http://pdp.andypj.xyz

#endif
来源：http://vzz.bbcook.cn

[S31] C++：Hello World
来源：http://mgw.ppjwa.cn

#include <iostream>
来源：http://pji.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://nvl.52xcode.cn

[S32] C++：字符串
来源：http://htt.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://moy.tarul.cn

[S33] C++：vector 增删
来源：http://nkt.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://adk.ctjpmb.com

[S34] C++：遍历 vector
来源：http://gmh.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://xsv.sxryk.cn

[S35] C++：map
来源：http://gqh.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fok.jianghu66.top

[S36] C++：unordered_map
来源：http://gwb.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bsm.yj20258.top

[S37] C++：set
来源：http://wth.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dtu.jiagoushi.top

[S38] C++：排序
来源：http://xkd.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://iyw.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://mry.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wxo.cqqwz.cn

[S40] C++：查找元素
来源：http://dyy.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uni.yvedp.cn

[S41] C++：类与构造函数
来源：http://ekf.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ldp.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://zed.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://xqm.sxryk.cn

[S43] C++：智能指针
来源：http://fqk.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://kuc.fengsongda.top

[S44] C++：引用传参
来源：http://snw.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://ojz.zhoulong.xyz

[S45] C++：lambda
来源：http://ngr.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jmq.tanke756.top

[S46] C++：函数模板
来源：http://aoh.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wgn.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://kpl.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nne.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://yep.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://dop.hammf.cn

while (std::getline(in, line)) { }
来源：http://yxh.fehbvm.com

[S49] C++：写文件
来源：http://gyu.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fgh.hnxiangtu.top

[S50] C++：格式化数字
来源：http://ubm.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jpy.tian-w.cn

[S51] C++：显式类型转换
来源：http://ojk.hywenlv.cn

static_cast<double>(a) / b
来源：http://fse.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://pyv.bjfxy.top

int size() const noexcept { return n_; }
来源：http://jbc.pengpengdd.cyou

[S53] C++：移动语义
来源：http://dmk.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://uzb.hesvh.cn

[S54] C++：异常处理
来源：http://ubm.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vhc.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://gtp.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hqg.cdnleiting.top

[S56] C++：optional
来源：http://bew.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vkc.dianchejie.cn

[S57] C++：编译期常量
来源：http://mmk.nanxuanxn.top

constexpr int N = 10;
来源：http://lvg.jiagoushi.top

[S58] C++：命名空间
来源：http://ijc.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://knx.zdbjq.cn

[S59] C++：静态断言
来源：http://ycl.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wqm.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://jwp.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yrk.tian-w.cn

================================================================================
来源：http://rts.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fda.hnxiangtu.top

================================================================================
来源：http://mkk.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://oba.redwolf501.top

println("Hello")
来源：http://cvl.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://gxj.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://frk.yj20258.top

[T03] Kotlin：字符串模板
来源：http://fgp.iojbl.cn

"值: $b"
来源：http://hjo.sysykeji.top

[T04] Kotlin：空安全
来源：http://bci.zycfv.cn

val n: String? = null;  n?.length
来源：http://llr.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://rhs.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ivw.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://gjv.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lut.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://fjp.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jhw.zycfv.cn

[T08] Kotlin：数据类
来源：http://vjl.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://jki.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://hnn.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://ogk.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://xga.jlsjyb.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://igx.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://nni.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ihc.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://bxj.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://vfb.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://nqg.cheryme.top

val m = mapOf("a" to 1)
来源：http://zqx.hnqzz.top

[T14] Kotlin：循环
来源：http://wjf.hysaishi.cn

for (i in 1..10) println(i)
来源：http://fqj.52xcode.cn

[T15] Kotlin：接口
来源：http://nhk.wangdashe.top

interface Shape { fun area(): Double }
来源：http://qst.kuanghao11.cn

[T16] Swift：Hello World
来源：http://krd.jinqigufen.top

print("Hello")
来源：http://bry.yueranfly.top

[T17] Swift：变量与常量
来源：http://hrc.zycfv.cn

var a = 1;  let b = 2
来源：http://fsv.hnqzz.top

[T18] Swift：字符串插值
来源：http://uzi.ydjk.org.cn

"值: \(b)"
来源：http://joe.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://nha.zhongyouzk.top

if let n = opt { print(n) }
来源：http://aaa.aibaodan.cn

[T20] Swift：数组操作
来源：http://cvm.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://pdi.hammf.cn

[T21] Swift：遍历
来源：http://yrg.jianghu66.top

for x in a { print(x) }
来源：http://gsd.yongpay.top

[T22] Swift：字典
来源：http://gwx.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://oqd.jinqigfzy.top

[T23] Swift：函数
来源：http://gar.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mxr.haohaochexian.top

[T24] Swift：闭包
来源：http://lmr.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gfc.yangfankeji.com

[T25] Swift：结构体
来源：http://icv.jinqigfzy.top

struct P { var x: Int }
来源：http://olp.hcnkem.com

[T26] Swift：类与重写
来源：http://xwi.uphjek.com

class A: Base { override func f() {} }
来源：http://sml.bbcook.cn

[T27] Swift：错误处理
来源：http://dap.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://hmk.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://brh.ppjwa.cn

enum Color { case red, green }
来源：http://wmq.pycfn.com

[T29] Swift：guard 提前返回
来源：http://mco.wangdashe.top

guard let x = opt else { return }
来源：http://sau.vehdjk.com

[T30] Swift：协议
来源：http://mps.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://gyk.gaohongyu789.top

[T31] Lua：Hello World
来源：http://duj.snrcjt.cn

print("Hello")
来源：http://sny.daria6918.cn

[T32] Lua：局部变量
来源：http://wqq.tanke756.top

local a = 1
来源：http://dts.ydzc1.top

[T33] Lua：表（数组）
来源：http://pku.xziqi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://owt.zycfv.cn

[T34] Lua：遍历表
来源：http://oty.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sye.yvedp.cn

[T35] Lua：字典表
来源：http://uqx.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://oap.jqgfzy.top

[T36] Lua：函数
来源：http://fqo.cashguo.top

function add(a, b) return a + b end
来源：http://jwz.snrcjt.cn

[T37] Lua：字符串拼接
来源：http://eet.svipenyu.cn

"a" .. "b"
来源：http://hph.shangyingyoupin.top

[T38] Lua：条件
来源：http://unl.tianlin.xyz

if x > 0 then print("正") end
来源：http://vhh.cqqwz.cn

[T39] Lua：模式匹配
来源：http://gjg.52xcode.cn

string.find(s, "%d+")
来源：http://wix.pycfn.com

[T40] Lua：元表
来源：http://vdr.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://hfy.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://low.yuanzhike.top

print "Hello\n";
来源：http://dab.zycfv.cn

[T42] Perl：变量类型
来源：http://gwn.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://unh.fehbvm.com

[T43] Perl：字符串插值
来源：http://zbx.gotoacloud.top

"值: $a"
来源：http://dwo.zhengqikj.top

[T44] Perl：条件
来源：http://ewl.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://sfn.yuxming.cn

[T45] Perl：数组遍历
来源：http://pwk.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://cui.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://uat.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://otb.shzxlz.cn

[T47] Perl：正则捕获
来源：http://pqz.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yzj.chenzaomai.com

[T48] Perl：正则替换
来源：http://cno.aizwys.cn

$s =~ s/old/new/g;
来源：http://lfh.ydzc1.top

[T49] Perl：函数
来源：http://lsv.xinyue.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://unt.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://mcy.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rxw.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://kct.havefunace.top

[T51] Scala：Hello World
来源：http://aqd.jqgfzy.top

println("Hello")
来源：http://mcf.uphjek.com

[T52] Scala：变量
来源：http://ieb.yfazqb.com

val a = 1;  var b = 2
来源：http://spx.nwbrower.top

[T53] Scala：字符串插值
来源：http://xyq.xylfe.cn

s"值: $b"
来源：http://jsv.sysykeji.top

[T54] Scala：集合映射
来源：http://ehz.hammf.cn

List(1, 2, 3).map(_ * 2)
来源：http://bsg.xuetiantiany.cn

[T55] Scala：集合过滤
来源：http://rpa.shuidangran.top

List(1, 2, 3).filter(_ > 1)
来源：http://bqd.xziqi.cn

[T56] Scala：样例类
来源：http://cps.zhixingplan.top

case class User(name: String, age: Int)
来源：http://han.cqqwz.cn

[T57] Scala：模式匹配
来源：http://oxw.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://weu.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://dus.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://fpl.yj20258888.top

[T59] Scala：循环
来源：http://uzy.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://que.yj20258888.top

[T60] Scala：折叠
来源：http://hll.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vvg.ppjwa.cn

================================================================================
来源：http://xdz.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bsg.sjlbkw.cn

================================================================================
来源：http://kpw.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://ngh.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://mzm.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://oym.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rmv.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://yql.sysykeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bry.cdnleiting.top

[U04] Py：变量调试打印
来源：http://sth.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kkr.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://xyh.havefunace.top

list(dict.fromkeys(arr))
来源：http://dgt.mhx1999.top

[U06] Py：合并两个字典
来源：http://krs.zdqjudy.top

{**a, **b}
来源：http://zit.0kj1m.cn

[U07] Py：反转字典键值
来源：http://cdh.yj20258.top

{v: k for k, v in d.items()}
来源：http://ash.fehbvm.com

[U08] Py：展平二维列表
来源：http://vvb.vqdsnc.cn

[y for x in nested for y in x]
来源：http://rcm.cheryme.top

[U09] Py：字典取最大值的键
来源：http://bqq.fengsongda.top

max(d, key=d.get)
来源：http://dpp.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://krs.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zaq.sufxvd.cn

[U11] Py：生成器表达式
来源：http://dnv.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://eqf.nanxuanxn.top

[U12] Py：取出现最多的 3 个元素
来源：http://cwd.chenlongwang.top

Counter(arr).most_common(3)
来源：http://uhy.yonumen.top

[U13] Py：固定长度队列
来源：http://lzm.daria6918.cn

deque(maxlen=10)
来源：http://nsi.jqgufenzy.top

[U14] Py：分组收集到列表
来源：http://ipd.yfazqb.com

defaultdict(list)
来源：http://lfu.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://ynr.chenjidiqi.icu

t = time.perf_counter()
来源：http://fzo.yj20258.top

[U16] Py：命令行参数解析
来源：http://ctp.fzhhl.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://irv.nanxuanxn.top

[U17] Py：初始化日志
来源：http://mqk.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://ukl.smart0.xyz

[U18] Py：预编译正则
来源：http://pmd.52xcode.cn

pat = re.compile(r"\d+")
来源：http://kjz.yuanzhike.top

[U19] Py：正则替换带回调
来源：http://cjd.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xge.xinyue.icu

[U20] Py：缓存函数结果
来源：http://ace.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://lzh.aizwys.cn

[U21] Py：自定义上下文管理器
来源：http://bdb.fengsongda.top

@contextlib.contextmanager
来源：http://glm.gzhubu.top

[U22] Py：矩阵转置
来源：http://lvp.xinyue.icu

list(zip(*m))
来源：http://bbn.yfazqb.com

[U23] Py：分块读取大文件
来源：http://qao.guannengcc.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tqu.gogol.net.cn

[U24] Py：路径操作
来源：http://yhx.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qjl.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://oug.gogol.net.cn

csv.DictReader(f)
来源：http://jcx.hongshengwenyu.top

[U26] Py：并发下载
来源：http://kad.aizwys.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dvm.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://lqo.zhixingplan.top

aiohttp.ClientSession() 配合 async with
来源：http://kaw.zhengqikj.top

[U28] Py：类型别名
来源：http://etj.hnqzz.top

UserId = int
来源：http://wgv.nwbrower.top

[U29] Py：属性校验
来源：http://wzv.yj202588.top

@property 与 @x.setter 配合
来源：http://ott.guowangkeji.top

[U30] Py：数据类
来源：http://ddx.pengpengdd.cyou

@dataclass(slots=True)
来源：http://itr.sxryk.cn

[U31] Py：单测
来源：http://icz.cucudq.cn

python -m pytest -q
来源：http://aro.52xcode.cn

[U32] Py：代码格式化
来源：http://ujy.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://smz.chenjidiqi.icu

[U33] Py：打包发布
来源：http://rxt.tarul.cn

python -m build  （依赖 pyproject.toml）
来源：http://guo.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://bdi.smart0.xyz

chardet.detect(raw)
来源：http://hnb.fengsongda.top


<!-- 参考信息 -->