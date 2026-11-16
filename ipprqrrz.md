代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://vze.jianghu66.top

[S15] C：类型转换
来源：http://sew.cqqwz.cn

(double) a / b
来源：http://tqn.vqdsnc.cn

[S16] C：位操作置位
来源：http://rif.havefunace.top

x |= (1 << 3);
来源：http://ntw.daria6918.cn

[S17] C：安全拼接字符串
来源：http://tty.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oqu.snrcjt.cn

[S18] C：命令行参数
来源：http://kyu.guannengcc.top

int main(int argc, char **argv)
来源：http://arn.hesvh.cn

[S19] C：快速排序
来源：http://ktr.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://mlo.yonumen.top

[S20] C：二分查找
来源：http://syz.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gmf.chenzaomai.com

[S21] C：字符类别判断
来源：http://oii.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uex.birdmap.top

[S22] C：字符串转数字
来源：http://snb.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wcp.cashguo.top

[S23] C：随机数
来源：http://dte.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jxd.tarul.cn

[S24] C：获取本地时间
来源：http://rqe.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eod.ctjpmb.com

[S25] C：内存拷贝
来源：http://gqk.yonumen.top

memcpy(dst, src, n);
来源：http://msg.dashuyun.cn

[S26] C：内存清零
来源：http://czy.52xcode.cn

memset(a, 0, sizeof a);
来源：http://yws.yuanzhike.top

[S27] C：定义常量
来源：http://vtb.jinqigufen.top

const double PI = 3.14159;
来源：http://brc.vehdjk.com

[S28] C：静态变量
来源：http://gbp.yj20258.top

static int counter = 0;
来源：http://fbb.iojbl.cn

[S29] C：变参函数
来源：http://ebl.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mlr.cashguo.top

[S30] C：头文件保护
来源：http://xrl.ctjpmb.com

#ifndef X_H
来源：http://fnb.hnxiangtu.top

#define X_H
来源：http://eqh.fzhhl.top

#endif
来源：http://lpx.guowangkeji.top

[S31] C++：Hello World
来源：http://bib.zhixingplan.top

#include <iostream>
来源：http://ukz.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://onp.ybcxt.top

[S32] C++：字符串
来源：http://vmo.sweek.top

std::string s = "hi";  s += "!";
来源：http://tsy.dianchejie.cn

[S33] C++：vector 增删
来源：http://ufy.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://umm.birdmap.top

[S34] C++：遍历 vector
来源：http://his.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://szw.ivvv.top

[S35] C++：map
来源：http://ytm.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sip.cashguo.top

[S36] C++：unordered_map
来源：http://mhv.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wmq.shangyingyoupin.top

[S37] C++：set
来源：http://qzf.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sdv.tianlin.xyz

[S38] C++：排序
来源：http://arv.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://jty.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://tgs.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fey.smart0.xyz

[S40] C++：查找元素
来源：http://akx.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tgj.tarul.cn

[S41] C++：类与构造函数
来源：http://ucd.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aqr.tian-w.cn

[S42] C++：继承与虚函数
来源：http://fln.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://vui.smart0.xyz

[S43] C++：智能指针
来源：http://opf.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://lda.chenjidiqi.icu

[S44] C++：引用传参
来源：http://rjj.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://mii.yj20258.top

[S45] C++：lambda
来源：http://tsx.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jpw.xuetiantiany.cn

[S46] C++：函数模板
来源：http://nwp.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://klz.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://jbf.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://htk.xinyue.icu

[S48] C++：逐行读文件
来源：http://aoz.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://rxz.yuxming.cn

while (std::getline(in, line)) { }
来源：http://jlf.xziqi.cn

[S49] C++：写文件
来源：http://lhi.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iyz.yonumen.top

[S50] C++：格式化数字
来源：http://pfs.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xqk.shzxlz.cn

[S51] C++：显式类型转换
来源：http://ycn.fengsongda.top

static_cast<double>(a) / b
来源：http://yqs.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://qjr.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://rgf.ppjwa.cn

[S53] C++：移动语义
来源：http://iuz.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://noc.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://iwy.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ghk.yuxming.cn

[S55] C++：结构化绑定
来源：http://yco.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jty.ivvv.top

[S56] C++：optional
来源：http://hqp.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cby.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://muh.xuetiantiany.cn

constexpr int N = 10;
来源：http://qja.zhijiandao.cn

[S58] C++：命名空间
来源：http://acf.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://uqn.yj202588.top

[S59] C++：静态断言
来源：http://wyz.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jyh.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://fde.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwk.zdbjq.cn

================================================================================
来源：http://sgz.daria6918.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fef.yueranfly.top

================================================================================
来源：http://vdu.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://wdv.dashuyun.cn

println("Hello")
来源：http://nbz.bjfxy.top

[T02] Kotlin：变量
来源：http://pnj.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ezm.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://fru.vqdsnc.cn

"值: $b"
来源：http://cbn.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://wrh.yangfankeji.com

val n: String? = null;  n?.length
来源：http://ofe.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://cyy.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://flk.tanke756.top

[T06] Kotlin：集合映射
来源：http://cqe.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhk.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://zsd.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vuo.snrcjt.cn

[T08] Kotlin：数据类
来源：http://etl.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://tak.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://dqt.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://zlh.52xcode.cn

[T10] Kotlin：默认参数
来源：http://jty.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iei.pycfn.com

[T11] Kotlin：协程
来源：http://ffu.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zsw.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://jtz.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://ixs.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://tja.fzhhl.top

val m = mapOf("a" to 1)
来源：http://cnu.zhongyouzk.top

[T14] Kotlin：循环
来源：http://ult.meibo888.top

for (i in 1..10) println(i)
来源：http://nzo.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://tsi.sxryk.cn

interface Shape { fun area(): Double }
来源：http://hng.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://szt.xingfuxueyuan.xyz

print("Hello")
来源：http://sue.daxiang520.top

[T17] Swift：变量与常量
来源：http://mhb.snrcjt.cn

var a = 1;  let b = 2
来源：http://llx.tian-w.cn

[T18] Swift：字符串插值
来源：http://fsg.ybcxt.top

"值: \(b)"
来源：http://kvd.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://gql.yj20258.top

if let n = opt { print(n) }
来源：http://dlp.gotoacloud.top

[T20] Swift：数组操作
来源：http://qgy.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gks.cucudq.cn

[T21] Swift：遍历
来源：http://gnb.xylfe.cn

for x in a { print(x) }
来源：http://twl.cashguo.top

[T22] Swift：字典
来源：http://xwr.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://yst.jlsjyb.cn

[T23] Swift：函数
来源：http://krw.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wdu.zhijiandao.cn

[T24] Swift：闭包
来源：http://etz.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tav.cqqwz.cn

[T25] Swift：结构体
来源：http://veo.fanxiaobao.xyz

struct P { var x: Int }
来源：http://wlf.xziqi.cn

[T26] Swift：类与重写
来源：http://jcc.tarul.cn

class A: Base { override func f() {} }
来源：http://lih.gaohongyu789.top

[T27] Swift：错误处理
来源：http://fei.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://iyf.hfpthk.cn

[T28] Swift：枚举
来源：http://flk.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://ter.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://bkw.yongpay.top

guard let x = opt else { return }
来源：http://jng.c1oappe.top

[T30] Swift：协议
来源：http://ytj.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://xyz.yongpay.top

[T31] Lua：Hello World
来源：http://kxn.cucudq.cn

print("Hello")
来源：http://fpf.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://ghv.xinyue.icu

local a = 1
来源：http://wnv.ctjpmb.com

[T33] Lua：表（数组）
来源：http://qib.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://xgm.hywenlv.cn

[T34] Lua：遍历表
来源：http://eag.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kfl.yuanzhike.top

[T35] Lua：字典表
来源：http://yll.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://wwd.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://ecl.tian-w.cn

function add(a, b) return a + b end
来源：http://srp.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://qkq.zhoulong.xyz

"a" .. "b"
来源：http://trr.nanxuanxn.top

[T38] Lua：条件
来源：http://qkl.ivvv.top

if x > 0 then print("正") end
来源：http://vot.yvedp.cn

[T39] Lua：模式匹配
来源：http://xwk.quarkkingdee.top

string.find(s, "%d+")
来源：http://jsm.haohaochexian.top

[T40] Lua：元表
来源：http://vtu.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://pdj.316326.xyz

[T41] Perl：Hello World
来源：http://lna.52xcode.cn

print "Hello\n";
来源：http://ecd.sxryk.cn

[T42] Perl：变量类型
来源：http://emy.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xoj.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://giw.mhx1999.top

"值: $a"
来源：http://jsb.yanxiufei.cn

[T44] Perl：条件
来源：http://tcl.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://ypg.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://rpb.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://ojg.yuanzhike.top

[T46] Perl：哈希操作
来源：http://chq.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zux.xziqi.cn

[T47] Perl：正则捕获
来源：http://eey.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dtb.wangdashe.top

[T48] Perl：正则替换
来源：http://wmu.316326.xyz

$s =~ s/old/new/g;
来源：http://kdd.yfazqb.com

[T49] Perl：函数
来源：http://jiq.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ncr.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://ylv.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ber.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://pew.hywenlv.cn

[T51] Scala：Hello World
来源：http://jsk.zhongyouzk.top

println("Hello")
来源：http://ean.jiagoushi.top

[T52] Scala：变量
来源：http://qvk.yanxiufei.cn

val a = 1;  var b = 2
来源：http://qcy.guannengcc.top

[T53] Scala：字符串插值
来源：http://kuo.pengpengdd.cyou

s"值: $b"
来源：http://oja.ybcxt.top

[T54] Scala：集合映射
来源：http://opl.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://bkw.birdmap.top

[T55] Scala：集合过滤
来源：http://art.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mhs.yfazqb.com

[T56] Scala：样例类
来源：http://hsg.jyoumei.cn

case class User(name: String, age: Int)
来源：http://cca.hesvh.cn

[T57] Scala：模式匹配
来源：http://cwl.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tzo.iojbl.cn

[T58] Scala：函数定义
来源：http://lhb.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://yif.jinqigfzy.top

[T59] Scala：循环
来源：http://jky.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://ydr.vehdjk.com

[T60] Scala：折叠
来源：http://sxl.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gel.guowangkeji.top

================================================================================
来源：http://jfm.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eez.jqgufenzy.top

================================================================================
来源：http://cvh.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://mcj.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zjx.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://ooz.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nio.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://liq.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://rrk.gotoacloud.top

[U04] Py：变量调试打印
来源：http://fml.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hal.fanxiaobao.xyz

[U05] Py：列表去重且保序
来源：http://oza.yanxiufei.cn

list(dict.fromkeys(arr))
来源：http://alv.aizwys.cn

[U06] Py：合并两个字典
来源：http://srk.yfazqb.com

{**a, **b}
来源：http://yeb.yonumen.top

[U07] Py：反转字典键值
来源：http://eww.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://qbs.cucudq.cn

[U08] Py：展平二维列表
来源：http://anq.jlsjyb.cn

[y for x in nested for y in x]
来源：http://wje.tarul.cn

[U09] Py：字典取最大值的键
来源：http://dpo.fehbvm.com

max(d, key=d.get)
来源：http://tqu.fengsongda.top

[U10] Py：按值排序字典
来源：http://dli.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sex.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://twq.316326.xyz

(x * 2 for x in arr)
来源：http://pga.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://zip.fehbvm.com

Counter(arr).most_common(3)
来源：http://ypi.shuidangran.top

[U13] Py：固定长度队列
来源：http://npg.cqqwz.cn

deque(maxlen=10)
来源：http://yqe.bbcook.cn

[U14] Py：分组收集到列表
来源：http://ajw.pycfn.com

defaultdict(list)
来源：http://ifw.fzhhl.top

[U15] Py：高精度计时
来源：http://xje.cqqwz.cn

t = time.perf_counter()
来源：http://wmk.hcnkem.com

[U16] Py：命令行参数解析
来源：http://pmb.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jse.svipenyu.cn

[U17] Py：初始化日志
来源：http://jfq.xingfuxueyuan.xyz

logging.basicConfig(level=logging.INFO)
来源：http://dhe.redwolf501.top

[U18] Py：预编译正则
来源：http://hqe.yfazqb.com

pat = re.compile(r"\d+")
来源：http://bxz.jlsjyb.cn

[U19] Py：正则替换带回调
来源：http://peq.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qox.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://hwe.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://obz.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://hez.gzhubu.top

@contextlib.contextmanager
来源：http://sgo.ydzc1.top

[U22] Py：矩阵转置
来源：http://atk.ydzc1.top

list(zip(*m))
来源：http://fnx.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://jku.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eqa.zycfv.cn

[U24] Py：路径操作
来源：http://ccg.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://epj.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://afq.jyoumei.cn

csv.DictReader(f)
来源：http://qeo.0kj1m.cn

[U26] Py：并发下载
来源：http://spi.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zun.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://zpm.snrcjt.cn

aiohttp.ClientSession() 配合 async with
来源：http://uvk.tian-w.cn

[U28] Py：类型别名
来源：http://dlp.ydzc1.top

UserId = int
来源：http://qqv.hcnkem.com

[U29] Py：属性校验
来源：http://dru.svipenyu.cn

@property 与 @x.setter 配合
来源：http://qee.birdmap.top

[U30] Py：数据类
来源：http://bsj.aibaodan.cn

@dataclass(slots=True)
来源：http://whi.cdnleiting.top

[U31] Py：单测
来源：http://jfz.aizwys.cn

python -m pytest -q
来源：http://oko.epnwcf.com

[U32] Py：代码格式化
来源：http://pky.chenlongwang.top

ruff format . && ruff check --fix .
来源：http://izi.wangshuangyany.cn

[U33] Py：打包发布
来源：http://gap.hywenlv.cn

python -m build  （依赖 pyproject.toml）
来源：http://lne.uphjek.com

[U34] Py：判断编码
来源：http://jro.chenjidiqi.icu

chardet.detect(raw)
来源：http://mvz.zdqjudy.top

[U35] Py：发送邮件
来源：http://npf.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hsr.hcnkem.com

[U36] Py：定时任务
来源：http://mlr.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://oie.uphjek.com

[U37] Py：读写 Excel
来源：http://jue.tarul.cn

pandas.read_excel / DataFrame.to_excel
来源：http://bih.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://lle.havefunace.top

Path(__file__).resolve().parent
来源：http://aoy.hfpthk.cn


<!-- 参考信息 -->