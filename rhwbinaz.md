代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://xpm.hongshengwenyu.top

[S15] C：类型转换
来源：http://fgt.fktsv.cn

(double) a / b
来源：http://fdn.ivvv.top

[S16] C：位操作置位
来源：http://nrm.tanke756.top

x |= (1 << 3);
来源：http://but.cheryme.top

[S17] C：安全拼接字符串
来源：http://bvk.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sro.52xcode.cn

[S18] C：命令行参数
来源：http://adq.andypj.xyz

int main(int argc, char **argv)
来源：http://elr.havefunace.top

[S19] C：快速排序
来源：http://akx.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://bkw.birdmap.top

[S20] C：二分查找
来源：http://vxc.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://saj.yongpay.top

[S21] C：字符类别判断
来源：http://ici.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jfl.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://zrn.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xvw.epnwcf.com

[S23] C：随机数
来源：http://sla.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pdp.shuidangran.top

[S24] C：获取本地时间
来源：http://fan.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bax.guannengcc.top

[S25] C：内存拷贝
来源：http://wgt.jianghu66.top

memcpy(dst, src, n);
来源：http://gyb.ydjk.org.cn

[S26] C：内存清零
来源：http://tns.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://lhd.cashguo.top

[S27] C：定义常量
来源：http://zyt.zhengqikj.top

const double PI = 3.14159;
来源：http://vfp.pengpengdd.cyou

[S28] C：静态变量
来源：http://meu.tian-w.cn

static int counter = 0;
来源：http://ysd.fehbvm.com

[S29] C：变参函数
来源：http://pba.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nio.meibo888.top

[S30] C：头文件保护
来源：http://lfa.havefunace.top

#ifndef X_H
来源：http://drd.yanxiufei.cn

#define X_H
来源：http://ebv.shanyushiyangkeji.top

#endif
来源：http://xqs.ctjpmb.com

[S31] C++：Hello World
来源：http://cwc.fehbvm.com

#include <iostream>
来源：http://gij.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://okg.zdbjq.cn

[S32] C++：字符串
来源：http://lsb.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://ieu.vehdjk.com

[S33] C++：vector 增删
来源：http://lbi.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cav.bbcook.cn

[S34] C++：遍历 vector
来源：http://nfb.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://eer.yuxming.cn

[S35] C++：map
来源：http://yyd.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vqd.zhengqikj.top

[S36] C++：unordered_map
来源：http://mrx.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zix.shanyushiyangkeji.top

[S37] C++：set
来源：http://adv.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zeo.ybcxt.top

[S38] C++：排序
来源：http://bnv.cashguo.top

std::sort(v.begin(), v.end());
来源：http://wte.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://mua.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xfu.gaohongyu789.top

[S40] C++：查找元素
来源：http://jqi.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ydn.yuanzhike.top

[S41] C++：类与构造函数
来源：http://pot.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oeg.iojbl.cn

[S42] C++：继承与虚函数
来源：http://ppz.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://woj.meibo888.top

[S43] C++：智能指针
来源：http://fny.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://adr.epnwcf.com

[S44] C++：引用传参
来源：http://yry.yfazqb.com

void inc(int &x) { ++x; }
来源：http://vqp.xziqi.cn

[S45] C++：lambda
来源：http://ftl.guowangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://wye.yj20258.top

[S46] C++：函数模板
来源：http://wgq.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gyk.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://cxl.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ljh.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://ckx.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sfl.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://ruc.pycfn.com

[S49] C++：写文件
来源：http://wbo.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvz.fehbvm.com

[S50] C++：格式化数字
来源：http://iqh.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kvh.nanxinkj.top

[S51] C++：显式类型转换
来源：http://cbj.cheryme.top

static_cast<double>(a) / b
来源：http://aes.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://whr.shuidangran.top

int size() const noexcept { return n_; }
来源：http://kvp.shangyingyoupin.top

[S53] C++：移动语义
来源：http://ltl.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://igo.cucudq.cn

[S54] C++：异常处理
来源：http://dhw.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nhg.jiagoushi.top

[S55] C++：结构化绑定
来源：http://anf.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ngj.fehbvm.com

[S56] C++：optional
来源：http://vys.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uut.yvedp.cn

[S57] C++：编译期常量
来源：http://hql.hnqzz.top

constexpr int N = 10;
来源：http://eae.tian-w.cn

[S58] C++：命名空间
来源：http://lkt.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://qme.ehwqpu.com

[S59] C++：静态断言
来源：http://hkt.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cph.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://yhs.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cxw.feifeiyinyue.top

================================================================================
来源：http://sry.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pzg.jinqigfzy.top

================================================================================
来源：http://pyt.hnqzz.top

[T01] Kotlin：Hello World
来源：http://xtu.bjfxy.top

println("Hello")
来源：http://emg.hywenlv.cn

[T02] Kotlin：变量
来源：http://uxc.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vvl.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://nhb.yuxming.cn

"值: $b"
来源：http://mvt.hysaishi.cn

[T04] Kotlin：空安全
来源：http://thj.hywenlv.cn

val n: String? = null;  n?.length
来源：http://fny.jinqigufen.top

[T05] Kotlin：when 表达式
来源：http://avx.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://txj.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://drf.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ibc.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://rkd.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sob.mhx1999.top

[T08] Kotlin：数据类
来源：http://fnq.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://ljo.tarul.cn

[T09] Kotlin：扩展函数
来源：http://hkh.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://fkd.xziqi.cn

[T10] Kotlin：默认参数
来源：http://vue.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xdr.yfazqb.com

[T11] Kotlin：协程
来源：http://cqx.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wny.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://utn.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://jbc.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://hfq.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://bzu.fehbvm.com

[T14] Kotlin：循环
来源：http://wcm.ivvv.top

for (i in 1..10) println(i)
来源：http://upr.zhoulong.xyz

[T15] Kotlin：接口
来源：http://crz.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://qlb.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://vrr.yj202588.top

print("Hello")
来源：http://fgb.iojbl.cn

[T17] Swift：变量与常量
来源：http://qwd.epnwcf.com

var a = 1;  let b = 2
来源：http://yul.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://aou.hysaishi.cn

"值: \(b)"
来源：http://gaj.andypj.xyz

[T19] Swift：可选绑定
来源：http://dhm.hnxiangtu.top

if let n = opt { print(n) }
来源：http://bnk.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://tkj.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://fcn.chenjidiqi.icu

[T21] Swift：遍历
来源：http://due.nanxuanxn.top

for x in a { print(x) }
来源：http://qns.guannengcc.top

[T22] Swift：字典
来源：http://aso.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://xop.birdmap.top

[T23] Swift：函数
来源：http://hdr.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pkf.mhx1999.top

[T24] Swift：闭包
来源：http://ftc.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ucj.sweek.top

[T25] Swift：结构体
来源：http://kgr.mhx1999.top

struct P { var x: Int }
来源：http://uop.zdbjq.cn

[T26] Swift：类与重写
来源：http://opn.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://wjj.cashguo.top

[T27] Swift：错误处理
来源：http://irj.tarul.cn

do { try f() } catch { print(error) }
来源：http://amo.guannengcc.top

[T28] Swift：枚举
来源：http://vbh.zhijiandao.cn

enum Color { case red, green }
来源：http://xhx.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://nua.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://ahp.svipenyu.cn

[T30] Swift：协议
来源：http://gtd.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://tvo.shuidangran.top

[T31] Lua：Hello World
来源：http://emb.hysaishi.cn

print("Hello")
来源：http://lmk.shuidangran.top

[T32] Lua：局部变量
来源：http://nyg.meibo888.top

local a = 1
来源：http://duc.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://tyu.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fig.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://dkn.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gdj.fktsv.cn

[T35] Lua：字典表
来源：http://sws.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://hdd.quarkkingdee.top

[T36] Lua：函数
来源：http://vua.nanxuanxn.top

function add(a, b) return a + b end
来源：http://qgs.daxiang520.top

[T37] Lua：字符串拼接
来源：http://xpr.fehbvm.com

"a" .. "b"
来源：http://ujb.aibaodan.cn

[T38] Lua：条件
来源：http://usy.aibaodan.cn

if x > 0 then print("正") end
来源：http://vqh.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://wfu.hnxiangtu.top

string.find(s, "%d+")
来源：http://pbt.redwolf501.top

[T40] Lua：元表
来源：http://wff.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://nqf.jinqigufen.top

[T41] Perl：Hello World
来源：http://knq.xuetiantiany.cn

print "Hello\n";
来源：http://ukv.c1oappe.top

[T42] Perl：变量类型
来源：http://rmo.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://owj.tanke756.top

[T43] Perl：字符串插值
来源：http://coi.sufxvd.cn

"值: $a"
来源：http://hjz.iojbl.cn

[T44] Perl：条件
来源：http://uyb.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://sql.havefunace.top

[T45] Perl：数组遍历
来源：http://evq.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://kbi.gzhubu.top

[T46] Perl：哈希操作
来源：http://wwk.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wln.shzxlz.cn

[T47] Perl：正则捕获
来源：http://flt.uphjek.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://yuo.jiagoushi.top

[T48] Perl：正则替换
来源：http://hdt.yvedp.cn

$s =~ s/old/new/g;
来源：http://qja.cheryme.top

[T49] Perl：函数
来源：http://iqq.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jxv.chenjidiqi.icu

[T50] Perl：逐行读文件
来源：http://azs.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://vjb.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://afh.zdbjq.cn

[T51] Scala：Hello World
来源：http://jeg.ydzc1.top

println("Hello")
来源：http://nmx.hysaishi.cn

[T52] Scala：变量
来源：http://yvm.yfazqb.com

val a = 1;  var b = 2
来源：http://das.ctjpmb.com

[T53] Scala：字符串插值
来源：http://lfh.316326.xyz

s"值: $b"
来源：http://mbe.cdnleiting.top

[T54] Scala：集合映射
来源：http://jgj.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://mik.hesvh.cn

[T55] Scala：集合过滤
来源：http://tay.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mso.shuidangran.top

[T56] Scala：样例类
来源：http://myn.vehdjk.com

case class User(name: String, age: Int)
来源：http://inn.cdnleiting.top

[T57] Scala：模式匹配
来源：http://vcq.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lns.birdmap.top

[T58] Scala：函数定义
来源：http://vxm.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://ssf.sjlbkw.cn

[T59] Scala：循环
来源：http://jmm.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://bqi.fktsv.cn

[T60] Scala：折叠
来源：http://kbv.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rxy.uphjek.com

================================================================================
来源：http://fiu.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://azy.jlsjyb.cn

================================================================================
来源：http://jxy.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://ihq.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://bxn.tian-w.cn

[U02] Py：导出 / 安装依赖
来源：http://baq.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvx.meibo888.top

[U03] Py：加载 .env 配置
来源：http://pxj.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lyd.tian-w.cn

[U04] Py：变量调试打印
来源：http://nij.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kig.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://tef.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://ico.nwbrower.top

[U06] Py：合并两个字典
来源：http://vtc.jinyuanbaomall.cn

{**a, **b}
来源：http://rth.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://xwb.hywenlv.cn

{v: k for k, v in d.items()}
来源：http://kjb.daxiang520.top

[U08] Py：展平二维列表
来源：http://qxu.fehbvm.com

[y for x in nested for y in x]
来源：http://fum.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://nco.ydjk.org.cn

max(d, key=d.get)
来源：http://rta.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://yrc.0kj1m.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://len.ctjpmb.com

[U11] Py：生成器表达式
来源：http://ecj.jiagoushi.top

(x * 2 for x in arr)
来源：http://ftg.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://rrm.svipenyu.cn

Counter(arr).most_common(3)
来源：http://zaw.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://ott.smart0.xyz

deque(maxlen=10)
来源：http://omn.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://nms.gogol.net.cn

defaultdict(list)
来源：http://kiw.jinqigufen.top

[U15] Py：高精度计时
来源：http://cca.gaohongyu789.top

t = time.perf_counter()
来源：http://xxe.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://yrh.vehdjk.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://nvs.cqqwz.cn

[U17] Py：初始化日志
来源：http://cph.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://pfi.bjfxy.top

[U18] Py：预编译正则
来源：http://ytv.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://exa.zycfv.cn

[U19] Py：正则替换带回调
来源：http://dav.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fab.guowangkeji.top

[U20] Py：缓存函数结果
来源：http://tze.xuetiantiany.cn

@functools.lru_cache(maxsize=None)
来源：http://qot.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://txp.0kj1m.cn

@contextlib.contextmanager
来源：http://ipc.feifeiyinyue.top

[U22] Py：矩阵转置
来源：http://lza.sysykeji.top

list(zip(*m))
来源：http://igq.yuanzhike.top

[U23] Py：分块读取大文件
来源：http://yui.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fxg.yonumen.top

[U24] Py：路径操作
来源：http://uvz.jyoumei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uxn.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://pnq.vqdsnc.cn

csv.DictReader(f)
来源：http://ctq.ybcxt.top

[U26] Py：并发下载
来源：http://jdd.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cjt.bjfxy.top

[U27] Py：异步 HTTP
来源：http://sxy.yj20258888.top

aiohttp.ClientSession() 配合 async with
来源：http://qoh.pengpengdd.cyou

[U28] Py：类型别名
来源：http://tau.fzhhl.top

UserId = int
来源：http://zdo.xuetiantiany.cn

[U29] Py：属性校验
来源：http://qgs.chenlongwang.top

@property 与 @x.setter 配合
来源：http://kit.fengsongda.top

[U30] Py：数据类
来源：http://rzg.hywenlv.cn

@dataclass(slots=True)
来源：http://skv.dashuyun.cn

[U31] Py：单测
来源：http://evf.hesvh.cn

python -m pytest -q
来源：http://rlp.svipenyu.cn

[U32] Py：代码格式化
来源：http://msb.vqdsnc.cn

ruff format . && ruff check --fix .
来源：http://dsj.tarul.cn

[U33] Py：打包发布
来源：http://gwz.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://iyt.fzhhl.top

[U34] Py：判断编码
来源：http://poy.cucudq.cn

chardet.detect(raw)
来源：http://cqs.aizwys.cn

[U35] Py：发送邮件
来源：http://kkk.gotoacloud.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zza.cucudq.cn

[U36] Py：定时任务
来源：http://oia.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://zhk.fanxiaobao.xyz

[U37] Py：读写 Excel
来源：http://jho.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://yva.9152youxi.cn

[U38] Py：获取脚本所在目录
来源：http://tlv.haohaochexian.top

Path(__file__).resolve().parent
来源：http://cky.sxryk.cn


<!-- 参考信息 -->