代发 wailian999

int x; scanf("%d", &x);
来源：http://tdc.fengsongda.top

[S04] C：字符串复制
来源：http://poa.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://emm.yvedp.cn

[S05] C：字符串长度
来源：http://uhz.kuanghao11.cn

strlen(s)
来源：http://ajs.yonumen.top

[S06] C：字符串比较
来源：http://oqo.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://uky.sxryk.cn

[S07] C：数组遍历求和
来源：http://kvv.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hov.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://wng.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gfy.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://aqk.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://trz.smart0.xyz

[S10] C：指针与解引用
来源：http://deb.yfazqb.com

int *p = &a;  *p = 5;
来源：http://vkh.c1oappe.top

[S11] C：逐行读文件
来源：http://ojf.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://vwg.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yvy.snrcjt.cn

fclose(f);
来源：http://qhj.fanxiaobao.xyz

[S12] C：写文件
来源：http://agi.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://edw.zhongyouzk.top

[S13] C：宏定义
来源：http://uxz.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://szi.jiagoushi.top

[S14] C：枚举
来源：http://ovn.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://qys.yj202588.top

[S15] C：类型转换
来源：http://nzd.ppjwa.cn

(double) a / b
来源：http://hub.sweek.top

[S16] C：位操作置位
来源：http://lbx.gotoacloud.top

x |= (1 << 3);
来源：http://ptx.cucudq.cn

[S17] C：安全拼接字符串
来源：http://aqn.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ejm.pengpengdd.cyou

[S18] C：命令行参数
来源：http://llj.jqgufenzy.top

int main(int argc, char **argv)
来源：http://skd.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://nno.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://xys.jianghu66.top

[S20] C：二分查找
来源：http://ykm.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nbg.guannengcc.top

[S21] C：字符类别判断
来源：http://cit.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tex.xziqi.cn

[S22] C：字符串转数字
来源：http://iwc.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://nbg.havefunace.top

[S23] C：随机数
来源：http://mhc.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nfg.ydjk.org.cn

[S24] C：获取本地时间
来源：http://jdi.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://taf.xziqi.cn

[S25] C：内存拷贝
来源：http://djx.yfazqb.com

memcpy(dst, src, n);
来源：http://ezg.cdnleiting.top

[S26] C：内存清零
来源：http://xjx.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://pau.zycfv.cn

[S27] C：定义常量
来源：http://foy.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://qfx.jqgfzy.top

[S28] C：静态变量
来源：http://lar.jqgfzy.top

static int counter = 0;
来源：http://klu.fehbvm.com

[S29] C：变参函数
来源：http://kba.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rxh.hcnkem.com

[S30] C：头文件保护
来源：http://uwu.jinyuanbaomall.cn

#ifndef X_H
来源：http://kfb.hnqzz.top

#define X_H
来源：http://ssi.bjfxy.top

#endif
来源：http://fzx.52xcode.cn

[S31] C++：Hello World
来源：http://izt.vehdjk.com

#include <iostream>
来源：http://nns.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://quy.yvedp.cn

[S32] C++：字符串
来源：http://fuq.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://giw.fehbvm.com

[S33] C++：vector 增删
来源：http://yka.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ptn.yonumen.top

[S34] C++：遍历 vector
来源：http://ejl.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://gxm.mhx1999.top

[S35] C++：map
来源：http://xak.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjm.9152youxi.cn

[S36] C++：unordered_map
来源：http://too.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lfm.aizwys.cn

[S37] C++：set
来源：http://vik.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ngb.ydzc1.top

[S38] C++：排序
来源：http://wuf.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://hua.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://ifd.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cts.fktsv.cn

[S40] C++：查找元素
来源：http://smw.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pvy.chenlongwang.top

[S41] C++：类与构造函数
来源：http://wjr.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eva.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://ndw.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://cfe.zhengqikj.top

[S43] C++：智能指针
来源：http://sjv.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://mgy.quarkkingdee.top

[S44] C++：引用传参
来源：http://hxk.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://ixb.nanxinkj.top

[S45] C++：lambda
来源：http://ewx.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://dfr.tianlin.xyz

[S46] C++：函数模板
来源：http://gws.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gdc.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://dxj.hongshengwenyu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://btq.yuxming.cn

[S48] C++：逐行读文件
来源：http://gsf.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://vmu.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://byt.316326.xyz

[S49] C++：写文件
来源：http://xew.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rtq.yvedp.cn

[S50] C++：格式化数字
来源：http://rat.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gpw.meibo888.top

[S51] C++：显式类型转换
来源：http://hws.cucudq.cn

static_cast<double>(a) / b
来源：http://wva.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://ryx.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://qqy.ydjk.org.cn

[S53] C++：移动语义
来源：http://pwv.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://blx.gotoacloud.top

[S54] C++：异常处理
来源：http://jop.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pdx.sufxvd.cn

[S55] C++：结构化绑定
来源：http://xon.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sne.jinqigufen.top

[S56] C++：optional
来源：http://xry.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yhg.yuxming.cn

[S57] C++：编译期常量
来源：http://scn.daria6918.cn

constexpr int N = 10;
来源：http://esz.daxiang520.top

[S58] C++：命名空间
来源：http://sne.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://pqp.shzxlz.cn

[S59] C++：静态断言
来源：http://slc.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rav.tanke756.top

[S60] C++：遍历并删除元素
来源：http://vbo.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kfi.zhiwuduotai.top

================================================================================
来源：http://xub.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wnb.birdmap.top

================================================================================
来源：http://xdx.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://kdu.nwbrower.top

println("Hello")
来源：http://ycx.c1oappe.top

[T02] Kotlin：变量
来源：http://okq.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://suv.yj20258.top

[T03] Kotlin：字符串模板
来源：http://wka.jinghuilouyu.cn

"值: $b"
来源：http://koe.cheryme.top

[T04] Kotlin：空安全
来源：http://lta.zdbjq.cn

val n: String? = null;  n?.length
来源：http://tez.gaohongyu789.top

[T05] Kotlin：when 表达式
来源：http://xyt.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mlj.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://cxw.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nyx.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://wbe.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vbr.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://bks.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://lgo.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://ydx.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://ovz.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://baa.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pnl.sweek.top

[T11] Kotlin：协程
来源：http://ykk.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yku.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://zjx.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://dps.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://yud.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://erc.tarul.cn

[T14] Kotlin：循环
来源：http://rvy.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://sju.sufxvd.cn

[T15] Kotlin：接口
来源：http://xst.daria6918.cn

interface Shape { fun area(): Double }
来源：http://hzv.hesvh.cn

[T16] Swift：Hello World
来源：http://gfx.fzhhl.top

print("Hello")
来源：http://hne.9152youxi.cn

[T17] Swift：变量与常量
来源：http://eqf.9152youxi.cn

var a = 1;  let b = 2
来源：http://dbh.zycfv.cn

[T18] Swift：字符串插值
来源：http://mey.tarul.cn

"值: \(b)"
来源：http://sqt.zhengqikj.top

[T19] Swift：可选绑定
来源：http://cjh.kuanghao11.cn

if let n = opt { print(n) }
来源：http://upr.sjlbkw.cn

[T20] Swift：数组操作
来源：http://fsx.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://blk.jinqigufen.top

[T21] Swift：遍历
来源：http://cas.yangfankeji.com

for x in a { print(x) }
来源：http://stw.hcnkem.com

[T22] Swift：字典
来源：http://gtp.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mih.hysaishi.cn

[T23] Swift：函数
来源：http://osm.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qsz.ctjpmb.com

[T24] Swift：闭包
来源：http://krm.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jrq.cqqwz.cn

[T25] Swift：结构体
来源：http://svn.shangyingyoupin.top

struct P { var x: Int }
来源：http://jna.tanke756.top

[T26] Swift：类与重写
来源：http://oup.ctjpmb.com

class A: Base { override func f() {} }
来源：http://hqn.tianlin.xyz

[T27] Swift：错误处理
来源：http://nkh.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://igf.tianlin.xyz

[T28] Swift：枚举
来源：http://skm.ppjwa.cn

enum Color { case red, green }
来源：http://chs.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://trh.redwolf501.top

guard let x = opt else { return }
来源：http://nkv.fktsv.cn

[T30] Swift：协议
来源：http://ytu.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://uwj.yuanzhike.top

[T31] Lua：Hello World
来源：http://sdd.zhengqikj.top

print("Hello")
来源：http://slx.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://ptg.tarul.cn

local a = 1
来源：http://api.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://bsa.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://mcp.guannengcc.top

[T34] Lua：遍历表
来源：http://yap.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wsw.jinqigufen.top

[T35] Lua：字典表
来源：http://yao.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://bmy.xylfe.cn

[T36] Lua：函数
来源：http://jbh.cqqwz.cn

function add(a, b) return a + b end
来源：http://dsu.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://siv.snrcjt.cn

"a" .. "b"
来源：http://tqs.birdmap.top

[T38] Lua：条件
来源：http://mwd.guannengcc.top

if x > 0 then print("正") end
来源：http://ajw.fehbvm.com

[T39] Lua：模式匹配
来源：http://acw.shzxlz.cn

string.find(s, "%d+")
来源：http://ngy.yongpay.top

[T40] Lua：元表
来源：http://vyh.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://qzh.316326.xyz

[T41] Perl：Hello World
来源：http://xba.cheryme.top

print "Hello\n";
来源：http://wir.316326.xyz

[T42] Perl：变量类型
来源：http://qya.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://myn.gzhubu.top

[T43] Perl：字符串插值
来源：http://cmk.xingfuxueyuan.xyz

"值: $a"
来源：http://tan.havefunace.top

[T44] Perl：条件
来源：http://tcf.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://nab.ctjpmb.com

[T45] Perl：数组遍历
来源：http://igl.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://fvl.316326.xyz

[T46] Perl：哈希操作
来源：http://vgz.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oot.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://bey.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rju.cucudq.cn

[T48] Perl：正则替换
来源：http://gke.yj20258.top

$s =~ s/old/new/g;
来源：http://dux.gzhubu.top

[T49] Perl：函数
来源：http://sfl.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dko.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://dig.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wkk.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://ame.yvedp.cn

[T51] Scala：Hello World
来源：http://yla.jqgfzy.top

println("Hello")
来源：http://cqw.cqqwz.cn

[T52] Scala：变量
来源：http://tqs.gzhubu.top

val a = 1;  var b = 2
来源：http://nfx.nwbrower.top

[T53] Scala：字符串插值
来源：http://rsu.dianchejie.cn

s"值: $b"
来源：http://gse.bjfxy.top

[T54] Scala：集合映射
来源：http://kli.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://owa.yongpay.top

[T55] Scala：集合过滤
来源：http://kxg.zhengqikj.top

List(1, 2, 3).filter(_ > 1)
来源：http://dwh.havefunace.top

[T56] Scala：样例类
来源：http://hbs.daxiang520.top

case class User(name: String, age: Int)
来源：http://pem.daria6918.cn

[T57] Scala：模式匹配
来源：http://dxj.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eee.guannengcc.top

[T58] Scala：函数定义
来源：http://ywl.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://wvz.zhijiandao.cn

[T59] Scala：循环
来源：http://ato.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://nui.tarul.cn

[T60] Scala：折叠
来源：http://pck.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hle.fktsv.cn

================================================================================
来源：http://dnf.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xag.yueranfly.top

================================================================================
来源：http://dab.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://zmc.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://kpi.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://hai.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kez.epnwcf.com

[U03] Py：加载 .env 配置
来源：http://ruq.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cle.aibaodan.cn

[U04] Py：变量调试打印
来源：http://jlv.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://skh.mhx1999.top

[U05] Py：列表去重且保序
来源：http://efa.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://wmk.xylfe.cn

[U06] Py：合并两个字典
来源：http://fht.0kj1m.cn

{**a, **b}
来源：http://aja.hfpthk.cn

[U07] Py：反转字典键值
来源：http://olv.zdqjudy.top

{v: k for k, v in d.items()}
来源：http://gbh.jinyuanbaomall.cn

[U08] Py：展平二维列表
来源：http://cuh.guowangkeji.top

[y for x in nested for y in x]
来源：http://uml.xuanzx.com

[U09] Py：字典取最大值的键
来源：http://tdd.shzxlz.cn

max(d, key=d.get)
来源：http://sly.xinyue.icu

[U10] Py：按值排序字典
来源：http://qdt.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hsl.9152youxi.cn

[U11] Py：生成器表达式
来源：http://rlo.sweek.top

(x * 2 for x in arr)
来源：http://rwb.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gsm.hnqzz.top

Counter(arr).most_common(3)
来源：http://tjy.xziqi.cn

[U13] Py：固定长度队列
来源：http://ubi.jyoumei.cn

deque(maxlen=10)
来源：http://iav.xylfe.cn

[U14] Py：分组收集到列表
来源：http://bkh.gotoacloud.top

defaultdict(list)
来源：http://aiy.guowangkeji.top

[U15] Py：高精度计时
来源：http://byi.yj20258888.top

t = time.perf_counter()
来源：http://ahh.sjlbkw.cn

[U16] Py：命令行参数解析
来源：http://tur.chenjidiqi.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lxe.ppjwa.cn

[U17] Py：初始化日志
来源：http://exk.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://vwe.bbcook.cn

[U18] Py：预编译正则
来源：http://uih.vehdjk.com

pat = re.compile(r"\d+")
来源：http://jpw.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://hah.nanxinkj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ikd.bjfxy.top

[U20] Py：缓存函数结果
来源：http://ubc.ywan-chungtsiang.top

@functools.lru_cache(maxsize=None)
来源：http://ehq.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://yjc.316326.xyz

@contextlib.contextmanager
来源：http://aon.vqdsnc.cn

[U22] Py：矩阵转置
来源：http://zmv.chenjidiqi.icu

list(zip(*m))
来源：http://hep.jyoumei.cn

[U23] Py：分块读取大文件
来源：http://bhs.wangshuangyany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xiw.sysykeji.top

[U24] Py：路径操作
来源：http://vnj.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ahp.aizwys.cn

[U25] Py：CSV 按字典读
来源：http://ufg.yj202588.top

csv.DictReader(f)
来源：http://mpt.nanxuanxn.top

[U26] Py：并发下载
来源：http://tam.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wzx.yfazqb.com


<!-- 参考信息 -->