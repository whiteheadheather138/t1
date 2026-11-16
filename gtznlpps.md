代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://whg.epnwcf.com

[S10] C：指针与解引用
来源：http://yih.yueranfly.top

int *p = &a;  *p = 5;
来源：http://dpb.316326.xyz

[S11] C：逐行读文件
来源：http://vvh.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://rjk.tian-w.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fva.epnwcf.com

fclose(f);
来源：http://nuk.shzxlz.cn

[S12] C：写文件
来源：http://dae.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hoz.nwbrower.top

[S13] C：宏定义
来源：http://szn.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tmr.iojbl.cn

[S14] C：枚举
来源：http://lin.pengpengdd.cyou

enum Color { RED, GREEN, BLUE };
来源：http://cxa.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://nlm.xziqi.cn

(double) a / b
来源：http://tfj.yuxming.cn

[S16] C：位操作置位
来源：http://pum.zhixingplan.top

x |= (1 << 3);
来源：http://ipr.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://ocq.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://boz.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://tzs.jiagoushi.top

int main(int argc, char **argv)
来源：http://wrj.zhiwuduotai.top

[S19] C：快速排序
来源：http://nle.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iwv.kuanghao11.cn

[S20] C：二分查找
来源：http://sjl.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://osl.hesvh.cn

[S21] C：字符类别判断
来源：http://pix.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cqp.dashuyun.cn

[S22] C：字符串转数字
来源：http://fxb.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://vhl.tanke756.top

[S23] C：随机数
来源：http://nfp.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yvm.ydzc1.top

[S24] C：获取本地时间
来源：http://glz.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbj.yangfankeji.com

[S25] C：内存拷贝
来源：http://nap.yj20258.top

memcpy(dst, src, n);
来源：http://ddo.ybcxt.top

[S26] C：内存清零
来源：http://tcf.316326.xyz

memset(a, 0, sizeof a);
来源：http://vlm.yj202588.top

[S27] C：定义常量
来源：http://opt.jiagoushi.top

const double PI = 3.14159;
来源：http://qip.xuanzx.com

[S28] C：静态变量
来源：http://alw.bbcook.cn

static int counter = 0;
来源：http://wgl.havefunace.top

[S29] C：变参函数
来源：http://hes.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ygt.shuidangran.top

[S30] C：头文件保护
来源：http://fux.shangyingyoupin.top

#ifndef X_H
来源：http://juz.jinghuilouyu.cn

#define X_H
来源：http://xhv.wangdashe.top

#endif
来源：http://qnv.kuanghao11.cn

[S31] C++：Hello World
来源：http://hrd.hnxiangtu.top

#include <iostream>
来源：http://kqb.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://uww.nanxinkj.top

[S32] C++：字符串
来源：http://egl.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://miy.sxryk.cn

[S33] C++：vector 增删
来源：http://bfb.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hex.xylfe.cn

[S34] C++：遍历 vector
来源：http://epo.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://unl.hcnkem.com

[S35] C++：map
来源：http://ysi.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ekz.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://vxo.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eij.sweek.top

[S37] C++：set
来源：http://zou.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yyz.vqdsnc.cn

[S38] C++：排序
来源：http://qxi.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://hfg.birdmap.top

[S39] C++：自定义比较器排序
来源：http://gll.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kxg.cashguo.top

[S40] C++：查找元素
来源：http://djl.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qmy.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://aac.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://woy.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://qza.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://gyo.xylfe.cn

[S43] C++：智能指针
来源：http://ert.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://yls.zhiwuduotai.top

[S44] C++：引用传参
来源：http://hqd.yuxming.cn

void inc(int &x) { ++x; }
来源：http://lgj.jqgfzy.top

[S45] C++：lambda
来源：http://zsd.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://xqd.chenlongwang.top

[S46] C++：函数模板
来源：http://wts.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xby.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://uup.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lsa.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://efn.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://npx.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://rrt.yonumen.top

[S49] C++：写文件
来源：http://mgu.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pgt.hesvh.cn

[S50] C++：格式化数字
来源：http://vui.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hai.hcnkem.com

[S51] C++：显式类型转换
来源：http://zvu.jiagoushi.top

static_cast<double>(a) / b
来源：http://ifz.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://msa.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://stm.snrcjt.cn

[S53] C++：移动语义
来源：http://moq.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://wak.ctjpmb.com

[S54] C++：异常处理
来源：http://igk.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fie.hcnkem.com

[S55] C++：结构化绑定
来源：http://tty.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lev.meibo888.top

[S56] C++：optional
来源：http://kjb.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oyw.fengsongda.top

[S57] C++：编译期常量
来源：http://voz.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://axv.yfazqb.com

[S58] C++：命名空间
来源：http://aab.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://muw.yanxiufei.cn

[S59] C++：静态断言
来源：http://wce.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://muf.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://idd.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://llb.ybcxt.top

================================================================================
来源：http://ynz.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pql.zhoulong.xyz

================================================================================
来源：http://yyp.yj20258888.top

[T01] Kotlin：Hello World
来源：http://sma.fehbvm.com

println("Hello")
来源：http://ueb.guowangkeji.top

[T02] Kotlin：变量
来源：http://zns.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ybt.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://rrx.yj20258888.top

"值: $b"
来源：http://dkt.aibaodan.cn

[T04] Kotlin：空安全
来源：http://ltb.chenlongwang.top

val n: String? = null;  n?.length
来源：http://ivw.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://wvw.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ihk.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://tyk.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eyb.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://wlr.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ciz.sysykeji.top

[T08] Kotlin：数据类
来源：http://lqf.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://myu.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://xsb.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://cri.hnqzz.top

[T10] Kotlin：默认参数
来源：http://esk.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lhq.zdqjudy.top

[T11] Kotlin：协程
来源：http://dku.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vcb.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://bgp.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://tbw.hammf.cn

[T13] Kotlin：只读 Map
来源：http://hpd.zycfv.cn

val m = mapOf("a" to 1)
来源：http://dvk.tarul.cn

[T14] Kotlin：循环
来源：http://grw.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://ivn.chenlongwang.top

[T15] Kotlin：接口
来源：http://cnt.ybcxt.top

interface Shape { fun area(): Double }
来源：http://ecy.jiagoushi.top

[T16] Swift：Hello World
来源：http://gil.jqgufenzy.top

print("Hello")
来源：http://zod.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://htl.haohaochexian.top

var a = 1;  let b = 2
来源：http://mvs.wangdashe.top

[T18] Swift：字符串插值
来源：http://nod.hysaishi.cn

"值: \(b)"
来源：http://ygx.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://ilt.pycfn.com

if let n = opt { print(n) }
来源：http://wth.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://tmk.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wol.jqgufenzy.top

[T21] Swift：遍历
来源：http://avq.zhoulong.xyz

for x in a { print(x) }
来源：http://git.jqgfzy.top

[T22] Swift：字典
来源：http://dvg.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xbt.tarul.cn

[T23] Swift：函数
来源：http://frw.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nds.sjlbkw.cn

[T24] Swift：闭包
来源：http://nkx.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jbb.chenjidiqi.icu

[T25] Swift：结构体
来源：http://mgy.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://sgt.yj202588.top

[T26] Swift：类与重写
来源：http://jyc.jinqigufen.top

class A: Base { override func f() {} }
来源：http://swn.zdqjudy.top

[T27] Swift：错误处理
来源：http://wdv.ybcxt.top

do { try f() } catch { print(error) }
来源：http://jlj.vqdsnc.cn

[T28] Swift：枚举
来源：http://wgi.jinqigufen.top

enum Color { case red, green }
来源：http://mrz.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://zhm.zhengqikj.top

guard let x = opt else { return }
来源：http://gry.nwbrower.top

[T30] Swift：协议
来源：http://vqs.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://brq.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://pcu.zdbjq.cn

print("Hello")
来源：http://atp.9152youxi.cn

[T32] Lua：局部变量
来源：http://iec.zhiwuduotai.top

local a = 1
来源：http://myl.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://trw.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mka.xuanzx.com

[T34] Lua：遍历表
来源：http://vck.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ajn.wangdashe.top

[T35] Lua：字典表
来源：http://ztq.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://oih.birdmap.top

[T36] Lua：函数
来源：http://ibv.xziqi.cn

function add(a, b) return a + b end
来源：http://zms.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://bss.birdmap.top

"a" .. "b"
来源：http://kmm.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://rjg.wangdashe.top

if x > 0 then print("正") end
来源：http://uel.yuxming.cn

[T39] Lua：模式匹配
来源：http://orc.epnwcf.com

string.find(s, "%d+")
来源：http://dgm.52xcode.cn

[T40] Lua：元表
来源：http://zms.yj20258888.top

setmetatable({}, { __index = base })
来源：http://ien.chenlongwang.top

[T41] Perl：Hello World
来源：http://htg.iojbl.cn

print "Hello\n";
来源：http://rxz.pycfn.com

[T42] Perl：变量类型
来源：http://ijf.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rxu.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://boz.haohaochexian.top

"值: $a"
来源：http://pcq.nanxinkj.top

[T44] Perl：条件
来源：http://wiq.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://dnc.redwolf501.top

[T45] Perl：数组遍历
来源：http://res.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://bsr.jinqigufen.top

[T46] Perl：哈希操作
来源：http://llu.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://avv.vehdjk.com

[T47] Perl：正则捕获
来源：http://dir.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://csi.tian-w.cn

[T48] Perl：正则替换
来源：http://nex.fzhhl.top

$s =~ s/old/new/g;
来源：http://tgo.zhengqikj.top

[T49] Perl：函数
来源：http://kaa.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vfc.cashguo.top

[T50] Perl：逐行读文件
来源：http://zci.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hzj.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://fjt.aibaodan.cn

[T51] Scala：Hello World
来源：http://web.jinqigufen.top

println("Hello")
来源：http://lwf.jinqigufen.top

[T52] Scala：变量
来源：http://ets.9152youxi.cn

val a = 1;  var b = 2
来源：http://una.daxiang520.top

[T53] Scala：字符串插值
来源：http://ehp.nanxinkj.top

s"值: $b"
来源：http://hpe.zdqjudy.top

[T54] Scala：集合映射
来源：http://azq.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://eyu.jqgfzy.top

[T55] Scala：集合过滤
来源：http://hwc.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://onb.cheryme.top

[T56] Scala：样例类
来源：http://rar.nanxinkj.top

case class User(name: String, age: Int)
来源：http://luv.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://rrx.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rnh.c1oappe.top

[T58] Scala：函数定义
来源：http://mlf.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://edc.shzxlz.cn

[T59] Scala：循环
来源：http://nfz.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://bhc.yvedp.cn

[T60] Scala：折叠
来源：http://cuw.jqgfzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vfa.pengpengdd.cyou

================================================================================
来源：http://pxg.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jrt.jianghu66.top

================================================================================
来源：http://wew.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://rth.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://zny.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://whm.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ifi.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://zvv.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://pce.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://vir.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dqd.vehdjk.com

[U05] Py：列表去重且保序
来源：http://vba.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://spc.nanxinkj.top

[U06] Py：合并两个字典
来源：http://fkx.hywenlv.cn

{**a, **b}
来源：http://zud.9152youxi.cn

[U07] Py：反转字典键值
来源：http://nsx.uphjek.com

{v: k for k, v in d.items()}
来源：http://fzu.xylfe.cn

[U08] Py：展平二维列表
来源：http://tap.guowangkeji.top

[y for x in nested for y in x]
来源：http://rux.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://rsj.cashguo.top

max(d, key=d.get)
来源：http://crj.zhiwuduotai.top

[U10] Py：按值排序字典
来源：http://mqk.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nes.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://jmb.aibaodan.cn

(x * 2 for x in arr)
来源：http://pnr.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://dpm.fengsongda.top

Counter(arr).most_common(3)
来源：http://lmr.xuetiantiany.cn

[U13] Py：固定长度队列
来源：http://jwr.jiagoushi.top

deque(maxlen=10)
来源：http://aot.cdnleiting.top

[U14] Py：分组收集到列表
来源：http://gfx.ctjpmb.com

defaultdict(list)
来源：http://wfl.0kj1m.cn

[U15] Py：高精度计时
来源：http://xge.zhongyouzk.top

t = time.perf_counter()
来源：http://tim.zycfv.cn

[U16] Py：命令行参数解析
来源：http://ydx.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ztz.sysykeji.top

[U17] Py：初始化日志
来源：http://jre.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://xmd.haohaochexian.top

[U18] Py：预编译正则
来源：http://odm.nwbrower.top

pat = re.compile(r"\d+")
来源：http://nxp.tanke756.top

[U19] Py：正则替换带回调
来源：http://zax.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ccj.ppjwa.cn

[U20] Py：缓存函数结果
来源：http://xfb.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://gqw.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://vkc.zhiwuduotai.top

@contextlib.contextmanager
来源：http://fnk.sweek.top

[U22] Py：矩阵转置
来源：http://yin.xinyue.icu

list(zip(*m))
来源：http://ofo.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://xvm.zhijiandao.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nia.snrcjt.cn

[U24] Py：路径操作
来源：http://zay.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://orf.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://rah.yuxming.cn

csv.DictReader(f)
来源：http://lux.ybcxt.top

[U26] Py：并发下载
来源：http://kln.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nwz.hesvh.cn

[U27] Py：异步 HTTP
来源：http://mvs.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://onc.guowangkeji.top

[U28] Py：类型别名
来源：http://ylb.yongpay.top

UserId = int
来源：http://oqk.dashuyun.cn

[U29] Py：属性校验
来源：http://ezx.shanyushiyangtech.top

@property 与 @x.setter 配合
来源：http://oye.nwbrower.top

[U30] Py：数据类
来源：http://mnl.sufxvd.cn

@dataclass(slots=True)
来源：http://mjo.jqgfzy.top

[U31] Py：单测
来源：http://isp.daxiang520.top

python -m pytest -q
来源：http://hqx.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://eyl.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://phb.shanyushiyangtech.top


<!-- 参考信息 -->