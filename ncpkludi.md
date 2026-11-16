代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://quz.pycfn.com

[S13] C：宏定义
来源：http://gnv.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dou.yuxming.cn

[S14] C：枚举
来源：http://aer.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://tsl.yvedp.cn

[S15] C：类型转换
来源：http://utt.jinghuilouyu.cn

(double) a / b
来源：http://qrl.9152youxi.cn

[S16] C：位操作置位
来源：http://pgc.zhixingplan.top

x |= (1 << 3);
来源：http://hgw.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://bgu.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rds.iojbl.cn

[S18] C：命令行参数
来源：http://cza.fzhhl.top

int main(int argc, char **argv)
来源：http://htq.yonumen.top

[S19] C：快速排序
来源：http://omp.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://nla.yueranfly.top

[S20] C：二分查找
来源：http://thd.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ztv.ctjpmb.com

[S21] C：字符类别判断
来源：http://pnp.shangyingyoupin.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nuu.tanke756.top

[S22] C：字符串转数字
来源：http://gvk.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://zbd.fanxiaobao.xyz

[S23] C：随机数
来源：http://vhs.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://han.yj20258.top

[S24] C：获取本地时间
来源：http://hur.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wfe.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://wrq.daxiang520.top

memcpy(dst, src, n);
来源：http://cyt.hywenlv.cn

[S26] C：内存清零
来源：http://hvj.jianghu66.top

memset(a, 0, sizeof a);
来源：http://juk.snrcjt.cn

[S27] C：定义常量
来源：http://zsw.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://zqp.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://krd.xuetiantiany.cn

static int counter = 0;
来源：http://cbx.cucudq.cn

[S29] C：变参函数
来源：http://nmu.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ngr.quarkkingdee.top

[S30] C：头文件保护
来源：http://fwp.52xcode.cn

#ifndef X_H
来源：http://vii.316326.xyz

#define X_H
来源：http://mro.jqgfzy.top

#endif
来源：http://rod.jinqigfzy.top

[S31] C++：Hello World
来源：http://xnr.xuetiantiany.cn

#include <iostream>
来源：http://iqx.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://rqy.hongshengwenyu.top

[S32] C++：字符串
来源：http://shr.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://ekg.cdnleiting.top

[S33] C++：vector 增删
来源：http://lks.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aiw.ybcxt.top

[S34] C++：遍历 vector
来源：http://sut.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://sng.jinghuilouyu.cn

[S35] C++：map
来源：http://pns.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dkb.yuanzhike.top

[S36] C++：unordered_map
来源：http://jzu.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dkv.gotoacloud.top

[S37] C++：set
来源：http://tad.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cxg.zycfv.cn

[S38] C++：排序
来源：http://ipi.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://xiy.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://mqv.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kfx.shzxlz.cn

[S40] C++：查找元素
来源：http://wzr.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vog.cdnleiting.top

[S41] C++：类与构造函数
来源：http://acv.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aae.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://oct.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://wkv.tarul.cn

[S43] C++：智能指针
来源：http://wdy.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://bfo.9152youxi.cn

[S44] C++：引用传参
来源：http://zri.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://kek.havefunace.top

[S45] C++：lambda
来源：http://arv.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://jnm.shuidangran.top

[S46] C++：函数模板
来源：http://dcs.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iis.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://mcs.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cpd.cashguo.top

[S48] C++：逐行读文件
来源：http://bbm.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://cvq.sxryk.cn

while (std::getline(in, line)) { }
来源：http://yjn.yj20258.top

[S49] C++：写文件
来源：http://vub.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ayl.tianlin.xyz

[S50] C++：格式化数字
来源：http://dhf.svipenyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://crj.guannengcc.top

[S51] C++：显式类型转换
来源：http://mir.jinqigufen.top

static_cast<double>(a) / b
来源：http://nke.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://myx.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://cnj.hcnkem.com

[S53] C++：移动语义
来源：http://dpe.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://etx.hnxiangtu.top

[S54] C++：异常处理
来源：http://wpm.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qtv.xuanzx.com

[S55] C++：结构化绑定
来源：http://vkl.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ame.zhixingplan.top

[S56] C++：optional
来源：http://opg.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xoa.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://hvt.yfazqb.com

constexpr int N = 10;
来源：http://wiw.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://eix.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://lqc.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://ysr.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fbg.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://czc.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pgg.gogol.net.cn

================================================================================
来源：http://odk.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nvv.tianlin.xyz

================================================================================
来源：http://hip.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://njm.0kj1m.cn

println("Hello")
来源：http://arq.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://tqv.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://afw.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://bla.ivvv.top

"值: $b"
来源：http://iho.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://uux.cucudq.cn

val n: String? = null;  n?.length
来源：http://plw.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://lpc.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yvl.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://fvt.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cqo.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://zcx.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gvj.nwbrower.top

[T08] Kotlin：数据类
来源：http://vjj.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://sim.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://vnl.sweek.top

fun String.exclaim() = this + "!"
来源：http://rpp.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://gid.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xlv.chenzaomai.com

[T11] Kotlin：协程
来源：http://vtk.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nhr.sysykeji.top

[T12] Kotlin：解构声明
来源：http://yeh.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://mpc.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://shz.redwolf501.top

val m = mapOf("a" to 1)
来源：http://oqa.gzhubu.top

[T14] Kotlin：循环
来源：http://dat.smart0.xyz

for (i in 1..10) println(i)
来源：http://jhp.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://kcs.zycfv.cn

interface Shape { fun area(): Double }
来源：http://xxa.iojbl.cn

[T16] Swift：Hello World
来源：http://mql.ctjpmb.com

print("Hello")
来源：http://zct.jqgfzy.top

[T17] Swift：变量与常量
来源：http://cpc.jinqigfzy.top

var a = 1;  let b = 2
来源：http://ezn.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://juf.sxryk.cn

"值: \(b)"
来源：http://kxa.yvedp.cn

[T19] Swift：可选绑定
来源：http://ezg.haohaochexian.top

if let n = opt { print(n) }
来源：http://pqq.zhixingplan.top

[T20] Swift：数组操作
来源：http://gnz.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://frj.nanxuanxn.top

[T21] Swift：遍历
来源：http://uis.aibaodan.cn

for x in a { print(x) }
来源：http://cmn.shangyingyoupin.top

[T22] Swift：字典
来源：http://dwn.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://xkz.0kj1m.cn

[T23] Swift：函数
来源：http://cbt.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dgf.jinqigfzy.top

[T24] Swift：闭包
来源：http://bjs.andypj.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://qyi.nanxuanxn.top

[T25] Swift：结构体
来源：http://dpm.zhongyouzk.top

struct P { var x: Int }
来源：http://fvh.vehdjk.com

[T26] Swift：类与重写
来源：http://mfv.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://axw.snrcjt.cn

[T27] Swift：错误处理
来源：http://lgl.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://fvm.hongshengwenyu.top

[T28] Swift：枚举
来源：http://wnk.xuetiantiany.cn

enum Color { case red, green }
来源：http://bwe.hammf.cn

[T29] Swift：guard 提前返回
来源：http://vkq.aizwys.cn

guard let x = opt else { return }
来源：http://wph.fehbvm.com

[T30] Swift：协议
来源：http://zhi.havefunace.top

protocol Shape { func area() -> Double }
来源：http://mmh.xinyue.icu

[T31] Lua：Hello World
来源：http://sth.xziqi.cn

print("Hello")
来源：http://bji.jlsjyb.cn

[T32] Lua：局部变量
来源：http://ulr.ehwqpu.com

local a = 1
来源：http://jit.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://ynx.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iiy.dianchejie.cn

[T34] Lua：遍历表
来源：http://lry.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://jbs.ctjpmb.com

[T35] Lua：字典表
来源：http://rwr.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://uhr.havefunace.top

[T36] Lua：函数
来源：http://qzl.snrcjt.cn

function add(a, b) return a + b end
来源：http://gao.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://cvu.andypj.xyz

"a" .. "b"
来源：http://gsk.hnxiangtu.top

[T38] Lua：条件
来源：http://rfz.yuanzhike.top

if x > 0 then print("正") end
来源：http://vrv.xziqi.cn

[T39] Lua：模式匹配
来源：http://mcu.smart0.xyz

string.find(s, "%d+")
来源：http://pfi.sufxvd.cn

[T40] Lua：元表
来源：http://smz.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://nit.cucudq.cn

[T41] Perl：Hello World
来源：http://igi.shanyushiyangtech.top

print "Hello\n";
来源：http://bab.yuanzhike.top

[T42] Perl：变量类型
来源：http://qrq.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kqx.yvedp.cn

[T43] Perl：字符串插值
来源：http://szj.gzhubu.top

"值: $a"
来源：http://ubr.guannengcc.top

[T44] Perl：条件
来源：http://dgq.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://goi.nanxinkj.top

[T45] Perl：数组遍历
来源：http://mtj.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://fjt.aibaodan.cn

[T46] Perl：哈希操作
来源：http://cdg.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vjo.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://dad.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mxy.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://wcm.hfpthk.cn

$s =~ s/old/new/g;
来源：http://lca.sjlbkw.cn

[T49] Perl：函数
来源：http://dvi.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ztp.bbcook.cn

[T50] Perl：逐行读文件
来源：http://kcj.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qid.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://bvk.sweek.top

[T51] Scala：Hello World
来源：http://plp.yueranfly.top

println("Hello")
来源：http://khg.yj20258.top

[T52] Scala：变量
来源：http://xhe.yfazqb.com

val a = 1;  var b = 2
来源：http://olu.zdbjq.cn

[T53] Scala：字符串插值
来源：http://hom.pengpengdd.cyou

s"值: $b"
来源：http://rph.cheryme.top

[T54] Scala：集合映射
来源：http://dfb.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://bgn.pycfn.com

[T55] Scala：集合过滤
来源：http://jww.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://rjw.snrcjt.cn

[T56] Scala：样例类
来源：http://dhb.guannengcc.top

case class User(name: String, age: Int)
来源：http://kqk.52xcode.cn

[T57] Scala：模式匹配
来源：http://cci.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wok.jyoumei.cn

[T58] Scala：函数定义
来源：http://gof.aizwys.cn

def add(a: Int, b: Int): Int = a + b
来源：http://swc.jianghu66.top

[T59] Scala：循环
来源：http://fef.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://yyr.tarul.cn

[T60] Scala：折叠
来源：http://cwu.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://krf.daria6918.cn

================================================================================
来源：http://fnl.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ctt.xuetiantiany.cn

================================================================================
来源：http://zhi.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://cqm.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://unw.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://fan.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sbb.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://plm.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://riz.snrcjt.cn

[U04] Py：变量调试打印
来源：http://gxg.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jtn.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://fub.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://vmb.chenzaomai.com

[U06] Py：合并两个字典
来源：http://ksf.shuidangran.top

{**a, **b}
来源：http://oof.pycfn.com

[U07] Py：反转字典键值
来源：http://evf.yuanzhike.top

{v: k for k, v in d.items()}
来源：http://kqj.gzhubu.top

[U08] Py：展平二维列表
来源：http://xde.zycfv.cn

[y for x in nested for y in x]
来源：http://yya.aizwys.cn

[U09] Py：字典取最大值的键
来源：http://ldd.cqqwz.cn

max(d, key=d.get)
来源：http://unl.hfpthk.cn

[U10] Py：按值排序字典
来源：http://cxb.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fjt.0kj1m.cn

[U11] Py：生成器表达式
来源：http://yec.sxryk.cn

(x * 2 for x in arr)
来源：http://pge.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dhs.hywenlv.cn

Counter(arr).most_common(3)
来源：http://ezr.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://rgj.shanyushiyangkeji.top

deque(maxlen=10)
来源：http://pqt.wangshuangyany.cn

[U14] Py：分组收集到列表
来源：http://lay.jiagoushi.top

defaultdict(list)
来源：http://jku.zdqjudy.top

[U15] Py：高精度计时
来源：http://jbr.shanyushiyangkeji.top

t = time.perf_counter()
来源：http://qmp.guannengcc.top

[U16] Py：命令行参数解析
来源：http://cws.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bxt.hnxiangtu.top

[U17] Py：初始化日志
来源：http://idw.sysykeji.top

logging.basicConfig(level=logging.INFO)
来源：http://pnv.iojbl.cn

[U18] Py：预编译正则
来源：http://nug.ydzc1.top

pat = re.compile(r"\d+")
来源：http://zyi.jinyuanbaomall.cn

[U19] Py：正则替换带回调
来源：http://kzt.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zac.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://pua.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://rno.yj202588.top

[U21] Py：自定义上下文管理器
来源：http://rpn.sjlbkw.cn

@contextlib.contextmanager
来源：http://hme.sysykeji.top

[U22] Py：矩阵转置
来源：http://zmd.yfazqb.com

list(zip(*m))
来源：http://akn.jinyuanbaomall.cn

[U23] Py：分块读取大文件
来源：http://lsu.tarul.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lal.zhijiandao.cn

[U24] Py：路径操作
来源：http://dks.xziqi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sgo.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://gnf.zhengqikj.top

csv.DictReader(f)
来源：http://uea.xuetiantiany.cn

[U26] Py：并发下载
来源：http://djr.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pug.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://wzd.bjfxy.top

aiohttp.ClientSession() 配合 async with
来源：http://mcu.kuanghao11.cn

[U28] Py：类型别名
来源：http://mai.jinqigufen.top

UserId = int
来源：http://tsx.svipenyu.cn

[U29] Py：属性校验
来源：http://ref.yonumen.top

@property 与 @x.setter 配合
来源：http://vpg.zhijiandao.cn

[U30] Py：数据类
来源：http://lva.sysykeji.top

@dataclass(slots=True)
来源：http://pzs.yj20258.top

[U31] Py：单测
来源：http://gpt.hfpthk.cn

python -m pytest -q
来源：http://srx.yuxming.cn

[U32] Py：代码格式化
来源：http://lfz.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://xtg.kuanghao11.cn

[U33] Py：打包发布
来源：http://gxc.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://ppz.ybcxt.top

[U34] Py：判断编码
来源：http://yzo.zhengqikj.top

chardet.detect(raw)
来源：http://bbp.316326.xyz

[U35] Py：发送邮件
来源：http://eqq.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://izb.xylfe.cn

[U36] Py：定时任务
来源：http://owk.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://zjp.xylfe.cn


<!-- 参考信息 -->