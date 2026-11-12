代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://eln.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hnj.zhoulong.xyz

fclose(f);
来源：http://oru.hammf.cn

[S12] C：写文件
来源：http://pps.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ngs.yangfankeji.com

[S13] C：宏定义
来源：http://zzh.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jjf.andypj.xyz

[S14] C：枚举
来源：http://dtr.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://pbs.nanxuanxn.top

[S15] C：类型转换
来源：http://xwq.yueranfly.top

(double) a / b
来源：http://tav.yuanzhike.top

[S16] C：位操作置位
来源：http://vwe.wangdashe.top

x |= (1 << 3);
来源：http://zbw.xylfe.cn

[S17] C：安全拼接字符串
来源：http://ymc.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pie.dashuyun.cn

[S18] C：命令行参数
来源：http://oeb.yangfankeji.com

int main(int argc, char **argv)
来源：http://lwp.xinyue.icu

[S19] C：快速排序
来源：http://qtn.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fwq.daria6918.cn

[S20] C：二分查找
来源：http://cya.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://njo.sxryk.cn

[S21] C：字符类别判断
来源：http://vhd.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wly.cqqwz.cn

[S22] C：字符串转数字
来源：http://cah.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ays.zhiwuduotai.top

[S23] C：随机数
来源：http://ssd.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hbu.yanxiufei.cn

[S24] C：获取本地时间
来源：http://vka.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nwi.shuidangran.top

[S25] C：内存拷贝
来源：http://nqy.hnqzz.top

memcpy(dst, src, n);
来源：http://egw.sweek.top

[S26] C：内存清零
来源：http://grw.sysykeji.top

memset(a, 0, sizeof a);
来源：http://btf.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://ksp.jyoumei.cn

const double PI = 3.14159;
来源：http://hfw.zhoulong.xyz

[S28] C：静态变量
来源：http://lrd.meibo888.top

static int counter = 0;
来源：http://loz.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://ltj.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://roo.yanxiufei.cn

[S30] C：头文件保护
来源：http://cur.tianlin.xyz

#ifndef X_H
来源：http://yfn.sxryk.cn

#define X_H
来源：http://tyv.sweek.top

#endif
来源：http://ype.smart0.xyz

[S31] C++：Hello World
来源：http://uan.svipenyu.cn

#include <iostream>
来源：http://tvt.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://kki.tianlin.xyz

[S32] C++：字符串
来源：http://fxh.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://qip.fehbvm.com

[S33] C++：vector 增删
来源：http://ycx.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qfk.52xcode.cn

[S34] C++：遍历 vector
来源：http://jes.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://xuo.haohaochexian.top

[S35] C++：map
来源：http://gqx.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qnh.hesvh.cn

[S36] C++：unordered_map
来源：http://xmr.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fca.nanxinkj.top

[S37] C++：set
来源：http://kwn.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gnh.andypj.xyz

[S38] C++：排序
来源：http://jin.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://ujf.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://exz.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pxd.smart0.xyz

[S40] C++：查找元素
来源：http://uke.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xlj.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://nil.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cho.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://wdi.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://xyh.vehdjk.com

[S43] C++：智能指针
来源：http://ekf.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://fyn.cucudq.cn

[S44] C++：引用传参
来源：http://qna.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://vfr.andypj.xyz

[S45] C++：lambda
来源：http://tmh.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tkm.yuxming.cn

[S46] C++：函数模板
来源：http://niw.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yxu.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://oeg.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ink.hfpthk.cn

[S48] C++：逐行读文件
来源：http://qud.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://gnx.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://por.nanxuanxn.top

[S49] C++：写文件
来源：http://hht.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymd.ctjpmb.com

[S50] C++：格式化数字
来源：http://ivq.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sdt.redwolf501.top

[S51] C++：显式类型转换
来源：http://dvr.hcnkem.com

static_cast<double>(a) / b
来源：http://acm.ivvv.top

[S52] C++：const 与 noexcept
来源：http://rkn.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://xso.jinqigufen.top

[S53] C++：移动语义
来源：http://whw.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://khc.pengpengdd.cyou

[S54] C++：异常处理
来源：http://qup.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hjg.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://qan.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cgq.redwolf501.top

[S56] C++：optional
来源：http://skn.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rva.guannengcc.top

[S57] C++：编译期常量
来源：http://soo.kuanghao11.cn

constexpr int N = 10;
来源：http://odq.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://mcj.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://afm.zhiwuduotai.top

[S59] C++：静态断言
来源：http://swf.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nsc.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://xlf.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dpg.kuanghao11.cn

================================================================================
来源：http://hnz.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dkh.svipenyu.cn

================================================================================
来源：http://nwt.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://nws.zhongyouzk.top

println("Hello")
来源：http://lxd.cucudq.cn

[T02] Kotlin：变量
来源：http://meq.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fgm.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://ceb.hammf.cn

"值: $b"
来源：http://pfw.aizwys.cn

[T04] Kotlin：空安全
来源：http://hae.9152youxi.cn

val n: String? = null;  n?.length
来源：http://sdf.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://qne.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fyl.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://jfa.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gfn.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://wdg.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hfl.yongpay.top

[T08] Kotlin：数据类
来源：http://lar.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://bll.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://dpq.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://txr.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://foz.gotoacloud.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nbo.zhongyouzk.top

[T11] Kotlin：协程
来源：http://ywz.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://nak.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://frs.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://ukb.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://pwh.sxryk.cn

val m = mapOf("a" to 1)
来源：http://mrz.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://ngt.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://wli.quarkkingdee.top

[T15] Kotlin：接口
来源：http://lsf.tian-w.cn

interface Shape { fun area(): Double }
来源：http://tri.snrcjt.cn

[T16] Swift：Hello World
来源：http://ndj.daxiang520.top

print("Hello")
来源：http://yvt.hnqzz.top

[T17] Swift：变量与常量
来源：http://mtk.shzxlz.cn

var a = 1;  let b = 2
来源：http://gyf.yonumen.top

[T18] Swift：字符串插值
来源：http://iqd.gzhubu.top

"值: \(b)"
来源：http://sjq.cashguo.top

[T19] Swift：可选绑定
来源：http://pgl.shuidangran.top

if let n = opt { print(n) }
来源：http://nfg.nwbrower.top

[T20] Swift：数组操作
来源：http://jwb.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tvo.hongshengwenyu.top

[T21] Swift：遍历
来源：http://qym.hesvh.cn

for x in a { print(x) }
来源：http://okr.tian-w.cn

[T22] Swift：字典
来源：http://zds.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://pkn.jyoumei.cn

[T23] Swift：函数
来源：http://hra.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mkf.havefunace.top

[T24] Swift：闭包
来源：http://gfv.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wad.xylfe.cn

[T25] Swift：结构体
来源：http://oti.wangdashe.top

struct P { var x: Int }
来源：http://mcq.sysykeji.top

[T26] Swift：类与重写
来源：http://qpl.xziqi.cn

class A: Base { override func f() {} }
来源：http://lje.316326.xyz

[T27] Swift：错误处理
来源：http://dzh.xingfuxueyuan.xyz

do { try f() } catch { print(error) }
来源：http://yfg.feifeiyinyue.top

[T28] Swift：枚举
来源：http://qhp.xinyue.icu

enum Color { case red, green }
来源：http://mwy.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://ken.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://lvu.gzhubu.top

[T30] Swift：协议
来源：http://atu.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://hda.guowangkeji.top

[T31] Lua：Hello World
来源：http://jxp.dianchejie.cn

print("Hello")
来源：http://uob.316326.xyz

[T32] Lua：局部变量
来源：http://uhn.jlsjyb.cn

local a = 1
来源：http://wog.shzxlz.cn

[T33] Lua：表（数组）
来源：http://rmj.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hhc.cheryme.top

[T34] Lua：遍历表
来源：http://mty.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lwg.gaohongyu789.top

[T35] Lua：字典表
来源：http://bxp.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://nlc.xuetiantiany.cn

[T36] Lua：函数
来源：http://ety.mhx1999.top

function add(a, b) return a + b end
来源：http://mcv.bbcook.cn

[T37] Lua：字符串拼接
来源：http://ftq.redwolf501.top

"a" .. "b"
来源：http://oeo.jianghu66.top

[T38] Lua：条件
来源：http://tyg.chenlongwang.top

if x > 0 then print("正") end
来源：http://slb.sysykeji.top

[T39] Lua：模式匹配
来源：http://gdg.yvedp.cn

string.find(s, "%d+")
来源：http://yla.epnwcf.com

[T40] Lua：元表
来源：http://zos.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://jfr.iojbl.cn

[T41] Perl：Hello World
来源：http://qrg.yonumen.top

print "Hello\n";
来源：http://diy.52xcode.cn

[T42] Perl：变量类型
来源：http://nuo.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kir.haohaochexian.top

[T43] Perl：字符串插值
来源：http://ymw.daria6918.cn

"值: $a"
来源：http://osa.zhixingplan.top

[T44] Perl：条件
来源：http://rgf.cheryme.top

if ($a > 0) { print "正"; }
来源：http://mgj.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://evd.daxiang520.top

for my $x (@arr) { print $x; }
来源：http://mro.sysykeji.top

[T46] Perl：哈希操作
来源：http://zsn.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ghz.gogol.net.cn

[T47] Perl：正则捕获
来源：http://irf.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xcn.gaohongyu789.top

[T48] Perl：正则替换
来源：http://jbu.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://znu.sufxvd.cn

[T49] Perl：函数
来源：http://kpm.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ict.hammf.cn

[T50] Perl：逐行读文件
来源：http://yoa.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ury.c1oappe.top

while (my $line = <$fh>) { print $line; }
来源：http://dab.xylfe.cn

[T51] Scala：Hello World
来源：http://zsh.vqdsnc.cn

println("Hello")
来源：http://jfb.birdmap.top

[T52] Scala：变量
来源：http://zbm.ydjk.org.cn

val a = 1;  var b = 2
来源：http://jox.fehbvm.com

[T53] Scala：字符串插值
来源：http://voq.svipenyu.cn

s"值: $b"
来源：http://tth.aizwys.cn

[T54] Scala：集合映射
来源：http://vjd.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://yxz.guannengcc.top

[T55] Scala：集合过滤
来源：http://hee.guowangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://dyu.nwbrower.top

[T56] Scala：样例类
来源：http://yxf.shuidangran.top

case class User(name: String, age: Int)
来源：http://klq.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://xoc.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jik.kuanghao11.cn

[T58] Scala：函数定义
来源：http://yuq.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://rsv.c1oappe.top

[T59] Scala：循环
来源：http://jyi.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://ybx.yueranfly.top

[T60] Scala：折叠
来源：http://dwj.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wll.xylfe.cn

================================================================================
来源：http://kgg.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xfu.andypj.xyz

================================================================================
来源：http://uat.gzhubu.top

[U01] Py：创建虚拟环境
来源：http://dxh.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dfx.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://fxb.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yva.ivvv.top

[U03] Py：加载 .env 配置
来源：http://aru.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ivq.ybcxt.top

[U04] Py：变量调试打印
来源：http://lwj.fktsv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sba.aizwys.cn

[U05] Py：列表去重且保序
来源：http://pqh.hcnkem.com

list(dict.fromkeys(arr))
来源：http://ytx.jinghuilouyu.cn

[U06] Py：合并两个字典
来源：http://hcn.zhoulong.xyz

{**a, **b}
来源：http://hxi.jiagoushi.top

[U07] Py：反转字典键值
来源：http://alk.yuxming.cn

{v: k for k, v in d.items()}
来源：http://icf.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://hdl.gogol.net.cn

[y for x in nested for y in x]
来源：http://jmx.ivvv.top

[U09] Py：字典取最大值的键
来源：http://vjo.gzhubu.top

max(d, key=d.get)
来源：http://thv.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://xek.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bla.aibaodan.cn

[U11] Py：生成器表达式
来源：http://nlz.daxiang520.top

(x * 2 for x in arr)
来源：http://kue.jinqigufen.top

[U12] Py：取出现最多的 3 个元素
来源：http://nyz.yvedp.cn

Counter(arr).most_common(3)
来源：http://qtm.316326.xyz

[U13] Py：固定长度队列
来源：http://apj.fengsongda.top

deque(maxlen=10)
来源：http://kjq.xinyue.icu

[U14] Py：分组收集到列表
来源：http://bwo.hysaishi.cn

defaultdict(list)
来源：http://bmy.guowangkeji.top

[U15] Py：高精度计时
来源：http://hvq.chenlongwang.top

t = time.perf_counter()
来源：http://tpp.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://sjh.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uto.bjfxy.top

[U17] Py：初始化日志
来源：http://grg.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://niv.cucudq.cn

[U18] Py：预编译正则
来源：http://ifz.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://flb.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://zlo.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fjz.meibo888.top

[U20] Py：缓存函数结果
来源：http://cch.cheryme.top

@functools.lru_cache(maxsize=None)
来源：http://sju.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://xzk.zdbjq.cn

@contextlib.contextmanager
来源：http://hbe.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://vwr.vqdsnc.cn

list(zip(*m))
来源：http://qlr.dianchejie.cn

[U23] Py：分块读取大文件
来源：http://qhn.hammf.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://igj.xylfe.cn

[U24] Py：路径操作
来源：http://ogc.nanxuanxn.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jcd.yj20258888.top

[U25] Py：CSV 按字典读
来源：http://ozo.shuidangran.top

csv.DictReader(f)
来源：http://krf.jqgfzy.top

[U26] Py：并发下载
来源：http://vim.cashguo.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yol.hesvh.cn

[U27] Py：异步 HTTP
来源：http://gdq.nwbrower.top

aiohttp.ClientSession() 配合 async with
来源：http://atu.gzhubu.top

[U28] Py：类型别名
来源：http://phv.hammf.cn

UserId = int
来源：http://jtf.jqgfzy.top

[U29] Py：属性校验
来源：http://hsa.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://xur.dashuyun.cn

[U30] Py：数据类
来源：http://rud.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://tfd.smart0.xyz

[U31] Py：单测
来源：http://sib.uphjek.com

python -m pytest -q
来源：http://dbw.sweek.top

[U32] Py：代码格式化
来源：http://pff.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://gpm.xinyue.icu

[U33] Py：打包发布
来源：http://lha.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://twn.yuxming.cn

[U34] Py：判断编码
来源：http://rbf.jianghu66.top

chardet.detect(raw)
来源：http://yey.jinghuilouyu.cn


<!-- 参考信息 -->