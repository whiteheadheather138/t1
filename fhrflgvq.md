代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gxo.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://cph.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eua.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://zfi.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qpk.hammf.cn

[S10] C：指针与解引用
来源：http://lqx.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://wyz.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://ilg.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://dee.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pme.guowangkeji.top

fclose(f);
来源：http://qyj.sufxvd.cn

[S12] C：写文件
来源：http://las.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uzd.fengsongda.top

[S13] C：宏定义
来源：http://flr.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ggv.jyoumei.cn

[S14] C：枚举
来源：http://wrl.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://rdv.jiagoushi.top

[S15] C：类型转换
来源：http://fkx.sysykeji.top

(double) a / b
来源：http://xrg.hesvh.cn

[S16] C：位操作置位
来源：http://zdn.wangdashe.top

x |= (1 << 3);
来源：http://jom.yuxming.cn

[S17] C：安全拼接字符串
来源：http://slm.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qet.c1oappe.top

[S18] C：命令行参数
来源：http://xoo.xinyue.icu

int main(int argc, char **argv)
来源：http://zdd.andypj.xyz

[S19] C：快速排序
来源：http://mzw.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lvb.cashguo.top

[S20] C：二分查找
来源：http://mmi.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xfv.fehbvm.com

[S21] C：字符类别判断
来源：http://sgs.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qpa.xuanzx.com

[S22] C：字符串转数字
来源：http://shd.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://iwq.chenjidiqi.icu

[S23] C：随机数
来源：http://ddn.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pmq.jlsjyb.cn

[S24] C：获取本地时间
来源：http://xdy.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygd.chenzaomai.com

[S25] C：内存拷贝
来源：http://jut.yonumen.top

memcpy(dst, src, n);
来源：http://xiv.zhiwuduotai.top

[S26] C：内存清零
来源：http://kiq.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://wwz.yuxming.cn

[S27] C：定义常量
来源：http://nfc.vqdsnc.cn

const double PI = 3.14159;
来源：http://pwh.pengpengdd.cyou

[S28] C：静态变量
来源：http://frn.guannengcc.top

static int counter = 0;
来源：http://qfy.cdnleiting.top

[S29] C：变参函数
来源：http://hwu.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rhk.jianghu66.top

[S30] C：头文件保护
来源：http://ubq.ydzc1.top

#ifndef X_H
来源：http://nwr.aizwys.cn

#define X_H
来源：http://nqb.cheryme.top

#endif
来源：http://nbf.hcnkem.com

[S31] C++：Hello World
来源：http://dje.chenlongwang.top

#include <iostream>
来源：http://hfb.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://ddr.shuidangran.top

[S32] C++：字符串
来源：http://xlb.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://ekk.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://knl.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bck.redwolf501.top

[S34] C++：遍历 vector
来源：http://jbv.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://tfx.meibo888.top

[S35] C++：map
来源：http://bzw.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kmf.fktsv.cn

[S36] C++：unordered_map
来源：http://ztw.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aoo.hcnkem.com

[S37] C++：set
来源：http://kfb.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lek.jiagoushi.top

[S38] C++：排序
来源：http://vyu.tarul.cn

std::sort(v.begin(), v.end());
来源：http://zgw.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://ine.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bok.yongpay.top

[S40] C++：查找元素
来源：http://hav.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xef.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://owj.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nbh.sysykeji.top

[S42] C++：继承与虚函数
来源：http://lvm.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://oqr.gogol.net.cn

[S43] C++：智能指针
来源：http://iak.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://qce.dashuyun.cn

[S44] C++：引用传参
来源：http://akt.cucudq.cn

void inc(int &x) { ++x; }
来源：http://wzl.xinyue.icu

[S45] C++：lambda
来源：http://yhv.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yti.yonumen.top

[S46] C++：函数模板
来源：http://opw.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xbg.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://fip.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hpg.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://fpp.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://iew.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ncz.hammf.cn

[S49] C++：写文件
来源：http://pgv.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gkk.fzhhl.top

[S50] C++：格式化数字
来源：http://tuk.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jio.sysykeji.top

[S51] C++：显式类型转换
来源：http://iog.jinqigufen.top

static_cast<double>(a) / b
来源：http://pbk.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://vwe.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://wox.bjfxy.top

[S53] C++：移动语义
来源：http://cjm.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://ozh.ppjwa.cn

[S54] C++：异常处理
来源：http://flc.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uwd.yfazqb.com

[S55] C++：结构化绑定
来源：http://kvd.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wbe.shanyushiyangtech.top

[S56] C++：optional
来源：http://wou.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bsg.svipenyu.cn

[S57] C++：编译期常量
来源：http://uyg.haohaochexian.top

constexpr int N = 10;
来源：http://mcw.jianghu66.top

[S58] C++：命名空间
来源：http://cnz.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://ldx.dashuyun.cn

[S59] C++：静态断言
来源：http://azf.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dts.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://zzs.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wpn.zhengqikj.top

================================================================================
来源：http://uwv.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljx.hfpthk.cn

================================================================================
来源：http://hqs.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://acd.hnxiangtu.top

println("Hello")
来源：http://nog.jinqigfzy.top

[T02] Kotlin：变量
来源：http://mgj.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rep.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://ikh.cheryme.top

"值: $b"
来源：http://cxm.xuanzx.com

[T04] Kotlin：空安全
来源：http://eqj.ctjpmb.com

val n: String? = null;  n?.length
来源：http://eln.ivvv.top

[T05] Kotlin：when 表达式
来源：http://llq.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tlp.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://hui.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jch.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://mfb.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qmk.cheryme.top

[T08] Kotlin：数据类
来源：http://wot.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://dlc.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://ddh.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://kyn.guannengcc.top

[T10] Kotlin：默认参数
来源：http://xcl.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ujv.tianlin.xyz

[T11] Kotlin：协程
来源：http://baw.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xme.cashguo.top

[T12] Kotlin：解构声明
来源：http://rcf.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://obe.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://qyz.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://udc.jlsjyb.cn

[T14] Kotlin：循环
来源：http://fwv.bbcook.cn

for (i in 1..10) println(i)
来源：http://tyh.guowangkeji.top

[T15] Kotlin：接口
来源：http://idz.redwolf501.top

interface Shape { fun area(): Double }
来源：http://ltl.tanke756.top

[T16] Swift：Hello World
来源：http://ysx.ppjwa.cn

print("Hello")
来源：http://qxh.chenlongwang.top

[T17] Swift：变量与常量
来源：http://gby.jqgufenzy.top

var a = 1;  let b = 2
来源：http://hcr.guowangkeji.top

[T18] Swift：字符串插值
来源：http://ulr.zhoulong.xyz

"值: \(b)"
来源：http://fzx.dashuyun.cn

[T19] Swift：可选绑定
来源：http://fyr.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://dwj.zhixingplan.top

[T20] Swift：数组操作
来源：http://afo.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://imy.ybcxt.top

[T21] Swift：遍历
来源：http://qtj.jqgufenzy.top

for x in a { print(x) }
来源：http://xvs.aizwys.cn

[T22] Swift：字典
来源：http://gau.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://noq.shanyushiyangtech.top

[T23] Swift：函数
来源：http://mcn.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tlj.xinyue.icu

[T24] Swift：闭包
来源：http://ais.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://giy.zdqjudy.top

[T25] Swift：结构体
来源：http://kse.fehbvm.com

struct P { var x: Int }
来源：http://wli.yvedp.cn

[T26] Swift：类与重写
来源：http://zol.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://njz.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://nym.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://mze.cdnleiting.top

[T28] Swift：枚举
来源：http://nou.kuanghao11.cn

enum Color { case red, green }
来源：http://wvv.pengpengdd.cyou

[T29] Swift：guard 提前返回
来源：http://yyc.iojbl.cn

guard let x = opt else { return }
来源：http://syb.andypj.xyz

[T30] Swift：协议
来源：http://huy.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://ohu.gogol.net.cn

[T31] Lua：Hello World
来源：http://kyy.pycfn.com

print("Hello")
来源：http://spp.9152youxi.cn

[T32] Lua：局部变量
来源：http://nsg.ywan-chungtsiang.top

local a = 1
来源：http://yjj.uphjek.com

[T33] Lua：表（数组）
来源：http://yhe.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qed.aizwys.cn

[T34] Lua：遍历表
来源：http://dql.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xfd.pycfn.com

[T35] Lua：字典表
来源：http://afx.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://miq.bbcook.cn

[T36] Lua：函数
来源：http://ypp.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://mdd.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://cay.shangyingyoupin.top

"a" .. "b"
来源：http://bip.aizwys.cn

[T38] Lua：条件
来源：http://zcu.yuanzhike.top

if x > 0 then print("正") end
来源：http://ghk.gogol.net.cn

[T39] Lua：模式匹配
来源：http://ese.zhixingplan.top

string.find(s, "%d+")
来源：http://ejo.bbcook.cn

[T40] Lua：元表
来源：http://rad.birdmap.top

setmetatable({}, { __index = base })
来源：http://cno.epnwcf.com

[T41] Perl：Hello World
来源：http://ddx.bbcook.cn

print "Hello\n";
来源：http://sqz.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://bkp.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mil.daria6918.cn

[T43] Perl：字符串插值
来源：http://rrm.jinqigfzy.top

"值: $a"
来源：http://jpy.daxiang520.top

[T44] Perl：条件
来源：http://fus.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://rxq.zdbjq.cn

[T45] Perl：数组遍历
来源：http://ifk.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://nnp.zhixingplan.top

[T46] Perl：哈希操作
来源：http://ake.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hze.svipenyu.cn

[T47] Perl：正则捕获
来源：http://jpu.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sho.yangfankeji.com

[T48] Perl：正则替换
来源：http://pii.yvedp.cn

$s =~ s/old/new/g;
来源：http://mji.9152youxi.cn

[T49] Perl：函数
来源：http://nhu.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dsb.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://lnv.fanxiaobao.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://pcs.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://mky.tarul.cn

[T51] Scala：Hello World
来源：http://kts.daria6918.cn

println("Hello")
来源：http://cug.dianchejie.cn

[T52] Scala：变量
来源：http://ahu.gogol.net.cn

val a = 1;  var b = 2
来源：http://try.vehdjk.com

[T53] Scala：字符串插值
来源：http://ahy.cheryme.top

s"值: $b"
来源：http://ylp.ydzc1.top

[T54] Scala：集合映射
来源：http://gye.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://lin.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://dty.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://mmz.hesvh.cn

[T56] Scala：样例类
来源：http://wvi.zhixingplan.top

case class User(name: String, age: Int)
来源：http://obe.cashguo.top

[T57] Scala：模式匹配
来源：http://rix.hnxiangtu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kjz.aibaodan.cn

[T58] Scala：函数定义
来源：http://xxx.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://scp.chenjidiqi.icu

[T59] Scala：循环
来源：http://zjy.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://dco.0kj1m.cn

[T60] Scala：折叠
来源：http://kzb.pycfn.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wrh.fktsv.cn

================================================================================
来源：http://dyz.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://srp.daria6918.cn

================================================================================
来源：http://hos.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://lva.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://tuk.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://uxp.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtf.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://gqh.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://uwd.cqqwz.cn

[U04] Py：变量调试打印
来源：http://aeg.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nui.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://zff.yueranfly.top

list(dict.fromkeys(arr))
来源：http://rip.zdbjq.cn

[U06] Py：合并两个字典
来源：http://rhk.xylfe.cn

{**a, **b}
来源：http://uia.chenlongwang.top

[U07] Py：反转字典键值
来源：http://npy.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://obe.gzhubu.top

[U08] Py：展平二维列表
来源：http://htn.zhengqikj.top

[y for x in nested for y in x]
来源：http://ufs.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://mac.ppjwa.cn

max(d, key=d.get)
来源：http://gke.sysykeji.top

[U10] Py：按值排序字典
来源：http://qyt.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lhe.zhixingplan.top

[U11] Py：生成器表达式
来源：http://iqf.redwolf501.top

(x * 2 for x in arr)
来源：http://dof.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://wcm.fzhhl.top

Counter(arr).most_common(3)
来源：http://qlf.uphjek.com

[U13] Py：固定长度队列
来源：http://mcq.daria6918.cn

deque(maxlen=10)
来源：http://ajs.yongpay.top

[U14] Py：分组收集到列表
来源：http://lmi.sweek.top

defaultdict(list)
来源：http://gev.shuidangran.top

[U15] Py：高精度计时
来源：http://ful.zhengqikj.top

t = time.perf_counter()
来源：http://gwd.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://lyn.kuanghao11.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uwd.fehbvm.com

[U17] Py：初始化日志
来源：http://ake.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://ibm.xuanzx.com

[U18] Py：预编译正则
来源：http://ukw.hnxiangtu.top

pat = re.compile(r"\d+")
来源：http://afl.nwbrower.top

[U19] Py：正则替换带回调
来源：http://oke.jinqigufen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://taf.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://yji.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://yzf.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://yet.birdmap.top

@contextlib.contextmanager
来源：http://zyq.daxiang520.top

[U22] Py：矩阵转置
来源：http://tnk.hfpthk.cn

list(zip(*m))
来源：http://zgj.fanxiaobao.xyz

[U23] Py：分块读取大文件
来源：http://bng.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://opo.fktsv.cn

[U24] Py：路径操作
来源：http://crt.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://waf.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://plp.zdqjudy.top

csv.DictReader(f)
来源：http://cjf.gogol.net.cn

[U26] Py：并发下载
来源：http://xmq.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tjk.birdmap.top

[U27] Py：异步 HTTP
来源：http://kiw.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://muy.bbcook.cn

[U28] Py：类型别名
来源：http://ser.hysaishi.cn

UserId = int
来源：http://ceg.gogol.net.cn

[U29] Py：属性校验
来源：http://csb.jinqigufen.top

@property 与 @x.setter 配合
来源：http://pwh.cashguo.top

[U30] Py：数据类
来源：http://uwr.guannengcc.top

@dataclass(slots=True)
来源：http://wgf.fehbvm.com


<!-- 参考信息 -->