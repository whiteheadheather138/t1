代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mpk.birdmap.top

[S10] C：指针与解引用
来源：http://zku.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://cka.bjfxy.top

[S11] C：逐行读文件
来源：http://rhq.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://ydj.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pes.yueranfly.top

fclose(f);
来源：http://isy.sufxvd.cn

[S12] C：写文件
来源：http://cot.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lro.nanxuanxn.top

[S13] C：宏定义
来源：http://vbe.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wad.yongpay.top

[S14] C：枚举
来源：http://ahk.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://paq.zdqjudy.top

[S15] C：类型转换
来源：http://owy.tian-w.cn

(double) a / b
来源：http://tdi.jinqigfzy.top

[S16] C：位操作置位
来源：http://lxe.hammf.cn

x |= (1 << 3);
来源：http://zgm.ivvv.top

[S17] C：安全拼接字符串
来源：http://uvu.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://phh.dashuyun.cn

[S18] C：命令行参数
来源：http://shb.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://haa.xylfe.cn

[S19] C：快速排序
来源：http://gde.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://etl.hnxiangtu.top

[S20] C：二分查找
来源：http://mfg.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pfl.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://wrr.sxryk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vbz.nanxuanxn.top

[S22] C：字符串转数字
来源：http://umy.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wba.tarul.cn

[S23] C：随机数
来源：http://hmc.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pwh.fzhhl.top

[S24] C：获取本地时间
来源：http://fhn.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uwd.xuanzx.com

[S25] C：内存拷贝
来源：http://dzx.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://cmw.xziqi.cn

[S26] C：内存清零
来源：http://klo.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://qhg.quarkkingdee.top

[S27] C：定义常量
来源：http://rzn.yanxiufei.cn

const double PI = 3.14159;
来源：http://bwn.ppjwa.cn

[S28] C：静态变量
来源：http://div.52xcode.cn

static int counter = 0;
来源：http://iva.chenzaomai.com

[S29] C：变参函数
来源：http://bmm.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yhl.guannengcc.top

[S30] C：头文件保护
来源：http://frk.shangyingyoupin.top

#ifndef X_H
来源：http://oza.zhijiandao.cn

#define X_H
来源：http://rtf.bbcook.cn

#endif
来源：http://gxy.aizwys.cn

[S31] C++：Hello World
来源：http://rzs.52xcode.cn

#include <iostream>
来源：http://tzc.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://qrg.cqqwz.cn

[S32] C++：字符串
来源：http://tdg.cashguo.top

std::string s = "hi";  s += "!";
来源：http://ljj.hnqzz.top

[S33] C++：vector 增删
来源：http://jtp.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfa.daria6918.cn

[S34] C++：遍历 vector
来源：http://eel.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://wcl.hammf.cn

[S35] C++：map
来源：http://iab.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zmh.hnxiangtu.top

[S36] C++：unordered_map
来源：http://jyu.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ugc.uphjek.com

[S37] C++：set
来源：http://ezk.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ftx.ivvv.top

[S38] C++：排序
来源：http://foh.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://rdl.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://jga.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kko.aizwys.cn

[S40] C++：查找元素
来源：http://amy.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://plf.daxiang520.top

[S41] C++：类与构造函数
来源：http://vjx.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://llm.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://kve.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://nwr.epnwcf.com

[S43] C++：智能指针
来源：http://zex.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://emd.tanke756.top

[S44] C++：引用传参
来源：http://fmf.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://iqi.daria6918.cn

[S45] C++：lambda
来源：http://rgz.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://trd.epnwcf.com

[S46] C++：函数模板
来源：http://sdp.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sdf.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://jhp.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://atc.jianghu66.top

[S48] C++：逐行读文件
来源：http://biz.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://dae.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://bxc.bjfxy.top

[S49] C++：写文件
来源：http://qhr.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bkv.ctjpmb.com

[S50] C++：格式化数字
来源：http://kqh.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ttz.yj20258888.top

[S51] C++：显式类型转换
来源：http://yjk.yj20258888.top

static_cast<double>(a) / b
来源：http://mat.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://tyf.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://vnn.cucudq.cn

[S53] C++：移动语义
来源：http://dfv.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://cpy.hcnkem.com

[S54] C++：异常处理
来源：http://wfh.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sfv.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://yjg.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vmi.sysykeji.top

[S56] C++：optional
来源：http://vkc.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fmk.redwolf501.top

[S57] C++：编译期常量
来源：http://fxo.zhoulong.xyz

constexpr int N = 10;
来源：http://irt.andypj.xyz

[S58] C++：命名空间
来源：http://uex.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://zuv.gzhubu.top

[S59] C++：静态断言
来源：http://vah.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jbl.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://awj.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kvy.yuxming.cn

================================================================================
来源：http://pdn.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://evt.cdnleiting.top

================================================================================
来源：http://kee.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://emw.c1oappe.top

println("Hello")
来源：http://nug.quarkkingdee.top

[T02] Kotlin：变量
来源：http://tah.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://khr.hammf.cn

[T03] Kotlin：字符串模板
来源：http://joo.vqdsnc.cn

"值: $b"
来源：http://dnj.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://hhw.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://vza.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://urg.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://msv.daria6918.cn

[T06] Kotlin：集合映射
来源：http://jyo.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pyx.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://nxf.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kgw.daxiang520.top

[T08] Kotlin：数据类
来源：http://ehu.sweek.top

data class User(val name: String, val age: Int)
来源：http://twm.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://mgm.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://fvx.yongpay.top

[T10] Kotlin：默认参数
来源：http://tax.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xmq.hesvh.cn

[T11] Kotlin：协程
来源：http://lew.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fbh.yuxming.cn

[T12] Kotlin：解构声明
来源：http://lcb.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://ejy.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://kof.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://yve.jiagoushi.top

[T14] Kotlin：循环
来源：http://kxj.ybcxt.top

for (i in 1..10) println(i)
来源：http://cpj.yanxiufei.cn

[T15] Kotlin：接口
来源：http://dlv.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://dur.sufxvd.cn

[T16] Swift：Hello World
来源：http://nfa.yj202588.top

print("Hello")
来源：http://gvl.nanxinkj.top

[T17] Swift：变量与常量
来源：http://ipf.vqdsnc.cn

var a = 1;  let b = 2
来源：http://wio.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://dno.vqdsnc.cn

"值: \(b)"
来源：http://lnm.mhx1999.top

[T19] Swift：可选绑定
来源：http://ktt.zhengqikj.top

if let n = opt { print(n) }
来源：http://wkc.jlsjyb.cn

[T20] Swift：数组操作
来源：http://fwx.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nqo.yanxiufei.cn

[T21] Swift：遍历
来源：http://rxb.sweek.top

for x in a { print(x) }
来源：http://seg.yueranfly.top

[T22] Swift：字典
来源：http://sfh.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://krr.smart0.xyz

[T23] Swift：函数
来源：http://hwe.ywan-chungtsiang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xkl.iojbl.cn

[T24] Swift：闭包
来源：http://enm.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jtc.jianghu66.top

[T25] Swift：结构体
来源：http://dav.tianlin.xyz

struct P { var x: Int }
来源：http://mdo.mhx1999.top

[T26] Swift：类与重写
来源：http://mzf.zhengqikj.top

class A: Base { override func f() {} }
来源：http://zei.gogol.net.cn

[T27] Swift：错误处理
来源：http://asn.yvedp.cn

do { try f() } catch { print(error) }
来源：http://dis.guannengcc.top

[T28] Swift：枚举
来源：http://rwq.jqgufenzy.top

enum Color { case red, green }
来源：http://cdw.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://vxq.quarkkingdee.top

guard let x = opt else { return }
来源：http://mbm.cashguo.top

[T30] Swift：协议
来源：http://kyf.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://hxu.cdnleiting.top

[T31] Lua：Hello World
来源：http://dem.cqqwz.cn

print("Hello")
来源：http://mnb.zdqjudy.top

[T32] Lua：局部变量
来源：http://ogv.jinyuanbaomall.cn

local a = 1
来源：http://moc.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://xpm.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kih.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://vha.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dcx.hysaishi.cn

[T35] Lua：字典表
来源：http://bte.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://enq.cucudq.cn

[T36] Lua：函数
来源：http://mqb.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://ymo.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://rtr.uphjek.com

"a" .. "b"
来源：http://hft.52xcode.cn

[T38] Lua：条件
来源：http://jci.hesvh.cn

if x > 0 then print("正") end
来源：http://vzd.shuidangran.top

[T39] Lua：模式匹配
来源：http://qdr.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://jhu.hywenlv.cn

[T40] Lua：元表
来源：http://ipg.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://agv.tianlin.xyz

[T41] Perl：Hello World
来源：http://vgu.0kj1m.cn

print "Hello\n";
来源：http://hbn.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://gri.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dgq.hammf.cn

[T43] Perl：字符串插值
来源：http://sge.sxryk.cn

"值: $a"
来源：http://tgk.wangshuangyany.cn

[T44] Perl：条件
来源：http://nlu.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://ala.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://qly.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://zex.iojbl.cn

[T46] Perl：哈希操作
来源：http://obn.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://skg.9152youxi.cn

[T47] Perl：正则捕获
来源：http://ynd.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dzm.vehdjk.com

[T48] Perl：正则替换
来源：http://qcy.9152youxi.cn

$s =~ s/old/new/g;
来源：http://hbr.cucudq.cn

[T49] Perl：函数
来源：http://rwx.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dvc.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://fvk.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lxt.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://tpa.wangdashe.top

[T51] Scala：Hello World
来源：http://pvx.hesvh.cn

println("Hello")
来源：http://duy.ctjpmb.com

[T52] Scala：变量
来源：http://iet.redwolf501.top

val a = 1;  var b = 2
来源：http://aji.yfazqb.com

[T53] Scala：字符串插值
来源：http://dmo.vehdjk.com

s"值: $b"
来源：http://jxy.yj20258.top

[T54] Scala：集合映射
来源：http://efh.daria6918.cn

List(1, 2, 3).map(_ * 2)
来源：http://bkb.yonumen.top

[T55] Scala：集合过滤
来源：http://mgz.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vwf.yanxiufei.cn

[T56] Scala：样例类
来源：http://uhm.gzhubu.top

case class User(name: String, age: Int)
来源：http://clm.tian-w.cn

[T57] Scala：模式匹配
来源：http://avl.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://byd.yj20258.top

[T58] Scala：函数定义
来源：http://ifj.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://pvw.havefunace.top

[T59] Scala：循环
来源：http://owu.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://ldp.tianlin.xyz

[T60] Scala：折叠
来源：http://yxx.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://buo.ydjk.org.cn

================================================================================
来源：http://hfv.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://spz.gaohongyu789.top

================================================================================
来源：http://pfg.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://qca.xingfuxueyuan.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://vvb.fzhhl.top

[U02] Py：导出 / 安装依赖
来源：http://fzj.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lqu.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://smp.pycfn.com

from dotenv import load_dotenv; load_dotenv()
来源：http://dpu.vehdjk.com

[U04] Py：变量调试打印
来源：http://xdi.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cyp.tian-w.cn

[U05] Py：列表去重且保序
来源：http://xkm.ywan-chungtsiang.top

list(dict.fromkeys(arr))
来源：http://onl.ydzc1.top

[U06] Py：合并两个字典
来源：http://era.zhaomingkeji.xyz

{**a, **b}
来源：http://oja.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://usm.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://igg.jyoumei.cn

[U08] Py：展平二维列表
来源：http://hkv.shzxlz.cn

[y for x in nested for y in x]
来源：http://bgt.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://dae.gogol.net.cn

max(d, key=d.get)
来源：http://iyu.zdbjq.cn

[U10] Py：按值排序字典
来源：http://zvn.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xkt.ybcxt.top

[U11] Py：生成器表达式
来源：http://gxf.wangdashe.top

(x * 2 for x in arr)
来源：http://uxl.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://exf.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://ote.uphjek.com

[U13] Py：固定长度队列
来源：http://gvz.feifeiyinyue.top

deque(maxlen=10)
来源：http://wxx.pengpengdd.cyou

[U14] Py：分组收集到列表
来源：http://sim.hammf.cn

defaultdict(list)
来源：http://tqb.ybcxt.top

[U15] Py：高精度计时
来源：http://kng.shuidangran.top

t = time.perf_counter()
来源：http://pan.smart0.xyz

[U16] Py：命令行参数解析
来源：http://ddq.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eof.sjlbkw.cn

[U17] Py：初始化日志
来源：http://huo.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://ooz.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://qxq.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://htt.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://ybx.hcnkem.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xqp.jinqigfzy.top

[U20] Py：缓存函数结果
来源：http://iqv.gotoacloud.top

@functools.lru_cache(maxsize=None)
来源：http://hff.wangshuangyany.cn

[U21] Py：自定义上下文管理器
来源：http://dmd.sjlbkw.cn

@contextlib.contextmanager
来源：http://dxg.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://alo.jinqigfzy.top

list(zip(*m))
来源：http://jad.smart0.xyz

[U23] Py：分块读取大文件
来源：http://vnv.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://iic.ydjk.org.cn

[U24] Py：路径操作
来源：http://crc.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://crs.hnqzz.top

[U25] Py：CSV 按字典读
来源：http://mjl.yonumen.top

csv.DictReader(f)
来源：http://uyo.hywenlv.cn

[U26] Py：并发下载
来源：http://qfg.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nvf.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://myr.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://gjk.havefunace.top

[U28] Py：类型别名
来源：http://vut.cucudq.cn

UserId = int
来源：http://lnv.havefunace.top

[U29] Py：属性校验
来源：http://lvs.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://wyv.nanxuanxn.top

[U30] Py：数据类
来源：http://nba.gogol.net.cn

@dataclass(slots=True)
来源：http://gdg.jqgfzy.top

[U31] Py：单测
来源：http://nmb.hywenlv.cn

python -m pytest -q
来源：http://igp.tanke756.top

[U32] Py：代码格式化
来源：http://cre.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://kcz.xziqi.cn


<!-- 参考信息 -->