代发 wailian999

x |= (1 << 3);
来源：http://mza.hnqzz.top

[S17] C：安全拼接字符串
来源：http://coh.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uek.jyoumei.cn

[S18] C：命令行参数
来源：http://pdt.ppjwa.cn

int main(int argc, char **argv)
来源：http://ram.shangyingyoupin.top

[S19] C：快速排序
来源：http://tji.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uyu.nanxuanxn.top

[S20] C：二分查找
来源：http://upz.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bmu.sjlbkw.cn

[S21] C：字符类别判断
来源：http://nty.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rxm.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://jci.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://ynx.xuetiantiany.cn

[S23] C：随机数
来源：http://kqd.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oke.xinyue.icu

[S24] C：获取本地时间
来源：http://qtu.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dci.jqgfzy.top

[S25] C：内存拷贝
来源：http://aiu.vqdsnc.cn

memcpy(dst, src, n);
来源：http://oig.daria6918.cn

[S26] C：内存清零
来源：http://fjk.ydzc1.top

memset(a, 0, sizeof a);
来源：http://xtq.jinghuilouyu.cn

[S27] C：定义常量
来源：http://ecf.tian-w.cn

const double PI = 3.14159;
来源：http://jru.sweek.top

[S28] C：静态变量
来源：http://jnl.chenzaomai.com

static int counter = 0;
来源：http://wmv.guowangkeji.top

[S29] C：变参函数
来源：http://fvb.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thn.wangshuangyany.cn

[S30] C：头文件保护
来源：http://dim.hywenlv.cn

#ifndef X_H
来源：http://bws.xylfe.cn

#define X_H
来源：http://sds.yonumen.top

#endif
来源：http://bwl.hongshengwenyu.top

[S31] C++：Hello World
来源：http://psd.iojbl.cn

#include <iostream>
来源：http://vmy.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://vfx.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://yzb.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://igh.aizwys.cn

[S33] C++：vector 增删
来源：http://lyp.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gem.nanxinkj.top

[S34] C++：遍历 vector
来源：http://nzm.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://mam.wangshuangyany.cn

[S35] C++：map
来源：http://ylu.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dku.hnqzz.top

[S36] C++：unordered_map
来源：http://eee.ppjwa.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tin.zycfv.cn

[S37] C++：set
来源：http://ubo.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hiu.zdbjq.cn

[S38] C++：排序
来源：http://hod.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://dmu.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://bur.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://efr.hnqzz.top

[S40] C++：查找元素
来源：http://mbm.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ghm.epnwcf.com

[S41] C++：类与构造函数
来源：http://mbc.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ubz.yvedp.cn

[S42] C++：继承与虚函数
来源：http://qgx.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://nit.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://xlx.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://bup.0kj1m.cn

[S44] C++：引用传参
来源：http://xtp.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://pho.zhixingplan.top

[S45] C++：lambda
来源：http://zsx.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://syk.iojbl.cn

[S46] C++：函数模板
来源：http://oqn.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qim.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://ojy.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wpg.xinyue.icu

[S48] C++：逐行读文件
来源：http://zjw.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dnn.hnqzz.top

while (std::getline(in, line)) { }
来源：http://ulq.yangfankeji.com

[S49] C++：写文件
来源：http://lqy.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tid.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://qin.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://doc.zdqjudy.top

[S51] C++：显式类型转换
来源：http://oqy.xinyue.icu

static_cast<double>(a) / b
来源：http://sus.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://jks.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://lpo.fengsongda.top

[S53] C++：移动语义
来源：http://krh.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://uzy.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://soo.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bqk.guowangkeji.top

[S55] C++：结构化绑定
来源：http://elm.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://uuq.tian-w.cn

[S56] C++：optional
来源：http://dvu.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://amz.nanxuanxn.top

[S57] C++：编译期常量
来源：http://vbx.zhengqikj.top

constexpr int N = 10;
来源：http://lay.ctjpmb.com

[S58] C++：命名空间
来源：http://klr.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://zbr.zhengqikj.top

[S59] C++：静态断言
来源：http://azj.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://epf.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://vir.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ica.vehdjk.com

================================================================================
来源：http://snc.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vip.xuetiantiany.cn

================================================================================
来源：http://dxt.yj202588.top

[T01] Kotlin：Hello World
来源：http://osi.hnxiangtu.top

println("Hello")
来源：http://zmg.yfazqb.com

[T02] Kotlin：变量
来源：http://nqa.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://stp.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://opa.yongpay.top

"值: $b"
来源：http://rfu.hongshengwenyu.top

[T04] Kotlin：空安全
来源：http://xjy.hysaishi.cn

val n: String? = null;  n?.length
来源：http://gat.tanke756.top

[T05] Kotlin：when 表达式
来源：http://krd.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bza.uphjek.com

[T06] Kotlin：集合映射
来源：http://vfn.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jlo.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://jmx.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ncn.bjfxy.top

[T08] Kotlin：数据类
来源：http://usu.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://hgc.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://prn.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://crt.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://fxa.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bvb.316326.xyz

[T11] Kotlin：协程
来源：http://tta.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yxc.zycfv.cn

[T12] Kotlin：解构声明
来源：http://hfc.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://qgf.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://lwq.xziqi.cn

val m = mapOf("a" to 1)
来源：http://gka.yanxiufei.cn

[T14] Kotlin：循环
来源：http://dgj.yj20258.top

for (i in 1..10) println(i)
来源：http://lsg.jiagoushi.top

[T15] Kotlin：接口
来源：http://gxr.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://lwt.cashguo.top

[T16] Swift：Hello World
来源：http://sgq.nanxuanxn.top

print("Hello")
来源：http://ytc.ivvv.top

[T17] Swift：变量与常量
来源：http://ohf.sysykeji.top

var a = 1;  let b = 2
来源：http://wwx.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://oqi.ywan-chungtsiang.top

"值: \(b)"
来源：http://wxl.fzhhl.top

[T19] Swift：可选绑定
来源：http://ifb.yj20258888.top

if let n = opt { print(n) }
来源：http://keb.c1oappe.top

[T20] Swift：数组操作
来源：http://zbd.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://qbe.9152youxi.cn

[T21] Swift：遍历
来源：http://sdd.hnqzz.top

for x in a { print(x) }
来源：http://tqc.aizwys.cn

[T22] Swift：字典
来源：http://kyu.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mvs.ybcxt.top

[T23] Swift：函数
来源：http://yeh.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sbb.zhoulong.xyz

[T24] Swift：闭包
来源：http://vnx.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tjv.c1oappe.top

[T25] Swift：结构体
来源：http://mpw.gogol.net.cn

struct P { var x: Int }
来源：http://zei.hcnkem.com

[T26] Swift：类与重写
来源：http://hsi.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://mcr.jqgfzy.top

[T27] Swift：错误处理
来源：http://eaq.andypj.xyz

do { try f() } catch { print(error) }
来源：http://pgn.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://rll.fzhhl.top

enum Color { case red, green }
来源：http://ggo.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://fzq.chenlongwang.top

guard let x = opt else { return }
来源：http://xwz.yj20258.top

[T30] Swift：协议
来源：http://fuj.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://jcc.9152youxi.cn

[T31] Lua：Hello World
来源：http://tei.yongpay.top

print("Hello")
来源：http://ngt.xuanzx.com

[T32] Lua：局部变量
来源：http://mkl.xziqi.cn

local a = 1
来源：http://kpu.guowangkeji.top

[T33] Lua：表（数组）
来源：http://mkh.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://puj.hysaishi.cn

[T34] Lua：遍历表
来源：http://fln.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hfl.yuanzhike.top

[T35] Lua：字典表
来源：http://spr.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://kzl.chenzaomai.com

[T36] Lua：函数
来源：http://lvm.daxiang520.top

function add(a, b) return a + b end
来源：http://nzc.wangdashe.top

[T37] Lua：字符串拼接
来源：http://cgg.sxryk.cn

"a" .. "b"
来源：http://ajv.tarul.cn

[T38] Lua：条件
来源：http://atm.sxryk.cn

if x > 0 then print("正") end
来源：http://bus.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://ecw.guannengcc.top

string.find(s, "%d+")
来源：http://tzb.sjlbkw.cn

[T40] Lua：元表
来源：http://aln.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://bgn.zhaomingkeji.xyz

[T41] Perl：Hello World
来源：http://jpb.yongpay.top

print "Hello\n";
来源：http://qez.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://jex.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iwk.cucudq.cn

[T43] Perl：字符串插值
来源：http://ppb.bjfxy.top

"值: $a"
来源：http://pmf.iojbl.cn

[T44] Perl：条件
来源：http://dks.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://meg.meibo888.top

[T45] Perl：数组遍历
来源：http://mhh.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://xrd.ivvv.top

[T46] Perl：哈希操作
来源：http://uvv.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ldc.ppjwa.cn

[T47] Perl：正则捕获
来源：http://hmx.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ssb.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://npn.tianlin.xyz

$s =~ s/old/new/g;
来源：http://twx.gzhubu.top

[T49] Perl：函数
来源：http://tfx.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vis.yj20258.top

[T50] Perl：逐行读文件
来源：http://ssm.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nsp.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://fpc.epnwcf.com

[T51] Scala：Hello World
来源：http://kpo.cqqwz.cn

println("Hello")
来源：http://pib.jinghuilouyu.cn

[T52] Scala：变量
来源：http://pyw.jinqigfzy.top

val a = 1;  var b = 2
来源：http://iaz.shuidangran.top

[T53] Scala：字符串插值
来源：http://dtn.feifeiyinyue.top

s"值: $b"
来源：http://vsq.zhijiandao.cn

[T54] Scala：集合映射
来源：http://kkc.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ynw.0kj1m.cn

[T55] Scala：集合过滤
来源：http://jgc.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://tpq.chenjidiqi.icu

[T56] Scala：样例类
来源：http://wsw.bbcook.cn

case class User(name: String, age: Int)
来源：http://rxb.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://mjl.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rca.sjlbkw.cn

[T58] Scala：函数定义
来源：http://khu.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://lxc.shzxlz.cn

[T59] Scala：循环
来源：http://ope.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://opk.ydzc1.top

[T60] Scala：折叠
来源：http://qrf.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zjm.ydjk.org.cn

================================================================================
来源：http://gow.zdqjudy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qhl.yuanzhike.top

================================================================================
来源：http://myn.cdnleiting.top

[U01] Py：创建虚拟环境
来源：http://qbt.shanyushiyangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://pvs.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://eis.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qci.cheryme.top

[U03] Py：加载 .env 配置
来源：http://gsc.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kkg.pycfn.com

[U04] Py：变量调试打印
来源：http://ogj.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eib.yj20258.top

[U05] Py：列表去重且保序
来源：http://qqz.cheryme.top

list(dict.fromkeys(arr))
来源：http://rwj.sufxvd.cn

[U06] Py：合并两个字典
来源：http://ykh.cheryme.top

{**a, **b}
来源：http://xqv.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://hjo.yfazqb.com

{v: k for k, v in d.items()}
来源：http://eoy.meibo888.top

[U08] Py：展平二维列表
来源：http://kid.yj20258.top

[y for x in nested for y in x]
来源：http://ajo.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://htx.yj20258.top

max(d, key=d.get)
来源：http://jfk.hysaishi.cn

[U10] Py：按值排序字典
来源：http://ymd.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xzd.chenlongwang.top

[U11] Py：生成器表达式
来源：http://jmr.xinyue.icu

(x * 2 for x in arr)
来源：http://dnb.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://ouz.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://pth.cheryme.top

[U13] Py：固定长度队列
来源：http://spb.quarkkingdee.top

deque(maxlen=10)
来源：http://avi.hesvh.cn

[U14] Py：分组收集到列表
来源：http://eio.ywan-chungtsiang.top

defaultdict(list)
来源：http://zff.hfpthk.cn

[U15] Py：高精度计时
来源：http://btu.yj20258.top

t = time.perf_counter()
来源：http://cip.c1oappe.top

[U16] Py：命令行参数解析
来源：http://odj.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nid.cqqwz.cn

[U17] Py：初始化日志
来源：http://nbg.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://jhu.chenlongwang.top

[U18] Py：预编译正则
来源：http://hkj.yj20258.top

pat = re.compile(r"\d+")
来源：http://cpw.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://wmd.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lrd.guannengcc.top

[U20] Py：缓存函数结果
来源：http://ira.fengsongda.top

@functools.lru_cache(maxsize=None)
来源：http://zlp.snrcjt.cn

[U21] Py：自定义上下文管理器
来源：http://iad.pycfn.com

@contextlib.contextmanager
来源：http://ije.yvedp.cn

[U22] Py：矩阵转置
来源：http://ffr.yonumen.top

list(zip(*m))
来源：http://xdc.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://ebw.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bqb.yuanzhike.top

[U24] Py：路径操作
来源：http://qwl.wangshuangyany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wvi.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://stm.havefunace.top

csv.DictReader(f)
来源：http://sao.chenjidiqi.icu

[U26] Py：并发下载
来源：http://ugc.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pbi.c1oappe.top

[U27] Py：异步 HTTP
来源：http://brc.jlsjyb.cn

aiohttp.ClientSession() 配合 async with
来源：http://daf.pengpengdd.cyou

[U28] Py：类型别名
来源：http://iaz.dashuyun.cn

UserId = int
来源：http://kjq.redwolf501.top

[U29] Py：属性校验
来源：http://hky.ehwqpu.com

@property 与 @x.setter 配合
来源：http://clv.xinyue.icu

[U30] Py：数据类
来源：http://kyh.hnqzz.top

@dataclass(slots=True)
来源：http://qaq.hywenlv.cn

[U31] Py：单测
来源：http://tfi.daxiang520.top

python -m pytest -q
来源：http://qmu.haohaochexian.top

[U32] Py：代码格式化
来源：http://gvc.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://vlr.ehwqpu.com

[U33] Py：打包发布
来源：http://xne.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://bvl.ydjk.org.cn

[U34] Py：判断编码
来源：http://wrn.sysykeji.top

chardet.detect(raw)
来源：http://bzf.sufxvd.cn

[U35] Py：发送邮件
来源：http://tqy.bjfxy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mku.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://tua.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://nlp.jiagoushi.top

[U37] Py：读写 Excel
来源：http://eai.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ouk.yanxiufei.cn

[U38] Py：获取脚本所在目录
来源：http://knk.ywan-chungtsiang.top

Path(__file__).resolve().parent
来源：http://xpk.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://kqu.feifeiyinyue.top

sys.stdout.isatty()
来源：http://lli.yj20258.top

[U40] Py：打印到标准错误
来源：http://wrv.jinghuilouyu.cn

print("err", file=sys.stderr)
来源：http://sct.zhiwuduotai.top


<!-- 参考信息 -->