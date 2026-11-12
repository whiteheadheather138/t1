代发 wailian999

strlen(s)
来源：http://hun.zhijiandao.cn

[S06] C：字符串比较
来源：http://hhm.zdqjudy.top

strcmp(a, b) == 0
来源：http://iaj.52xcode.cn

[S07] C：数组遍历求和
来源：http://eeq.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jow.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://ltg.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qtu.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://bzz.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ihy.andypj.xyz

[S10] C：指针与解引用
来源：http://bpg.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://agg.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://cvz.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://shb.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vix.316326.xyz

fclose(f);
来源：http://dok.pycfn.com

[S12] C：写文件
来源：http://tyu.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ejt.svipenyu.cn

[S13] C：宏定义
来源：http://udk.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hoc.fengsongda.top

[S14] C：枚举
来源：http://lfe.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://mso.yj20258888.top

[S15] C：类型转换
来源：http://gym.hnqzz.top

(double) a / b
来源：http://yju.ctjpmb.com

[S16] C：位操作置位
来源：http://nwi.316326.xyz

x |= (1 << 3);
来源：http://fsk.fktsv.cn

[S17] C：安全拼接字符串
来源：http://gzr.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ahz.gogol.net.cn

[S18] C：命令行参数
来源：http://fgk.daxiang520.top

int main(int argc, char **argv)
来源：http://lxv.shzxlz.cn

[S19] C：快速排序
来源：http://ukd.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dij.xuanzx.com

[S20] C：二分查找
来源：http://hrw.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://brk.daxiang520.top

[S21] C：字符类别判断
来源：http://mre.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mrn.aizwys.cn

[S22] C：字符串转数字
来源：http://dlb.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kfh.ybcxt.top

[S23] C：随机数
来源：http://esn.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tar.tanke756.top

[S24] C：获取本地时间
来源：http://yjs.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwp.yueranfly.top

[S25] C：内存拷贝
来源：http://mbn.yueranfly.top

memcpy(dst, src, n);
来源：http://uwv.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://jyo.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://oow.shzxlz.cn

[S27] C：定义常量
来源：http://jej.nanxuanxn.top

const double PI = 3.14159;
来源：http://nlp.zdqjudy.top

[S28] C：静态变量
来源：http://hql.yuxming.cn

static int counter = 0;
来源：http://why.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://igg.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uas.jyoumei.cn

[S30] C：头文件保护
来源：http://qaq.shuidangran.top

#ifndef X_H
来源：http://cbv.xinyue.icu

#define X_H
来源：http://vmr.hfpthk.cn

#endif
来源：http://xke.hnqzz.top

[S31] C++：Hello World
来源：http://fcx.haohaochexian.top

#include <iostream>
来源：http://tsj.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://ulc.redwolf501.top

[S32] C++：字符串
来源：http://hmm.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://hdd.sjlbkw.cn

[S33] C++：vector 增删
来源：http://ypb.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rgj.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://zin.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://oyy.shanyushiyangtech.top

[S35] C++：map
来源：http://vbp.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://abt.hywenlv.cn

[S36] C++：unordered_map
来源：http://uaj.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kqq.gogol.net.cn

[S37] C++：set
来源：http://kmv.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gsv.aibaodan.cn

[S38] C++：排序
来源：http://qbx.meibo888.top

std::sort(v.begin(), v.end());
来源：http://qiy.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://pcf.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pbe.hesvh.cn

[S40] C++：查找元素
来源：http://epu.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://swy.9152youxi.cn

[S41] C++：类与构造函数
来源：http://zmq.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nbz.yj202588.top

[S42] C++：继承与虚函数
来源：http://gpc.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://phd.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ydu.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://sny.kuanghao11.cn

[S44] C++：引用传参
来源：http://vjn.jianghu66.top

void inc(int &x) { ++x; }
来源：http://lcf.feifeiyinyue.top

[S45] C++：lambda
来源：http://hhz.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://pbw.cdnleiting.top

[S46] C++：函数模板
来源：http://sif.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bsz.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://arw.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://afb.cucudq.cn

[S48] C++：逐行读文件
来源：http://xel.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://pwk.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://but.shanyushiyangtech.top

[S49] C++：写文件
来源：http://moj.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ejv.fzhhl.top

[S50] C++：格式化数字
来源：http://euu.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tof.xziqi.cn

[S51] C++：显式类型转换
来源：http://wdp.birdmap.top

static_cast<double>(a) / b
来源：http://axt.yonumen.top

[S52] C++：const 与 noexcept
来源：http://dyy.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://nll.xziqi.cn

[S53] C++：移动语义
来源：http://jfs.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://xhw.jinqigufen.top

[S54] C++：异常处理
来源：http://jxq.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eeb.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://otg.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qwe.wangdashe.top

[S56] C++：optional
来源：http://dio.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crm.yanxiufei.cn

[S57] C++：编译期常量
来源：http://nmk.hnxiangtu.top

constexpr int N = 10;
来源：http://jkc.hongshengwenyu.top

[S58] C++：命名空间
来源：http://myg.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://tdm.chenjidiqi.icu

[S59] C++：静态断言
来源：http://qgm.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgc.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://vuz.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://guw.smart0.xyz

================================================================================
来源：http://efy.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uis.9152youxi.cn

================================================================================
来源：http://xvd.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://mes.gzhubu.top

println("Hello")
来源：http://jqz.hammf.cn

[T02] Kotlin：变量
来源：http://oqv.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vrr.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://ike.9152youxi.cn

"值: $b"
来源：http://sju.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://bku.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://gfb.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://paa.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bwm.yonumen.top

[T06] Kotlin：集合映射
来源：http://typ.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lwt.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://phe.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xib.hnqzz.top

[T08] Kotlin：数据类
来源：http://xkt.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://ogh.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://wzp.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://lyi.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://eec.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uzp.nanxuanxn.top

[T11] Kotlin：协程
来源：http://haz.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://jer.ybcxt.top

[T12] Kotlin：解构声明
来源：http://gou.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://dma.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://vfy.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://otc.jinqigfzy.top

[T14] Kotlin：循环
来源：http://mhc.yfazqb.com

for (i in 1..10) println(i)
来源：http://efx.yvedp.cn

[T15] Kotlin：接口
来源：http://ucb.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://ngz.haohaochexian.top

[T16] Swift：Hello World
来源：http://pzq.hysaishi.cn

print("Hello")
来源：http://llj.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://kmk.yj20258888.top

var a = 1;  let b = 2
来源：http://rcu.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://shp.aibaodan.cn

"值: \(b)"
来源：http://jfd.ctjpmb.com

[T19] Swift：可选绑定
来源：http://wli.yj20258.top

if let n = opt { print(n) }
来源：http://whx.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://sdk.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mot.xinyue.icu

[T21] Swift：遍历
来源：http://xwg.cqqwz.cn

for x in a { print(x) }
来源：http://apr.snrcjt.cn

[T22] Swift：字典
来源：http://xus.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://vva.fanxiaobao.xyz

[T23] Swift：函数
来源：http://pml.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uvz.jlsjyb.cn

[T24] Swift：闭包
来源：http://omt.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jqs.hfpthk.cn

[T25] Swift：结构体
来源：http://yvc.ppjwa.cn

struct P { var x: Int }
来源：http://fry.guowangkeji.top

[T26] Swift：类与重写
来源：http://amz.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://bih.shzxlz.cn

[T27] Swift：错误处理
来源：http://nnz.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://vgd.redwolf501.top

[T28] Swift：枚举
来源：http://dpa.epnwcf.com

enum Color { case red, green }
来源：http://wcg.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://grt.tian-w.cn

guard let x = opt else { return }
来源：http://ggd.hnxiangtu.top

[T30] Swift：协议
来源：http://wor.cashguo.top

protocol Shape { func area() -> Double }
来源：http://hnn.shuidangran.top

[T31] Lua：Hello World
来源：http://vnz.hnqzz.top

print("Hello")
来源：http://fnl.ppjwa.cn

[T32] Lua：局部变量
来源：http://duw.zhaomingkeji.xyz

local a = 1
来源：http://uag.nanxinkj.top

[T33] Lua：表（数组）
来源：http://poj.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://skn.yangfankeji.com

[T34] Lua：遍历表
来源：http://oju.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hee.yuxming.cn

[T35] Lua：字典表
来源：http://roi.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://zle.pengpengdd.cyou

[T36] Lua：函数
来源：http://phu.zdqjudy.top

function add(a, b) return a + b end
来源：http://gjo.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://ckh.snrcjt.cn

"a" .. "b"
来源：http://mpx.jinqigufen.top

[T38] Lua：条件
来源：http://nmg.ydzc1.top

if x > 0 then print("正") end
来源：http://gcz.jyoumei.cn

[T39] Lua：模式匹配
来源：http://zen.vqdsnc.cn

string.find(s, "%d+")
来源：http://lgt.cdnleiting.top

[T40] Lua：元表
来源：http://ecv.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://pzc.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://mzj.aibaodan.cn

print "Hello\n";
来源：http://eiq.shangyingyoupin.top

[T42] Perl：变量类型
来源：http://bqo.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fiz.tianlin.xyz

[T43] Perl：字符串插值
来源：http://brx.vehdjk.com

"值: $a"
来源：http://gdl.yangfankeji.com

[T44] Perl：条件
来源：http://kyx.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://cly.jqgfzy.top

[T45] Perl：数组遍历
来源：http://qtp.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://gew.tian-w.cn

[T46] Perl：哈希操作
来源：http://opk.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sav.aibaodan.cn

[T47] Perl：正则捕获
来源：http://fnm.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sjt.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://qyh.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://ree.dashuyun.cn

[T49] Perl：函数
来源：http://brz.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xsg.mhx1999.top

[T50] Perl：逐行读文件
来源：http://lfx.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ead.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://jlu.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://ioi.iojbl.cn

println("Hello")
来源：http://zns.fzhhl.top

[T52] Scala：变量
来源：http://vjo.shzxlz.cn

val a = 1;  var b = 2
来源：http://ucm.jyoumei.cn

[T53] Scala：字符串插值
来源：http://ngg.yanxiufei.cn

s"值: $b"
来源：http://npr.jinqigufen.top

[T54] Scala：集合映射
来源：http://hjp.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://fzk.52xcode.cn

[T55] Scala：集合过滤
来源：http://vsy.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://bkx.ppjwa.cn

[T56] Scala：样例类
来源：http://qkq.jyoumei.cn

case class User(name: String, age: Int)
来源：http://zek.ppjwa.cn

[T57] Scala：模式匹配
来源：http://kjf.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tou.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://ivb.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://pcx.dianchejie.cn

[T59] Scala：循环
来源：http://upu.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://uqm.xuanzx.com

[T60] Scala：折叠
来源：http://ybi.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://inn.fehbvm.com

================================================================================
来源：http://qvx.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aup.fanxiaobao.xyz

================================================================================
来源：http://tlk.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://ibf.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://lox.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://rwh.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rzu.yanxiufei.cn

[U03] Py：加载 .env 配置
来源：http://pxe.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://nvi.nanxinkj.top

[U04] Py：变量调试打印
来源：http://hss.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jyc.guannengcc.top

[U05] Py：列表去重且保序
来源：http://pzx.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://ivr.hammf.cn

[U06] Py：合并两个字典
来源：http://fyt.hcnkem.com

{**a, **b}
来源：http://bbh.haohaochexian.top

[U07] Py：反转字典键值
来源：http://aar.yj20258.top

{v: k for k, v in d.items()}
来源：http://wgk.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://jnv.havefunace.top

[y for x in nested for y in x]
来源：http://gjz.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://mue.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://xlb.zhaomingkeji.xyz

[U10] Py：按值排序字典
来源：http://uix.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sfk.cucudq.cn

[U11] Py：生成器表达式
来源：http://uuz.jianghu66.top

(x * 2 for x in arr)
来源：http://qmv.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://hud.daria6918.cn

Counter(arr).most_common(3)
来源：http://bvl.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://sby.yj202588.top

deque(maxlen=10)
来源：http://mop.hysaishi.cn

[U14] Py：分组收集到列表
来源：http://doo.vehdjk.com

defaultdict(list)
来源：http://osj.guowangkeji.top

[U15] Py：高精度计时
来源：http://jyz.hywenlv.cn

t = time.perf_counter()
来源：http://wfw.zhixingplan.top

[U16] Py：命令行参数解析
来源：http://wzb.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://axj.wangshuangyany.cn

[U17] Py：初始化日志
来源：http://hmt.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://ppx.hysaishi.cn

[U18] Py：预编译正则
来源：http://syv.jianghu66.top

pat = re.compile(r"\d+")
来源：http://tcp.yuxming.cn

[U19] Py：正则替换带回调
来源：http://vut.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xfi.shuidangran.top

[U20] Py：缓存函数结果
来源：http://ekm.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://ypz.daria6918.cn

[U21] Py：自定义上下文管理器
来源：http://hzq.cheryme.top

@contextlib.contextmanager
来源：http://klj.bbcook.cn

[U22] Py：矩阵转置
来源：http://vyx.zdbjq.cn

list(zip(*m))
来源：http://poe.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://fjo.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tbl.hongshengwenyu.top

[U24] Py：路径操作
来源：http://zfh.feifeiyinyue.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://neb.fzhhl.top

[U25] Py：CSV 按字典读
来源：http://mtj.daria6918.cn

csv.DictReader(f)
来源：http://uva.nanxuanxn.top

[U26] Py：并发下载
来源：http://dja.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://adf.yongpay.top

[U27] Py：异步 HTTP
来源：http://yvo.meibo888.top

aiohttp.ClientSession() 配合 async with
来源：http://xyr.ydjk.org.cn

[U28] Py：类型别名
来源：http://zhb.birdmap.top

UserId = int
来源：http://sje.yangfankeji.com


<!-- 参考信息 -->