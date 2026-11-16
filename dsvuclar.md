代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://pfx.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://huz.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://mve.hnqzz.top

[S03] C：读入整数
来源：http://kqo.snrcjt.cn

int x; scanf("%d", &x);
来源：http://lea.ivvv.top

[S04] C：字符串复制
来源：http://exq.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://evo.fzhhl.top

[S05] C：字符串长度
来源：http://yfw.pengpengdd.cyou

strlen(s)
来源：http://aag.quarkkingdee.top

[S06] C：字符串比较
来源：http://wyt.fzhhl.top

strcmp(a, b) == 0
来源：http://gae.fehbvm.com

[S07] C：数组遍历求和
来源：http://sxu.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kpd.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://arf.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qex.tarul.cn

[S09] C：结构体定义与初始化
来源：http://omh.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gur.cdnleiting.top

[S10] C：指针与解引用
来源：http://zpw.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://kpj.xinyue.icu

[S11] C：逐行读文件
来源：http://awf.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://bds.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://vii.sufxvd.cn

fclose(f);
来源：http://nig.yanxiufei.cn

[S12] C：写文件
来源：http://rjb.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://inu.vehdjk.com

[S13] C：宏定义
来源：http://oly.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmp.gogol.net.cn

[S14] C：枚举
来源：http://ezj.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://njp.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://edh.jianghu66.top

(double) a / b
来源：http://nfn.daxiang520.top

[S16] C：位操作置位
来源：http://pdi.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://mvd.yj20258888.top

[S17] C：安全拼接字符串
来源：http://ybn.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yhm.bjfxy.top

[S18] C：命令行参数
来源：http://cfh.hcnkem.com

int main(int argc, char **argv)
来源：http://efl.cucudq.cn

[S19] C：快速排序
来源：http://geo.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dtk.tianlin.xyz

[S20] C：二分查找
来源：http://swt.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zxa.bjfxy.top

[S21] C：字符类别判断
来源：http://cuf.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rcf.316326.xyz

[S22] C：字符串转数字
来源：http://ajf.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://rhj.shangyingyoupin.top

[S23] C：随机数
来源：http://ksx.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uhb.kuanghao11.cn

[S24] C：获取本地时间
来源：http://zeq.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eir.jinqigfzy.top

[S25] C：内存拷贝
来源：http://usz.tian-w.cn

memcpy(dst, src, n);
来源：http://apq.jqgfzy.top

[S26] C：内存清零
来源：http://hge.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://kca.svipenyu.cn

[S27] C：定义常量
来源：http://ptw.smart0.xyz

const double PI = 3.14159;
来源：http://jho.ydjk.org.cn

[S28] C：静态变量
来源：http://sli.nanxuanxn.top

static int counter = 0;
来源：http://sdd.yueranfly.top

[S29] C：变参函数
来源：http://bis.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aed.zhijiandao.cn

[S30] C：头文件保护
来源：http://dqp.jinqigufen.top

#ifndef X_H
来源：http://giz.zhixingplan.top

#define X_H
来源：http://gni.hysaishi.cn

#endif
来源：http://wll.yanxiufei.cn

[S31] C++：Hello World
来源：http://lpx.hesvh.cn

#include <iostream>
来源：http://erj.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://kmw.cashguo.top

[S32] C++：字符串
来源：http://cpt.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://xul.yuanzhike.top

[S33] C++：vector 增删
来源：http://kfi.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rph.yueranfly.top

[S34] C++：遍历 vector
来源：http://jwj.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://xrs.aibaodan.cn

[S35] C++：map
来源：http://glg.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xpq.ehwqpu.com

[S36] C++：unordered_map
来源：http://zqa.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ofp.uphjek.com

[S37] C++：set
来源：http://rgd.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lba.yj20258.top

[S38] C++：排序
来源：http://lyo.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://djn.uphjek.com

[S39] C++：自定义比较器排序
来源：http://jzi.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iwi.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://uzo.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahq.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://ylw.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zdp.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://lds.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://zjd.mhx1999.top

[S43] C++：智能指针
来源：http://xhs.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://voo.nanxuanxn.top

[S44] C++：引用传参
来源：http://vxz.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://bii.jlsjyb.cn

[S45] C++：lambda
来源：http://kgd.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://jav.xinyue.icu

[S46] C++：函数模板
来源：http://uwb.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mfb.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://ygr.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zna.sysykeji.top

[S48] C++：逐行读文件
来源：http://fcy.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://wvi.smart0.xyz

while (std::getline(in, line)) { }
来源：http://dup.redwolf501.top

[S49] C++：写文件
来源：http://dwx.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yic.ppjwa.cn

[S50] C++：格式化数字
来源：http://xhl.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iuc.tian-w.cn

[S51] C++：显式类型转换
来源：http://lps.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://pbo.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://jsu.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://gxf.jlsjyb.cn

[S53] C++：移动语义
来源：http://umn.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://oas.ydzc1.top

[S54] C++：异常处理
来源：http://axx.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bst.zhengqikj.top

[S55] C++：结构化绑定
来源：http://cvz.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ivd.havefunace.top

[S56] C++：optional
来源：http://izo.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fkb.yanxiufei.cn

[S57] C++：编译期常量
来源：http://hts.xuetiantiany.cn

constexpr int N = 10;
来源：http://vab.gogol.net.cn

[S58] C++：命名空间
来源：http://nts.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://tso.fehbvm.com

[S59] C++：静态断言
来源：http://heo.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fpo.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://pdz.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cpv.aibaodan.cn

================================================================================
来源：http://sly.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vvd.daria6918.cn

================================================================================
来源：http://mom.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://dlq.yj20258888.top

println("Hello")
来源：http://eqr.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://hgr.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://liw.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://mkk.aizwys.cn

"值: $b"
来源：http://mrp.dashuyun.cn

[T04] Kotlin：空安全
来源：http://oar.fehbvm.com

val n: String? = null;  n?.length
来源：http://mtq.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://yqf.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tiq.bbcook.cn

[T06] Kotlin：集合映射
来源：http://vpt.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qun.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://wkt.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dts.yangfankeji.com

[T08] Kotlin：数据类
来源：http://qjv.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://jib.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://lbm.yonumen.top

fun String.exclaim() = this + "!"
来源：http://kpi.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://rss.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sty.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://jxc.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oph.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://pjn.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://syn.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://zun.nwbrower.top

val m = mapOf("a" to 1)
来源：http://rol.zhoulong.xyz

[T14] Kotlin：循环
来源：http://byz.shzxlz.cn

for (i in 1..10) println(i)
来源：http://yto.vehdjk.com

[T15] Kotlin：接口
来源：http://jwu.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://ycx.iojbl.cn

[T16] Swift：Hello World
来源：http://aef.fktsv.cn

print("Hello")
来源：http://nof.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://pnb.xinyue.icu

var a = 1;  let b = 2
来源：http://yoy.gzhubu.top

[T18] Swift：字符串插值
来源：http://shu.c1oappe.top

"值: \(b)"
来源：http://cxa.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://aco.yj20258.top

if let n = opt { print(n) }
来源：http://gwk.xuanzx.com

[T20] Swift：数组操作
来源：http://fai.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cwz.shuidangran.top

[T21] Swift：遍历
来源：http://rzx.9152youxi.cn

for x in a { print(x) }
来源：http://hmb.shangyingyoupin.top

[T22] Swift：字典
来源：http://eyg.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://hwk.fengsongda.top

[T23] Swift：函数
来源：http://koh.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zux.birdmap.top

[T24] Swift：闭包
来源：http://uoq.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://zfl.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://moe.zhengqikj.top

struct P { var x: Int }
来源：http://jny.jqgufenzy.top

[T26] Swift：类与重写
来源：http://mid.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://tmv.chenzaomai.com

[T27] Swift：错误处理
来源：http://hbm.hammf.cn

do { try f() } catch { print(error) }
来源：http://qme.iojbl.cn

[T28] Swift：枚举
来源：http://boa.yfazqb.com

enum Color { case red, green }
来源：http://axl.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://pts.jqgufenzy.top

guard let x = opt else { return }
来源：http://iri.ctjpmb.com

[T30] Swift：协议
来源：http://awj.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://wvz.yfazqb.com

[T31] Lua：Hello World
来源：http://eho.jlsjyb.cn

print("Hello")
来源：http://czf.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://frh.jinghuilouyu.cn

local a = 1
来源：http://ane.fengsongda.top

[T33] Lua：表（数组）
来源：http://gzb.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://say.hnxiangtu.top

[T34] Lua：遍历表
来源：http://kgb.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://nxn.hnxiangtu.top

[T35] Lua：字典表
来源：http://jjm.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://ixi.snrcjt.cn

[T36] Lua：函数
来源：http://ffm.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://mmc.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://hac.bbcook.cn

"a" .. "b"
来源：http://nyr.zhoulong.xyz

[T38] Lua：条件
来源：http://jpy.ehwqpu.com

if x > 0 then print("正") end
来源：http://kiw.fehbvm.com

[T39] Lua：模式匹配
来源：http://oqj.jianghu66.top

string.find(s, "%d+")
来源：http://vrf.tanke756.top

[T40] Lua：元表
来源：http://nyp.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://eqq.tianlin.xyz

[T41] Perl：Hello World
来源：http://auh.jlsjyb.cn

print "Hello\n";
来源：http://oqi.jqgufenzy.top

[T42] Perl：变量类型
来源：http://dei.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lli.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://uvy.xuanzx.com

"值: $a"
来源：http://znk.ivvv.top

[T44] Perl：条件
来源：http://ifm.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://xdl.andypj.xyz

[T45] Perl：数组遍历
来源：http://wqz.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://wlz.snrcjt.cn

[T46] Perl：哈希操作
来源：http://zrs.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bpk.316326.xyz

[T47] Perl：正则捕获
来源：http://yut.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rjg.cucudq.cn

[T48] Perl：正则替换
来源：http://hkh.bbcook.cn

$s =~ s/old/new/g;
来源：http://ohl.yanxiufei.cn

[T49] Perl：函数
来源：http://yma.tarul.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nww.aizwys.cn

[T50] Perl：逐行读文件
来源：http://dym.daria6918.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wyt.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://egp.ivvv.top

[T51] Scala：Hello World
来源：http://lko.chenlongwang.top

println("Hello")
来源：http://pve.sufxvd.cn

[T52] Scala：变量
来源：http://son.hfpthk.cn

val a = 1;  var b = 2
来源：http://ueb.xylfe.cn

[T53] Scala：字符串插值
来源：http://iou.pengpengdd.cyou

s"值: $b"
来源：http://see.bbcook.cn

[T54] Scala：集合映射
来源：http://prz.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://rwb.wangdashe.top

[T55] Scala：集合过滤
来源：http://kzt.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://rna.sysykeji.top

[T56] Scala：样例类
来源：http://kvy.zdbjq.cn

case class User(name: String, age: Int)
来源：http://xki.aizwys.cn

[T57] Scala：模式匹配
来源：http://ufa.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qcs.yangfankeji.com

[T58] Scala：函数定义
来源：http://suq.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://hag.quarkkingdee.top

[T59] Scala：循环
来源：http://fos.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://pri.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://obw.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://alu.c1oappe.top

================================================================================
来源：http://ebz.chenzaomai.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uuq.uphjek.com

================================================================================
来源：http://dsc.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://lln.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ywp.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://dxn.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kbl.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://bjo.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rvt.xuetiantiany.cn

[U04] Py：变量调试打印
来源：http://kvz.tanke756.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bin.fktsv.cn

[U05] Py：列表去重且保序
来源：http://vlx.ydzc1.top

list(dict.fromkeys(arr))
来源：http://ndd.cqqwz.cn

[U06] Py：合并两个字典
来源：http://ivg.tianlin.xyz

{**a, **b}
来源：http://nit.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://euy.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://mde.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://znx.cqqwz.cn

[y for x in nested for y in x]
来源：http://wje.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://rby.sweek.top

max(d, key=d.get)
来源：http://zha.smart0.xyz

[U10] Py：按值排序字典
来源：http://noy.yuxming.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ejr.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://nkw.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://omz.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://sca.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://kdj.zhiwuduotai.top

[U13] Py：固定长度队列
来源：http://xig.hfpthk.cn

deque(maxlen=10)
来源：http://qrz.nwbrower.top

[U14] Py：分组收集到列表
来源：http://liv.52xcode.cn

defaultdict(list)
来源：http://yjt.chenlongwang.top

[U15] Py：高精度计时
来源：http://ydm.0kj1m.cn

t = time.perf_counter()
来源：http://ilq.cucudq.cn

[U16] Py：命令行参数解析
来源：http://zwt.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bag.cdnleiting.top

[U17] Py：初始化日志
来源：http://vss.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://tgm.fehbvm.com

[U18] Py：预编译正则
来源：http://snj.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://rro.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://wop.vehdjk.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iqo.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://ojn.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://rbb.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://cqk.cucudq.cn

@contextlib.contextmanager
来源：http://rum.yonumen.top

[U22] Py：矩阵转置
来源：http://cdc.gotoacloud.top

list(zip(*m))
来源：http://xxs.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://yyh.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ftb.daria6918.cn

[U24] Py：路径操作
来源：http://cjr.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rtp.mhx1999.top


<!-- 参考信息 -->