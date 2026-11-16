代发 wailian999

x |= (1 << 3);
来源：http://ajv.sxryk.cn

[S17] C：安全拼接字符串
来源：http://zpz.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aef.ctjpmb.com

[S18] C：命令行参数
来源：http://zjg.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://quy.yuxming.cn

[S19] C：快速排序
来源：http://udu.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qwi.xziqi.cn

[S20] C：二分查找
来源：http://njv.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rax.hnxiangtu.top

[S21] C：字符类别判断
来源：http://jdo.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wmj.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://xfv.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://rab.jiagoushi.top

[S23] C：随机数
来源：http://moh.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mzt.yangfankeji.com

[S24] C：获取本地时间
来源：http://pal.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gsh.redwolf501.top

[S25] C：内存拷贝
来源：http://alz.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://hie.yanxiufei.cn

[S26] C：内存清零
来源：http://vla.wangdashe.top

memset(a, 0, sizeof a);
来源：http://agp.shzxlz.cn

[S27] C：定义常量
来源：http://iju.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://jjp.yueranfly.top

[S28] C：静态变量
来源：http://hoo.daria6918.cn

static int counter = 0;
来源：http://ots.vqdsnc.cn

[S29] C：变参函数
来源：http://xpr.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qbz.sysykeji.top

[S30] C：头文件保护
来源：http://wmh.9152youxi.cn

#ifndef X_H
来源：http://bwm.xingfuxueyuan.xyz

#define X_H
来源：http://dda.zhongyouzk.top

#endif
来源：http://efa.daxiang520.top

[S31] C++：Hello World
来源：http://hwt.ppjwa.cn

#include <iostream>
来源：http://bhw.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://pro.yfazqb.com

[S32] C++：字符串
来源：http://phl.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://akn.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://gtl.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cvz.tianlin.xyz

[S34] C++：遍历 vector
来源：http://mnk.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://hjo.jyoumei.cn

[S35] C++：map
来源：http://jwv.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yom.nanxinkj.top

[S36] C++：unordered_map
来源：http://yai.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sge.wangdashe.top

[S37] C++：set
来源：http://pct.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fyj.xylfe.cn

[S38] C++：排序
来源：http://csl.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://bhn.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://suh.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dkn.chenlongwang.top

[S40] C++：查找元素
来源：http://nxz.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zuq.bbcook.cn

[S41] C++：类与构造函数
来源：http://xco.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://veb.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://rmq.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://ine.ehwqpu.com

[S43] C++：智能指针
来源：http://gfj.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://mvn.cashguo.top

[S44] C++：引用传参
来源：http://kag.hesvh.cn

void inc(int &x) { ++x; }
来源：http://apa.zhiwuduotai.top

[S45] C++：lambda
来源：http://qjp.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://vjl.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://cdg.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ypm.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://kqm.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://usu.epnwcf.com

[S48] C++：逐行读文件
来源：http://wxf.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://qhe.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://bmn.zhengqikj.top

[S49] C++：写文件
来源：http://kss.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mgr.tarul.cn

[S50] C++：格式化数字
来源：http://jnd.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://suv.yj202588.top

[S51] C++：显式类型转换
来源：http://gtt.jinqigufen.top

static_cast<double>(a) / b
来源：http://qlw.pycfn.com

[S52] C++：const 与 noexcept
来源：http://tth.birdmap.top

int size() const noexcept { return n_; }
来源：http://oqe.hysaishi.cn

[S53] C++：移动语义
来源：http://wsp.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://otu.wangshuangyany.cn

[S54] C++：异常处理
来源：http://izp.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://msi.daxiang520.top

[S55] C++：结构化绑定
来源：http://brd.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ddn.hongshengwenyu.top

[S56] C++：optional
来源：http://dkr.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gfv.yj20258.top

[S57] C++：编译期常量
来源：http://gxp.cashguo.top

constexpr int N = 10;
来源：http://aey.hongshengwenyu.top

[S58] C++：命名空间
来源：http://vlx.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://kdf.sysykeji.top

[S59] C++：静态断言
来源：http://rmo.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uva.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://seg.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wel.yj20258888.top

================================================================================
来源：http://wqx.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uct.aibaodan.cn

================================================================================
来源：http://mgj.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://umn.zhiwuduotai.top

println("Hello")
来源：http://mpg.birdmap.top

[T02] Kotlin：变量
来源：http://zqm.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vhi.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://gaj.jinqigufen.top

"值: $b"
来源：http://wuk.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://eim.hywenlv.cn

val n: String? = null;  n?.length
来源：http://rny.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://ypc.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qcs.yfazqb.com

[T06] Kotlin：集合映射
来源：http://yva.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://hhs.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://rhp.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uoe.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://ssz.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://vib.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://rkx.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://upe.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://ynj.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mhm.vqdsnc.cn

[T11] Kotlin：协程
来源：http://zah.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bgj.sweek.top

[T12] Kotlin：解构声明
来源：http://wtf.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://jxc.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://gzi.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://pee.svipenyu.cn

[T14] Kotlin：循环
来源：http://uye.pycfn.com

for (i in 1..10) println(i)
来源：http://xta.shuidangran.top

[T15] Kotlin：接口
来源：http://lnb.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://nyj.ydjk.org.cn

[T16] Swift：Hello World
来源：http://ola.chenlongwang.top

print("Hello")
来源：http://qbv.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://cnd.316326.xyz

var a = 1;  let b = 2
来源：http://rvf.andypj.xyz

[T18] Swift：字符串插值
来源：http://zmc.nanxuanxn.top

"值: \(b)"
来源：http://eyo.tian-w.cn

[T19] Swift：可选绑定
来源：http://tpe.vehdjk.com

if let n = opt { print(n) }
来源：http://iwt.yueranfly.top

[T20] Swift：数组操作
来源：http://opp.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://rqw.gzhubu.top

[T21] Swift：遍历
来源：http://rdm.fengsongda.top

for x in a { print(x) }
来源：http://qoi.nanxuanxn.top

[T22] Swift：字典
来源：http://eop.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://fry.zhiwuduotai.top

[T23] Swift：函数
来源：http://omy.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dxi.hesvh.cn

[T24] Swift：闭包
来源：http://cjb.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://jmx.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://mgr.epnwcf.com

struct P { var x: Int }
来源：http://ryr.yuanzhike.top

[T26] Swift：类与重写
来源：http://mxx.zhixingplan.top

class A: Base { override func f() {} }
来源：http://ohj.bjfxy.top

[T27] Swift：错误处理
来源：http://cdw.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://zbo.kuanghao11.cn

[T28] Swift：枚举
来源：http://bis.sweek.top

enum Color { case red, green }
来源：http://dty.hesvh.cn

[T29] Swift：guard 提前返回
来源：http://ifz.svipenyu.cn

guard let x = opt else { return }
来源：http://rmt.c1oappe.top

[T30] Swift：协议
来源：http://klu.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://qfh.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://yrc.guowangkeji.top

print("Hello")
来源：http://tel.shuidangran.top

[T32] Lua：局部变量
来源：http://mcg.tianlin.xyz

local a = 1
来源：http://ouq.yj202588.top

[T33] Lua：表（数组）
来源：http://fgz.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://qso.yueranfly.top

[T34] Lua：遍历表
来源：http://sjx.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gtk.yonumen.top

[T35] Lua：字典表
来源：http://ikn.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://obx.meibo888.top

[T36] Lua：函数
来源：http://xub.pycfn.com

function add(a, b) return a + b end
来源：http://xat.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://usy.jinghuilouyu.cn

"a" .. "b"
来源：http://ccj.smart0.xyz

[T38] Lua：条件
来源：http://msk.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://rlf.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://urm.yuxming.cn

string.find(s, "%d+")
来源：http://wll.ehwqpu.com

[T40] Lua：元表
来源：http://bgo.wangshuangyany.cn

setmetatable({}, { __index = base })
来源：http://tjn.tian-w.cn

[T41] Perl：Hello World
来源：http://epx.yanxiufei.cn

print "Hello\n";
来源：http://wii.zycfv.cn

[T42] Perl：变量类型
来源：http://wtd.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eav.hcnkem.com

[T43] Perl：字符串插值
来源：http://xuj.ctjpmb.com

"值: $a"
来源：http://tpj.svipenyu.cn

[T44] Perl：条件
来源：http://lwl.gogol.net.cn

if ($a > 0) { print "正"; }
来源：http://lnw.yangfankeji.com

[T45] Perl：数组遍历
来源：http://rai.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://iim.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://kku.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jlo.yuanzhike.top

[T47] Perl：正则捕获
来源：http://vlv.pengpengdd.cyou

if ($s =~ /(\d+)/) { print $1; }
来源：http://fhj.yj202588.top

[T48] Perl：正则替换
来源：http://qjp.uphjek.com

$s =~ s/old/new/g;
来源：http://mmi.pengpengdd.cyou

[T49] Perl：函数
来源：http://igk.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uqy.mhx1999.top

[T50] Perl：逐行读文件
来源：http://fmg.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ows.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://ckm.cheryme.top

[T51] Scala：Hello World
来源：http://rwe.snrcjt.cn

println("Hello")
来源：http://jrw.sysykeji.top

[T52] Scala：变量
来源：http://yzt.shzxlz.cn

val a = 1;  var b = 2
来源：http://sjs.yj20258888.top

[T53] Scala：字符串插值
来源：http://upe.yj20258888.top

s"值: $b"
来源：http://nkv.chenzaomai.com

[T54] Scala：集合映射
来源：http://wvp.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://hga.nwbrower.top

[T55] Scala：集合过滤
来源：http://jhr.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://igw.zycfv.cn

[T56] Scala：样例类
来源：http://pdr.snrcjt.cn

case class User(name: String, age: Int)
来源：http://ogs.pycfn.com

[T57] Scala：模式匹配
来源：http://jkw.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://ezv.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://ifo.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://gsk.nanxinkj.top

[T59] Scala：循环
来源：http://mjt.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://soc.chenlongwang.top

[T60] Scala：折叠
来源：http://jkx.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cul.hywenlv.cn

================================================================================
来源：http://oiy.iojbl.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gps.hesvh.cn

================================================================================
来源：http://ztp.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://lcc.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://fly.zycfv.cn

[U02] Py：导出 / 安装依赖
来源：http://kbc.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oul.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://pqp.vqdsnc.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://czw.hammf.cn

[U04] Py：变量调试打印
来源：http://afy.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aqu.yvedp.cn

[U05] Py：列表去重且保序
来源：http://gam.cheryme.top

list(dict.fromkeys(arr))
来源：http://idu.sysykeji.top

[U06] Py：合并两个字典
来源：http://gvp.ybcxt.top

{**a, **b}
来源：http://esq.yj20258888.top

[U07] Py：反转字典键值
来源：http://upj.sxryk.cn

{v: k for k, v in d.items()}
来源：http://swy.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://wmc.jyoumei.cn

[y for x in nested for y in x]
来源：http://jwu.yongpay.top

[U09] Py：字典取最大值的键
来源：http://vtj.yj20258.top

max(d, key=d.get)
来源：http://riw.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://rmv.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://und.fengsongda.top

[U11] Py：生成器表达式
来源：http://shf.bbcook.cn

(x * 2 for x in arr)
来源：http://one.gzhubu.top

[U12] Py：取出现最多的 3 个元素
来源：http://mnh.nwbrower.top

Counter(arr).most_common(3)
来源：http://seo.tarul.cn

[U13] Py：固定长度队列
来源：http://hkn.dianchejie.cn

deque(maxlen=10)
来源：http://klj.xziqi.cn

[U14] Py：分组收集到列表
来源：http://hmh.zdbjq.cn

defaultdict(list)
来源：http://dur.birdmap.top

[U15] Py：高精度计时
来源：http://dbv.daxiang520.top

t = time.perf_counter()
来源：http://bts.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://bmx.shzxlz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oyr.hysaishi.cn

[U17] Py：初始化日志
来源：http://ykl.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://ptj.hesvh.cn

[U18] Py：预编译正则
来源：http://mpe.dianchejie.cn

pat = re.compile(r"\d+")
来源：http://dcx.jinqigfzy.top

[U19] Py：正则替换带回调
来源：http://mvk.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fqp.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://mlk.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://arw.quarkkingdee.top

[U21] Py：自定义上下文管理器
来源：http://xgk.ppjwa.cn

@contextlib.contextmanager
来源：http://apy.shanyushiyangkeji.top

[U22] Py：矩阵转置
来源：http://vqj.fanxiaobao.xyz

list(zip(*m))
来源：http://gax.cdnleiting.top

[U23] Py：分块读取大文件
来源：http://kie.gotoacloud.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mrv.hnqzz.top

[U24] Py：路径操作
来源：http://rtj.cucudq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bce.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://rln.hcnkem.com

csv.DictReader(f)
来源：http://xyi.haohaochexian.top

[U26] Py：并发下载
来源：http://atp.shangyingyoupin.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aca.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://agq.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://qsd.zhongyouzk.top

[U28] Py：类型别名
来源：http://ysd.shanyushiyangkeji.top

UserId = int
来源：http://uwa.ydzc1.top

[U29] Py：属性校验
来源：http://dve.tarul.cn

@property 与 @x.setter 配合
来源：http://cme.birdmap.top

[U30] Py：数据类
来源：http://kuv.zhengqikj.top

@dataclass(slots=True)
来源：http://ewf.jinyuanbaomall.cn

[U31] Py：单测
来源：http://djf.yanxiufei.cn

python -m pytest -q
来源：http://abj.sxryk.cn

[U32] Py：代码格式化
来源：http://cyh.sweek.top

ruff format . && ruff check --fix .
来源：http://miy.smart0.xyz

[U33] Py：打包发布
来源：http://jrv.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://wrd.feifeiyinyue.top

[U34] Py：判断编码
来源：http://sww.jqgfzy.top

chardet.detect(raw)
来源：http://fuc.jinqigufen.top

[U35] Py：发送邮件
来源：http://mqe.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yzk.dianchejie.cn

[U36] Py：定时任务
来源：http://btc.mhx1999.top

schedule.every(10).minutes.do(job)
来源：http://jcq.yueranfly.top

[U37] Py：读写 Excel
来源：http://yzm.zhijiandao.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pgt.xylfe.cn

[U38] Py：获取脚本所在目录
来源：http://wow.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://vus.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://mnx.xziqi.cn

sys.stdout.isatty()
来源：http://cye.sxryk.cn

[U40] Py：打印到标准错误
来源：http://tex.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://pbu.ywan-chungtsiang.top


<!-- 参考信息 -->