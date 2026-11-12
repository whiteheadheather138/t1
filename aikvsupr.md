代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yva.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://wky.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqo.ctjpmb.com

[S14] C：枚举
来源：http://yjr.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://mji.316326.xyz

[S15] C：类型转换
来源：http://ebn.jinqigfzy.top

(double) a / b
来源：http://sop.shzxlz.cn

[S16] C：位操作置位
来源：http://lmf.zhengqikj.top

x |= (1 << 3);
来源：http://ybr.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://nlz.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vko.ybcxt.top

[S18] C：命令行参数
来源：http://tzo.yj202588.top

int main(int argc, char **argv)
来源：http://ncy.sysykeji.top

[S19] C：快速排序
来源：http://nea.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://jgo.jinghuilouyu.cn

[S20] C：二分查找
来源：http://phv.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qax.hnxiangtu.top

[S21] C：字符类别判断
来源：http://sbr.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tha.nwbrower.top

[S22] C：字符串转数字
来源：http://sac.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://yaz.ywan-chungtsiang.top

[S23] C：随机数
来源：http://pbf.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://icu.chenlongwang.top

[S24] C：获取本地时间
来源：http://iyh.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jpw.fktsv.cn

[S25] C：内存拷贝
来源：http://pcv.andypj.xyz

memcpy(dst, src, n);
来源：http://ona.fktsv.cn

[S26] C：内存清零
来源：http://jfa.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://dar.hnqzz.top

[S27] C：定义常量
来源：http://sxc.gotoacloud.top

const double PI = 3.14159;
来源：http://vkm.smart0.xyz

[S28] C：静态变量
来源：http://zca.shangyingyoupin.top

static int counter = 0;
来源：http://dyy.c1oappe.top

[S29] C：变参函数
来源：http://ukx.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ewl.yj20258.top

[S30] C：头文件保护
来源：http://pcs.pengpengdd.cyou

#ifndef X_H
来源：http://ofd.yvedp.cn

#define X_H
来源：http://xab.yj202588.top

#endif
来源：http://web.yongpay.top

[S31] C++：Hello World
来源：http://zfc.birdmap.top

#include <iostream>
来源：http://zvg.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://kjo.c1oappe.top

[S32] C++：字符串
来源：http://qpc.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://yyu.hesvh.cn

[S33] C++：vector 增删
来源：http://vop.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://okf.nanxinkj.top

[S34] C++：遍历 vector
来源：http://hkz.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://yxn.hywenlv.cn

[S35] C++：map
来源：http://zqh.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jue.yuxming.cn

[S36] C++：unordered_map
来源：http://yck.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oxm.ppjwa.cn

[S37] C++：set
来源：http://oqx.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lyt.bbcook.cn

[S38] C++：排序
来源：http://ljk.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://sby.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://cje.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcz.shuidangran.top

[S40] C++：查找元素
来源：http://nzm.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pfe.tarul.cn

[S41] C++：类与构造函数
来源：http://tdr.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sdq.bbcook.cn

[S42] C++：继承与虚函数
来源：http://nde.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://pjd.chenzaomai.com

[S43] C++：智能指针
来源：http://njj.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://dph.tian-w.cn

[S44] C++：引用传参
来源：http://iqw.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://ana.gogol.net.cn

[S45] C++：lambda
来源：http://zsf.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://pkr.daria6918.cn

[S46] C++：函数模板
来源：http://hrd.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://beg.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://fnb.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mfb.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://eex.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://shg.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://mur.yfazqb.com

[S49] C++：写文件
来源：http://irm.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dzy.chenlongwang.top

[S50] C++：格式化数字
来源：http://msa.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yui.cashguo.top

[S51] C++：显式类型转换
来源：http://ghg.meibo888.top

static_cast<double>(a) / b
来源：http://wbz.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://smv.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://wav.iojbl.cn

[S53] C++：移动语义
来源：http://kvw.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://fpa.pycfn.com

[S54] C++：异常处理
来源：http://uxe.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://whq.xuanzx.com

[S55] C++：结构化绑定
来源：http://jve.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kgt.yfazqb.com

[S56] C++：optional
来源：http://qus.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xej.yfazqb.com

[S57] C++：编译期常量
来源：http://lis.sweek.top

constexpr int N = 10;
来源：http://nye.xziqi.cn

[S58] C++：命名空间
来源：http://jeb.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://nbf.sweek.top

[S59] C++：静态断言
来源：http://qhw.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvm.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://cmr.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://car.chenlongwang.top

================================================================================
来源：http://xpo.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xlc.vehdjk.com

================================================================================
来源：http://iiu.ybcxt.top

[T01] Kotlin：Hello World
来源：http://whf.zycfv.cn

println("Hello")
来源：http://too.cashguo.top

[T02] Kotlin：变量
来源：http://ymb.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hhf.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://eit.yj20258.top

"值: $b"
来源：http://ijk.gzhubu.top

[T04] Kotlin：空安全
来源：http://pdb.jqgfzy.top

val n: String? = null;  n?.length
来源：http://yns.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://jvp.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://let.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://mnk.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fnt.cashguo.top

[T07] Kotlin：集合过滤
来源：http://kpg.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jsi.iojbl.cn

[T08] Kotlin：数据类
来源：http://ohb.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://ynb.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://kih.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://atv.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://pji.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://flm.jiagoushi.top

[T11] Kotlin：协程
来源：http://saf.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vqh.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://ppp.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://zlq.tanke756.top

[T13] Kotlin：只读 Map
来源：http://esc.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://tqi.hywenlv.cn

[T14] Kotlin：循环
来源：http://cky.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://ckx.hcnkem.com

[T15] Kotlin：接口
来源：http://wyl.xylfe.cn

interface Shape { fun area(): Double }
来源：http://qon.nanxinkj.top

[T16] Swift：Hello World
来源：http://mtl.redwolf501.top

print("Hello")
来源：http://imz.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://mgy.hcnkem.com

var a = 1;  let b = 2
来源：http://pnd.gogol.net.cn

[T18] Swift：字符串插值
来源：http://vqr.wangshuangyany.cn

"值: \(b)"
来源：http://jzu.tianlin.xyz

[T19] Swift：可选绑定
来源：http://cww.cashguo.top

if let n = opt { print(n) }
来源：http://jim.yanxiufei.cn

[T20] Swift：数组操作
来源：http://gjs.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://ycw.zhiwuduotai.top

[T21] Swift：遍历
来源：http://kqu.zhixingplan.top

for x in a { print(x) }
来源：http://xsc.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://uea.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://tyz.hnqzz.top

[T23] Swift：函数
来源：http://tgk.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cyb.wangshuangyany.cn

[T24] Swift：闭包
来源：http://qav.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dao.xylfe.cn

[T25] Swift：结构体
来源：http://gxx.zhiwuduotai.top

struct P { var x: Int }
来源：http://awi.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://cje.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://mkl.fehbvm.com

[T27] Swift：错误处理
来源：http://kel.cucudq.cn

do { try f() } catch { print(error) }
来源：http://mgy.xinyue.icu

[T28] Swift：枚举
来源：http://dex.sxryk.cn

enum Color { case red, green }
来源：http://dfx.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://lxb.yuanzhike.top

guard let x = opt else { return }
来源：http://fwc.quarkkingdee.top

[T30] Swift：协议
来源：http://mys.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://pfx.guowangkeji.top

[T31] Lua：Hello World
来源：http://zxz.c1oappe.top

print("Hello")
来源：http://fdb.yj20258.top

[T32] Lua：局部变量
来源：http://yjl.zhaomingkeji.xyz

local a = 1
来源：http://pxb.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://bwh.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qha.hfpthk.cn

[T34] Lua：遍历表
来源：http://ddo.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qmc.jiagoushi.top

[T35] Lua：字典表
来源：http://dxv.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://knn.hfpthk.cn

[T36] Lua：函数
来源：http://nfr.haohaochexian.top

function add(a, b) return a + b end
来源：http://noz.yj202588.top

[T37] Lua：字符串拼接
来源：http://sai.tian-w.cn

"a" .. "b"
来源：http://hfm.zhiwuduotai.top

[T38] Lua：条件
来源：http://uxg.jqgufenzy.top

if x > 0 then print("正") end
来源：http://msp.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://gcy.cucudq.cn

string.find(s, "%d+")
来源：http://hkr.sufxvd.cn

[T40] Lua：元表
来源：http://pxv.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://wak.chenlongwang.top

[T41] Perl：Hello World
来源：http://ubv.yfazqb.com

print "Hello\n";
来源：http://boq.ppjwa.cn

[T42] Perl：变量类型
来源：http://xgf.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gys.smart0.xyz

[T43] Perl：字符串插值
来源：http://fvw.chenzaomai.com

"值: $a"
来源：http://nlu.yuanzhike.top

[T44] Perl：条件
来源：http://bgp.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://rti.ydzc1.top

[T45] Perl：数组遍历
来源：http://pqa.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://vjz.vehdjk.com

[T46] Perl：哈希操作
来源：http://fjg.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://drj.xinyue.icu

[T47] Perl：正则捕获
来源：http://ond.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://swn.xylfe.cn

[T48] Perl：正则替换
来源：http://rux.yangfankeji.com

$s =~ s/old/new/g;
来源：http://xka.gogol.net.cn

[T49] Perl：函数
来源：http://plz.hongshengwenyu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qiv.yuxming.cn

[T50] Perl：逐行读文件
来源：http://jtn.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://twm.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://cxg.tian-w.cn

[T51] Scala：Hello World
来源：http://tro.ydzc1.top

println("Hello")
来源：http://gds.c1oappe.top

[T52] Scala：变量
来源：http://bcc.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://jvc.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://ran.316326.xyz

s"值: $b"
来源：http://wno.cucudq.cn

[T54] Scala：集合映射
来源：http://ias.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://zwk.cashguo.top

[T55] Scala：集合过滤
来源：http://cio.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://zyf.hammf.cn

[T56] Scala：样例类
来源：http://caw.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://jrh.haohaochexian.top

[T57] Scala：模式匹配
来源：http://ngi.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ffj.jqgfzy.top

[T58] Scala：函数定义
来源：http://ocv.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fio.zhijiandao.cn

[T59] Scala：循环
来源：http://ytd.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://umh.yuanzhike.top

[T60] Scala：折叠
来源：http://hzn.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ojc.ywan-chungtsiang.top

================================================================================
来源：http://srj.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ncd.wangshuangyany.cn

================================================================================
来源：http://qcf.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://tid.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://etf.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://ddk.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bov.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://bxu.tarul.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vht.jianghu66.top

[U04] Py：变量调试打印
来源：http://ewa.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qcy.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://gvb.dashuyun.cn

list(dict.fromkeys(arr))
来源：http://dor.0kj1m.cn

[U06] Py：合并两个字典
来源：http://cww.ehwqpu.com

{**a, **b}
来源：http://bfh.xuanzx.com

[U07] Py：反转字典键值
来源：http://oyc.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://ypz.redwolf501.top

[U08] Py：展平二维列表
来源：http://lkw.hfpthk.cn

[y for x in nested for y in x]
来源：http://yvz.fengsongda.top

[U09] Py：字典取最大值的键
来源：http://gjo.yanxiufei.cn

max(d, key=d.get)
来源：http://nmi.jqgfzy.top

[U10] Py：按值排序字典
来源：http://uye.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tvp.dashuyun.cn

[U11] Py：生成器表达式
来源：http://dbl.andypj.xyz

(x * 2 for x in arr)
来源：http://cgc.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xcf.cashguo.top

Counter(arr).most_common(3)
来源：http://wgz.nanxinkj.top

[U13] Py：固定长度队列
来源：http://miz.iojbl.cn

deque(maxlen=10)
来源：http://wut.pycfn.com

[U14] Py：分组收集到列表
来源：http://vje.daxiang520.top

defaultdict(list)
来源：http://gby.zhengqikj.top

[U15] Py：高精度计时
来源：http://qyw.hongshengwenyu.top

t = time.perf_counter()
来源：http://sns.xuanzx.com

[U16] Py：命令行参数解析
来源：http://shr.chenzaomai.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ora.jqgfzy.top

[U17] Py：初始化日志
来源：http://ewu.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://abh.sufxvd.cn

[U18] Py：预编译正则
来源：http://hyw.andypj.xyz

pat = re.compile(r"\d+")
来源：http://yku.cheryme.top

[U19] Py：正则替换带回调
来源：http://mah.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kwk.zhaomingkeji.xyz

[U20] Py：缓存函数结果
来源：http://wgm.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://zvp.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://ofc.fzhhl.top

@contextlib.contextmanager
来源：http://yeq.svipenyu.cn

[U22] Py：矩阵转置
来源：http://dgr.cheryme.top

list(zip(*m))
来源：http://gog.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://jnp.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bvu.tarul.cn

[U24] Py：路径操作
来源：http://sam.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gdi.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://mcb.chenlongwang.top

csv.DictReader(f)
来源：http://dvw.fengsongda.top

[U26] Py：并发下载
来源：http://yap.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yrh.ybcxt.top

[U27] Py：异步 HTTP
来源：http://ymi.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://szx.wangshuangyany.cn

[U28] Py：类型别名
来源：http://rni.svipenyu.cn

UserId = int
来源：http://doq.zhixingplan.top

[U29] Py：属性校验
来源：http://omv.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://vbn.iojbl.cn

[U30] Py：数据类
来源：http://xzz.bjfxy.top

@dataclass(slots=True)
来源：http://tsc.52xcode.cn

[U31] Py：单测
来源：http://cyt.jianghu66.top

python -m pytest -q
来源：http://ucb.meibo888.top

[U32] Py：代码格式化
来源：http://lvx.iojbl.cn

ruff format . && ruff check --fix .
来源：http://vll.gzhubu.top

[U33] Py：打包发布
来源：http://zem.wangshuangyany.cn

python -m build  （依赖 pyproject.toml）
来源：http://vwq.mhx1999.top

[U34] Py：判断编码
来源：http://bth.zdqjudy.top

chardet.detect(raw)
来源：http://qqd.aizwys.cn

[U35] Py：发送邮件
来源：http://dum.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://thb.zhengqikj.top

[U36] Py：定时任务
来源：http://ngu.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://tcb.gzhubu.top


<!-- 参考信息 -->