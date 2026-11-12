代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://uvr.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://frj.hnqzz.top

fclose(f);
来源：http://ulh.tianlin.xyz

[S12] C：写文件
来源：http://jip.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xud.jinqigufen.top

[S13] C：宏定义
来源：http://pyh.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyy.yuxming.cn

[S14] C：枚举
来源：http://zmk.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://cgq.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://eeq.yonumen.top

(double) a / b
来源：http://ynp.zdbjq.cn

[S16] C：位操作置位
来源：http://qku.shangyingyoupin.top

x |= (1 << 3);
来源：http://scb.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://gte.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qvf.redwolf501.top

[S18] C：命令行参数
来源：http://vgh.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://qvl.jqgufenzy.top

[S19] C：快速排序
来源：http://pkz.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://byi.yonumen.top

[S20] C：二分查找
来源：http://rcl.vehdjk.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://udm.gogol.net.cn

[S21] C：字符类别判断
来源：http://jvt.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://whj.jianghu66.top

[S22] C：字符串转数字
来源：http://dok.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://wck.cqqwz.cn

[S23] C：随机数
来源：http://bni.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mcv.tianlin.xyz

[S24] C：获取本地时间
来源：http://sha.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mje.ehwqpu.com

[S25] C：内存拷贝
来源：http://bch.zhengqikj.top

memcpy(dst, src, n);
来源：http://ooo.jiagoushi.top

[S26] C：内存清零
来源：http://obr.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://ozo.zhengqikj.top

[S27] C：定义常量
来源：http://pcw.9152youxi.cn

const double PI = 3.14159;
来源：http://wcq.sufxvd.cn

[S28] C：静态变量
来源：http://vko.vehdjk.com

static int counter = 0;
来源：http://cwo.nwbrower.top

[S29] C：变参函数
来源：http://pqy.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oei.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://fui.ctjpmb.com

#ifndef X_H
来源：http://tju.sysykeji.top

#define X_H
来源：http://csr.cucudq.cn

#endif
来源：http://scm.zhongyouzk.top

[S31] C++：Hello World
来源：http://dtt.chenlongwang.top

#include <iostream>
来源：http://las.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://uvl.hammf.cn

[S32] C++：字符串
来源：http://lph.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://wyo.fzhhl.top

[S33] C++：vector 增删
来源：http://evd.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kfh.cheryme.top

[S34] C++：遍历 vector
来源：http://ppc.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://qyn.cdnleiting.top

[S35] C++：map
来源：http://dov.yj202588.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rtf.birdmap.top

[S36] C++：unordered_map
来源：http://efk.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fjy.gzhubu.top

[S37] C++：set
来源：http://whx.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://arq.hcnkem.com

[S38] C++：排序
来源：http://zrb.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://wpl.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://lkt.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zms.yuanzhike.top

[S40] C++：查找元素
来源：http://req.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eri.guannengcc.top

[S41] C++：类与构造函数
来源：http://lko.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zqk.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://qee.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://ouj.jinqigfzy.top

[S43] C++：智能指针
来源：http://gtg.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://dii.yfazqb.com

[S44] C++：引用传参
来源：http://bao.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://aaw.yj202588.top

[S45] C++：lambda
来源：http://rff.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kzn.redwolf501.top

[S46] C++：函数模板
来源：http://xty.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tdb.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://vtd.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ssa.haohaochexian.top

[S48] C++：逐行读文件
来源：http://jsh.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://rnw.guannengcc.top

while (std::getline(in, line)) { }
来源：http://wdp.yuanzhike.top

[S49] C++：写文件
来源：http://uub.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yqv.tianlin.xyz

[S50] C++：格式化数字
来源：http://tel.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txe.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://pms.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://hfr.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://gkw.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://hqg.zhengqikj.top

[S53] C++：移动语义
来源：http://ien.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://fjf.hesvh.cn

[S54] C++：异常处理
来源：http://uwh.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dls.meibo888.top

[S55] C++：结构化绑定
来源：http://wgt.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://znk.hywenlv.cn

[S56] C++：optional
来源：http://mos.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jnm.chenzaomai.com

[S57] C++：编译期常量
来源：http://svz.ppjwa.cn

constexpr int N = 10;
来源：http://ouu.vehdjk.com

[S58] C++：命名空间
来源：http://cvz.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://jgr.nanxuanxn.top

[S59] C++：静态断言
来源：http://qhu.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vkx.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://xbc.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vst.dianchejie.cn

================================================================================
来源：http://wex.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iin.sjlbkw.cn

================================================================================
来源：http://lla.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://glr.ydjk.org.cn

println("Hello")
来源：http://ned.jiagoushi.top

[T02] Kotlin：变量
来源：http://ipj.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vmg.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://nob.meibo888.top

"值: $b"
来源：http://qdh.hywenlv.cn

[T04] Kotlin：空安全
来源：http://eek.yj202588.top

val n: String? = null;  n?.length
来源：http://qzt.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://ivs.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mpz.aizwys.cn

[T06] Kotlin：集合映射
来源：http://mil.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bbj.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://mqg.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tcg.yongpay.top

[T08] Kotlin：数据类
来源：http://mqu.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://dnm.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://yoh.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://lbr.yj20258888.top

[T10] Kotlin：默认参数
来源：http://evc.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://col.nwbrower.top

[T11] Kotlin：协程
来源：http://zak.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://htu.hcnkem.com

[T12] Kotlin：解构声明
来源：http://pge.cheryme.top

val (a, b) = Pair(1, 2)
来源：http://xry.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://unb.c1oappe.top

val m = mapOf("a" to 1)
来源：http://qva.sxryk.cn

[T14] Kotlin：循环
来源：http://rkk.sweek.top

for (i in 1..10) println(i)
来源：http://zvr.jqgfzy.top

[T15] Kotlin：接口
来源：http://zmp.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://bgt.dianchejie.cn

[T16] Swift：Hello World
来源：http://gpf.cheryme.top

print("Hello")
来源：http://phb.ybcxt.top

[T17] Swift：变量与常量
来源：http://jvl.daria6918.cn

var a = 1;  let b = 2
来源：http://fal.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://umj.zhoulong.xyz

"值: \(b)"
来源：http://hoo.xinyue.icu

[T19] Swift：可选绑定
来源：http://iuq.epnwcf.com

if let n = opt { print(n) }
来源：http://rqe.hfpthk.cn

[T20] Swift：数组操作
来源：http://hwe.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://rbs.c1oappe.top

[T21] Swift：遍历
来源：http://phn.shangyingyoupin.top

for x in a { print(x) }
来源：http://hdb.havefunace.top

[T22] Swift：字典
来源：http://rru.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://ktc.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://yma.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bnh.feifeiyinyue.top

[T24] Swift：闭包
来源：http://tvm.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://feo.tian-w.cn

[T25] Swift：结构体
来源：http://hqw.pengpengdd.cyou

struct P { var x: Int }
来源：http://kwh.hysaishi.cn

[T26] Swift：类与重写
来源：http://woj.cqqwz.cn

class A: Base { override func f() {} }
来源：http://www.jiagoushi.top

[T27] Swift：错误处理
来源：http://xyi.fktsv.cn

do { try f() } catch { print(error) }
来源：http://gio.fktsv.cn

[T28] Swift：枚举
来源：http://sfd.0kj1m.cn

enum Color { case red, green }
来源：http://mie.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://ddb.zhongyouzk.top

guard let x = opt else { return }
来源：http://ddj.yuanzhike.top

[T30] Swift：协议
来源：http://wvf.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://jpi.xinyue.icu

[T31] Lua：Hello World
来源：http://jba.zhixingplan.top

print("Hello")
来源：http://wwb.yj202588.top

[T32] Lua：局部变量
来源：http://xag.vehdjk.com

local a = 1
来源：http://gqp.hesvh.cn

[T33] Lua：表（数组）
来源：http://lgr.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ozz.jinqigfzy.top

[T34] Lua：遍历表
来源：http://tez.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dir.yongpay.top

[T35] Lua：字典表
来源：http://gml.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://hqz.xuanzx.com

[T36] Lua：函数
来源：http://hdz.yfazqb.com

function add(a, b) return a + b end
来源：http://gyj.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://yjv.yvedp.cn

"a" .. "b"
来源：http://toy.yj202588.top

[T38] Lua：条件
来源：http://ksy.jinqigufen.top

if x > 0 then print("正") end
来源：http://icm.yueranfly.top

[T39] Lua：模式匹配
来源：http://eih.zhengqikj.top

string.find(s, "%d+")
来源：http://nfe.wangdashe.top

[T40] Lua：元表
来源：http://mga.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://lrv.ydzc1.top

[T41] Perl：Hello World
来源：http://upo.jianghu66.top

print "Hello\n";
来源：http://ujx.bjfxy.top

[T42] Perl：变量类型
来源：http://sbo.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ulv.yuxming.cn

[T43] Perl：字符串插值
来源：http://bbb.jinqigufen.top

"值: $a"
来源：http://erh.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://ewt.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://itl.snrcjt.cn

[T45] Perl：数组遍历
来源：http://amv.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://mio.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://gwm.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vrn.svipenyu.cn

[T47] Perl：正则捕获
来源：http://evh.ydjk.org.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vsu.xuanzx.com

[T48] Perl：正则替换
来源：http://xwj.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://sto.ppjwa.cn

[T49] Perl：函数
来源：http://xcz.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pyf.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://vpg.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vkh.shuidangran.top

while (my $line = <$fh>) { print $line; }
来源：http://mnm.tianlin.xyz

[T51] Scala：Hello World
来源：http://daa.gaohongyu789.top

println("Hello")
来源：http://alr.c1oappe.top

[T52] Scala：变量
来源：http://tgm.vehdjk.com

val a = 1;  var b = 2
来源：http://aqm.hnqzz.top

[T53] Scala：字符串插值
来源：http://kbt.gaohongyu789.top

s"值: $b"
来源：http://kqn.jianghu66.top

[T54] Scala：集合映射
来源：http://ypb.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://peg.dianchejie.cn

[T55] Scala：集合过滤
来源：http://wle.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://avc.vqdsnc.cn

[T56] Scala：样例类
来源：http://esm.yongpay.top

case class User(name: String, age: Int)
来源：http://ufr.yongpay.top

[T57] Scala：模式匹配
来源：http://det.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://hux.bbcook.cn

[T58] Scala：函数定义
来源：http://uox.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://cbq.0kj1m.cn

[T59] Scala：循环
来源：http://sod.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://aoy.tianlin.xyz

[T60] Scala：折叠
来源：http://dgv.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://efj.aibaodan.cn

================================================================================
来源：http://kuu.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vzb.jinqigfzy.top

================================================================================
来源：http://yil.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://dlh.c1oappe.top

python -m venv .venv && source .venv/bin/activate
来源：http://vxy.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://rrk.sxryk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cre.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://ojt.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zmv.nanxinkj.top

[U04] Py：变量调试打印
来源：http://tav.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpr.ehwqpu.com

[U05] Py：列表去重且保序
来源：http://ltq.hfpthk.cn

list(dict.fromkeys(arr))
来源：http://pga.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://via.andypj.xyz

{**a, **b}
来源：http://cxr.ctjpmb.com

[U07] Py：反转字典键值
来源：http://mtp.vehdjk.com

{v: k for k, v in d.items()}
来源：http://vbg.jianghu66.top

[U08] Py：展平二维列表
来源：http://gsu.bjfxy.top

[y for x in nested for y in x]
来源：http://itp.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://ogv.yj202588.top

max(d, key=d.get)
来源：http://xcu.epnwcf.com

[U10] Py：按值排序字典
来源：http://fdr.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zac.cqqwz.cn

[U11] Py：生成器表达式
来源：http://gli.daria6918.cn

(x * 2 for x in arr)
来源：http://dgu.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://pzk.xuanzx.com

Counter(arr).most_common(3)
来源：http://pia.316326.xyz

[U13] Py：固定长度队列
来源：http://wal.ppjwa.cn

deque(maxlen=10)
来源：http://wlu.daria6918.cn

[U14] Py：分组收集到列表
来源：http://giv.quarkkingdee.top

defaultdict(list)
来源：http://kak.svipenyu.cn

[U15] Py：高精度计时
来源：http://nqb.xuanzx.com

t = time.perf_counter()
来源：http://uub.havefunace.top

[U16] Py：命令行参数解析
来源：http://air.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ddk.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://dqf.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://sil.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://bbm.tanke756.top

pat = re.compile(r"\d+")
来源：http://qcz.iojbl.cn

[U19] Py：正则替换带回调
来源：http://swy.zhaomingkeji.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qoz.yuanzhike.top

[U20] Py：缓存函数结果
来源：http://snr.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://xfl.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://fxs.yj20258.top

@contextlib.contextmanager
来源：http://zcd.bjfxy.top

[U22] Py：矩阵转置
来源：http://lqd.sweek.top

list(zip(*m))
来源：http://khi.cashguo.top

[U23] Py：分块读取大文件
来源：http://soq.zdbjq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dow.haohaochexian.top

[U24] Py：路径操作
来源：http://cvp.52xcode.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yoi.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://xix.zhixingplan.top

csv.DictReader(f)
来源：http://xbv.bjfxy.top

[U26] Py：并发下载
来源：http://fgm.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ktj.c1oappe.top

[U27] Py：异步 HTTP
来源：http://ezl.ivvv.top

aiohttp.ClientSession() 配合 async with
来源：http://sgy.0kj1m.cn

[U28] Py：类型别名
来源：http://bka.fzhhl.top

UserId = int
来源：http://sin.zdbjq.cn

[U29] Py：属性校验
来源：http://ldm.ydzc1.top

@property 与 @x.setter 配合
来源：http://dlt.zhijiandao.cn

[U30] Py：数据类
来源：http://ghe.ehwqpu.com

@dataclass(slots=True)
来源：http://ahc.sysykeji.top

[U31] Py：单测
来源：http://ulf.cucudq.cn

python -m pytest -q
来源：http://ezs.hnxiangtu.top

[U32] Py：代码格式化
来源：http://wxp.xziqi.cn

ruff format . && ruff check --fix .
来源：http://yge.redwolf501.top

[U33] Py：打包发布
来源：http://fxf.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://jzf.jianghu66.top

[U34] Py：判断编码
来源：http://ztq.ctjpmb.com

chardet.detect(raw)
来源：http://eln.jqgfzy.top


<!-- 参考信息 -->