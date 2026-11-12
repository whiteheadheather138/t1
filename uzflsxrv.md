代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bir.mhx1999.top

[S10] C：指针与解引用
来源：http://cis.hammf.cn

int *p = &a;  *p = 5;
来源：http://dqb.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://cky.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://mhn.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://det.xuanzx.com

fclose(f);
来源：http://exa.sufxvd.cn

[S12] C：写文件
来源：http://skd.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aok.feifeiyinyue.top

[S13] C：宏定义
来源：http://wsb.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcz.pycfn.com

[S14] C：枚举
来源：http://skv.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://mcq.nanxuanxn.top

[S15] C：类型转换
来源：http://adg.pengpengdd.cyou

(double) a / b
来源：http://rkf.aizwys.cn

[S16] C：位操作置位
来源：http://oqs.jinqigufen.top

x |= (1 << 3);
来源：http://ppr.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://ovl.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eex.zdbjq.cn

[S18] C：命令行参数
来源：http://xgk.gogol.net.cn

int main(int argc, char **argv)
来源：http://rre.shanyushiyangtech.top

[S19] C：快速排序
来源：http://bss.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xnz.aibaodan.cn

[S20] C：二分查找
来源：http://ggl.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tui.cashguo.top

[S21] C：字符类别判断
来源：http://kqp.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zaj.yongpay.top

[S22] C：字符串转数字
来源：http://gqj.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://lug.fengsongda.top

[S23] C：随机数
来源：http://rio.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://irk.ivvv.top

[S24] C：获取本地时间
来源：http://erh.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ble.nwbrower.top

[S25] C：内存拷贝
来源：http://rnt.zhoulong.xyz

memcpy(dst, src, n);
来源：http://dzq.zhongyouzk.top

[S26] C：内存清零
来源：http://lqe.guannengcc.top

memset(a, 0, sizeof a);
来源：http://kat.ivvv.top

[S27] C：定义常量
来源：http://lgr.havefunace.top

const double PI = 3.14159;
来源：http://mwe.52xcode.cn

[S28] C：静态变量
来源：http://yvz.zhijiandao.cn

static int counter = 0;
来源：http://ygu.shzxlz.cn

[S29] C：变参函数
来源：http://qql.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hmg.jqgfzy.top

[S30] C：头文件保护
来源：http://gpt.0kj1m.cn

#ifndef X_H
来源：http://cao.epnwcf.com

#define X_H
来源：http://moz.yfazqb.com

#endif
来源：http://sxj.snrcjt.cn

[S31] C++：Hello World
来源：http://zer.jiagoushi.top

#include <iostream>
来源：http://uqq.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ojj.ctjpmb.com

[S32] C++：字符串
来源：http://opl.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://wbo.fengsongda.top

[S33] C++：vector 增删
来源：http://wtc.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xcc.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://jln.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://pwd.ppjwa.cn

[S35] C++：map
来源：http://wwm.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sna.vqdsnc.cn

[S36] C++：unordered_map
来源：http://lwg.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://haq.cucudq.cn

[S37] C++：set
来源：http://vbs.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bbg.sjlbkw.cn

[S38] C++：排序
来源：http://ujd.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://gmv.jinyuanbaomall.cn

[S39] C++：自定义比较器排序
来源：http://ino.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qgj.hcnkem.com

[S40] C++：查找元素
来源：http://mmz.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yar.dianchejie.cn

[S41] C++：类与构造函数
来源：http://mes.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hkz.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://gup.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://gga.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://oux.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://vlk.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://ydu.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://hvl.snrcjt.cn

[S45] C++：lambda
来源：http://sfn.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://bid.yangfankeji.com

[S46] C++：函数模板
来源：http://jtm.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kjy.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://yjc.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mmd.9152youxi.cn

[S48] C++：逐行读文件
来源：http://ygw.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://bcg.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://usa.haohaochexian.top

[S49] C++：写文件
来源：http://ujn.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljc.hnxiangtu.top

[S50] C++：格式化数字
来源：http://uoe.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hjr.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://gfv.fzhhl.top

static_cast<double>(a) / b
来源：http://bed.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://nnf.wangdashe.top

int size() const noexcept { return n_; }
来源：http://xin.cashguo.top

[S53] C++：移动语义
来源：http://rpt.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://eps.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://ten.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ljo.fengsongda.top

[S55] C++：结构化绑定
来源：http://stb.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hrd.jinyuanbaomall.cn

[S56] C++：optional
来源：http://ufg.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jhj.aizwys.cn

[S57] C++：编译期常量
来源：http://ahl.ppjwa.cn

constexpr int N = 10;
来源：http://zxp.wangdashe.top

[S58] C++：命名空间
来源：http://qdi.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://ybn.c1oappe.top

[S59] C++：静态断言
来源：http://uaq.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://etz.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://pqz.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bwh.xylfe.cn

================================================================================
来源：http://wbz.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sko.epnwcf.com

================================================================================
来源：http://tjs.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://dfk.hysaishi.cn

println("Hello")
来源：http://nbh.9152youxi.cn

[T02] Kotlin：变量
来源：http://tzg.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hsm.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://ids.gzhubu.top

"值: $b"
来源：http://pxd.fengsongda.top

[T04] Kotlin：空安全
来源：http://nbu.pycfn.com

val n: String? = null;  n?.length
来源：http://moi.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://bgo.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://puz.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://zok.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://srj.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://nuh.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://acv.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://pqx.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://ztl.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://dpa.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://xqz.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://eia.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://avs.snrcjt.cn

[T11] Kotlin：协程
来源：http://ckh.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jzf.yfazqb.com

[T12] Kotlin：解构声明
来源：http://dwb.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://lzv.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://btx.shuidangran.top

val m = mapOf("a" to 1)
来源：http://uqk.fktsv.cn

[T14] Kotlin：循环
来源：http://plg.cheryme.top

for (i in 1..10) println(i)
来源：http://cvx.zhixingplan.top

[T15] Kotlin：接口
来源：http://kwc.vehdjk.com

interface Shape { fun area(): Double }
来源：http://qzw.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://boc.daria6918.cn

print("Hello")
来源：http://cqu.hnqzz.top

[T17] Swift：变量与常量
来源：http://jmq.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://mpx.smart0.xyz

[T18] Swift：字符串插值
来源：http://uxo.shanyushiyangkeji.top

"值: \(b)"
来源：http://qbl.bbcook.cn

[T19] Swift：可选绑定
来源：http://lye.fzhhl.top

if let n = opt { print(n) }
来源：http://udi.316326.xyz

[T20] Swift：数组操作
来源：http://uek.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://jva.haohaochexian.top

[T21] Swift：遍历
来源：http://hsf.hammf.cn

for x in a { print(x) }
来源：http://pci.tanke756.top

[T22] Swift：字典
来源：http://ohh.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://nyn.hnqzz.top

[T23] Swift：函数
来源：http://hhr.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogd.ctjpmb.com

[T24] Swift：闭包
来源：http://zml.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bii.xuanzx.com

[T25] Swift：结构体
来源：http://eyn.cucudq.cn

struct P { var x: Int }
来源：http://yap.gotoacloud.top

[T26] Swift：类与重写
来源：http://yzf.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://pvs.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://pwo.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://fmx.feifeiyinyue.top

[T28] Swift：枚举
来源：http://jee.hfpthk.cn

enum Color { case red, green }
来源：http://cvn.havefunace.top

[T29] Swift：guard 提前返回
来源：http://adn.tianlin.xyz

guard let x = opt else { return }
来源：http://jwg.hfpthk.cn

[T30] Swift：协议
来源：http://xft.havefunace.top

protocol Shape { func area() -> Double }
来源：http://pde.jqgufenzy.top

[T31] Lua：Hello World
来源：http://jzc.hongshengwenyu.top

print("Hello")
来源：http://keo.meibo888.top

[T32] Lua：局部变量
来源：http://ehh.tianlin.xyz

local a = 1
来源：http://tkz.haohaochexian.top

[T33] Lua：表（数组）
来源：http://vfn.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mvc.chenlongwang.top

[T34] Lua：遍历表
来源：http://zdx.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aie.yj20258.top

[T35] Lua：字典表
来源：http://lia.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://tkb.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://gwv.316326.xyz

function add(a, b) return a + b end
来源：http://mft.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://aoo.wangdashe.top

"a" .. "b"
来源：http://edr.ydzc1.top

[T38] Lua：条件
来源：http://bqp.nanxuanxn.top

if x > 0 then print("正") end
来源：http://zup.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://hpa.nwbrower.top

string.find(s, "%d+")
来源：http://gqf.daria6918.cn

[T40] Lua：元表
来源：http://pad.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://tlv.sufxvd.cn

[T41] Perl：Hello World
来源：http://ydm.yongpay.top

print "Hello\n";
来源：http://vjd.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://wcd.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mmg.iojbl.cn

[T43] Perl：字符串插值
来源：http://rmx.haohaochexian.top

"值: $a"
来源：http://zku.andypj.xyz

[T44] Perl：条件
来源：http://lro.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://ytp.bjfxy.top

[T45] Perl：数组遍历
来源：http://eqy.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://gyn.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://vll.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wzo.quarkkingdee.top

[T47] Perl：正则捕获
来源：http://tke.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://whb.jqgufenzy.top

[T48] Perl：正则替换
来源：http://frz.sysykeji.top

$s =~ s/old/new/g;
来源：http://wdq.zhaomingkeji.xyz

[T49] Perl：函数
来源：http://sxc.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zvh.uphjek.com

[T50] Perl：逐行读文件
来源：http://dbm.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ofc.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://nct.ywan-chungtsiang.top

[T51] Scala：Hello World
来源：http://eed.shanyushiyangkeji.top

println("Hello")
来源：http://dxr.zhiwuduotai.top

[T52] Scala：变量
来源：http://zoa.ydjk.org.cn

val a = 1;  var b = 2
来源：http://cij.zhijiandao.cn

[T53] Scala：字符串插值
来源：http://kfg.hysaishi.cn

s"值: $b"
来源：http://viu.zhongyouzk.top

[T54] Scala：集合映射
来源：http://dns.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://hju.hammf.cn

[T55] Scala：集合过滤
来源：http://vka.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://acc.gaohongyu789.top

[T56] Scala：样例类
来源：http://vfd.daria6918.cn

case class User(name: String, age: Int)
来源：http://pik.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://azo.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://laz.shanyushiyangkeji.top

[T58] Scala：函数定义
来源：http://csg.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://clb.guannengcc.top

[T59] Scala：循环
来源：http://biw.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://arm.jqgufenzy.top

[T60] Scala：折叠
来源：http://ysw.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvc.andypj.xyz

================================================================================
来源：http://xdv.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ztd.vqdsnc.cn

================================================================================
来源：http://sno.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://czn.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://xrg.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://ndv.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rig.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://vli.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kzc.aibaodan.cn

[U04] Py：变量调试打印
来源：http://sdx.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trp.daria6918.cn

[U05] Py：列表去重且保序
来源：http://dat.andypj.xyz

list(dict.fromkeys(arr))
来源：http://sdf.nanxinkj.top

[U06] Py：合并两个字典
来源：http://plg.uphjek.com

{**a, **b}
来源：http://zbz.fktsv.cn

[U07] Py：反转字典键值
来源：http://uyn.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://oqt.guowangkeji.top

[U08] Py：展平二维列表
来源：http://agg.yj20258.top

[y for x in nested for y in x]
来源：http://mpg.tarul.cn

[U09] Py：字典取最大值的键
来源：http://bml.gzhubu.top

max(d, key=d.get)
来源：http://fku.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://klh.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hbh.wangdashe.top

[U11] Py：生成器表达式
来源：http://agv.xinyue.icu

(x * 2 for x in arr)
来源：http://pdi.yonumen.top

[U12] Py：取出现最多的 3 个元素
来源：http://bpr.bjfxy.top

Counter(arr).most_common(3)
来源：http://ctr.hfpthk.cn

[U13] Py：固定长度队列
来源：http://ntq.xinyue.icu

deque(maxlen=10)
来源：http://nfp.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://loe.0kj1m.cn

defaultdict(list)
来源：http://jus.nwbrower.top

[U15] Py：高精度计时
来源：http://zpu.xuetiantiany.cn

t = time.perf_counter()
来源：http://elu.tian-w.cn

[U16] Py：命令行参数解析
来源：http://ikx.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mek.hfpthk.cn

[U17] Py：初始化日志
来源：http://qib.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://rro.yueranfly.top

[U18] Py：预编译正则
来源：http://qwy.andypj.xyz

pat = re.compile(r"\d+")
来源：http://wsl.tarul.cn

[U19] Py：正则替换带回调
来源：http://tcm.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dqw.c1oappe.top

[U20] Py：缓存函数结果
来源：http://ufa.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://jyv.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://cvj.jiagoushi.top

@contextlib.contextmanager
来源：http://hyo.ehwqpu.com

[U22] Py：矩阵转置
来源：http://kda.aizwys.cn

list(zip(*m))
来源：http://feo.daria6918.cn

[U23] Py：分块读取大文件
来源：http://ami.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aei.ehwqpu.com

[U24] Py：路径操作
来源：http://rhu.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://keb.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://ugv.chenlongwang.top

csv.DictReader(f)
来源：http://pwh.zycfv.cn

[U26] Py：并发下载
来源：http://cjh.316326.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qwv.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://atj.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://jtf.kuanghao11.cn

[U28] Py：类型别名
来源：http://app.uphjek.com

UserId = int
来源：http://isk.ctjpmb.com

[U29] Py：属性校验
来源：http://xbs.nanxinkj.top

@property 与 @x.setter 配合
来源：http://sqr.aibaodan.cn

[U30] Py：数据类
来源：http://uye.ctjpmb.com

@dataclass(slots=True)
来源：http://ymj.kuanghao11.cn

[U31] Py：单测
来源：http://aqp.guannengcc.top

python -m pytest -q
来源：http://ekb.hnxiangtu.top

[U32] Py：代码格式化
来源：http://ugj.xylfe.cn

ruff format . && ruff check --fix .
来源：http://cxy.daria6918.cn


<!-- 参考信息 -->