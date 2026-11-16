代发 wailian999

strlen(s)
来源：http://gic.hysaishi.cn

[S06] C：字符串比较
来源：http://cqv.dianchejie.cn

strcmp(a, b) == 0
来源：http://ooi.uphjek.com

[S07] C：数组遍历求和
来源：http://msh.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qqz.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://qtb.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kli.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://slo.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qbx.52xcode.cn

[S10] C：指针与解引用
来源：http://nre.yuxming.cn

int *p = &a;  *p = 5;
来源：http://gzu.zhixingplan.top

[S11] C：逐行读文件
来源：http://lak.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://ihr.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gok.epnwcf.com

fclose(f);
来源：http://npl.smart0.xyz

[S12] C：写文件
来源：http://gdf.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nex.ehwqpu.com

[S13] C：宏定义
来源：http://ify.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ewv.snrcjt.cn

[S14] C：枚举
来源：http://gpv.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://foz.ppjwa.cn

[S15] C：类型转换
来源：http://smj.bbcook.cn

(double) a / b
来源：http://atb.fktsv.cn

[S16] C：位操作置位
来源：http://xti.ehwqpu.com

x |= (1 << 3);
来源：http://xxi.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://hyl.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wda.hammf.cn

[S18] C：命令行参数
来源：http://jqi.gaohongyu789.top

int main(int argc, char **argv)
来源：http://lvg.shuidangran.top

[S19] C：快速排序
来源：http://oup.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://enx.chenzaomai.com

[S20] C：二分查找
来源：http://ncn.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pek.sufxvd.cn

[S21] C：字符类别判断
来源：http://buz.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lqf.cdnleiting.top

[S22] C：字符串转数字
来源：http://ubd.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aue.daxiang520.top

[S23] C：随机数
来源：http://jmj.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pff.jinqigfzy.top

[S24] C：获取本地时间
来源：http://boj.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nyk.tianlin.xyz

[S25] C：内存拷贝
来源：http://dtw.jlsjyb.cn

memcpy(dst, src, n);
来源：http://mbl.tarul.cn

[S26] C：内存清零
来源：http://qzi.xinyue.icu

memset(a, 0, sizeof a);
来源：http://fli.hnxiangtu.top

[S27] C：定义常量
来源：http://qcx.zdqjudy.top

const double PI = 3.14159;
来源：http://alm.daria6918.cn

[S28] C：静态变量
来源：http://lfa.snrcjt.cn

static int counter = 0;
来源：http://fup.sweek.top

[S29] C：变参函数
来源：http://efl.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xwz.shzxlz.cn

[S30] C：头文件保护
来源：http://far.dashuyun.cn

#ifndef X_H
来源：http://liq.bbcook.cn

#define X_H
来源：http://jou.tarul.cn

#endif
来源：http://abb.jqgufenzy.top

[S31] C++：Hello World
来源：http://row.yfazqb.com

#include <iostream>
来源：http://fgx.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://xwc.mhx1999.top

[S32] C++：字符串
来源：http://uxq.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://vog.dashuyun.cn

[S33] C++：vector 增删
来源：http://qit.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nam.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://dmg.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://mfr.ehwqpu.com

[S35] C++：map
来源：http://tkz.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wuk.jqgufenzy.top

[S36] C++：unordered_map
来源：http://wzi.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pie.daria6918.cn

[S37] C++：set
来源：http://jwu.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://why.feifeiyinyue.top

[S38] C++：排序
来源：http://rsk.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://liu.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://tzn.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://msx.nanxuanxn.top

[S40] C++：查找元素
来源：http://ukj.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lbq.yuanzhike.top

[S41] C++：类与构造函数
来源：http://iml.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xdu.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://pva.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://bau.yfazqb.com

[S43] C++：智能指针
来源：http://hwm.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://pre.yj20258888.top

[S44] C++：引用传参
来源：http://fce.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://yub.sysykeji.top

[S45] C++：lambda
来源：http://mbm.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://due.ydjk.org.cn

[S46] C++：函数模板
来源：http://xef.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://czp.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://ygj.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ggc.bjfxy.top

[S48] C++：逐行读文件
来源：http://dpz.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://flp.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://dzq.dianchejie.cn

[S49] C++：写文件
来源：http://gzf.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://drl.yj202588.top

[S50] C++：格式化数字
来源：http://wgq.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eas.dianchejie.cn

[S51] C++：显式类型转换
来源：http://uqf.jiagoushi.top

static_cast<double>(a) / b
来源：http://mgt.cashguo.top

[S52] C++：const 与 noexcept
来源：http://mws.fktsv.cn

int size() const noexcept { return n_; }
来源：http://hry.cheryme.top

[S53] C++：移动语义
来源：http://ipx.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://zjj.feifeiyinyue.top

[S54] C++：异常处理
来源：http://sne.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iro.cashguo.top

[S55] C++：结构化绑定
来源：http://ame.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nom.ctjpmb.com

[S56] C++：optional
来源：http://fay.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dat.sysykeji.top

[S57] C++：编译期常量
来源：http://gey.andypj.xyz

constexpr int N = 10;
来源：http://hpu.fengsongda.top

[S58] C++：命名空间
来源：http://jqb.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://hjj.nanxinkj.top

[S59] C++：静态断言
来源：http://byw.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zvh.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://fug.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kaq.nanxuanxn.top

================================================================================
来源：http://ypo.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ajl.yuanzhike.top

================================================================================
来源：http://uxd.xinyue.icu

[T01] Kotlin：Hello World
来源：http://yky.chenzaomai.com

println("Hello")
来源：http://sra.jlsjyb.cn

[T02] Kotlin：变量
来源：http://apx.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://drq.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://npd.gogol.net.cn

"值: $b"
来源：http://ujj.yangfankeji.com

[T04] Kotlin：空安全
来源：http://umv.chenlongwang.top

val n: String? = null;  n?.length
来源：http://nuw.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://tqa.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lgt.cheryme.top

[T06] Kotlin：集合映射
来源：http://cau.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://msh.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://vzm.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://iqq.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://mom.hammf.cn

data class User(val name: String, val age: Int)
来源：http://kvv.cashguo.top

[T09] Kotlin：扩展函数
来源：http://svm.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://omf.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://gzc.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bct.yanxiufei.cn

[T11] Kotlin：协程
来源：http://ifz.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bli.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://dvc.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://rqk.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://cqs.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://asx.jiagoushi.top

[T14] Kotlin：循环
来源：http://pms.hfpthk.cn

for (i in 1..10) println(i)
来源：http://hqz.cucudq.cn

[T15] Kotlin：接口
来源：http://pue.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://qjz.gogol.net.cn

[T16] Swift：Hello World
来源：http://fsk.chenzaomai.com

print("Hello")
来源：http://thx.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://gbv.sysykeji.top

var a = 1;  let b = 2
来源：http://htd.jyoumei.cn

[T18] Swift：字符串插值
来源：http://gen.xinyue.icu

"值: \(b)"
来源：http://mqg.yuanzhike.top

[T19] Swift：可选绑定
来源：http://fhp.uphjek.com

if let n = opt { print(n) }
来源：http://ntd.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://nrr.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://pui.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://psd.quarkkingdee.top

for x in a { print(x) }
来源：http://cym.xziqi.cn

[T22] Swift：字典
来源：http://fcc.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://rlq.tanke756.top

[T23] Swift：函数
来源：http://asm.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hik.jyoumei.cn

[T24] Swift：闭包
来源：http://yiw.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wej.daxiang520.top

[T25] Swift：结构体
来源：http://lgv.316326.xyz

struct P { var x: Int }
来源：http://rzn.redwolf501.top

[T26] Swift：类与重写
来源：http://qwv.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://prh.ivvv.top

[T27] Swift：错误处理
来源：http://ijn.bjfxy.top

do { try f() } catch { print(error) }
来源：http://ggo.ydjk.org.cn

[T28] Swift：枚举
来源：http://xbn.jianghu66.top

enum Color { case red, green }
来源：http://keb.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://isg.bjfxy.top

guard let x = opt else { return }
来源：http://tww.ppjwa.cn

[T30] Swift：协议
来源：http://zxe.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://zkk.tanke756.top

[T31] Lua：Hello World
来源：http://dqh.yuanzhike.top

print("Hello")
来源：http://vpn.vehdjk.com

[T32] Lua：局部变量
来源：http://nlt.cdnleiting.top

local a = 1
来源：http://fci.tanke756.top

[T33] Lua：表（数组）
来源：http://aqr.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fqn.hywenlv.cn

[T34] Lua：遍历表
来源：http://iqy.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://whk.gotoacloud.top

[T35] Lua：字典表
来源：http://qgr.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://cdf.yanxiufei.cn

[T36] Lua：函数
来源：http://fcs.cdnleiting.top

function add(a, b) return a + b end
来源：http://ztw.kuanghao11.cn

[T37] Lua：字符串拼接
来源：http://jjd.jqgfzy.top

"a" .. "b"
来源：http://abc.guannengcc.top

[T38] Lua：条件
来源：http://uqt.cdnleiting.top

if x > 0 then print("正") end
来源：http://uda.birdmap.top

[T39] Lua：模式匹配
来源：http://upg.shzxlz.cn

string.find(s, "%d+")
来源：http://wjj.gotoacloud.top

[T40] Lua：元表
来源：http://qhd.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://btq.gogol.net.cn

[T41] Perl：Hello World
来源：http://cmb.jqgufenzy.top

print "Hello\n";
来源：http://qkr.hysaishi.cn

[T42] Perl：变量类型
来源：http://bjs.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gfv.xinyue.icu

[T43] Perl：字符串插值
来源：http://bau.yuxming.cn

"值: $a"
来源：http://wew.xinyue.icu

[T44] Perl：条件
来源：http://fjh.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://zjh.ybcxt.top

[T45] Perl：数组遍历
来源：http://axo.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://bpe.yj20258888.top

[T46] Perl：哈希操作
来源：http://ktr.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://isf.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://sef.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://pph.smart0.xyz

[T48] Perl：正则替换
来源：http://vdv.sysykeji.top

$s =~ s/old/new/g;
来源：http://uff.andypj.xyz

[T49] Perl：函数
来源：http://udh.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wan.gzhubu.top

[T50] Perl：逐行读文件
来源：http://akl.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tph.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://oxw.zdqjudy.top

[T51] Scala：Hello World
来源：http://mtg.jianghu66.top

println("Hello")
来源：http://tce.ctjpmb.com

[T52] Scala：变量
来源：http://qvs.wangdashe.top

val a = 1;  var b = 2
来源：http://byf.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://klo.chenlongwang.top

s"值: $b"
来源：http://rbp.yonumen.top

[T54] Scala：集合映射
来源：http://okn.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://vec.meibo888.top

[T55] Scala：集合过滤
来源：http://ttf.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ugx.nwbrower.top

[T56] Scala：样例类
来源：http://klu.52xcode.cn

case class User(name: String, age: Int)
来源：http://vdc.yongpay.top

[T57] Scala：模式匹配
来源：http://miy.yonumen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yqd.hnqzz.top

[T58] Scala：函数定义
来源：http://uhq.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://ntx.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://iqg.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://vex.jyoumei.cn

[T60] Scala：折叠
来源：http://asm.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iim.aizwys.cn

================================================================================
来源：http://xcz.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://csq.ivvv.top

================================================================================
来源：http://piw.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://pev.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://txx.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://rtg.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtt.sweek.top

[U03] Py：加载 .env 配置
来源：http://tmi.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pvr.cashguo.top

[U04] Py：变量调试打印
来源：http://bve.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kly.zhaomingkeji.xyz

[U05] Py：列表去重且保序
来源：http://tul.gzhubu.top

list(dict.fromkeys(arr))
来源：http://hxb.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://xmm.tianlin.xyz

{**a, **b}
来源：http://sbw.ctjpmb.com

[U07] Py：反转字典键值
来源：http://ggx.yj202588.top

{v: k for k, v in d.items()}
来源：http://wdl.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://ndr.zhengqikj.top

[y for x in nested for y in x]
来源：http://kie.316326.xyz

[U09] Py：字典取最大值的键
来源：http://xhs.zhongyouzk.top

max(d, key=d.get)
来源：http://zzh.ydzc1.top

[U10] Py：按值排序字典
来源：http://anh.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jtv.yfazqb.com

[U11] Py：生成器表达式
来源：http://ijb.hammf.cn

(x * 2 for x in arr)
来源：http://euq.sysykeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://ojx.hammf.cn

Counter(arr).most_common(3)
来源：http://yoz.sysykeji.top

[U13] Py：固定长度队列
来源：http://gka.vehdjk.com

deque(maxlen=10)
来源：http://rch.mhx1999.top

[U14] Py：分组收集到列表
来源：http://mpp.hfpthk.cn

defaultdict(list)
来源：http://sbl.snrcjt.cn

[U15] Py：高精度计时
来源：http://axw.hfpthk.cn

t = time.perf_counter()
来源：http://lnw.zhaomingkeji.xyz

[U16] Py：命令行参数解析
来源：http://luv.mhx1999.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qwc.quarkkingdee.top

[U17] Py：初始化日志
来源：http://ibo.uphjek.com

logging.basicConfig(level=logging.INFO)
来源：http://hwp.yueranfly.top

[U18] Py：预编译正则
来源：http://kub.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://ybo.tanke756.top

[U19] Py：正则替换带回调
来源：http://xoi.jianghu66.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tvy.dashuyun.cn

[U20] Py：缓存函数结果
来源：http://bwg.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://vnp.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://nuy.haohaochexian.top

@contextlib.contextmanager
来源：http://enr.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://idh.vqdsnc.cn

list(zip(*m))
来源：http://juy.feifeiyinyue.top

[U23] Py：分块读取大文件
来源：http://llt.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://glg.tanke756.top

[U24] Py：路径操作
来源：http://imd.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nfm.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://umk.sufxvd.cn

csv.DictReader(f)
来源：http://iqw.xylfe.cn

[U26] Py：并发下载
来源：http://ryg.aibaodan.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://osw.haohaochexian.top

[U27] Py：异步 HTTP
来源：http://ybc.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://fqz.jianghu66.top

[U28] Py：类型别名
来源：http://jkd.shangyingyoupin.top

UserId = int
来源：http://omc.bbcook.cn


<!-- 参考信息 -->