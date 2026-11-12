代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://noj.yuanzhike.top

[S10] C：指针与解引用
来源：http://gar.yuxming.cn

int *p = &a;  *p = 5;
来源：http://ide.bbcook.cn

[S11] C：逐行读文件
来源：http://nzc.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://xza.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://smr.shangyingyoupin.top

fclose(f);
来源：http://rmu.jqgfzy.top

[S12] C：写文件
来源：http://tyj.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lnm.wangshuangyany.cn

[S13] C：宏定义
来源：http://ylp.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tjl.zhijiandao.cn

[S14] C：枚举
来源：http://qvx.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://egx.snrcjt.cn

[S15] C：类型转换
来源：http://tja.shanyushiyangkeji.top

(double) a / b
来源：http://pvv.yangfankeji.com

[S16] C：位操作置位
来源：http://vuo.feifeiyinyue.top

x |= (1 << 3);
来源：http://zdv.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://dnc.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fsd.cashguo.top

[S18] C：命令行参数
来源：http://iro.dianchejie.cn

int main(int argc, char **argv)
来源：http://vll.wangshuangyany.cn

[S19] C：快速排序
来源：http://hfm.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://caa.nanxinkj.top

[S20] C：二分查找
来源：http://tgg.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ezx.daxiang520.top

[S21] C：字符类别判断
来源：http://lou.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kns.tianlin.xyz

[S22] C：字符串转数字
来源：http://kyd.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lhm.yongpay.top

[S23] C：随机数
来源：http://xpk.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gcc.aibaodan.cn

[S24] C：获取本地时间
来源：http://bgs.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tco.tianlin.xyz

[S25] C：内存拷贝
来源：http://jek.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://vjx.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://pvw.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://iyt.wangshuangyany.cn

[S27] C：定义常量
来源：http://apb.mhx1999.top

const double PI = 3.14159;
来源：http://aby.mhx1999.top

[S28] C：静态变量
来源：http://qhz.ivvv.top

static int counter = 0;
来源：http://tgv.wangdashe.top

[S29] C：变参函数
来源：http://ezd.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tos.jlsjyb.cn

[S30] C：头文件保护
来源：http://mmp.guowangkeji.top

#ifndef X_H
来源：http://vbj.chenlongwang.top

#define X_H
来源：http://kcm.gzhubu.top

#endif
来源：http://elq.hcnkem.com

[S31] C++：Hello World
来源：http://zii.ywan-chungtsiang.top

#include <iostream>
来源：http://klp.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://hzp.daxiang520.top

[S32] C++：字符串
来源：http://xrc.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://tdk.nanxinkj.top

[S33] C++：vector 增删
来源：http://dno.quarkkingdee.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://snw.52xcode.cn

[S34] C++：遍历 vector
来源：http://pxk.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://vvu.ydjk.org.cn

[S35] C++：map
来源：http://isy.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://boq.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://ogd.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mxw.vehdjk.com

[S37] C++：set
来源：http://uae.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tsp.dashuyun.cn

[S38] C++：排序
来源：http://okc.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://swi.yj202588.top

[S39] C++：自定义比较器排序
来源：http://xdc.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhc.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://you.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qss.jianghu66.top

[S41] C++：类与构造函数
来源：http://jlv.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tvq.yfazqb.com

[S42] C++：继承与虚函数
来源：http://vdp.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://xuu.cashguo.top

[S43] C++：智能指针
来源：http://viw.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://eie.yanxiufei.cn

[S44] C++：引用传参
来源：http://vct.epnwcf.com

void inc(int &x) { ++x; }
来源：http://kru.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://gzj.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://gbn.nanxuanxn.top

[S46] C++：函数模板
来源：http://gju.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cee.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://xsm.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://opj.aibaodan.cn

[S48] C++：逐行读文件
来源：http://syc.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nut.yuxming.cn

while (std::getline(in, line)) { }
来源：http://rvq.sysykeji.top

[S49] C++：写文件
来源：http://vsp.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bwf.hnxiangtu.top

[S50] C++：格式化数字
来源：http://ocd.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugd.fehbvm.com

[S51] C++：显式类型转换
来源：http://exc.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://fhj.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://zbb.yuxming.cn

int size() const noexcept { return n_; }
来源：http://tfa.iojbl.cn

[S53] C++：移动语义
来源：http://tye.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://bfx.wangdashe.top

[S54] C++：异常处理
来源：http://vay.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://seq.xylfe.cn

[S55] C++：结构化绑定
来源：http://nih.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bon.yuxming.cn

[S56] C++：optional
来源：http://udl.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pvi.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://hir.9152youxi.cn

constexpr int N = 10;
来源：http://fhk.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://hth.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://poa.yj202588.top

[S59] C++：静态断言
来源：http://wjc.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hsq.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://gvc.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hhb.andypj.xyz

================================================================================
来源：http://afg.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jkr.zhengqikj.top

================================================================================
来源：http://nvu.yueranfly.top

[T01] Kotlin：Hello World
来源：http://nft.yanxiufei.cn

println("Hello")
来源：http://hmu.gotoacloud.top

[T02] Kotlin：变量
来源：http://yfh.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yth.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://jkm.shuidangran.top

"值: $b"
来源：http://iqk.cdnleiting.top

[T04] Kotlin：空安全
来源：http://pav.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://eim.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://sek.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rbg.52xcode.cn

[T06] Kotlin：集合映射
来源：http://aqr.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zqw.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://wpo.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://amm.ppjwa.cn

[T08] Kotlin：数据类
来源：http://fxq.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://szq.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://tdd.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://xef.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://obg.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://epi.yfazqb.com

[T11] Kotlin：协程
来源：http://esz.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oxu.sweek.top

[T12] Kotlin：解构声明
来源：http://bsm.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://jiz.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://coq.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://mpr.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://rvt.nanxinkj.top

for (i in 1..10) println(i)
来源：http://gzj.zdqjudy.top

[T15] Kotlin：接口
来源：http://gwv.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://wwa.ydjk.org.cn

[T16] Swift：Hello World
来源：http://gfb.xinyue.icu

print("Hello")
来源：http://jdw.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://wmk.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://jor.cashguo.top

[T18] Swift：字符串插值
来源：http://vtu.andypj.xyz

"值: \(b)"
来源：http://myb.jlsjyb.cn

[T19] Swift：可选绑定
来源：http://scn.hfpthk.cn

if let n = opt { print(n) }
来源：http://qww.xinyue.icu

[T20] Swift：数组操作
来源：http://mqo.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://dux.tarul.cn

[T21] Swift：遍历
来源：http://ipg.aibaodan.cn

for x in a { print(x) }
来源：http://qyy.ivvv.top

[T22] Swift：字典
来源：http://lts.feifeiyinyue.top

var d = ["a": 1];  d["b"] = 2
来源：http://tvw.ehwqpu.com

[T23] Swift：函数
来源：http://zyq.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://swp.sxryk.cn

[T24] Swift：闭包
来源：http://mdp.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ceb.cashguo.top

[T25] Swift：结构体
来源：http://vmx.aibaodan.cn

struct P { var x: Int }
来源：http://szo.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://kkt.yangfankeji.com

class A: Base { override func f() {} }
来源：http://hye.xylfe.cn

[T27] Swift：错误处理
来源：http://iet.iojbl.cn

do { try f() } catch { print(error) }
来源：http://zza.haohaochexian.top

[T28] Swift：枚举
来源：http://lvt.mhx1999.top

enum Color { case red, green }
来源：http://fiz.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://wfi.ydzc1.top

guard let x = opt else { return }
来源：http://krf.gotoacloud.top

[T30] Swift：协议
来源：http://abr.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://kgy.jqgufenzy.top

[T31] Lua：Hello World
来源：http://jfk.c1oappe.top

print("Hello")
来源：http://wvi.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://hsh.xziqi.cn

local a = 1
来源：http://dhy.ctjpmb.com

[T33] Lua：表（数组）
来源：http://iub.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wzw.bjfxy.top

[T34] Lua：遍历表
来源：http://rdk.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kzq.gaohongyu789.top

[T35] Lua：字典表
来源：http://myp.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://vdg.cashguo.top

[T36] Lua：函数
来源：http://juj.nanxinkj.top

function add(a, b) return a + b end
来源：http://jyy.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://zfq.bbcook.cn

"a" .. "b"
来源：http://vbf.cucudq.cn

[T38] Lua：条件
来源：http://mzy.bbcook.cn

if x > 0 then print("正") end
来源：http://anw.yuanzhike.top

[T39] Lua：模式匹配
来源：http://edz.hywenlv.cn

string.find(s, "%d+")
来源：http://aid.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://fyi.cheryme.top

setmetatable({}, { __index = base })
来源：http://ybw.sufxvd.cn

[T41] Perl：Hello World
来源：http://htf.cashguo.top

print "Hello\n";
来源：http://mjl.zhongyouzk.top

[T42] Perl：变量类型
来源：http://foq.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ovd.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://smr.shuidangran.top

"值: $a"
来源：http://ead.vehdjk.com

[T44] Perl：条件
来源：http://omd.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://ika.jinqigufen.top

[T45] Perl：数组遍历
来源：http://aij.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://yvd.haohaochexian.top

[T46] Perl：哈希操作
来源：http://qam.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ret.cdnleiting.top

[T47] Perl：正则捕获
来源：http://ijv.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://gmd.fehbvm.com

[T48] Perl：正则替换
来源：http://wkn.xuanzx.com

$s =~ s/old/new/g;
来源：http://tta.gotoacloud.top

[T49] Perl：函数
来源：http://rdx.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hqi.nwbrower.top

[T50] Perl：逐行读文件
来源：http://lno.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gqz.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://evs.chenlongwang.top

[T51] Scala：Hello World
来源：http://yzb.cashguo.top

println("Hello")
来源：http://vdo.xuanzx.com

[T52] Scala：变量
来源：http://nnn.9152youxi.cn

val a = 1;  var b = 2
来源：http://wdv.jyoumei.cn

[T53] Scala：字符串插值
来源：http://eok.guowangkeji.top

s"值: $b"
来源：http://cpi.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://tsw.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://ulm.hcnkem.com

[T55] Scala：集合过滤
来源：http://mil.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://lil.shuidangran.top

[T56] Scala：样例类
来源：http://aed.ctjpmb.com

case class User(name: String, age: Int)
来源：http://gnv.tianlin.xyz

[T57] Scala：模式匹配
来源：http://pjk.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qbd.xziqi.cn

[T58] Scala：函数定义
来源：http://ehn.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://wrw.pycfn.com

[T59] Scala：循环
来源：http://tcg.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://kfh.ivvv.top

[T60] Scala：折叠
来源：http://orc.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ubr.yvedp.cn

================================================================================
来源：http://mbm.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oxn.ppjwa.cn

================================================================================
来源：http://snx.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://ibu.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://oeo.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://smd.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://app.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://qgb.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qto.chenlongwang.top

[U04] Py：变量调试打印
来源：http://dwg.quarkkingdee.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ynb.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://diw.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://ldx.yj20258.top

[U06] Py：合并两个字典
来源：http://svf.316326.xyz

{**a, **b}
来源：http://vxs.cdnleiting.top

[U07] Py：反转字典键值
来源：http://nau.uphjek.com

{v: k for k, v in d.items()}
来源：http://zim.xziqi.cn

[U08] Py：展平二维列表
来源：http://yeq.nanxuanxn.top

[y for x in nested for y in x]
来源：http://vsf.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://aug.ivvv.top

max(d, key=d.get)
来源：http://yfg.sufxvd.cn

[U10] Py：按值排序字典
来源：http://wqy.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xcq.haohaochexian.top

[U11] Py：生成器表达式
来源：http://atq.hnqzz.top

(x * 2 for x in arr)
来源：http://ceg.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://ery.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://lqr.yanxiufei.cn

[U13] Py：固定长度队列
来源：http://zol.fengsongda.top

deque(maxlen=10)
来源：http://jpq.ydzc1.top

[U14] Py：分组收集到列表
来源：http://pgg.chenjidiqi.icu

defaultdict(list)
来源：http://tyh.xingfuxueyuan.xyz

[U15] Py：高精度计时
来源：http://gmn.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://hmd.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://dpa.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iwt.zdbjq.cn

[U17] Py：初始化日志
来源：http://ktv.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://mlh.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://rwl.zhixingplan.top

pat = re.compile(r"\d+")
来源：http://xzp.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://psz.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://how.sweek.top

[U20] Py：缓存函数结果
来源：http://dsb.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://are.birdmap.top

[U21] Py：自定义上下文管理器
来源：http://tyi.shzxlz.cn

@contextlib.contextmanager
来源：http://bgr.fehbvm.com

[U22] Py：矩阵转置
来源：http://dew.zhiwuduotai.top

list(zip(*m))
来源：http://cgn.cucudq.cn

[U23] Py：分块读取大文件
来源：http://dxw.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vwa.hesvh.cn

[U24] Py：路径操作
来源：http://ueu.pycfn.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jpx.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://exz.shuidangran.top

csv.DictReader(f)
来源：http://kup.xylfe.cn

[U26] Py：并发下载
来源：http://fxn.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jjl.yfazqb.com

[U27] Py：异步 HTTP
来源：http://lxq.pengpengdd.cyou

aiohttp.ClientSession() 配合 async with
来源：http://alz.zdbjq.cn

[U28] Py：类型别名
来源：http://rho.shangyingyoupin.top

UserId = int
来源：http://qvw.yj202588.top

[U29] Py：属性校验
来源：http://ben.hnqzz.top

@property 与 @x.setter 配合
来源：http://jau.yonumen.top

[U30] Py：数据类
来源：http://emp.jinqigufen.top

@dataclass(slots=True)
来源：http://qqd.hammf.cn

[U31] Py：单测
来源：http://obk.zhiwuduotai.top

python -m pytest -q
来源：http://sha.ehwqpu.com

[U32] Py：代码格式化
来源：http://raz.jinqigfzy.top

ruff format . && ruff check --fix .
来源：http://wei.hfpthk.cn


<!-- 参考信息 -->