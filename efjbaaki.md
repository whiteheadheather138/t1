代发 wailian999

strlen(s)
来源：http://lhj.redwolf501.top

[S06] C：字符串比较
来源：http://igj.ydzc1.top

strcmp(a, b) == 0
来源：http://tqx.hysaishi.cn

[S07] C：数组遍历求和
来源：http://rtn.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tri.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://eit.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pmb.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://bvh.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qgp.meibo888.top

[S10] C：指针与解引用
来源：http://voc.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://zvo.cucudq.cn

[S11] C：逐行读文件
来源：http://wmz.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://zbz.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mcp.haohaochexian.top

fclose(f);
来源：http://pzd.zycfv.cn

[S12] C：写文件
来源：http://huw.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rdm.jqgfzy.top

[S13] C：宏定义
来源：http://btd.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bkq.yj20258.top

[S14] C：枚举
来源：http://lxx.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://mqo.zycfv.cn

[S15] C：类型转换
来源：http://xsu.jianghu66.top

(double) a / b
来源：http://zva.smart0.xyz

[S16] C：位操作置位
来源：http://tdp.zdqjudy.top

x |= (1 << 3);
来源：http://rkt.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://czd.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mai.meibo888.top

[S18] C：命令行参数
来源：http://ylg.hywenlv.cn

int main(int argc, char **argv)
来源：http://sui.zdqjudy.top

[S19] C：快速排序
来源：http://xca.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://don.xuanzx.com

[S20] C：二分查找
来源：http://yab.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zfb.yfazqb.com

[S21] C：字符类别判断
来源：http://zvg.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ems.epnwcf.com

[S22] C：字符串转数字
来源：http://ifg.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://lhe.yongpay.top

[S23] C：随机数
来源：http://fpp.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://azx.ydjk.org.cn

[S24] C：获取本地时间
来源：http://ehp.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nvz.gzhubu.top

[S25] C：内存拷贝
来源：http://eme.yvedp.cn

memcpy(dst, src, n);
来源：http://kqq.cashguo.top

[S26] C：内存清零
来源：http://vxg.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://zhl.sxryk.cn

[S27] C：定义常量
来源：http://gbe.vehdjk.com

const double PI = 3.14159;
来源：http://uee.uphjek.com

[S28] C：静态变量
来源：http://ovw.jyoumei.cn

static int counter = 0;
来源：http://xym.shzxlz.cn

[S29] C：变参函数
来源：http://cdr.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ukm.xinyue.icu

[S30] C：头文件保护
来源：http://mjh.shanyushiyangtech.top

#ifndef X_H
来源：http://cej.yj20258.top

#define X_H
来源：http://kkq.ydjk.org.cn

#endif
来源：http://fhz.nanxuanxn.top

[S31] C++：Hello World
来源：http://wyr.birdmap.top

#include <iostream>
来源：http://ves.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ffl.snrcjt.cn

[S32] C++：字符串
来源：http://dgq.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://yqh.cheryme.top

[S33] C++：vector 增删
来源：http://uou.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://woy.chenzaomai.com

[S34] C++：遍历 vector
来源：http://amq.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://rnl.daria6918.cn

[S35] C++：map
来源：http://xtc.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eyj.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://bpc.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dny.ctjpmb.com

[S37] C++：set
来源：http://xeq.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tvt.feifeiyinyue.top

[S38] C++：排序
来源：http://obh.yonumen.top

std::sort(v.begin(), v.end());
来源：http://cht.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://uiu.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://owx.zycfv.cn

[S40] C++：查找元素
来源：http://yty.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zxj.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://aji.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jak.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://itt.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://veg.chenlongwang.top

[S43] C++：智能指针
来源：http://pcs.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://cpb.cqqwz.cn

[S44] C++：引用传参
来源：http://ocv.mhx1999.top

void inc(int &x) { ++x; }
来源：http://uim.bbcook.cn

[S45] C++：lambda
来源：http://vga.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://sin.fengsongda.top

[S46] C++：函数模板
来源：http://ylh.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://men.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://mje.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aop.hammf.cn

[S48] C++：逐行读文件
来源：http://xqd.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://rvy.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://set.haohaochexian.top

[S49] C++：写文件
来源：http://pbv.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cjf.yfazqb.com

[S50] C++：格式化数字
来源：http://rsm.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zst.sysykeji.top

[S51] C++：显式类型转换
来源：http://kis.hysaishi.cn

static_cast<double>(a) / b
来源：http://jvk.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://mhp.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://oaz.xziqi.cn

[S53] C++：移动语义
来源：http://dyo.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://bjc.feifeiyinyue.top

[S54] C++：异常处理
来源：http://ujt.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iaq.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://zid.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gyw.gotoacloud.top

[S56] C++：optional
来源：http://nbb.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zvr.dashuyun.cn

[S57] C++：编译期常量
来源：http://efy.zhijiandao.cn

constexpr int N = 10;
来源：http://iox.sysykeji.top

[S58] C++：命名空间
来源：http://wuz.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://kpg.dashuyun.cn

[S59] C++：静态断言
来源：http://htm.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cpu.tanke756.top

[S60] C++：遍历并删除元素
来源：http://fds.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fyj.daria6918.cn

================================================================================
来源：http://ewo.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ilo.52xcode.cn

================================================================================
来源：http://qzq.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://ezz.c1oappe.top

println("Hello")
来源：http://jsm.dashuyun.cn

[T02] Kotlin：变量
来源：http://mxm.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yvg.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://cke.cashguo.top

"值: $b"
来源：http://mau.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://syw.guowangkeji.top

val n: String? = null;  n?.length
来源：http://upt.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://jle.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uxu.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://arl.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://glk.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://fim.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pkh.ybcxt.top

[T08] Kotlin：数据类
来源：http://wrh.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://tpt.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://bgz.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://ent.yongpay.top

[T10] Kotlin：默认参数
来源：http://lgu.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://llf.zhixingplan.top

[T11] Kotlin：协程
来源：http://ecm.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://uyb.hammf.cn

[T12] Kotlin：解构声明
来源：http://iou.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://cok.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://wyy.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://lew.0kj1m.cn

[T14] Kotlin：循环
来源：http://qvf.havefunace.top

for (i in 1..10) println(i)
来源：http://jbw.smart0.xyz

[T15] Kotlin：接口
来源：http://idt.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://fcc.sysykeji.top

[T16] Swift：Hello World
来源：http://pec.zhiwuduotai.top

print("Hello")
来源：http://pad.yj202588.top

[T17] Swift：变量与常量
来源：http://bvf.sxryk.cn

var a = 1;  let b = 2
来源：http://tnt.ydzc1.top

[T18] Swift：字符串插值
来源：http://rtv.smart0.xyz

"值: \(b)"
来源：http://kux.gogol.net.cn

[T19] Swift：可选绑定
来源：http://gfb.zhixingplan.top

if let n = opt { print(n) }
来源：http://gnb.jinqigufen.top

[T20] Swift：数组操作
来源：http://lbd.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tgq.wangdashe.top

[T21] Swift：遍历
来源：http://kus.shuidangran.top

for x in a { print(x) }
来源：http://ijy.meibo888.top

[T22] Swift：字典
来源：http://ytc.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://fgc.redwolf501.top

[T23] Swift：函数
来源：http://oei.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mks.yuanzhike.top

[T24] Swift：闭包
来源：http://jra.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wkn.nanxuanxn.top

[T25] Swift：结构体
来源：http://pfp.sufxvd.cn

struct P { var x: Int }
来源：http://khv.hcnkem.com

[T26] Swift：类与重写
来源：http://prx.xuanzx.com

class A: Base { override func f() {} }
来源：http://kxv.quarkkingdee.top

[T27] Swift：错误处理
来源：http://ctp.birdmap.top

do { try f() } catch { print(error) }
来源：http://edy.aizwys.cn

[T28] Swift：枚举
来源：http://ydj.zhongyouzk.top

enum Color { case red, green }
来源：http://zjx.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://ryq.vehdjk.com

guard let x = opt else { return }
来源：http://kce.hywenlv.cn

[T30] Swift：协议
来源：http://ayu.aizwys.cn

protocol Shape { func area() -> Double }
来源：http://mad.zhijiandao.cn

[T31] Lua：Hello World
来源：http://gyt.jqgufenzy.top

print("Hello")
来源：http://hoo.yj20258888.top

[T32] Lua：局部变量
来源：http://ctj.fzhhl.top

local a = 1
来源：http://bcm.dianchejie.cn

[T33] Lua：表（数组）
来源：http://jcy.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mig.yj202588.top

[T34] Lua：遍历表
来源：http://xca.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://tzu.tanke756.top

[T35] Lua：字典表
来源：http://eed.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://jqr.sjlbkw.cn

[T36] Lua：函数
来源：http://uvw.fengsongda.top

function add(a, b) return a + b end
来源：http://zho.nwbrower.top

[T37] Lua：字符串拼接
来源：http://hdq.ehwqpu.com

"a" .. "b"
来源：http://jni.hfpthk.cn

[T38] Lua：条件
来源：http://pep.jqgufenzy.top

if x > 0 then print("正") end
来源：http://tqp.cdnleiting.top

[T39] Lua：模式匹配
来源：http://zzy.fktsv.cn

string.find(s, "%d+")
来源：http://cqr.hcnkem.com

[T40] Lua：元表
来源：http://fcg.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://amg.pengpengdd.cyou

[T41] Perl：Hello World
来源：http://dmi.vehdjk.com

print "Hello\n";
来源：http://aas.tarul.cn

[T42] Perl：变量类型
来源：http://jqz.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qyn.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://vfe.jlsjyb.cn

"值: $a"
来源：http://mgl.jinqigufen.top

[T44] Perl：条件
来源：http://gce.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://mlr.ctjpmb.com

[T45] Perl：数组遍历
来源：http://exo.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://ttf.zdqjudy.top

[T46] Perl：哈希操作
来源：http://wdi.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://idd.meibo888.top

[T47] Perl：正则捕获
来源：http://fpt.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tjo.sjlbkw.cn

[T48] Perl：正则替换
来源：http://cyh.redwolf501.top

$s =~ s/old/new/g;
来源：http://ysw.hammf.cn

[T49] Perl：函数
来源：http://hhl.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wvb.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://edf.ivvv.top

open my $fh, "<", "a.txt" or die $!;
来源：http://skq.fanxiaobao.xyz

while (my $line = <$fh>) { print $line; }
来源：http://cjw.zdqjudy.top

[T51] Scala：Hello World
来源：http://ink.yj20258888.top

println("Hello")
来源：http://nra.jinqigufen.top

[T52] Scala：变量
来源：http://vtj.ydjk.org.cn

val a = 1;  var b = 2
来源：http://nnz.zdqjudy.top

[T53] Scala：字符串插值
来源：http://kew.chenzaomai.com

s"值: $b"
来源：http://hte.fehbvm.com

[T54] Scala：集合映射
来源：http://hcf.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://tbe.cucudq.cn

[T55] Scala：集合过滤
来源：http://gsq.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://ftx.birdmap.top

[T56] Scala：样例类
来源：http://fst.jianghu66.top

case class User(name: String, age: Int)
来源：http://wcr.ppjwa.cn

[T57] Scala：模式匹配
来源：http://pno.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oqp.xylfe.cn

[T58] Scala：函数定义
来源：http://vlv.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://siq.shanyushiyangtech.top

[T59] Scala：循环
来源：http://apb.tarul.cn

for (i <- 1 to 10) println(i)
来源：http://aiw.zhongyouzk.top

[T60] Scala：折叠
来源：http://ymz.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nnr.shzxlz.cn

================================================================================
来源：http://yvl.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://deo.hnxiangtu.top

================================================================================
来源：http://nla.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://iuy.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://sex.nanxuanxn.top

[U02] Py：导出 / 安装依赖
来源：http://ply.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://flv.yuanzhike.top

[U03] Py：加载 .env 配置
来源：http://blc.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://uzf.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://kbl.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqk.zycfv.cn

[U05] Py：列表去重且保序
来源：http://buq.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://ins.sxryk.cn

[U06] Py：合并两个字典
来源：http://hpn.cucudq.cn

{**a, **b}
来源：http://wdn.316326.xyz

[U07] Py：反转字典键值
来源：http://jqp.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://kzh.daxiang520.top

[U08] Py：展平二维列表
来源：http://snk.hysaishi.cn

[y for x in nested for y in x]
来源：http://gcc.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://rxf.sysykeji.top

max(d, key=d.get)
来源：http://gmd.yfazqb.com

[U10] Py：按值排序字典
来源：http://gfx.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://efk.uphjek.com

[U11] Py：生成器表达式
来源：http://xtr.sjlbkw.cn

(x * 2 for x in arr)
来源：http://vdk.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://fks.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://wed.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://ltc.jinyuanbaomall.cn

deque(maxlen=10)
来源：http://sqt.chenzaomai.com

[U14] Py：分组收集到列表
来源：http://qhg.shangyingyoupin.top

defaultdict(list)
来源：http://wyt.yanxiufei.cn

[U15] Py：高精度计时
来源：http://ube.xingfuxueyuan.xyz

t = time.perf_counter()
来源：http://mql.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://jrb.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vtf.sxryk.cn

[U17] Py：初始化日志
来源：http://dxi.zhiwuduotai.top

logging.basicConfig(level=logging.INFO)
来源：http://uqv.ivvv.top

[U18] Py：预编译正则
来源：http://kad.smart0.xyz

pat = re.compile(r"\d+")
来源：http://flb.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://aou.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vnt.daxiang520.top

[U20] Py：缓存函数结果
来源：http://jkb.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://lsk.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://hcf.yuanzhike.top

@contextlib.contextmanager
来源：http://jlo.ybcxt.top

[U22] Py：矩阵转置
来源：http://jym.vqdsnc.cn

list(zip(*m))
来源：http://ola.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://cwe.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gpa.jlsjyb.cn

[U24] Py：路径操作
来源：http://vrj.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hsg.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://fug.yuxming.cn

csv.DictReader(f)
来源：http://xjv.aizwys.cn

[U26] Py：并发下载
来源：http://gue.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tjt.aizwys.cn

[U27] Py：异步 HTTP
来源：http://bbt.aizwys.cn

aiohttp.ClientSession() 配合 async with
来源：http://obr.ywan-chungtsiang.top

[U28] Py：类型别名
来源：http://pry.9152youxi.cn

UserId = int
来源：http://tum.jqgufenzy.top


<!-- 参考信息 -->