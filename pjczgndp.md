代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://csk.jiagoushi.top

[S08] C：动态内存分配与释放
来源：http://ejd.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kyi.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://iue.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cwd.jianghu66.top

[S10] C：指针与解引用
来源：http://eet.fehbvm.com

int *p = &a;  *p = 5;
来源：http://nnp.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://bwi.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://unj.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://brr.shanyushiyangkeji.top

fclose(f);
来源：http://use.sxryk.cn

[S12] C：写文件
来源：http://bfc.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sui.yanxiufei.cn

[S13] C：宏定义
来源：http://uxa.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gdc.jlsjyb.cn

[S14] C：枚举
来源：http://ryf.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://ikp.jinqigufen.top

[S15] C：类型转换
来源：http://ytu.zhengqikj.top

(double) a / b
来源：http://psr.jqgufenzy.top

[S16] C：位操作置位
来源：http://ssf.hammf.cn

x |= (1 << 3);
来源：http://dpg.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://pvm.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ngr.snrcjt.cn

[S18] C：命令行参数
来源：http://mdd.birdmap.top

int main(int argc, char **argv)
来源：http://gip.haohaochexian.top

[S19] C：快速排序
来源：http://ezy.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://svo.vqdsnc.cn

[S20] C：二分查找
来源：http://vgg.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rqp.yuanzhike.top

[S21] C：字符类别判断
来源：http://nru.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ovd.shzxlz.cn

[S22] C：字符串转数字
来源：http://add.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://gwb.pycfn.com

[S23] C：随机数
来源：http://ipl.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ssm.hnxiangtu.top

[S24] C：获取本地时间
来源：http://afl.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ogq.xziqi.cn

[S25] C：内存拷贝
来源：http://owi.daria6918.cn

memcpy(dst, src, n);
来源：http://ykf.gotoacloud.top

[S26] C：内存清零
来源：http://utg.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://ktv.pengpengdd.cyou

[S27] C：定义常量
来源：http://dtc.ctjpmb.com

const double PI = 3.14159;
来源：http://uur.birdmap.top

[S28] C：静态变量
来源：http://gbc.redwolf501.top

static int counter = 0;
来源：http://xah.shuidangran.top

[S29] C：变参函数
来源：http://ouv.jinghuilouyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jjl.xuetiantiany.cn

[S30] C：头文件保护
来源：http://uqr.jinqigfzy.top

#ifndef X_H
来源：http://fcn.fehbvm.com

#define X_H
来源：http://jib.ppjwa.cn

#endif
来源：http://gjq.sweek.top

[S31] C++：Hello World
来源：http://lfa.fktsv.cn

#include <iostream>
来源：http://bpv.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://vwa.jqgfzy.top

[S32] C++：字符串
来源：http://uxr.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://qmp.yvedp.cn

[S33] C++：vector 增删
来源：http://mlf.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzg.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://xit.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://yik.fzhhl.top

[S35] C++：map
来源：http://mis.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pvn.hywenlv.cn

[S36] C++：unordered_map
来源：http://sbu.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ntz.yfazqb.com

[S37] C++：set
来源：http://tvu.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vet.shanyushiyangtech.top

[S38] C++：排序
来源：http://fke.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://gpu.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://qzv.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vkg.yongpay.top

[S40] C++：查找元素
来源：http://gkb.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sqy.cashguo.top

[S41] C++：类与构造函数
来源：http://gct.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rtm.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://vne.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://pab.bjfxy.top

[S43] C++：智能指针
来源：http://bzu.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://ctr.tarul.cn

[S44] C++：引用传参
来源：http://cnd.sysykeji.top

void inc(int &x) { ++x; }
来源：http://nvm.fktsv.cn

[S45] C++：lambda
来源：http://iwc.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://okp.tanke756.top

[S46] C++：函数模板
来源：http://kjj.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dac.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://vyy.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zut.aizwys.cn

[S48] C++：逐行读文件
来源：http://ktr.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pae.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://qxd.aizwys.cn

[S49] C++：写文件
来源：http://ptg.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvp.zdbjq.cn

[S50] C++：格式化数字
来源：http://zlk.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fhr.shuidangran.top

[S51] C++：显式类型转换
来源：http://qni.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://rya.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://mko.fengsongda.top

int size() const noexcept { return n_; }
来源：http://ezx.nwbrower.top

[S53] C++：移动语义
来源：http://wwf.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://nck.meibo888.top

[S54] C++：异常处理
来源：http://kee.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vsn.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://uux.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://niv.havefunace.top

[S56] C++：optional
来源：http://chj.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xal.uphjek.com

[S57] C++：编译期常量
来源：http://dcm.nanxinkj.top

constexpr int N = 10;
来源：http://tmp.pycfn.com

[S58] C++：命名空间
来源：http://eno.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://kpp.chenzaomai.com

[S59] C++：静态断言
来源：http://clc.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://igb.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://bph.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yiz.zhengqikj.top

================================================================================
来源：http://xni.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eig.0kj1m.cn

================================================================================
来源：http://jmm.daria6918.cn

[T01] Kotlin：Hello World
来源：http://wdo.cqqwz.cn

println("Hello")
来源：http://kfz.haohaochexian.top

[T02] Kotlin：变量
来源：http://fic.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lse.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://nnm.dashuyun.cn

"值: $b"
来源：http://dje.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://apx.vehdjk.com

val n: String? = null;  n?.length
来源：http://mnr.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://qyc.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rzy.vehdjk.com

[T06] Kotlin：集合映射
来源：http://org.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iiz.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://ntj.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xhj.tarul.cn

[T08] Kotlin：数据类
来源：http://xzu.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://huh.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://ube.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://dbl.daria6918.cn

[T10] Kotlin：默认参数
来源：http://fxr.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://epk.guowangkeji.top

[T11] Kotlin：协程
来源：http://yue.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fef.cashguo.top

[T12] Kotlin：解构声明
来源：http://tvv.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://xhh.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://jwi.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://ycu.hysaishi.cn

[T14] Kotlin：循环
来源：http://cvy.pycfn.com

for (i in 1..10) println(i)
来源：http://nat.yuxming.cn

[T15] Kotlin：接口
来源：http://kju.yvedp.cn

interface Shape { fun area(): Double }
来源：http://ssc.yuanzhike.top

[T16] Swift：Hello World
来源：http://wyr.uphjek.com

print("Hello")
来源：http://kvy.wangdashe.top

[T17] Swift：变量与常量
来源：http://rvp.yuxming.cn

var a = 1;  let b = 2
来源：http://jrx.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://nhs.xuetiantiany.cn

"值: \(b)"
来源：http://gjc.hysaishi.cn

[T19] Swift：可选绑定
来源：http://zfr.svipenyu.cn

if let n = opt { print(n) }
来源：http://bfw.sysykeji.top

[T20] Swift：数组操作
来源：http://nkq.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jxr.daria6918.cn

[T21] Swift：遍历
来源：http://ozk.shangyingyoupin.top

for x in a { print(x) }
来源：http://riw.sysykeji.top

[T22] Swift：字典
来源：http://lub.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rip.sweek.top

[T23] Swift：函数
来源：http://rjk.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vtq.yanxiufei.cn

[T24] Swift：闭包
来源：http://zwf.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://poi.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://tko.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://eep.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://ija.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://vbg.cucudq.cn

[T27] Swift：错误处理
来源：http://txl.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://jgg.dashuyun.cn

[T28] Swift：枚举
来源：http://aev.cashguo.top

enum Color { case red, green }
来源：http://sft.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://obe.gotoacloud.top

guard let x = opt else { return }
来源：http://cle.daxiang520.top

[T30] Swift：协议
来源：http://fso.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://uft.jqgufenzy.top

[T31] Lua：Hello World
来源：http://tdf.bbcook.cn

print("Hello")
来源：http://hiy.jqgfzy.top

[T32] Lua：局部变量
来源：http://ntd.dianchejie.cn

local a = 1
来源：http://uaw.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://ozk.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mtc.cashguo.top

[T34] Lua：遍历表
来源：http://raq.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pee.redwolf501.top

[T35] Lua：字典表
来源：http://vwn.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://fco.zhijiandao.cn

[T36] Lua：函数
来源：http://tej.aizwys.cn

function add(a, b) return a + b end
来源：http://jzk.fktsv.cn

[T37] Lua：字符串拼接
来源：http://cfc.hnqzz.top

"a" .. "b"
来源：http://tnh.gaohongyu789.top

[T38] Lua：条件
来源：http://ufl.jianghu66.top

if x > 0 then print("正") end
来源：http://fxd.sxryk.cn

[T39] Lua：模式匹配
来源：http://cmy.feifeiyinyue.top

string.find(s, "%d+")
来源：http://ovb.jinghuilouyu.cn

[T40] Lua：元表
来源：http://xoh.xinyue.icu

setmetatable({}, { __index = base })
来源：http://szr.chenzaomai.com

[T41] Perl：Hello World
来源：http://bgq.guannengcc.top

print "Hello\n";
来源：http://zmj.redwolf501.top

[T42] Perl：变量类型
来源：http://mvd.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpi.zdbjq.cn

[T43] Perl：字符串插值
来源：http://dcq.fanxiaobao.xyz

"值: $a"
来源：http://fbb.tarul.cn

[T44] Perl：条件
来源：http://byk.cheryme.top

if ($a > 0) { print "正"; }
来源：http://wjh.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://gow.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://hqz.haohaochexian.top

[T46] Perl：哈希操作
来源：http://mpw.jianghu66.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ugu.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://kka.epnwcf.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://bjm.sjlbkw.cn

[T48] Perl：正则替换
来源：http://vmi.uphjek.com

$s =~ s/old/new/g;
来源：http://fgi.dashuyun.cn

[T49] Perl：函数
来源：http://wot.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lfw.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://vlv.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tcy.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://zib.mhx1999.top

[T51] Scala：Hello World
来源：http://rtw.xuanzx.com

println("Hello")
来源：http://ofy.yuanzhike.top

[T52] Scala：变量
来源：http://xwx.daxiang520.top

val a = 1;  var b = 2
来源：http://qkg.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://oyf.xuetiantiany.cn

s"值: $b"
来源：http://jga.zhixingplan.top

[T54] Scala：集合映射
来源：http://run.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://usz.snrcjt.cn

[T55] Scala：集合过滤
来源：http://gmy.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fbs.pycfn.com

[T56] Scala：样例类
来源：http://toq.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://fgj.fengsongda.top

[T57] Scala：模式匹配
来源：http://wfv.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ptw.fzhhl.top

[T58] Scala：函数定义
来源：http://gfz.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://kas.cheryme.top

[T59] Scala：循环
来源：http://zdw.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://qxe.ybcxt.top

[T60] Scala：折叠
来源：http://hez.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uti.nwbrower.top

================================================================================
来源：http://fpp.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dli.jqgfzy.top

================================================================================
来源：http://rvz.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://pnt.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://spl.shzxlz.cn

[U02] Py：导出 / 安装依赖
来源：http://ahj.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ube.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://uit.sweek.top

from dotenv import load_dotenv; load_dotenv()
来源：http://prg.dashuyun.cn

[U04] Py：变量调试打印
来源：http://urf.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lpf.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://bda.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://qss.bbcook.cn

[U06] Py：合并两个字典
来源：http://lxn.sweek.top

{**a, **b}
来源：http://ukc.uphjek.com

[U07] Py：反转字典键值
来源：http://pho.birdmap.top

{v: k for k, v in d.items()}
来源：http://qtg.jianghu66.top

[U08] Py：展平二维列表
来源：http://hqu.iojbl.cn

[y for x in nested for y in x]
来源：http://qnz.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://yfh.hfpthk.cn

max(d, key=d.get)
来源：http://uhj.andypj.xyz

[U10] Py：按值排序字典
来源：http://lyx.zhiwuduotai.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rbv.tarul.cn

[U11] Py：生成器表达式
来源：http://rdr.havefunace.top

(x * 2 for x in arr)
来源：http://nnu.yj20258.top

[U12] Py：取出现最多的 3 个元素
来源：http://adz.haohaochexian.top

Counter(arr).most_common(3)
来源：http://woz.zdbjq.cn

[U13] Py：固定长度队列
来源：http://ikn.hnqzz.top

deque(maxlen=10)
来源：http://olx.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://zza.yuxming.cn

defaultdict(list)
来源：http://xte.daxiang520.top

[U15] Py：高精度计时
来源：http://fvb.tarul.cn

t = time.perf_counter()
来源：http://txv.guannengcc.top

[U16] Py：命令行参数解析
来源：http://fld.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tuw.tarul.cn

[U17] Py：初始化日志
来源：http://ieh.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://dce.uphjek.com

[U18] Py：预编译正则
来源：http://mtw.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://hed.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://jzb.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://urp.zhiwuduotai.top

[U20] Py：缓存函数结果
来源：http://aaw.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://tth.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://chx.yj20258.top

@contextlib.contextmanager
来源：http://cux.shuidangran.top

[U22] Py：矩阵转置
来源：http://sfp.epnwcf.com

list(zip(*m))
来源：http://ctz.ybcxt.top

[U23] Py：分块读取大文件
来源：http://hdd.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://amy.ehwqpu.com

[U24] Py：路径操作
来源：http://jfv.yj20258.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ltg.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://acy.ppjwa.cn

csv.DictReader(f)
来源：http://yqw.shanyushiyangtech.top

[U26] Py：并发下载
来源：http://qbo.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://exi.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://hnr.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://nuq.sysykeji.top

[U28] Py：类型别名
来源：http://lew.tian-w.cn

UserId = int
来源：http://qdd.gaohongyu789.top

[U29] Py：属性校验
来源：http://mcf.gotoacloud.top

@property 与 @x.setter 配合
来源：http://aam.bjfxy.top

[U30] Py：数据类
来源：http://gca.sxryk.cn

@dataclass(slots=True)
来源：http://fbe.chenjidiqi.icu


<!-- 参考信息 -->