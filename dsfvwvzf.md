代发 wailian999

strlen(s)
来源：http://eff.tianlin.xyz

[S06] C：字符串比较
来源：http://mep.vehdjk.com

strcmp(a, b) == 0
来源：http://opa.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://zwc.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ikt.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://ftb.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nbo.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://inq.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bry.jinqigfzy.top

[S10] C：指针与解引用
来源：http://szl.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://fag.hammf.cn

[S11] C：逐行读文件
来源：http://knn.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://tzt.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pby.xuanzx.com

fclose(f);
来源：http://fsd.shangyingyoupin.top

[S12] C：写文件
来源：http://jty.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cjt.yfazqb.com

[S13] C：宏定义
来源：http://ywx.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vgi.hywenlv.cn

[S14] C：枚举
来源：http://ecp.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://afp.yongpay.top

[S15] C：类型转换
来源：http://kmk.pengpengdd.cyou

(double) a / b
来源：http://jcp.shangyingyoupin.top

[S16] C：位操作置位
来源：http://tkg.gotoacloud.top

x |= (1 << 3);
来源：http://ywx.nwbrower.top

[S17] C：安全拼接字符串
来源：http://yyf.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://won.cashguo.top

[S18] C：命令行参数
来源：http://fhz.zhijiandao.cn

int main(int argc, char **argv)
来源：http://yqx.jinqigfzy.top

[S19] C：快速排序
来源：http://mtf.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://njy.nanxuanxn.top

[S20] C：二分查找
来源：http://pkr.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hiz.0kj1m.cn

[S21] C：字符类别判断
来源：http://maw.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jmf.fengsongda.top

[S22] C：字符串转数字
来源：http://mkh.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://igx.yanxiufei.cn

[S23] C：随机数
来源：http://slb.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vvj.shzxlz.cn

[S24] C：获取本地时间
来源：http://kov.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fgs.jqgfzy.top

[S25] C：内存拷贝
来源：http://bfp.yj20258888.top

memcpy(dst, src, n);
来源：http://olj.9152youxi.cn

[S26] C：内存清零
来源：http://quu.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://prk.yuxming.cn

[S27] C：定义常量
来源：http://lxu.hnxiangtu.top

const double PI = 3.14159;
来源：http://tcp.zdbjq.cn

[S28] C：静态变量
来源：http://twk.cucudq.cn

static int counter = 0;
来源：http://cen.zhiwuduotai.top

[S29] C：变参函数
来源：http://uug.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mqf.yongpay.top

[S30] C：头文件保护
来源：http://xpi.tianlin.xyz

#ifndef X_H
来源：http://wqo.zhongyouzk.top

#define X_H
来源：http://rom.hfpthk.cn

#endif
来源：http://ltd.hcnkem.com

[S31] C++：Hello World
来源：http://qjf.ydzc1.top

#include <iostream>
来源：http://eud.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://brm.redwolf501.top

[S32] C++：字符串
来源：http://lvu.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://enh.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://wsj.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aqg.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://eoe.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://snv.zhoulong.xyz

[S35] C++：map
来源：http://wap.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ees.hcnkem.com

[S36] C++：unordered_map
来源：http://mov.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gap.ppjwa.cn

[S37] C++：set
来源：http://nye.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ywh.tanke756.top

[S38] C++：排序
来源：http://ajy.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://doi.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://gcj.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qzw.zhoulong.xyz

[S40] C++：查找元素
来源：http://kcp.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://imr.hammf.cn

[S41] C++：类与构造函数
来源：http://ubg.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ahm.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://mhf.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://iih.ydzc1.top

[S43] C++：智能指针
来源：http://muh.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://nvw.52xcode.cn

[S44] C++：引用传参
来源：http://kpd.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://ozx.yongpay.top

[S45] C++：lambda
来源：http://wyz.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://izb.yvedp.cn

[S46] C++：函数模板
来源：http://nvb.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hnt.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://aqa.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hez.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://kqk.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://vhx.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://uqq.zdbjq.cn

[S49] C++：写文件
来源：http://uag.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nyx.zdqjudy.top

[S50] C++：格式化数字
来源：http://zxu.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uyo.xuanzx.com

[S51] C++：显式类型转换
来源：http://new.cucudq.cn

static_cast<double>(a) / b
来源：http://cqj.yonumen.top

[S52] C++：const 与 noexcept
来源：http://cxg.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://fmy.ivvv.top

[S53] C++：移动语义
来源：http://dth.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://gvl.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://byr.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://orj.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://buw.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://mcy.sysykeji.top

[S56] C++：optional
来源：http://kvo.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mkk.hnqzz.top

[S57] C++：编译期常量
来源：http://rpj.daria6918.cn

constexpr int N = 10;
来源：http://pwg.quarkkingdee.top

[S58] C++：命名空间
来源：http://oht.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://ajg.gzhubu.top

[S59] C++：静态断言
来源：http://yza.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qxo.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://gxb.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://znn.yvedp.cn

================================================================================
来源：http://trp.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tqa.zdqjudy.top

================================================================================
来源：http://yfq.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://lws.zhiwuduotai.top

println("Hello")
来源：http://mle.jlsjyb.cn

[T02] Kotlin：变量
来源：http://kdn.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://awr.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://pno.zhiwuduotai.top

"值: $b"
来源：http://cmy.xuanzx.com

[T04] Kotlin：空安全
来源：http://yxb.316326.xyz

val n: String? = null;  n?.length
来源：http://col.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://eff.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pfg.fehbvm.com

[T06] Kotlin：集合映射
来源：http://dfv.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://utj.hammf.cn

[T07] Kotlin：集合过滤
来源：http://xco.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vsl.hammf.cn

[T08] Kotlin：数据类
来源：http://oqv.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://gwf.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://xef.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://zaq.bbcook.cn

[T10] Kotlin：默认参数
来源：http://fkr.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rhm.xziqi.cn

[T11] Kotlin：协程
来源：http://mdy.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://doi.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://dan.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://yrj.yj202588.top

[T13] Kotlin：只读 Map
来源：http://fro.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://qxo.sweek.top

[T14] Kotlin：循环
来源：http://xbl.316326.xyz

for (i in 1..10) println(i)
来源：http://svd.yanxiufei.cn

[T15] Kotlin：接口
来源：http://unb.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://ngm.hfpthk.cn

[T16] Swift：Hello World
来源：http://uao.pycfn.com

print("Hello")
来源：http://bqu.yuxming.cn

[T17] Swift：变量与常量
来源：http://gnh.daria6918.cn

var a = 1;  let b = 2
来源：http://lcp.cdnleiting.top

[T18] Swift：字符串插值
来源：http://lnh.snrcjt.cn

"值: \(b)"
来源：http://vzo.yueranfly.top

[T19] Swift：可选绑定
来源：http://gex.ehwqpu.com

if let n = opt { print(n) }
来源：http://tsp.zycfv.cn

[T20] Swift：数组操作
来源：http://gap.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tsk.daria6918.cn

[T21] Swift：遍历
来源：http://squ.jiagoushi.top

for x in a { print(x) }
来源：http://hxg.vqdsnc.cn

[T22] Swift：字典
来源：http://bdl.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xpy.nanxuanxn.top

[T23] Swift：函数
来源：http://xqg.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jfu.nwbrower.top

[T24] Swift：闭包
来源：http://oos.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ugm.guannengcc.top

[T25] Swift：结构体
来源：http://myb.haohaochexian.top

struct P { var x: Int }
来源：http://hdy.yanxiufei.cn

[T26] Swift：类与重写
来源：http://hay.havefunace.top

class A: Base { override func f() {} }
来源：http://daz.zhixingplan.top

[T27] Swift：错误处理
来源：http://sak.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://fwk.gogol.net.cn

[T28] Swift：枚举
来源：http://nic.fzhhl.top

enum Color { case red, green }
来源：http://zyl.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://zqg.ydjk.org.cn

guard let x = opt else { return }
来源：http://hwr.gaohongyu789.top

[T30] Swift：协议
来源：http://bve.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://exp.52xcode.cn

[T31] Lua：Hello World
来源：http://xrn.xziqi.cn

print("Hello")
来源：http://nhd.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://ghg.yuanzhike.top

local a = 1
来源：http://pwy.guowangkeji.top

[T33] Lua：表（数组）
来源：http://gyd.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kff.tarul.cn

[T34] Lua：遍历表
来源：http://nzw.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vlt.shzxlz.cn

[T35] Lua：字典表
来源：http://fcr.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://wnm.fehbvm.com

[T36] Lua：函数
来源：http://xpd.epnwcf.com

function add(a, b) return a + b end
来源：http://glg.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://uux.sufxvd.cn

"a" .. "b"
来源：http://fqb.shuidangran.top

[T38] Lua：条件
来源：http://doq.nwbrower.top

if x > 0 then print("正") end
来源：http://kko.xziqi.cn

[T39] Lua：模式匹配
来源：http://dxv.havefunace.top

string.find(s, "%d+")
来源：http://yjr.tarul.cn

[T40] Lua：元表
来源：http://tvl.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://mgz.52xcode.cn

[T41] Perl：Hello World
来源：http://tkp.xuanzx.com

print "Hello\n";
来源：http://rsg.jqgufenzy.top

[T42] Perl：变量类型
来源：http://ufd.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gsw.jiagoushi.top

[T43] Perl：字符串插值
来源：http://vxl.zhongyouzk.top

"值: $a"
来源：http://arw.bbcook.cn

[T44] Perl：条件
来源：http://tbp.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://oqz.hywenlv.cn

[T45] Perl：数组遍历
来源：http://eda.sweek.top

for my $x (@arr) { print $x; }
来源：http://tvf.yj20258888.top

[T46] Perl：哈希操作
来源：http://mej.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hns.jinqigfzy.top

[T47] Perl：正则捕获
来源：http://xhx.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://sqn.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://yvj.hywenlv.cn

$s =~ s/old/new/g;
来源：http://gga.jlsjyb.cn

[T49] Perl：函数
来源：http://ewt.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tsr.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://opz.jqgfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://eky.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://roh.zhongyouzk.top

[T51] Scala：Hello World
来源：http://url.shanyushiyangtech.top

println("Hello")
来源：http://upj.hesvh.cn

[T52] Scala：变量
来源：http://daf.zhengqikj.top

val a = 1;  var b = 2
来源：http://ozx.ivvv.top

[T53] Scala：字符串插值
来源：http://yok.gotoacloud.top

s"值: $b"
来源：http://spz.hongshengwenyu.top

[T54] Scala：集合映射
来源：http://bzn.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://lze.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://jnq.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://mui.vqdsnc.cn

[T56] Scala：样例类
来源：http://szc.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://ryj.52xcode.cn

[T57] Scala：模式匹配
来源：http://yfc.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fst.snrcjt.cn

[T58] Scala：函数定义
来源：http://abo.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vxa.gaohongyu789.top

[T59] Scala：循环
来源：http://cit.316326.xyz

for (i <- 1 to 10) println(i)
来源：http://dvr.0kj1m.cn

[T60] Scala：折叠
来源：http://imk.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ggw.wangshuangyany.cn

================================================================================
来源：http://vkr.sxryk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ecn.hysaishi.cn

================================================================================
来源：http://llb.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://ord.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://bxt.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://jak.hammf.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://akn.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://pod.snrcjt.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fuk.shzxlz.cn

[U04] Py：变量调试打印
来源：http://bip.hongshengwenyu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kod.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://mws.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://qst.snrcjt.cn

[U06] Py：合并两个字典
来源：http://dnl.jlsjyb.cn

{**a, **b}
来源：http://mvb.cheryme.top

[U07] Py：反转字典键值
来源：http://ayf.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://xhc.yangfankeji.com

[U08] Py：展平二维列表
来源：http://ins.sweek.top

[y for x in nested for y in x]
来源：http://ehw.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://cts.hnxiangtu.top

max(d, key=d.get)
来源：http://rac.tarul.cn

[U10] Py：按值排序字典
来源：http://roe.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://odh.xingfuxueyuan.xyz

[U11] Py：生成器表达式
来源：http://lrb.gzhubu.top

(x * 2 for x in arr)
来源：http://uvf.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fcx.hesvh.cn

Counter(arr).most_common(3)
来源：http://deh.gotoacloud.top

[U13] Py：固定长度队列
来源：http://gdj.yuanzhike.top

deque(maxlen=10)
来源：http://iyy.gzhubu.top

[U14] Py：分组收集到列表
来源：http://ryy.zhaomingkeji.xyz

defaultdict(list)
来源：http://pmy.dianchejie.cn

[U15] Py：高精度计时
来源：http://psg.xuetiantiany.cn

t = time.perf_counter()
来源：http://lng.hysaishi.cn

[U16] Py：命令行参数解析
来源：http://cgd.vqdsnc.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://auv.sweek.top

[U17] Py：初始化日志
来源：http://sip.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://dzt.tian-w.cn

[U18] Py：预编译正则
来源：http://nco.nwbrower.top

pat = re.compile(r"\d+")
来源：http://pnj.uphjek.com

[U19] Py：正则替换带回调
来源：http://ayn.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ywa.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://ixh.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://lvv.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://ace.shanyushiyangtech.top

@contextlib.contextmanager
来源：http://msx.ctjpmb.com

[U22] Py：矩阵转置
来源：http://uye.yueranfly.top

list(zip(*m))
来源：http://dxo.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://npj.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xgs.fzhhl.top

[U24] Py：路径操作
来源：http://itm.daria6918.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wsl.hammf.cn

[U25] Py：CSV 按字典读
来源：http://uqm.pengpengdd.cyou

csv.DictReader(f)
来源：http://drx.andypj.xyz

[U26] Py：并发下载
来源：http://dpo.zycfv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://sap.jianghu66.top

[U27] Py：异步 HTTP
来源：http://gss.wangdashe.top

aiohttp.ClientSession() 配合 async with
来源：http://cxa.316326.xyz

[U28] Py：类型别名
来源：http://lur.gaohongyu789.top

UserId = int
来源：http://fkp.epnwcf.com


<!-- 参考信息 -->