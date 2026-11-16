代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qbu.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://hmy.nanxinkj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mep.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://rnq.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vim.dianchejie.cn

[S10] C：指针与解引用
来源：http://dzy.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://ecs.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://ngb.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://npp.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://vus.ehwqpu.com

fclose(f);
来源：http://bci.sjlbkw.cn

[S12] C：写文件
来源：http://sda.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ebo.zycfv.cn

[S13] C：宏定义
来源：http://bav.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gin.wangdashe.top

[S14] C：枚举
来源：http://mjt.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://itx.cqqwz.cn

[S15] C：类型转换
来源：http://jol.zhaomingkeji.xyz

(double) a / b
来源：http://grh.guowangkeji.top

[S16] C：位操作置位
来源：http://ctf.c1oappe.top

x |= (1 << 3);
来源：http://hcd.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://jew.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zrc.cqqwz.cn

[S18] C：命令行参数
来源：http://yjj.bjfxy.top

int main(int argc, char **argv)
来源：http://cun.jqgfzy.top

[S19] C：快速排序
来源：http://geb.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://alm.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://cbu.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xgo.cheryme.top

[S21] C：字符类别判断
来源：http://ouv.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mht.zhixingplan.top

[S22] C：字符串转数字
来源：http://otg.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uau.9152youxi.cn

[S23] C：随机数
来源：http://yxu.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sxi.uphjek.com

[S24] C：获取本地时间
来源：http://fvh.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ujc.jqgufenzy.top

[S25] C：内存拷贝
来源：http://nrd.jqgfzy.top

memcpy(dst, src, n);
来源：http://oby.zhengqikj.top

[S26] C：内存清零
来源：http://fqa.smart0.xyz

memset(a, 0, sizeof a);
来源：http://mkx.redwolf501.top

[S27] C：定义常量
来源：http://tgd.cucudq.cn

const double PI = 3.14159;
来源：http://rmf.fanxiaobao.xyz

[S28] C：静态变量
来源：http://wqj.wangdashe.top

static int counter = 0;
来源：http://bbe.cucudq.cn

[S29] C：变参函数
来源：http://yxx.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ujx.yj20258.top

[S30] C：头文件保护
来源：http://uak.ivvv.top

#ifndef X_H
来源：http://rdt.ctjpmb.com

#define X_H
来源：http://uod.yj20258.top

#endif
来源：http://cbo.sweek.top

[S31] C++：Hello World
来源：http://goo.shuidangran.top

#include <iostream>
来源：http://euv.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://gzp.aizwys.cn

[S32] C++：字符串
来源：http://hpd.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://ttj.hammf.cn

[S33] C++：vector 增删
来源：http://fea.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://clt.svipenyu.cn

[S34] C++：遍历 vector
来源：http://unc.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://ipw.daxiang520.top

[S35] C++：map
来源：http://odx.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pog.ydzc1.top

[S36] C++：unordered_map
来源：http://fvb.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jpt.bbcook.cn

[S37] C++：set
来源：http://usm.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qnw.yvedp.cn

[S38] C++：排序
来源：http://wrx.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://red.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://izk.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yui.shuidangran.top

[S40] C++：查找元素
来源：http://xyi.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://toy.epnwcf.com

[S41] C++：类与构造函数
来源：http://klf.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pao.epnwcf.com

[S42] C++：继承与虚函数
来源：http://awa.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://cqx.daxiang520.top

[S43] C++：智能指针
来源：http://opj.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://xyw.fzhhl.top

[S44] C++：引用传参
来源：http://nbo.yuxming.cn

void inc(int &x) { ++x; }
来源：http://oet.fehbvm.com

[S45] C++：lambda
来源：http://ogj.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://jrj.dashuyun.cn

[S46] C++：函数模板
来源：http://cqn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hpy.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://ood.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uqd.tianlin.xyz

[S48] C++：逐行读文件
来源：http://val.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://ylg.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://vcr.hammf.cn

[S49] C++：写文件
来源：http://fzu.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://trb.dashuyun.cn

[S50] C++：格式化数字
来源：http://rzx.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zxj.jyoumei.cn

[S51] C++：显式类型转换
来源：http://xfu.wangdashe.top

static_cast<double>(a) / b
来源：http://lbh.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://ela.aizwys.cn

int size() const noexcept { return n_; }
来源：http://xrn.nwbrower.top

[S53] C++：移动语义
来源：http://zxc.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://dvy.sufxvd.cn

[S54] C++：异常处理
来源：http://xot.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://djm.yfazqb.com

[S55] C++：结构化绑定
来源：http://tky.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xzi.cheryme.top

[S56] C++：optional
来源：http://xxe.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khe.yonumen.top

[S57] C++：编译期常量
来源：http://gus.zhongyouzk.top

constexpr int N = 10;
来源：http://vrd.dashuyun.cn

[S58] C++：命名空间
来源：http://ogc.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://hfi.52xcode.cn

[S59] C++：静态断言
来源：http://avr.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ohn.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://jde.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rlq.tanke756.top

================================================================================
来源：http://jew.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymq.wangdashe.top

================================================================================
来源：http://wlm.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://vuq.dianchejie.cn

println("Hello")
来源：http://eur.kuanghao11.cn

[T02] Kotlin：变量
来源：http://nwn.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hwv.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://lgq.jqgufenzy.top

"值: $b"
来源：http://dki.zdqjudy.top

[T04] Kotlin：空安全
来源：http://nxl.316326.xyz

val n: String? = null;  n?.length
来源：http://efq.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://mrq.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://opg.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://fgc.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nyr.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://tmj.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vjo.pycfn.com

[T08] Kotlin：数据类
来源：http://dzz.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://qhg.yonumen.top

[T09] Kotlin：扩展函数
来源：http://vsp.yongpay.top

fun String.exclaim() = this + "!"
来源：http://cvu.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://jkc.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://uak.sysykeji.top

[T11] Kotlin：协程
来源：http://kch.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vya.yuxming.cn

[T12] Kotlin：解构声明
来源：http://smv.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://bzh.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://lig.xziqi.cn

val m = mapOf("a" to 1)
来源：http://mxu.chenlongwang.top

[T14] Kotlin：循环
来源：http://rze.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://uor.dianchejie.cn

[T15] Kotlin：接口
来源：http://gql.316326.xyz

interface Shape { fun area(): Double }
来源：http://bcg.jianghu66.top

[T16] Swift：Hello World
来源：http://rwl.jqgufenzy.top

print("Hello")
来源：http://qjd.dashuyun.cn

[T17] Swift：变量与常量
来源：http://zgu.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://kjl.yj202588.top

[T18] Swift：字符串插值
来源：http://vcp.pengpengdd.cyou

"值: \(b)"
来源：http://qzc.cashguo.top

[T19] Swift：可选绑定
来源：http://erf.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://srp.zycfv.cn

[T20] Swift：数组操作
来源：http://qro.shanyushiyangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://yen.wangshuangyany.cn

[T21] Swift：遍历
来源：http://pgo.jinqigfzy.top

for x in a { print(x) }
来源：http://kth.hysaishi.cn

[T22] Swift：字典
来源：http://ohf.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://tdi.sjlbkw.cn

[T23] Swift：函数
来源：http://ppo.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvy.gaohongyu789.top

[T24] Swift：闭包
来源：http://zsx.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sbc.ehwqpu.com

[T25] Swift：结构体
来源：http://psx.yvedp.cn

struct P { var x: Int }
来源：http://vye.yj20258888.top

[T26] Swift：类与重写
来源：http://tgc.hfpthk.cn

class A: Base { override func f() {} }
来源：http://dff.svipenyu.cn

[T27] Swift：错误处理
来源：http://lmu.uphjek.com

do { try f() } catch { print(error) }
来源：http://bza.fengsongda.top

[T28] Swift：枚举
来源：http://pbx.cashguo.top

enum Color { case red, green }
来源：http://xnt.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://any.tarul.cn

guard let x = opt else { return }
来源：http://jih.yonumen.top

[T30] Swift：协议
来源：http://jty.yj20258.top

protocol Shape { func area() -> Double }
来源：http://xvy.yonumen.top

[T31] Lua：Hello World
来源：http://hpl.cucudq.cn

print("Hello")
来源：http://gpl.bbcook.cn

[T32] Lua：局部变量
来源：http://pes.xingfuxueyuan.xyz

local a = 1
来源：http://cmu.jiagoushi.top

[T33] Lua：表（数组）
来源：http://exd.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xvz.fengsongda.top

[T34] Lua：遍历表
来源：http://fww.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://agw.hysaishi.cn

[T35] Lua：字典表
来源：http://jgt.birdmap.top

local d = { a = 1 };  d.b = 2
来源：http://tgn.cucudq.cn

[T36] Lua：函数
来源：http://qvd.yonumen.top

function add(a, b) return a + b end
来源：http://bji.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://czv.xziqi.cn

"a" .. "b"
来源：http://zlv.0kj1m.cn

[T38] Lua：条件
来源：http://xwv.uphjek.com

if x > 0 then print("正") end
来源：http://uhy.aibaodan.cn

[T39] Lua：模式匹配
来源：http://vse.kuanghao11.cn

string.find(s, "%d+")
来源：http://lug.yj20258888.top

[T40] Lua：元表
来源：http://ccl.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://djc.sjlbkw.cn

[T41] Perl：Hello World
来源：http://qoa.shuidangran.top

print "Hello\n";
来源：http://vbw.yueranfly.top

[T42] Perl：变量类型
来源：http://umx.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hgl.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://ukp.aibaodan.cn

"值: $a"
来源：http://rql.epnwcf.com

[T44] Perl：条件
来源：http://ryk.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://sjq.tian-w.cn

[T45] Perl：数组遍历
来源：http://bcj.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://wbe.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://lxy.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oqh.chenlongwang.top

[T47] Perl：正则捕获
来源：http://nze.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jeq.yj202588.top

[T48] Perl：正则替换
来源：http://ibe.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://jmm.jyoumei.cn

[T49] Perl：函数
来源：http://cfa.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zvg.wangdashe.top

[T50] Perl：逐行读文件
来源：http://hnw.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://smf.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://qlu.jianghu66.top

[T51] Scala：Hello World
来源：http://tod.yfazqb.com

println("Hello")
来源：http://aqf.zdbjq.cn

[T52] Scala：变量
来源：http://nyf.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://nrm.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://fnf.hysaishi.cn

s"值: $b"
来源：http://mum.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://iig.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://hab.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://cwh.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://zzl.jianghu66.top

[T56] Scala：样例类
来源：http://tvg.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://xxx.yonumen.top

[T57] Scala：模式匹配
来源：http://hmy.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nbl.jinqigfzy.top

[T58] Scala：函数定义
来源：http://ozb.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mgo.epnwcf.com

[T59] Scala：循环
来源：http://qat.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://gvm.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://tyo.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nij.wangshuangyany.cn

================================================================================
来源：http://nio.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bux.tanke756.top

================================================================================
来源：http://oba.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://btn.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qoy.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://mrh.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cgp.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://rwz.zdbjq.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ycw.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://rlr.jinqigufen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gpb.yueranfly.top

[U05] Py：列表去重且保序
来源：http://eqx.fengsongda.top

list(dict.fromkeys(arr))
来源：http://qfu.sweek.top

[U06] Py：合并两个字典
来源：http://dbo.zdqjudy.top

{**a, **b}
来源：http://hqo.9152youxi.cn

[U07] Py：反转字典键值
来源：http://exr.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://roi.xinyue.icu

[U08] Py：展平二维列表
来源：http://eac.fehbvm.com

[y for x in nested for y in x]
来源：http://yfd.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://npn.xuanzx.com

max(d, key=d.get)
来源：http://quf.cdnleiting.top

[U10] Py：按值排序字典
来源：http://bcy.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bze.yuxming.cn

[U11] Py：生成器表达式
来源：http://gwd.nwbrower.top

(x * 2 for x in arr)
来源：http://tly.jinghuilouyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lpg.sweek.top

Counter(arr).most_common(3)
来源：http://nmh.zdbjq.cn

[U13] Py：固定长度队列
来源：http://bkz.52xcode.cn

deque(maxlen=10)
来源：http://yuz.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://tet.shuidangran.top

defaultdict(list)
来源：http://ibo.xuanzx.com

[U15] Py：高精度计时
来源：http://mch.zhoulong.xyz

t = time.perf_counter()
来源：http://xhr.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://qkx.quarkkingdee.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nka.guowangkeji.top

[U17] Py：初始化日志
来源：http://kdl.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://ovj.fengsongda.top

[U18] Py：预编译正则
来源：http://fks.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://ary.zycfv.cn

[U19] Py：正则替换带回调
来源：http://rvi.ppjwa.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vbz.redwolf501.top

[U20] Py：缓存函数结果
来源：http://wdg.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://ndw.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://jgb.dashuyun.cn

@contextlib.contextmanager
来源：http://jvf.chenzaomai.com

[U22] Py：矩阵转置
来源：http://zko.tian-w.cn

list(zip(*m))
来源：http://fea.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://ogl.zhongyouzk.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bjo.andypj.xyz

[U24] Py：路径操作
来源：http://heu.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://alp.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://xqt.aibaodan.cn

csv.DictReader(f)
来源：http://ude.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://mhz.jinqigufen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://idp.ybcxt.top

[U27] Py：异步 HTTP
来源：http://jdp.hongshengwenyu.top

aiohttp.ClientSession() 配合 async with
来源：http://ost.yanxiufei.cn

[U28] Py：类型别名
来源：http://cjf.vehdjk.com

UserId = int
来源：http://pch.c1oappe.top

[U29] Py：属性校验
来源：http://vzt.9152youxi.cn

@property 与 @x.setter 配合
来源：http://pww.haohaochexian.top

[U30] Py：数据类
来源：http://qwx.shangyingyoupin.top

@dataclass(slots=True)
来源：http://zcy.xuetiantiany.cn


<!-- 参考信息 -->