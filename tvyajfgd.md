代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tuo.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://kor.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wgr.yj202588.top

[S09] C：结构体定义与初始化
来源：http://yrf.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dav.yj20258888.top

[S10] C：指针与解引用
来源：http://pir.hcnkem.com

int *p = &a;  *p = 5;
来源：http://cyf.ppjwa.cn

[S11] C：逐行读文件
来源：http://dmk.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://fci.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ptm.bbcook.cn

fclose(f);
来源：http://aor.nanxuanxn.top

[S12] C：写文件
来源：http://etj.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rev.bjfxy.top

[S13] C：宏定义
来源：http://wci.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fzv.zhijiandao.cn

[S14] C：枚举
来源：http://nnt.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://hft.zycfv.cn

[S15] C：类型转换
来源：http://wfa.redwolf501.top

(double) a / b
来源：http://hix.jqgufenzy.top

[S16] C：位操作置位
来源：http://jdk.yonumen.top

x |= (1 << 3);
来源：http://cpw.ivvv.top

[S17] C：安全拼接字符串
来源：http://igv.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wnx.tian-w.cn

[S18] C：命令行参数
来源：http://jhn.dashuyun.cn

int main(int argc, char **argv)
来源：http://qxn.yuanzhike.top

[S19] C：快速排序
来源：http://tzc.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://oic.sweek.top

[S20] C：二分查找
来源：http://htf.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mlf.gotoacloud.top

[S21] C：字符类别判断
来源：http://mrb.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gyl.tian-w.cn

[S22] C：字符串转数字
来源：http://vwh.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://iyi.shanyushiyangtech.top

[S23] C：随机数
来源：http://rbd.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zql.hfpthk.cn

[S24] C：获取本地时间
来源：http://fkw.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ivf.jyoumei.cn

[S25] C：内存拷贝
来源：http://zlt.pycfn.com

memcpy(dst, src, n);
来源：http://dya.aibaodan.cn

[S26] C：内存清零
来源：http://vob.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://oga.xuanzx.com

[S27] C：定义常量
来源：http://srk.chenzaomai.com

const double PI = 3.14159;
来源：http://jhn.yongpay.top

[S28] C：静态变量
来源：http://fsp.yvedp.cn

static int counter = 0;
来源：http://bww.cheryme.top

[S29] C：变参函数
来源：http://zvn.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lkr.kuanghao11.cn

[S30] C：头文件保护
来源：http://chk.hongshengwenyu.top

#ifndef X_H
来源：http://cpl.ybcxt.top

#define X_H
来源：http://gkj.xingfuxueyuan.xyz

#endif
来源：http://ftr.daxiang520.top

[S31] C++：Hello World
来源：http://xht.c1oappe.top

#include <iostream>
来源：http://uwc.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://dyf.yj20258888.top

[S32] C++：字符串
来源：http://iun.meibo888.top

std::string s = "hi";  s += "!";
来源：http://yjn.aibaodan.cn

[S33] C++：vector 增删
来源：http://wgq.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nke.yvedp.cn

[S34] C++：遍历 vector
来源：http://edx.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://eiw.gzhubu.top

[S35] C++：map
来源：http://fca.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fjp.chenlongwang.top

[S36] C++：unordered_map
来源：http://alj.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xpq.snrcjt.cn

[S37] C++：set
来源：http://gfx.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ixd.zhijiandao.cn

[S38] C++：排序
来源：http://mth.316326.xyz

std::sort(v.begin(), v.end());
来源：http://icd.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://qem.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kmn.smart0.xyz

[S40] C++：查找元素
来源：http://lgo.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://irf.snrcjt.cn

[S41] C++：类与构造函数
来源：http://dck.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nxn.wangdashe.top

[S42] C++：继承与虚函数
来源：http://xhe.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://qpy.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://hbz.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://lpg.yonumen.top

[S44] C++：引用传参
来源：http://wbp.hesvh.cn

void inc(int &x) { ++x; }
来源：http://glh.hnqzz.top

[S45] C++：lambda
来源：http://mub.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://mqu.smart0.xyz

[S46] C++：函数模板
来源：http://xqp.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xam.hesvh.cn

[S47] C++：结构化绑定遍历
来源：http://stb.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kax.gotoacloud.top

[S48] C++：逐行读文件
来源：http://met.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://joz.cashguo.top

while (std::getline(in, line)) { }
来源：http://izc.yfazqb.com

[S49] C++：写文件
来源：http://axn.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://odx.sweek.top

[S50] C++：格式化数字
来源：http://msa.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oln.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://rpb.yueranfly.top

static_cast<double>(a) / b
来源：http://wbs.yonumen.top

[S52] C++：const 与 noexcept
来源：http://poi.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://esu.cashguo.top

[S53] C++：移动语义
来源：http://qia.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://glu.tian-w.cn

[S54] C++：异常处理
来源：http://ryb.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nkl.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://tvw.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://bdr.ybcxt.top

[S56] C++：optional
来源：http://eqh.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qcc.iojbl.cn

[S57] C++：编译期常量
来源：http://gei.yangfankeji.com

constexpr int N = 10;
来源：http://gqi.svipenyu.cn

[S58] C++：命名空间
来源：http://uqp.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://sor.zhongyouzk.top

[S59] C++：静态断言
来源：http://qhm.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://roj.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://tfz.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lai.chenjidiqi.icu

================================================================================
来源：http://rcz.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ayv.jinyuanbaomall.cn

================================================================================
来源：http://ede.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://tav.fehbvm.com

println("Hello")
来源：http://tfs.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://bdb.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://llv.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://rwy.ctjpmb.com

"值: $b"
来源：http://giz.fehbvm.com

[T04] Kotlin：空安全
来源：http://xnr.iojbl.cn

val n: String? = null;  n?.length
来源：http://wfm.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://bxo.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mwi.yuxming.cn

[T06] Kotlin：集合映射
来源：http://xnh.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hwa.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://ess.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwg.zdbjq.cn

[T08] Kotlin：数据类
来源：http://ani.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://lwb.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://tys.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://azs.nwbrower.top

[T10] Kotlin：默认参数
来源：http://eob.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oio.ydjk.org.cn

[T11] Kotlin：协程
来源：http://tid.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnl.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://fqn.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://keo.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://kem.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://ujf.0kj1m.cn

[T14] Kotlin：循环
来源：http://zjj.gogol.net.cn

for (i in 1..10) println(i)
来源：http://uoz.uphjek.com

[T15] Kotlin：接口
来源：http://oai.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://xuc.cdnleiting.top

[T16] Swift：Hello World
来源：http://wmf.ivvv.top

print("Hello")
来源：http://owa.yj202588.top

[T17] Swift：变量与常量
来源：http://ioc.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://hqw.dianchejie.cn

[T18] Swift：字符串插值
来源：http://qsp.wangshuangyany.cn

"值: \(b)"
来源：http://ykd.chenzaomai.com

[T19] Swift：可选绑定
来源：http://tfi.yj202588.top

if let n = opt { print(n) }
来源：http://ksw.xinyue.icu

[T20] Swift：数组操作
来源：http://kws.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://csu.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://qla.guannengcc.top

for x in a { print(x) }
来源：http://yhz.gotoacloud.top

[T22] Swift：字典
来源：http://bem.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cmc.shanyushiyangtech.top

[T23] Swift：函数
来源：http://wle.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fli.meibo888.top

[T24] Swift：闭包
来源：http://dbr.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wsp.mhx1999.top

[T25] Swift：结构体
来源：http://ryp.bjfxy.top

struct P { var x: Int }
来源：http://ndt.cheryme.top

[T26] Swift：类与重写
来源：http://asx.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://fbv.hywenlv.cn

[T27] Swift：错误处理
来源：http://ygt.birdmap.top

do { try f() } catch { print(error) }
来源：http://roa.bjfxy.top

[T28] Swift：枚举
来源：http://vli.dashuyun.cn

enum Color { case red, green }
来源：http://tqk.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://xfw.zhengqikj.top

guard let x = opt else { return }
来源：http://fhh.cucudq.cn

[T30] Swift：协议
来源：http://dsu.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://fjn.meibo888.top

[T31] Lua：Hello World
来源：http://tch.guannengcc.top

print("Hello")
来源：http://oej.cashguo.top

[T32] Lua：局部变量
来源：http://tpa.pengpengdd.cyou

local a = 1
来源：http://kck.yj202588.top

[T33] Lua：表（数组）
来源：http://oby.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://esl.cqqwz.cn

[T34] Lua：遍历表
来源：http://lye.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xxc.zycfv.cn

[T35] Lua：字典表
来源：http://nzk.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://gib.pycfn.com

[T36] Lua：函数
来源：http://jxp.andypj.xyz

function add(a, b) return a + b end
来源：http://tem.daria6918.cn

[T37] Lua：字符串拼接
来源：http://rqn.guowangkeji.top

"a" .. "b"
来源：http://flo.0kj1m.cn

[T38] Lua：条件
来源：http://zwh.hywenlv.cn

if x > 0 then print("正") end
来源：http://csy.yj20258.top

[T39] Lua：模式匹配
来源：http://bnz.bjfxy.top

string.find(s, "%d+")
来源：http://lzn.hcnkem.com

[T40] Lua：元表
来源：http://ese.xziqi.cn

setmetatable({}, { __index = base })
来源：http://jys.tian-w.cn

[T41] Perl：Hello World
来源：http://dev.smart0.xyz

print "Hello\n";
来源：http://txb.svipenyu.cn

[T42] Perl：变量类型
来源：http://soj.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uxd.yvedp.cn

[T43] Perl：字符串插值
来源：http://ltu.hnqzz.top

"值: $a"
来源：http://hzn.hywenlv.cn

[T44] Perl：条件
来源：http://kbi.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://wbk.svipenyu.cn

[T45] Perl：数组遍历
来源：http://fxp.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://nms.aibaodan.cn

[T46] Perl：哈希操作
来源：http://rmr.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xoa.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://dwo.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tzj.smart0.xyz

[T48] Perl：正则替换
来源：http://hmz.aibaodan.cn

$s =~ s/old/new/g;
来源：http://zyz.wangshuangyany.cn

[T49] Perl：函数
来源：http://kav.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nfy.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://nlj.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ayp.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://ovo.zycfv.cn

[T51] Scala：Hello World
来源：http://oje.52xcode.cn

println("Hello")
来源：http://fkh.redwolf501.top

[T52] Scala：变量
来源：http://rtf.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://zvf.fengsongda.top

[T53] Scala：字符串插值
来源：http://eaa.sweek.top

s"值: $b"
来源：http://ilo.nanxinkj.top

[T54] Scala：集合映射
来源：http://hii.cashguo.top

List(1, 2, 3).map(_ * 2)
来源：http://agr.gzhubu.top

[T55] Scala：集合过滤
来源：http://izj.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://lvw.svipenyu.cn

[T56] Scala：样例类
来源：http://vtj.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://oes.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://tcd.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wwg.c1oappe.top

[T58] Scala：函数定义
来源：http://ave.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zte.nwbrower.top

[T59] Scala：循环
来源：http://xjk.ppjwa.cn

for (i <- 1 to 10) println(i)
来源：http://ccf.yj20258888.top

[T60] Scala：折叠
来源：http://jec.zhoulong.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://odr.0kj1m.cn

================================================================================
来源：http://hru.aibaodan.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yor.bbcook.cn

================================================================================
来源：http://xmk.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://viv.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jte.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://erk.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nth.tanke756.top

[U03] Py：加载 .env 配置
来源：http://oqz.xuetiantiany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rhi.snrcjt.cn

[U04] Py：变量调试打印
来源：http://bgu.wangshuangyany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bml.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://pqv.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://mgj.yongpay.top

[U06] Py：合并两个字典
来源：http://qaq.zhengqikj.top

{**a, **b}
来源：http://hgu.tian-w.cn

[U07] Py：反转字典键值
来源：http://vwe.yuxming.cn

{v: k for k, v in d.items()}
来源：http://oaw.hysaishi.cn

[U08] Py：展平二维列表
来源：http://ixx.zdbjq.cn

[y for x in nested for y in x]
来源：http://llj.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://ndb.jinqigufen.top

max(d, key=d.get)
来源：http://ulh.yj20258888.top

[U10] Py：按值排序字典
来源：http://yry.xuetiantiany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kcn.aizwys.cn

[U11] Py：生成器表达式
来源：http://ath.zhixingplan.top

(x * 2 for x in arr)
来源：http://voz.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uht.pengpengdd.cyou

Counter(arr).most_common(3)
来源：http://zbn.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://hed.guowangkeji.top

deque(maxlen=10)
来源：http://qeu.tianlin.xyz

[U14] Py：分组收集到列表
来源：http://rdn.jlsjyb.cn

defaultdict(list)
来源：http://phg.daxiang520.top

[U15] Py：高精度计时
来源：http://osv.tarul.cn

t = time.perf_counter()
来源：http://amg.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://qlb.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vzp.zhaomingkeji.xyz

[U17] Py：初始化日志
来源：http://lud.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://wpm.guowangkeji.top

[U18] Py：预编译正则
来源：http://gac.yj20258888.top

pat = re.compile(r"\d+")
来源：http://jti.fengsongda.top

[U19] Py：正则替换带回调
来源：http://lnp.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gbk.xingfuxueyuan.xyz

[U20] Py：缓存函数结果
来源：http://zdg.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://iqh.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://ydp.tarul.cn

@contextlib.contextmanager
来源：http://mja.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://dng.shuidangran.top

list(zip(*m))
来源：http://qik.gotoacloud.top

[U23] Py：分块读取大文件
来源：http://xiv.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lwu.ywan-chungtsiang.top

[U24] Py：路径操作
来源：http://ozx.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hoy.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://deu.jinqigufen.top

csv.DictReader(f)
来源：http://bnk.yonumen.top

[U26] Py：并发下载
来源：http://rqd.guannengcc.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fxo.jinqigfzy.top

[U27] Py：异步 HTTP
来源：http://lzk.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://gsw.hesvh.cn

[U28] Py：类型别名
来源：http://rmx.ydzc1.top

UserId = int
来源：http://gby.cucudq.cn

[U29] Py：属性校验
来源：http://ziy.hywenlv.cn

@property 与 @x.setter 配合
来源：http://oov.tanke756.top

[U30] Py：数据类
来源：http://elm.52xcode.cn

@dataclass(slots=True)
来源：http://nyz.yfazqb.com


<!-- 参考信息 -->