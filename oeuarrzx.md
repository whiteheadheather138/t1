代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fqa.ivvv.top

[S08] C：动态内存分配与释放
来源：http://qht.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cwg.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://vpl.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mzr.aizwys.cn

[S10] C：指针与解引用
来源：http://vga.fktsv.cn

int *p = &a;  *p = 5;
来源：http://tlk.zdbjq.cn

[S11] C：逐行读文件
来源：http://qzf.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://lhu.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://oeh.gotoacloud.top

fclose(f);
来源：http://wsf.smart0.xyz

[S12] C：写文件
来源：http://sva.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnq.haohaochexian.top

[S13] C：宏定义
来源：http://shh.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vvp.gogol.net.cn

[S14] C：枚举
来源：http://piz.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://tdc.yueranfly.top

[S15] C：类型转换
来源：http://gkd.tarul.cn

(double) a / b
来源：http://rvh.zhiwuduotai.top

[S16] C：位操作置位
来源：http://phh.meibo888.top

x |= (1 << 3);
来源：http://zpq.xinyue.icu

[S17] C：安全拼接字符串
来源：http://npn.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lzf.9152youxi.cn

[S18] C：命令行参数
来源：http://yrh.yueranfly.top

int main(int argc, char **argv)
来源：http://hor.yj20258.top

[S19] C：快速排序
来源：http://bdn.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jdq.9152youxi.cn

[S20] C：二分查找
来源：http://miy.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cml.wangdashe.top

[S21] C：字符类别判断
来源：http://dlb.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jew.jlsjyb.cn

[S22] C：字符串转数字
来源：http://chh.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://rcj.yonumen.top

[S23] C：随机数
来源：http://fsf.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fmh.zycfv.cn

[S24] C：获取本地时间
来源：http://jnn.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lie.ctjpmb.com

[S25] C：内存拷贝
来源：http://hbt.aibaodan.cn

memcpy(dst, src, n);
来源：http://clt.iojbl.cn

[S26] C：内存清零
来源：http://yhz.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://vcr.ybcxt.top

[S27] C：定义常量
来源：http://djx.ivvv.top

const double PI = 3.14159;
来源：http://agx.yfazqb.com

[S28] C：静态变量
来源：http://hfl.xinyue.icu

static int counter = 0;
来源：http://nam.ybcxt.top

[S29] C：变参函数
来源：http://tte.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vtc.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://ovh.aibaodan.cn

#ifndef X_H
来源：http://vsc.cucudq.cn

#define X_H
来源：http://uiz.zycfv.cn

#endif
来源：http://vet.hesvh.cn

[S31] C++：Hello World
来源：http://cfk.jinqigufen.top

#include <iostream>
来源：http://rcm.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://xmg.jianghu66.top

[S32] C++：字符串
来源：http://dxf.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://fhm.daxiang520.top

[S33] C++：vector 增删
来源：http://csb.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://otc.xylfe.cn

[S34] C++：遍历 vector
来源：http://tyq.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://dyw.ywan-chungtsiang.top

[S35] C++：map
来源：http://aed.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyb.tanke756.top

[S36] C++：unordered_map
来源：http://cjd.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tsi.pycfn.com

[S37] C++：set
来源：http://oto.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://avw.jinqigfzy.top

[S38] C++：排序
来源：http://jvm.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://xbb.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://zwf.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://myr.yj20258.top

[S40] C++：查找元素
来源：http://ejv.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://egd.hysaishi.cn

[S41] C++：类与构造函数
来源：http://pmi.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pmj.redwolf501.top

[S42] C++：继承与虚函数
来源：http://mzj.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://gcr.bjfxy.top

[S43] C++：智能指针
来源：http://ftq.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://gew.zhiwuduotai.top

[S44] C++：引用传参
来源：http://elk.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://zqj.jyoumei.cn

[S45] C++：lambda
来源：http://caj.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://qda.xuanzx.com

[S46] C++：函数模板
来源：http://sqs.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://shc.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://hwe.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kut.havefunace.top

[S48] C++：逐行读文件
来源：http://atf.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uig.sxryk.cn

while (std::getline(in, line)) { }
来源：http://iqe.feifeiyinyue.top

[S49] C++：写文件
来源：http://vvc.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ach.jinqigufen.top

[S50] C++：格式化数字
来源：http://sao.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mft.yangfankeji.com

[S51] C++：显式类型转换
来源：http://wao.zdbjq.cn

static_cast<double>(a) / b
来源：http://vpn.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://icc.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://rwe.aibaodan.cn

[S53] C++：移动语义
来源：http://ybo.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://evz.zhiwuduotai.top

[S54] C++：异常处理
来源：http://xfg.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ilj.hywenlv.cn

[S55] C++：结构化绑定
来源：http://ceq.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wma.tianlin.xyz

[S56] C++：optional
来源：http://llb.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uhs.yj20258888.top

[S57] C++：编译期常量
来源：http://dpl.cqqwz.cn

constexpr int N = 10;
来源：http://jfl.guowangkeji.top

[S58] C++：命名空间
来源：http://nsy.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://ffw.zycfv.cn

[S59] C++：静态断言
来源：http://epd.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fvt.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://jea.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ouy.zdbjq.cn

================================================================================
来源：http://khc.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ssv.zhijiandao.cn

================================================================================
来源：http://inq.yj20258888.top

[T01] Kotlin：Hello World
来源：http://vfe.xylfe.cn

println("Hello")
来源：http://rgi.9152youxi.cn

[T02] Kotlin：变量
来源：http://sqt.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqe.yj202588.top

[T03] Kotlin：字符串模板
来源：http://bje.shanyushiyangkeji.top

"值: $b"
来源：http://ysq.dashuyun.cn

[T04] Kotlin：空安全
来源：http://iiv.tian-w.cn

val n: String? = null;  n?.length
来源：http://dlw.havefunace.top

[T05] Kotlin：when 表达式
来源：http://dsq.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sar.52xcode.cn

[T06] Kotlin：集合映射
来源：http://qdq.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bai.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://nmw.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tch.zdqjudy.top

[T08] Kotlin：数据类
来源：http://nlj.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://bgn.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://mau.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://upn.havefunace.top

[T10] Kotlin：默认参数
来源：http://wjq.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dfw.zycfv.cn

[T11] Kotlin：协程
来源：http://yll.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tvp.yj20258.top

[T12] Kotlin：解构声明
来源：http://rvk.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://tlk.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://byc.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://egc.ehwqpu.com

[T14] Kotlin：循环
来源：http://aop.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://jwz.tanke756.top

[T15] Kotlin：接口
来源：http://tks.yfazqb.com

interface Shape { fun area(): Double }
来源：http://cwm.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://dur.andypj.xyz

print("Hello")
来源：http://bup.vehdjk.com

[T17] Swift：变量与常量
来源：http://oac.sufxvd.cn

var a = 1;  let b = 2
来源：http://ywo.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://lfe.jinghuilouyu.cn

"值: \(b)"
来源：http://usd.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://yft.zhengqikj.top

if let n = opt { print(n) }
来源：http://piy.zhixingplan.top

[T20] Swift：数组操作
来源：http://ovj.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://txe.xuetiantiany.cn

[T21] Swift：遍历
来源：http://bzf.vehdjk.com

for x in a { print(x) }
来源：http://gkc.havefunace.top

[T22] Swift：字典
来源：http://dwq.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://ggj.wangshuangyany.cn

[T23] Swift：函数
来源：http://pod.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tfn.hongshengwenyu.top

[T24] Swift：闭包
来源：http://ohh.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zjo.andypj.xyz

[T25] Swift：结构体
来源：http://sea.sysykeji.top

struct P { var x: Int }
来源：http://oie.chenzaomai.com

[T26] Swift：类与重写
来源：http://gkf.smart0.xyz

class A: Base { override func f() {} }
来源：http://khh.cqqwz.cn

[T27] Swift：错误处理
来源：http://hug.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://sss.316326.xyz

[T28] Swift：枚举
来源：http://vnz.uphjek.com

enum Color { case red, green }
来源：http://uid.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://gzt.jiagoushi.top

guard let x = opt else { return }
来源：http://wjn.aizwys.cn

[T30] Swift：协议
来源：http://nmb.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://yio.guannengcc.top

[T31] Lua：Hello World
来源：http://gtr.ctjpmb.com

print("Hello")
来源：http://ntp.mhx1999.top

[T32] Lua：局部变量
来源：http://vry.yueranfly.top

local a = 1
来源：http://gmg.hcnkem.com

[T33] Lua：表（数组）
来源：http://pvk.epnwcf.com

local t = {1, 2, 3};  t[4] = 4
来源：http://lli.cashguo.top

[T34] Lua：遍历表
来源：http://adq.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lhy.hnxiangtu.top

[T35] Lua：字典表
来源：http://imj.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://ade.zdbjq.cn

[T36] Lua：函数
来源：http://wso.hnqzz.top

function add(a, b) return a + b end
来源：http://tcv.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://uks.ydzc1.top

"a" .. "b"
来源：http://ciy.9152youxi.cn

[T38] Lua：条件
来源：http://vtg.chenlongwang.top

if x > 0 then print("正") end
来源：http://wwe.svipenyu.cn

[T39] Lua：模式匹配
来源：http://ljo.wangdashe.top

string.find(s, "%d+")
来源：http://wcx.xziqi.cn

[T40] Lua：元表
来源：http://nin.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://mat.guowangkeji.top

[T41] Perl：Hello World
来源：http://rwo.cucudq.cn

print "Hello\n";
来源：http://eix.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://jeq.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lox.birdmap.top

[T43] Perl：字符串插值
来源：http://qfd.aizwys.cn

"值: $a"
来源：http://cyh.hcnkem.com

[T44] Perl：条件
来源：http://wfg.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://liv.yj20258888.top

[T45] Perl：数组遍历
来源：http://ouy.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://vyc.birdmap.top

[T46] Perl：哈希操作
来源：http://xmi.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ubo.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://wnr.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://nqm.cashguo.top

[T48] Perl：正则替换
来源：http://qpv.fengsongda.top

$s =~ s/old/new/g;
来源：http://rpn.redwolf501.top

[T49] Perl：函数
来源：http://bwt.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ccw.gzhubu.top

[T50] Perl：逐行读文件
来源：http://bed.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://hku.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://lzz.cucudq.cn

[T51] Scala：Hello World
来源：http://wdn.redwolf501.top

println("Hello")
来源：http://dna.yuanzhike.top

[T52] Scala：变量
来源：http://tbn.daxiang520.top

val a = 1;  var b = 2
来源：http://doa.bbcook.cn

[T53] Scala：字符串插值
来源：http://xxv.chenjidiqi.icu

s"值: $b"
来源：http://jak.ybcxt.top

[T54] Scala：集合映射
来源：http://aho.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://niu.316326.xyz

[T55] Scala：集合过滤
来源：http://xfy.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://xfo.zhiwuduotai.top

[T56] Scala：样例类
来源：http://bjl.mhx1999.top

case class User(name: String, age: Int)
来源：http://pys.andypj.xyz

[T57] Scala：模式匹配
来源：http://zgg.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gbv.ctjpmb.com

[T58] Scala：函数定义
来源：http://acy.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://vcu.yuanzhike.top

[T59] Scala：循环
来源：http://dbr.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://zkd.hnxiangtu.top

[T60] Scala：折叠
来源：http://lfg.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bkd.tianlin.xyz

================================================================================
来源：http://cpt.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fai.nwbrower.top

================================================================================
来源：http://wfq.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://usu.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://quv.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://vvk.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fih.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://vjj.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rjp.guowangkeji.top

[U04] Py：变量调试打印
来源：http://ibw.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oeb.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://bfn.xuanzx.com

list(dict.fromkeys(arr))
来源：http://ifr.andypj.xyz

[U06] Py：合并两个字典
来源：http://ruo.yuanzhike.top

{**a, **b}
来源：http://ogp.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://kcc.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://zci.jinqigufen.top

[U08] Py：展平二维列表
来源：http://aiz.quarkkingdee.top

[y for x in nested for y in x]
来源：http://ctl.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://kjp.bbcook.cn

max(d, key=d.get)
来源：http://szc.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://qex.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jpx.kuanghao11.cn

[U11] Py：生成器表达式
来源：http://vxh.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://fgk.sxryk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jhh.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://cpz.smart0.xyz

[U13] Py：固定长度队列
来源：http://eqi.jqgfzy.top

deque(maxlen=10)
来源：http://cnb.sxryk.cn

[U14] Py：分组收集到列表
来源：http://lib.ydzc1.top

defaultdict(list)
来源：http://luj.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://tyz.zhiwuduotai.top

t = time.perf_counter()
来源：http://hru.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://zyz.tanke756.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ygo.ybcxt.top

[U17] Py：初始化日志
来源：http://kfl.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://slh.chenlongwang.top

[U18] Py：预编译正则
来源：http://bzr.9152youxi.cn

pat = re.compile(r"\d+")
来源：http://xlx.hcnkem.com

[U19] Py：正则替换带回调
来源：http://jhi.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mag.nwbrower.top

[U20] Py：缓存函数结果
来源：http://jox.smart0.xyz

@functools.lru_cache(maxsize=None)
来源：http://fwx.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://rhv.guowangkeji.top

@contextlib.contextmanager
来源：http://fwy.havefunace.top

[U22] Py：矩阵转置
来源：http://ypz.sufxvd.cn

list(zip(*m))
来源：http://ktx.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://cmf.andypj.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eta.aizwys.cn

[U24] Py：路径操作
来源：http://dun.wangdashe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pkp.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://qvs.aizwys.cn

csv.DictReader(f)
来源：http://twe.shangyingyoupin.top

[U26] Py：并发下载
来源：http://nqe.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jjl.yj20258.top

[U27] Py：异步 HTTP
来源：http://dmq.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://oup.sweek.top

[U28] Py：类型别名
来源：http://ate.sysykeji.top

UserId = int
来源：http://ipt.hesvh.cn

[U29] Py：属性校验
来源：http://jtu.ybcxt.top

@property 与 @x.setter 配合
来源：http://zvv.hywenlv.cn

[U30] Py：数据类
来源：http://ubl.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://via.cqqwz.cn


<!-- 参考信息 -->