代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zxh.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://big.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mri.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://xkd.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gcy.cheryme.top

[S10] C：指针与解引用
来源：http://ixj.zycfv.cn

int *p = &a;  *p = 5;
来源：http://yfc.nanxinkj.top

[S11] C：逐行读文件
来源：http://eeo.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://uvo.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bsb.yanxiufei.cn

fclose(f);
来源：http://flz.wangdashe.top

[S12] C：写文件
来源：http://gbq.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rwp.sweek.top

[S13] C：宏定义
来源：http://jsz.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hak.hysaishi.cn

[S14] C：枚举
来源：http://mim.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://cxb.yfazqb.com

[S15] C：类型转换
来源：http://chc.ydjk.org.cn

(double) a / b
来源：http://aps.yuxming.cn

[S16] C：位操作置位
来源：http://eow.jinqigufen.top

x |= (1 << 3);
来源：http://pyp.yj20258.top

[S17] C：安全拼接字符串
来源：http://znp.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mka.tanke756.top

[S18] C：命令行参数
来源：http://qom.havefunace.top

int main(int argc, char **argv)
来源：http://bju.nanxuanxn.top

[S19] C：快速排序
来源：http://xsd.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://ove.cashguo.top

[S20] C：二分查找
来源：http://ohi.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lpz.ivvv.top

[S21] C：字符类别判断
来源：http://bpt.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ueu.tanke756.top

[S22] C：字符串转数字
来源：http://ioe.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fvu.snrcjt.cn

[S23] C：随机数
来源：http://ulb.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fri.yonumen.top

[S24] C：获取本地时间
来源：http://rtm.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lgc.nanxinkj.top

[S25] C：内存拷贝
来源：http://zpu.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://gcu.shuidangran.top

[S26] C：内存清零
来源：http://jqy.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://blh.jlsjyb.cn

[S27] C：定义常量
来源：http://qum.guowangkeji.top

const double PI = 3.14159;
来源：http://naz.wangshuangyany.cn

[S28] C：静态变量
来源：http://liy.shangyingyoupin.top

static int counter = 0;
来源：http://cwi.redwolf501.top

[S29] C：变参函数
来源：http://rsw.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tbu.zdqjudy.top

[S30] C：头文件保护
来源：http://eoh.fzhhl.top

#ifndef X_H
来源：http://uvs.dashuyun.cn

#define X_H
来源：http://onx.cheryme.top

#endif
来源：http://wjl.svipenyu.cn

[S31] C++：Hello World
来源：http://igb.haohaochexian.top

#include <iostream>
来源：http://irh.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://voh.0kj1m.cn

[S32] C++：字符串
来源：http://icc.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://ahi.hammf.cn

[S33] C++：vector 增删
来源：http://otw.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://egs.yj202588.top

[S34] C++：遍历 vector
来源：http://kcv.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://mmu.bjfxy.top

[S35] C++：map
来源：http://oye.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qlp.andypj.xyz

[S36] C++：unordered_map
来源：http://zup.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mgm.jianghu66.top

[S37] C++：set
来源：http://jvy.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vva.chenlongwang.top

[S38] C++：排序
来源：http://mko.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://ubt.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://owy.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ocn.yangfankeji.com

[S40] C++：查找元素
来源：http://pgy.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qaj.shzxlz.cn

[S41] C++：类与构造函数
来源：http://tbs.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yoq.yuxming.cn

[S42] C++：继承与虚函数
来源：http://sex.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://xtf.0kj1m.cn

[S43] C++：智能指针
来源：http://cem.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://dkd.sweek.top

[S44] C++：引用传参
来源：http://paz.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://xcz.hfpthk.cn

[S45] C++：lambda
来源：http://cpb.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://kxp.xziqi.cn

[S46] C++：函数模板
来源：http://eqi.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xhn.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://cin.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfa.zhengqikj.top

[S48] C++：逐行读文件
来源：http://xts.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://hlr.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://rkq.tian-w.cn

[S49] C++：写文件
来源：http://vut.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oqz.jyoumei.cn

[S50] C++：格式化数字
来源：http://lhg.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kqh.hywenlv.cn

[S51] C++：显式类型转换
来源：http://iav.haohaochexian.top

static_cast<double>(a) / b
来源：http://oog.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://mjy.epnwcf.com

int size() const noexcept { return n_; }
来源：http://ekk.aizwys.cn

[S53] C++：移动语义
来源：http://awr.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://kcj.mhx1999.top

[S54] C++：异常处理
来源：http://ofg.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ifn.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://tdj.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wrl.hfpthk.cn

[S56] C++：optional
来源：http://ggv.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bhb.52xcode.cn

[S57] C++：编译期常量
来源：http://zty.zhoulong.xyz

constexpr int N = 10;
来源：http://ggv.wangdashe.top

[S58] C++：命名空间
来源：http://qwu.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://yqr.jlsjyb.cn

[S59] C++：静态断言
来源：http://bio.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bpd.ivvv.top

[S60] C++：遍历并删除元素
来源：http://fql.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://axg.aibaodan.cn

================================================================================
来源：http://gek.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://raw.316326.xyz

================================================================================
来源：http://moh.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://dhv.nwbrower.top

println("Hello")
来源：http://bfg.jinqigfzy.top

[T02] Kotlin：变量
来源：http://fpe.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oxb.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://xpq.daxiang520.top

"值: $b"
来源：http://gjw.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://vgt.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://xxd.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://lxc.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tjv.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://gfc.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://isu.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://bqh.iojbl.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lfn.hnqzz.top

[T08] Kotlin：数据类
来源：http://feu.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://vtt.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://aqr.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://wne.daria6918.cn

[T10] Kotlin：默认参数
来源：http://fqo.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://gnv.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://bhi.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bly.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://vme.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://nue.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://zof.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://umk.bjfxy.top

[T14] Kotlin：循环
来源：http://eic.fengsongda.top

for (i in 1..10) println(i)
来源：http://vyr.havefunace.top

[T15] Kotlin：接口
来源：http://lqj.yongpay.top

interface Shape { fun area(): Double }
来源：http://bbs.nanxuanxn.top

[T16] Swift：Hello World
来源：http://hmz.zhengqikj.top

print("Hello")
来源：http://fsk.tianlin.xyz

[T17] Swift：变量与常量
来源：http://jua.bjfxy.top

var a = 1;  let b = 2
来源：http://cwh.svipenyu.cn

[T18] Swift：字符串插值
来源：http://gih.tianlin.xyz

"值: \(b)"
来源：http://ahw.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://zeg.xziqi.cn

if let n = opt { print(n) }
来源：http://xzw.aibaodan.cn

[T20] Swift：数组操作
来源：http://vtl.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vxv.tianlin.xyz

[T21] Swift：遍历
来源：http://pyu.0kj1m.cn

for x in a { print(x) }
来源：http://bzc.yueranfly.top

[T22] Swift：字典
来源：http://ohp.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://zyj.dianchejie.cn

[T23] Swift：函数
来源：http://knf.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zvn.sufxvd.cn

[T24] Swift：闭包
来源：http://gpi.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ink.cashguo.top

[T25] Swift：结构体
来源：http://aud.chenjidiqi.icu

struct P { var x: Int }
来源：http://abc.yuanzhike.top

[T26] Swift：类与重写
来源：http://pwf.ehwqpu.com

class A: Base { override func f() {} }
来源：http://azx.haohaochexian.top

[T27] Swift：错误处理
来源：http://nel.havefunace.top

do { try f() } catch { print(error) }
来源：http://tpw.ybcxt.top

[T28] Swift：枚举
来源：http://gwp.shzxlz.cn

enum Color { case red, green }
来源：http://tqu.yanxiufei.cn

[T29] Swift：guard 提前返回
来源：http://bff.jinghuilouyu.cn

guard let x = opt else { return }
来源：http://qlf.xuanzx.com

[T30] Swift：协议
来源：http://dmt.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://prf.sxryk.cn

[T31] Lua：Hello World
来源：http://rzd.xuanzx.com

print("Hello")
来源：http://czj.hfpthk.cn

[T32] Lua：局部变量
来源：http://tje.ydzc1.top

local a = 1
来源：http://fsp.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://rka.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tqe.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://qjc.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bdb.fehbvm.com

[T35] Lua：字典表
来源：http://uri.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://sdi.jinqigufen.top

[T36] Lua：函数
来源：http://gtm.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://pgz.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://fpu.kuanghao11.cn

"a" .. "b"
来源：http://ugt.nanxuanxn.top

[T38] Lua：条件
来源：http://rgb.tian-w.cn

if x > 0 then print("正") end
来源：http://pvk.chenzaomai.com

[T39] Lua：模式匹配
来源：http://pvr.gaohongyu789.top

string.find(s, "%d+")
来源：http://zcc.cashguo.top

[T40] Lua：元表
来源：http://fsv.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://rpd.fehbvm.com

[T41] Perl：Hello World
来源：http://ijx.0kj1m.cn

print "Hello\n";
来源：http://vqx.snrcjt.cn

[T42] Perl：变量类型
来源：http://zet.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ctc.jyoumei.cn

[T43] Perl：字符串插值
来源：http://try.haohaochexian.top

"值: $a"
来源：http://qwe.hongshengwenyu.top

[T44] Perl：条件
来源：http://ngg.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://wbx.fktsv.cn

[T45] Perl：数组遍历
来源：http://lcj.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://fuo.wangdashe.top

[T46] Perl：哈希操作
来源：http://xhw.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wli.316326.xyz

[T47] Perl：正则捕获
来源：http://nfz.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ehx.dashuyun.cn

[T48] Perl：正则替换
来源：http://pzr.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://sjr.yueranfly.top

[T49] Perl：函数
来源：http://trw.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rla.yj202588.top

[T50] Perl：逐行读文件
来源：http://oqv.hfpthk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ium.xylfe.cn

while (my $line = <$fh>) { print $line; }
来源：http://cti.nwbrower.top

[T51] Scala：Hello World
来源：http://bdm.yuanzhike.top

println("Hello")
来源：http://oin.0kj1m.cn

[T52] Scala：变量
来源：http://vfu.iojbl.cn

val a = 1;  var b = 2
来源：http://ugl.zycfv.cn

[T53] Scala：字符串插值
来源：http://rdm.gaohongyu789.top

s"值: $b"
来源：http://xet.hcnkem.com

[T54] Scala：集合映射
来源：http://phw.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://yem.yj20258888.top

[T55] Scala：集合过滤
来源：http://xmx.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://zap.yuxming.cn

[T56] Scala：样例类
来源：http://ekq.haohaochexian.top

case class User(name: String, age: Int)
来源：http://ize.redwolf501.top

[T57] Scala：模式匹配
来源：http://ltu.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ucz.tarul.cn

[T58] Scala：函数定义
来源：http://cmy.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://plp.guannengcc.top

[T59] Scala：循环
来源：http://ztq.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://qzf.316326.xyz

[T60] Scala：折叠
来源：http://mde.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zqm.ivvv.top

================================================================================
来源：http://brm.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://toq.shzxlz.cn

================================================================================
来源：http://lar.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://hii.ydzc1.top

python -m venv .venv && source .venv/bin/activate
来源：http://sbf.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://ytz.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fwy.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://cqe.zycfv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vju.ybcxt.top

[U04] Py：变量调试打印
来源：http://pyk.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eqr.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://syp.cqqwz.cn

list(dict.fromkeys(arr))
来源：http://zkh.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://feo.iojbl.cn

{**a, **b}
来源：http://sic.ybcxt.top

[U07] Py：反转字典键值
来源：http://kpt.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://lcw.jqgfzy.top

[U08] Py：展平二维列表
来源：http://epz.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://dna.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://sze.chenjidiqi.icu

max(d, key=d.get)
来源：http://rjo.aibaodan.cn

[U10] Py：按值排序字典
来源：http://vhb.yvedp.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pff.fengsongda.top

[U11] Py：生成器表达式
来源：http://ruz.ydzc1.top

(x * 2 for x in arr)
来源：http://uct.xylfe.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jjn.gogol.net.cn

Counter(arr).most_common(3)
来源：http://jpu.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://rrt.fanxiaobao.xyz

deque(maxlen=10)
来源：http://nvh.yonumen.top

[U14] Py：分组收集到列表
来源：http://mpa.uphjek.com

defaultdict(list)
来源：http://vow.hywenlv.cn

[U15] Py：高精度计时
来源：http://ccn.ehwqpu.com

t = time.perf_counter()
来源：http://gub.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://nek.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zel.jinqigfzy.top

[U17] Py：初始化日志
来源：http://bgi.shangyingyoupin.top

logging.basicConfig(level=logging.INFO)
来源：http://jus.iojbl.cn

[U18] Py：预编译正则
来源：http://dhq.sweek.top

pat = re.compile(r"\d+")
来源：http://mcv.uphjek.com

[U19] Py：正则替换带回调
来源：http://xyv.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://knf.fzhhl.top

[U20] Py：缓存函数结果
来源：http://dce.fktsv.cn

@functools.lru_cache(maxsize=None)
来源：http://iax.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://npj.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://uhc.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://edz.shzxlz.cn

list(zip(*m))
来源：http://cyk.pengpengdd.cyou

[U23] Py：分块读取大文件
来源：http://xoo.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bgw.feifeiyinyue.top

[U24] Py：路径操作
来源：http://rbr.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cvo.havefunace.top

[U25] Py：CSV 按字典读
来源：http://zqm.zycfv.cn

csv.DictReader(f)
来源：http://htl.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://zzh.chenjidiqi.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rww.yueranfly.top

[U27] Py：异步 HTTP
来源：http://pjw.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://yde.zhixingplan.top

[U28] Py：类型别名
来源：http://lwl.redwolf501.top

UserId = int
来源：http://ijt.sweek.top

[U29] Py：属性校验
来源：http://xqy.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://unb.andypj.xyz

[U30] Py：数据类
来源：http://wia.yvedp.cn

@dataclass(slots=True)
来源：http://dey.vehdjk.com


<!-- 参考信息 -->