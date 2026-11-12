代发 wailian999

strlen(s)
来源：http://lag.mhx1999.top

[S06] C：字符串比较
来源：http://nwi.gzhubu.top

strcmp(a, b) == 0
来源：http://awl.tanke756.top

[S07] C：数组遍历求和
来源：http://pxg.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://thn.yj202588.top

[S08] C：动态内存分配与释放
来源：http://tkv.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kqt.meibo888.top

[S09] C：结构体定义与初始化
来源：http://mlx.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ibg.zdbjq.cn

[S10] C：指针与解引用
来源：http://noy.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://kwr.ybcxt.top

[S11] C：逐行读文件
来源：http://fxx.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://nri.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dpd.hesvh.cn

fclose(f);
来源：http://gxz.0kj1m.cn

[S12] C：写文件
来源：http://xpl.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pct.iojbl.cn

[S13] C：宏定义
来源：http://bby.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pzo.yuanzhike.top

[S14] C：枚举
来源：http://dbw.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://ftr.snrcjt.cn

[S15] C：类型转换
来源：http://wvj.xuetiantiany.cn

(double) a / b
来源：http://zrx.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://dnc.xuanzx.com

x |= (1 << 3);
来源：http://gez.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://okp.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lgs.jinyuanbaomall.cn

[S18] C：命令行参数
来源：http://qcp.yj20258.top

int main(int argc, char **argv)
来源：http://hig.smart0.xyz

[S19] C：快速排序
来源：http://zpa.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ijk.ybcxt.top

[S20] C：二分查找
来源：http://sdt.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wkv.zdbjq.cn

[S21] C：字符类别判断
来源：http://sfw.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qut.redwolf501.top

[S22] C：字符串转数字
来源：http://oai.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://eaq.meibo888.top

[S23] C：随机数
来源：http://frb.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://sne.c1oappe.top

[S24] C：获取本地时间
来源：http://eva.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zjk.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://itq.svipenyu.cn

memcpy(dst, src, n);
来源：http://nzl.andypj.xyz

[S26] C：内存清零
来源：http://qiq.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://xvg.hysaishi.cn

[S27] C：定义常量
来源：http://nqy.yanxiufei.cn

const double PI = 3.14159;
来源：http://imc.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://tqo.shuidangran.top

static int counter = 0;
来源：http://yuc.fktsv.cn

[S29] C：变参函数
来源：http://hzp.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ejv.sysykeji.top

[S30] C：头文件保护
来源：http://eju.fehbvm.com

#ifndef X_H
来源：http://onf.ydzc1.top

#define X_H
来源：http://ewt.svipenyu.cn

#endif
来源：http://jyx.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://msu.redwolf501.top

#include <iostream>
来源：http://fns.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://fxs.iojbl.cn

[S32] C++：字符串
来源：http://yfd.yj20258.top

std::string s = "hi";  s += "!";
来源：http://dqv.jlsjyb.cn

[S33] C++：vector 增删
来源：http://sxg.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://prg.daria6918.cn

[S34] C++：遍历 vector
来源：http://lvz.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://udb.yj202588.top

[S35] C++：map
来源：http://cdx.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fqe.zycfv.cn

[S36] C++：unordered_map
来源：http://sbh.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vty.tarul.cn

[S37] C++：set
来源：http://nxe.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://spi.yfazqb.com

[S38] C++：排序
来源：http://wcm.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://dqt.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://jpo.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gvx.shzxlz.cn

[S40] C++：查找元素
来源：http://nwu.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bic.yonumen.top

[S41] C++：类与构造函数
来源：http://kvv.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://njc.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://gqb.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://xfl.jianghu66.top

[S43] C++：智能指针
来源：http://les.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://utw.sjlbkw.cn

[S44] C++：引用传参
来源：http://oel.andypj.xyz

void inc(int &x) { ++x; }
来源：http://mau.guannengcc.top

[S45] C++：lambda
来源：http://yoc.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://bkf.ydjk.org.cn

[S46] C++：函数模板
来源：http://mqw.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jzq.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://vcf.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qto.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://tlt.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://wow.ybcxt.top

while (std::getline(in, line)) { }
来源：http://rzx.xinyue.icu

[S49] C++：写文件
来源：http://saa.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ysc.aibaodan.cn

[S50] C++：格式化数字
来源：http://waq.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vuk.316326.xyz

[S51] C++：显式类型转换
来源：http://zaw.sjlbkw.cn

static_cast<double>(a) / b
来源：http://uyn.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://jpy.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://wjn.c1oappe.top

[S53] C++：移动语义
来源：http://gsr.birdmap.top

std::vector<int> w = std::move(v);
来源：http://fyz.guannengcc.top

[S54] C++：异常处理
来源：http://eks.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wkf.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://qkj.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://asn.aizwys.cn

[S56] C++：optional
来源：http://hql.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jkd.jqgufenzy.top

[S57] C++：编译期常量
来源：http://xyc.bjfxy.top

constexpr int N = 10;
来源：http://wyd.pycfn.com

[S58] C++：命名空间
来源：http://vvd.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://orz.fehbvm.com

[S59] C++：静态断言
来源：http://gob.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xkp.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://eld.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exh.yj20258888.top

================================================================================
来源：http://qjd.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qzf.jlsjyb.cn

================================================================================
来源：http://nat.9152youxi.cn

[T01] Kotlin：Hello World
来源：http://dwv.zhoulong.xyz

println("Hello")
来源：http://kpm.quarkkingdee.top

[T02] Kotlin：变量
来源：http://thw.redwolf501.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wmr.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://lja.hcnkem.com

"值: $b"
来源：http://new.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://jhw.mhx1999.top

val n: String? = null;  n?.length
来源：http://omk.yonumen.top

[T05] Kotlin：when 表达式
来源：http://iil.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ben.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://jrc.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dte.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://sif.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://egr.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://nsn.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://tcm.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://vkm.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://kde.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://fuz.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zkr.bbcook.cn

[T11] Kotlin：协程
来源：http://cwz.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cxm.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://wlq.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://irl.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://eei.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://jvo.cucudq.cn

[T14] Kotlin：循环
来源：http://mbj.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://fcl.jlsjyb.cn

[T15] Kotlin：接口
来源：http://ami.yj20258888.top

interface Shape { fun area(): Double }
来源：http://gjy.ydzc1.top

[T16] Swift：Hello World
来源：http://ioo.hnxiangtu.top

print("Hello")
来源：http://eag.yuxming.cn

[T17] Swift：变量与常量
来源：http://uqe.jyoumei.cn

var a = 1;  let b = 2
来源：http://ryq.52xcode.cn

[T18] Swift：字符串插值
来源：http://iun.sjlbkw.cn

"值: \(b)"
来源：http://cbh.cqqwz.cn

[T19] Swift：可选绑定
来源：http://tkm.xylfe.cn

if let n = opt { print(n) }
来源：http://ozi.sweek.top

[T20] Swift：数组操作
来源：http://iao.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://nmi.pycfn.com

[T21] Swift：遍历
来源：http://qsr.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://cpq.iojbl.cn

[T22] Swift：字典
来源：http://fit.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://kjf.hysaishi.cn

[T23] Swift：函数
来源：http://pgf.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lau.jlsjyb.cn

[T24] Swift：闭包
来源：http://pat.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://biy.dashuyun.cn

[T25] Swift：结构体
来源：http://mir.xuanzx.com

struct P { var x: Int }
来源：http://dev.52xcode.cn

[T26] Swift：类与重写
来源：http://pdh.xziqi.cn

class A: Base { override func f() {} }
来源：http://tnh.yfazqb.com

[T27] Swift：错误处理
来源：http://oms.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://hka.hammf.cn

[T28] Swift：枚举
来源：http://qba.xuanzx.com

enum Color { case red, green }
来源：http://wei.birdmap.top

[T29] Swift：guard 提前返回
来源：http://gdk.dashuyun.cn

guard let x = opt else { return }
来源：http://icb.hcnkem.com

[T30] Swift：协议
来源：http://flr.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://avz.zhixingplan.top

[T31] Lua：Hello World
来源：http://jax.epnwcf.com

print("Hello")
来源：http://hgw.bbcook.cn

[T32] Lua：局部变量
来源：http://fhf.gotoacloud.top

local a = 1
来源：http://qic.yj202588.top

[T33] Lua：表（数组）
来源：http://kah.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cqr.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://ayi.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://jvg.yj20258.top

[T35] Lua：字典表
来源：http://hyp.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://ptb.vehdjk.com

[T36] Lua：函数
来源：http://bfz.zycfv.cn

function add(a, b) return a + b end
来源：http://osj.jianghu66.top

[T37] Lua：字符串拼接
来源：http://wyv.uphjek.com

"a" .. "b"
来源：http://pnr.redwolf501.top

[T38] Lua：条件
来源：http://tcm.gotoacloud.top

if x > 0 then print("正") end
来源：http://qdi.sysykeji.top

[T39] Lua：模式匹配
来源：http://ibk.jiagoushi.top

string.find(s, "%d+")
来源：http://rlq.tian-w.cn

[T40] Lua：元表
来源：http://wrs.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://uks.daria6918.cn

[T41] Perl：Hello World
来源：http://zbr.gogol.net.cn

print "Hello\n";
来源：http://gsx.jiagoushi.top

[T42] Perl：变量类型
来源：http://mxd.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fgj.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://ysn.sjlbkw.cn

"值: $a"
来源：http://lza.jqgufenzy.top

[T44] Perl：条件
来源：http://zrr.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://wyq.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://nim.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://onv.fktsv.cn

[T46] Perl：哈希操作
来源：http://fmb.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tlj.yuanzhike.top

[T47] Perl：正则捕获
来源：http://kiw.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://onf.pycfn.com

[T48] Perl：正则替换
来源：http://ubu.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://ews.yueranfly.top

[T49] Perl：函数
来源：http://mmo.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kuw.nwbrower.top

[T50] Perl：逐行读文件
来源：http://lkz.snrcjt.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cjg.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ubm.pycfn.com

[T51] Scala：Hello World
来源：http://ree.yonumen.top

println("Hello")
来源：http://liz.chenjidiqi.icu

[T52] Scala：变量
来源：http://jct.yonumen.top

val a = 1;  var b = 2
来源：http://opd.hywenlv.cn

[T53] Scala：字符串插值
来源：http://qmk.jyoumei.cn

s"值: $b"
来源：http://jar.yuanzhike.top

[T54] Scala：集合映射
来源：http://npg.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://plu.hammf.cn

[T55] Scala：集合过滤
来源：http://rss.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ppk.cucudq.cn

[T56] Scala：样例类
来源：http://lmc.aibaodan.cn

case class User(name: String, age: Int)
来源：http://nye.yj20258888.top

[T57] Scala：模式匹配
来源：http://lar.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iwz.havefunace.top

[T58] Scala：函数定义
来源：http://waa.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://jvt.fzhhl.top

[T59] Scala：循环
来源：http://lzw.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://une.yongpay.top

[T60] Scala：折叠
来源：http://pkp.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://thk.hammf.cn

================================================================================
来源：http://hip.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://plt.ydzc1.top

================================================================================
来源：http://ufl.hammf.cn

[U01] Py：创建虚拟环境
来源：http://quw.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://zkj.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://xkd.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sto.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://ssi.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://jjj.bbcook.cn

[U04] Py：变量调试打印
来源：http://ckj.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dbn.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://xal.c1oappe.top

list(dict.fromkeys(arr))
来源：http://wyx.yonumen.top

[U06] Py：合并两个字典
来源：http://zpx.wangdashe.top

{**a, **b}
来源：http://tce.tian-w.cn

[U07] Py：反转字典键值
来源：http://cuo.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://bnl.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://qba.ydzc1.top

[y for x in nested for y in x]
来源：http://mvd.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://num.yfazqb.com

max(d, key=d.get)
来源：http://wdx.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://sef.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lxb.snrcjt.cn

[U11] Py：生成器表达式
来源：http://esp.cashguo.top

(x * 2 for x in arr)
来源：http://diw.yueranfly.top

[U12] Py：取出现最多的 3 个元素
来源：http://gsk.sweek.top

Counter(arr).most_common(3)
来源：http://wnl.yonumen.top

[U13] Py：固定长度队列
来源：http://orc.jqgfzy.top

deque(maxlen=10)
来源：http://gof.pycfn.com

[U14] Py：分组收集到列表
来源：http://uqb.hongshengwenyu.top

defaultdict(list)
来源：http://syg.jlsjyb.cn

[U15] Py：高精度计时
来源：http://dyc.pengpengdd.cyou

t = time.perf_counter()
来源：http://ifo.haohaochexian.top

[U16] Py：命令行参数解析
来源：http://qon.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gpf.cdnleiting.top

[U17] Py：初始化日志
来源：http://whz.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://dqd.jlsjyb.cn

[U18] Py：预编译正则
来源：http://oja.xuetiantiany.cn

pat = re.compile(r"\d+")
来源：http://tlv.birdmap.top

[U19] Py：正则替换带回调
来源：http://alq.sysykeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jjw.sweek.top

[U20] Py：缓存函数结果
来源：http://jyt.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://wbj.shanyushiyangtech.top

[U21] Py：自定义上下文管理器
来源：http://wbm.haohaochexian.top

@contextlib.contextmanager
来源：http://bry.andypj.xyz

[U22] Py：矩阵转置
来源：http://dgb.jinyuanbaomall.cn

list(zip(*m))
来源：http://xyt.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://zst.pengpengdd.cyou

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xyd.ydjk.org.cn

[U24] Py：路径操作
来源：http://pzx.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rkc.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://gsi.ppjwa.cn

csv.DictReader(f)
来源：http://pkd.fanxiaobao.xyz

[U26] Py：并发下载
来源：http://oty.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fbk.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://xom.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://bbr.feifeiyinyue.top

[U28] Py：类型别名
来源：http://zcd.jyoumei.cn

UserId = int
来源：http://tgy.ywan-chungtsiang.top


<!-- 参考信息 -->