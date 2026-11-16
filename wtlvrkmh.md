代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://esn.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ebf.epnwcf.com

fclose(f);
来源：http://ohf.cashguo.top

[S12] C：写文件
来源：http://dey.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rxj.52xcode.cn

[S13] C：宏定义
来源：http://eyc.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mef.jiagoushi.top

[S14] C：枚举
来源：http://vrr.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://rrv.gaohongyu789.top

[S15] C：类型转换
来源：http://nnv.smart0.xyz

(double) a / b
来源：http://lsk.bbcook.cn

[S16] C：位操作置位
来源：http://mjq.vehdjk.com

x |= (1 << 3);
来源：http://oyz.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://nzx.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wgl.zhoulong.xyz

[S18] C：命令行参数
来源：http://tjl.jinqigfzy.top

int main(int argc, char **argv)
来源：http://uyr.yangfankeji.com

[S19] C：快速排序
来源：http://wgh.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://gpv.hesvh.cn

[S20] C：二分查找
来源：http://qyo.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uwu.fengsongda.top

[S21] C：字符类别判断
来源：http://kef.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvo.snrcjt.cn

[S22] C：字符串转数字
来源：http://csn.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://oik.guannengcc.top

[S23] C：随机数
来源：http://rxr.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://yws.shzxlz.cn

[S24] C：获取本地时间
来源：http://kqg.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mpj.xylfe.cn

[S25] C：内存拷贝
来源：http://vds.aibaodan.cn

memcpy(dst, src, n);
来源：http://atf.ppjwa.cn

[S26] C：内存清零
来源：http://iwc.yuxming.cn

memset(a, 0, sizeof a);
来源：http://fdr.52xcode.cn

[S27] C：定义常量
来源：http://ucc.shangyingyoupin.top

const double PI = 3.14159;
来源：http://bdg.wangdashe.top

[S28] C：静态变量
来源：http://hdk.tanke756.top

static int counter = 0;
来源：http://zmt.shzxlz.cn

[S29] C：变参函数
来源：http://jtm.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfa.zhiwuduotai.top

[S30] C：头文件保护
来源：http://yte.jqgfzy.top

#ifndef X_H
来源：http://kyw.gotoacloud.top

#define X_H
来源：http://amq.tanke756.top

#endif
来源：http://zus.zdbjq.cn

[S31] C++：Hello World
来源：http://omm.ywan-chungtsiang.top

#include <iostream>
来源：http://alo.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://djb.hesvh.cn

[S32] C++：字符串
来源：http://brz.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://zwd.ppjwa.cn

[S33] C++：vector 增删
来源：http://hbj.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kem.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://xly.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://paa.xuanzx.com

[S35] C++：map
来源：http://nhi.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xzh.iojbl.cn

[S36] C++：unordered_map
来源：http://ncr.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yie.zhoulong.xyz

[S37] C++：set
来源：http://rux.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xlx.shanyushiyangkeji.top

[S38] C++：排序
来源：http://rxy.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://fef.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://axv.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ivn.sufxvd.cn

[S40] C++：查找元素
来源：http://brh.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jtm.aizwys.cn

[S41] C++：类与构造函数
来源：http://oby.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pnk.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://pfq.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://xbb.ppjwa.cn

[S43] C++：智能指针
来源：http://hul.yueranfly.top

auto p = std::make_unique<int>(5);
来源：http://hqz.zycfv.cn

[S44] C++：引用传参
来源：http://vus.birdmap.top

void inc(int &x) { ++x; }
来源：http://vyw.svipenyu.cn

[S45] C++：lambda
来源：http://xtb.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dij.hnxiangtu.top

[S46] C++：函数模板
来源：http://ueo.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://igw.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://hgn.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fhj.haohaochexian.top

[S48] C++：逐行读文件
来源：http://gox.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://xdo.fengsongda.top

while (std::getline(in, line)) { }
来源：http://vsy.sjlbkw.cn

[S49] C++：写文件
来源：http://rvr.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://byv.svipenyu.cn

[S50] C++：格式化数字
来源：http://wvh.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nis.ydzc1.top

[S51] C++：显式类型转换
来源：http://ptx.havefunace.top

static_cast<double>(a) / b
来源：http://tnt.cashguo.top

[S52] C++：const 与 noexcept
来源：http://izm.fzhhl.top

int size() const noexcept { return n_; }
来源：http://slb.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://hos.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://fea.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://uds.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rcv.yj20258.top

[S55] C++：结构化绑定
来源：http://lqr.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gpd.quarkkingdee.top

[S56] C++：optional
来源：http://xyp.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://org.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://aad.sxryk.cn

constexpr int N = 10;
来源：http://aqd.yuanzhike.top

[S58] C++：命名空间
来源：http://zjl.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://dyy.jinqigufen.top

[S59] C++：静态断言
来源：http://vnj.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hbv.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://wqz.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pjv.9152youxi.cn

================================================================================
来源：http://lmh.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dqz.aizwys.cn

================================================================================
来源：http://ycd.bjfxy.top

[T01] Kotlin：Hello World
来源：http://okf.ppjwa.cn

println("Hello")
来源：http://lab.yj20258.top

[T02] Kotlin：变量
来源：http://zkl.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zgp.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://xsw.zhixingplan.top

"值: $b"
来源：http://nxk.vehdjk.com

[T04] Kotlin：空安全
来源：http://tmi.hesvh.cn

val n: String? = null;  n?.length
来源：http://hph.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://acm.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dwd.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://xhk.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vxr.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://pvl.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wle.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://hkq.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://wdg.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://ncq.tanke756.top

fun String.exclaim() = this + "!"
来源：http://vyf.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://qxf.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uby.ehwqpu.com

[T11] Kotlin：协程
来源：http://tme.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kxp.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://gmk.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://mwd.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://rui.pycfn.com

val m = mapOf("a" to 1)
来源：http://art.dashuyun.cn

[T14] Kotlin：循环
来源：http://bar.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://ubv.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://hmz.fengsongda.top

interface Shape { fun area(): Double }
来源：http://ydp.andypj.xyz

[T16] Swift：Hello World
来源：http://giw.tarul.cn

print("Hello")
来源：http://glm.hesvh.cn

[T17] Swift：变量与常量
来源：http://nbc.havefunace.top

var a = 1;  let b = 2
来源：http://yjy.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://vvc.sweek.top

"值: \(b)"
来源：http://jvl.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://fui.andypj.xyz

if let n = opt { print(n) }
来源：http://zns.vehdjk.com

[T20] Swift：数组操作
来源：http://pup.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://pwz.zhijiandao.cn

[T21] Swift：遍历
来源：http://kxl.cqqwz.cn

for x in a { print(x) }
来源：http://upt.wangshuangyany.cn

[T22] Swift：字典
来源：http://yks.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xpg.wangdashe.top

[T23] Swift：函数
来源：http://ixe.tanke756.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zpm.gogol.net.cn

[T24] Swift：闭包
来源：http://wyk.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://azq.shangyingyoupin.top

[T25] Swift：结构体
来源：http://wom.aibaodan.cn

struct P { var x: Int }
来源：http://zpz.birdmap.top

[T26] Swift：类与重写
来源：http://tfv.guowangkeji.top

class A: Base { override func f() {} }
来源：http://bdp.shuidangran.top

[T27] Swift：错误处理
来源：http://cbs.yongpay.top

do { try f() } catch { print(error) }
来源：http://ost.yuanzhike.top

[T28] Swift：枚举
来源：http://ngl.gogol.net.cn

enum Color { case red, green }
来源：http://rzw.sweek.top

[T29] Swift：guard 提前返回
来源：http://qne.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://cap.jyoumei.cn

[T30] Swift：协议
来源：http://mba.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://btr.hysaishi.cn

[T31] Lua：Hello World
来源：http://kzy.hongshengwenyu.top

print("Hello")
来源：http://msv.haohaochexian.top

[T32] Lua：局部变量
来源：http://eby.daxiang520.top

local a = 1
来源：http://ztj.0kj1m.cn

[T33] Lua：表（数组）
来源：http://sds.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nfz.jinqigufen.top

[T34] Lua：遍历表
来源：http://uqy.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wdf.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://dgi.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://xoy.chenzaomai.com

[T36] Lua：函数
来源：http://jor.yuxming.cn

function add(a, b) return a + b end
来源：http://vad.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://fqz.daxiang520.top

"a" .. "b"
来源：http://xde.pycfn.com

[T38] Lua：条件
来源：http://txp.c1oappe.top

if x > 0 then print("正") end
来源：http://imx.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://dem.chenlongwang.top

string.find(s, "%d+")
来源：http://gno.jyoumei.cn

[T40] Lua：元表
来源：http://uwd.hcnkem.com

setmetatable({}, { __index = base })
来源：http://jup.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://lki.hywenlv.cn

print "Hello\n";
来源：http://emg.fehbvm.com

[T42] Perl：变量类型
来源：http://rfl.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mzr.cqqwz.cn

[T43] Perl：字符串插值
来源：http://ofj.sjlbkw.cn

"值: $a"
来源：http://bix.vqdsnc.cn

[T44] Perl：条件
来源：http://eqd.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://uso.ehwqpu.com

[T45] Perl：数组遍历
来源：http://efc.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://ioa.xinyue.icu

[T46] Perl：哈希操作
来源：http://pwg.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dor.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://xyg.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ncz.tianlin.xyz

[T48] Perl：正则替换
来源：http://tcp.shanyushiyangtech.top

$s =~ s/old/new/g;
来源：http://obg.xinyue.icu

[T49] Perl：函数
来源：http://sen.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xzs.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://bfl.316326.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://piv.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ove.jqgfzy.top

[T51] Scala：Hello World
来源：http://zmv.cheryme.top

println("Hello")
来源：http://tar.uphjek.com

[T52] Scala：变量
来源：http://add.aizwys.cn

val a = 1;  var b = 2
来源：http://cee.meibo888.top

[T53] Scala：字符串插值
来源：http://zmc.tarul.cn

s"值: $b"
来源：http://xga.zdbjq.cn

[T54] Scala：集合映射
来源：http://beh.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://bry.nwbrower.top

[T55] Scala：集合过滤
来源：http://wyg.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://kmd.aizwys.cn

[T56] Scala：样例类
来源：http://bqm.zdqjudy.top

case class User(name: String, age: Int)
来源：http://rxo.mhx1999.top

[T57] Scala：模式匹配
来源：http://bop.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lio.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://xef.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://vlz.nanxinkj.top

[T59] Scala：循环
来源：http://iyi.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://evk.chenlongwang.top

[T60] Scala：折叠
来源：http://zhv.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://asq.fehbvm.com

================================================================================
来源：http://hjt.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hfu.jinghuilouyu.cn

================================================================================
来源：http://mas.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://zao.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ryn.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://wlv.shanyushiyangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gkb.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://bkf.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://aqn.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://dnh.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gnf.epnwcf.com

[U05] Py：列表去重且保序
来源：http://kam.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://qat.ydjk.org.cn

[U06] Py：合并两个字典
来源：http://uqf.yongpay.top

{**a, **b}
来源：http://qgs.andypj.xyz

[U07] Py：反转字典键值
来源：http://ewt.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://fcy.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://xfj.dashuyun.cn

[y for x in nested for y in x]
来源：http://gnv.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://hnv.hesvh.cn

max(d, key=d.get)
来源：http://jyr.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://gbc.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pbc.chenzaomai.com

[U11] Py：生成器表达式
来源：http://tkq.jqgufenzy.top

(x * 2 for x in arr)
来源：http://cdg.andypj.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://cfc.nanxinkj.top

Counter(arr).most_common(3)
来源：http://bij.daxiang520.top

[U13] Py：固定长度队列
来源：http://afj.birdmap.top

deque(maxlen=10)
来源：http://zxc.sxryk.cn

[U14] Py：分组收集到列表
来源：http://wwk.chenjidiqi.icu

defaultdict(list)
来源：http://uyh.gzhubu.top

[U15] Py：高精度计时
来源：http://dkg.jqgfzy.top

t = time.perf_counter()
来源：http://hyu.xuanzx.com

[U16] Py：命令行参数解析
来源：http://tev.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://umz.gzhubu.top

[U17] Py：初始化日志
来源：http://xla.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://mle.xinyue.icu

[U18] Py：预编译正则
来源：http://nli.xuanzx.com

pat = re.compile(r"\d+")
来源：http://pau.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://ebl.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wnl.jlsjyb.cn

[U20] Py：缓存函数结果
来源：http://btm.xinyue.icu

@functools.lru_cache(maxsize=None)
来源：http://ois.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://ejx.ppjwa.cn

@contextlib.contextmanager
来源：http://bjt.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://dmq.mhx1999.top

list(zip(*m))
来源：http://neg.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://qoq.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://slb.hywenlv.cn

[U24] Py：路径操作
来源：http://soe.redwolf501.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nuo.cashguo.top

[U25] Py：CSV 按字典读
来源：http://wyq.hammf.cn

csv.DictReader(f)
来源：http://pzo.redwolf501.top

[U26] Py：并发下载
来源：http://bia.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ohs.bbcook.cn

[U27] Py：异步 HTTP
来源：http://fvg.hcnkem.com

aiohttp.ClientSession() 配合 async with
来源：http://neq.ppjwa.cn

[U28] Py：类型别名
来源：http://oqg.haohaochexian.top

UserId = int
来源：http://rzm.gzhubu.top

[U29] Py：属性校验
来源：http://ege.cucudq.cn

@property 与 @x.setter 配合
来源：http://uke.haohaochexian.top

[U30] Py：数据类
来源：http://eas.cashguo.top

@dataclass(slots=True)
来源：http://bba.xziqi.cn

[U31] Py：单测
来源：http://chj.jinyuanbaomall.cn

python -m pytest -q
来源：http://yiy.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://fkt.shzxlz.cn

ruff format . && ruff check --fix .
来源：http://qew.svipenyu.cn

[U33] Py：打包发布
来源：http://khc.gaohongyu789.top

python -m build  （依赖 pyproject.toml）
来源：http://hng.nanxinkj.top

[U34] Py：判断编码
来源：http://ytk.jiagoushi.top

chardet.detect(raw)
来源：http://azx.bbcook.cn


<!-- 参考信息 -->