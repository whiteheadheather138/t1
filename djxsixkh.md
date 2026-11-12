代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://xxl.dashuyun.cn

[S15] C：类型转换
来源：http://wwy.chenlongwang.top

(double) a / b
来源：http://mrk.yuxming.cn

[S16] C：位操作置位
来源：http://gmo.hnxiangtu.top

x |= (1 << 3);
来源：http://zlp.iojbl.cn

[S17] C：安全拼接字符串
来源：http://dvq.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dad.xziqi.cn

[S18] C：命令行参数
来源：http://tfv.aizwys.cn

int main(int argc, char **argv)
来源：http://bne.gzhubu.top

[S19] C：快速排序
来源：http://lic.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jbg.dashuyun.cn

[S20] C：二分查找
来源：http://wwu.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zhs.ppjwa.cn

[S21] C：字符类别判断
来源：http://teb.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fkf.fktsv.cn

[S22] C：字符串转数字
来源：http://iqn.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xvv.yuanzhike.top

[S23] C：随机数
来源：http://nxt.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dms.zhongyouzk.top

[S24] C：获取本地时间
来源：http://pqe.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://idy.jqgufenzy.top

[S25] C：内存拷贝
来源：http://zlf.fengsongda.top

memcpy(dst, src, n);
来源：http://ukz.yfazqb.com

[S26] C：内存清零
来源：http://rmr.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://yvo.bbcook.cn

[S27] C：定义常量
来源：http://dpl.snrcjt.cn

const double PI = 3.14159;
来源：http://tnu.shuidangran.top

[S28] C：静态变量
来源：http://lff.daxiang520.top

static int counter = 0;
来源：http://xxg.epnwcf.com

[S29] C：变参函数
来源：http://efv.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bqf.andypj.xyz

[S30] C：头文件保护
来源：http://dyh.tanke756.top

#ifndef X_H
来源：http://qhx.gaohongyu789.top

#define X_H
来源：http://hjb.bbcook.cn

#endif
来源：http://kye.cucudq.cn

[S31] C++：Hello World
来源：http://scp.xuanzx.com

#include <iostream>
来源：http://bjj.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://uls.xziqi.cn

[S32] C++：字符串
来源：http://fsm.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://amu.c1oappe.top

[S33] C++：vector 增删
来源：http://ukd.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fdz.fehbvm.com

[S34] C++：遍历 vector
来源：http://wtd.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://lhr.yfazqb.com

[S35] C++：map
来源：http://eil.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nqm.ydzc1.top

[S36] C++：unordered_map
来源：http://hzj.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iwo.gaohongyu789.top

[S37] C++：set
来源：http://oia.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wat.zycfv.cn

[S38] C++：排序
来源：http://gaz.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://lqr.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://yqh.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xag.hcnkem.com

[S40] C++：查找元素
来源：http://kqt.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gxh.316326.xyz

[S41] C++：类与构造函数
来源：http://hwb.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vpo.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://udf.yj20258888.top

class B : public Base { public: void f() override {} };
来源：http://var.nanxuanxn.top

[S43] C++：智能指针
来源：http://zsc.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://ygp.chenzaomai.com

[S44] C++：引用传参
来源：http://ene.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://msj.yj20258.top

[S45] C++：lambda
来源：http://pws.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://iun.cucudq.cn

[S46] C++：函数模板
来源：http://usf.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gah.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://qze.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cyw.c1oappe.top

[S48] C++：逐行读文件
来源：http://ktn.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://psp.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://dhc.c1oappe.top

[S49] C++：写文件
来源：http://iej.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qxu.guannengcc.top

[S50] C++：格式化数字
来源：http://lfe.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://thk.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://vya.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://kcv.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://idc.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://qpr.sjlbkw.cn

[S53] C++：移动语义
来源：http://mbq.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://ccb.nwbrower.top

[S54] C++：异常处理
来源：http://zej.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ula.nanxinkj.top

[S55] C++：结构化绑定
来源：http://zdk.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wbe.chenzaomai.com

[S56] C++：optional
来源：http://zqh.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uzg.yuanzhike.top

[S57] C++：编译期常量
来源：http://vva.xylfe.cn

constexpr int N = 10;
来源：http://jxd.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://pwk.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://edf.yuanzhike.top

[S59] C++：静态断言
来源：http://fus.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nkx.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://pch.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cdo.bbcook.cn

================================================================================
来源：http://lye.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bwe.sjlbkw.cn

================================================================================
来源：http://vzx.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://xeh.nanxuanxn.top

println("Hello")
来源：http://nff.havefunace.top

[T02] Kotlin：变量
来源：http://eau.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://llq.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://syw.pycfn.com

"值: $b"
来源：http://tka.shzxlz.cn

[T04] Kotlin：空安全
来源：http://zho.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://rri.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://uur.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsm.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://ymm.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://mpv.yonumen.top

[T07] Kotlin：集合过滤
来源：http://fhl.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://toc.xziqi.cn

[T08] Kotlin：数据类
来源：http://eka.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://rft.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://srv.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://zcr.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://sjc.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://kcf.ctjpmb.com

[T11] Kotlin：协程
来源：http://qhh.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xct.xziqi.cn

[T12] Kotlin：解构声明
来源：http://emn.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://vvj.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://upa.hnqzz.top

val m = mapOf("a" to 1)
来源：http://oiv.fehbvm.com

[T14] Kotlin：循环
来源：http://snu.nwbrower.top

for (i in 1..10) println(i)
来源：http://lub.yuanzhike.top

[T15] Kotlin：接口
来源：http://qza.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://qgk.c1oappe.top

[T16] Swift：Hello World
来源：http://vvm.cucudq.cn

print("Hello")
来源：http://wbd.ctjpmb.com

[T17] Swift：变量与常量
来源：http://iwb.epnwcf.com

var a = 1;  let b = 2
来源：http://wlj.shuidangran.top

[T18] Swift：字符串插值
来源：http://vlz.xuanzx.com

"值: \(b)"
来源：http://dup.ivvv.top

[T19] Swift：可选绑定
来源：http://ron.wangdashe.top

if let n = opt { print(n) }
来源：http://izx.zhongyouzk.top

[T20] Swift：数组操作
来源：http://irw.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://mjw.fehbvm.com

[T21] Swift：遍历
来源：http://ccz.smart0.xyz

for x in a { print(x) }
来源：http://xex.tanke756.top

[T22] Swift：字典
来源：http://rem.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://gzn.c1oappe.top

[T23] Swift：函数
来源：http://hcx.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hou.xziqi.cn

[T24] Swift：闭包
来源：http://pub.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fsw.zhixingplan.top

[T25] Swift：结构体
来源：http://fev.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://odm.uphjek.com

[T26] Swift：类与重写
来源：http://lsk.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://uqg.yuanzhike.top

[T27] Swift：错误处理
来源：http://kgw.meibo888.top

do { try f() } catch { print(error) }
来源：http://xmv.zhiwuduotai.top

[T28] Swift：枚举
来源：http://jto.zhiwuduotai.top

enum Color { case red, green }
来源：http://gzr.havefunace.top

[T29] Swift：guard 提前返回
来源：http://jue.hammf.cn

guard let x = opt else { return }
来源：http://zli.cdnleiting.top

[T30] Swift：协议
来源：http://azj.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://zec.9152youxi.cn

[T31] Lua：Hello World
来源：http://gpv.zhengqikj.top

print("Hello")
来源：http://ynh.sweek.top

[T32] Lua：局部变量
来源：http://kqc.jinyuanbaomall.cn

local a = 1
来源：http://dvo.jinqigufen.top

[T33] Lua：表（数组）
来源：http://pbh.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zar.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://wtq.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://nls.gogol.net.cn

[T35] Lua：字典表
来源：http://jxs.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://vxm.nanxinkj.top

[T36] Lua：函数
来源：http://igu.sjlbkw.cn

function add(a, b) return a + b end
来源：http://yto.xziqi.cn

[T37] Lua：字符串拼接
来源：http://eix.jqgufenzy.top

"a" .. "b"
来源：http://dlc.smart0.xyz

[T38] Lua：条件
来源：http://azh.fktsv.cn

if x > 0 then print("正") end
来源：http://dpm.gotoacloud.top

[T39] Lua：模式匹配
来源：http://kyj.cheryme.top

string.find(s, "%d+")
来源：http://akc.pycfn.com

[T40] Lua：元表
来源：http://qdr.fktsv.cn

setmetatable({}, { __index = base })
来源：http://wga.xziqi.cn

[T41] Perl：Hello World
来源：http://pts.iojbl.cn

print "Hello\n";
来源：http://wwn.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://gqp.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iws.guowangkeji.top

[T43] Perl：字符串插值
来源：http://qwq.yj20258888.top

"值: $a"
来源：http://wmw.chenjidiqi.icu

[T44] Perl：条件
来源：http://imv.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://uva.sufxvd.cn

[T45] Perl：数组遍历
来源：http://vos.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://oyd.jinqigufen.top

[T46] Perl：哈希操作
来源：http://zox.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://chw.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://pry.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ltt.ctjpmb.com

[T48] Perl：正则替换
来源：http://jch.uphjek.com

$s =~ s/old/new/g;
来源：http://ldb.cdnleiting.top

[T49] Perl：函数
来源：http://qpi.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qvj.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://gxf.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hor.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://sbn.haohaochexian.top

[T51] Scala：Hello World
来源：http://ywk.wangdashe.top

println("Hello")
来源：http://jkg.zycfv.cn

[T52] Scala：变量
来源：http://ezg.daxiang520.top

val a = 1;  var b = 2
来源：http://rlu.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://vdf.pengpengdd.cyou

s"值: $b"
来源：http://rnj.dashuyun.cn

[T54] Scala：集合映射
来源：http://vij.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://scs.shuidangran.top

[T55] Scala：集合过滤
来源：http://gej.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oyl.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://uwj.ivvv.top

case class User(name: String, age: Int)
来源：http://bqo.gotoacloud.top

[T57] Scala：模式匹配
来源：http://hfu.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://udp.cashguo.top

[T58] Scala：函数定义
来源：http://iux.shangyingyoupin.top

def add(a: Int, b: Int): Int = a + b
来源：http://urn.jlsjyb.cn

[T59] Scala：循环
来源：http://fyt.feifeiyinyue.top

for (i <- 1 to 10) println(i)
来源：http://rmy.cucudq.cn

[T60] Scala：折叠
来源：http://hpx.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ict.zhijiandao.cn

================================================================================
来源：http://rzu.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yqg.yuanzhike.top

================================================================================
来源：http://hhf.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://vjw.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://ato.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://hbl.jiagoushi.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hdh.nanxinkj.top

[U03] Py：加载 .env 配置
来源：http://rqh.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://obp.chenlongwang.top

[U04] Py：变量调试打印
来源：http://guu.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://glo.52xcode.cn

[U05] Py：列表去重且保序
来源：http://gwq.yj202588.top

list(dict.fromkeys(arr))
来源：http://pqi.iojbl.cn

[U06] Py：合并两个字典
来源：http://ltg.nanxuanxn.top

{**a, **b}
来源：http://nrd.0kj1m.cn

[U07] Py：反转字典键值
来源：http://ixj.xziqi.cn

{v: k for k, v in d.items()}
来源：http://jul.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://heq.haohaochexian.top

[y for x in nested for y in x]
来源：http://xjk.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://tra.cqqwz.cn

max(d, key=d.get)
来源：http://oij.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://lkm.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kwr.316326.xyz

[U11] Py：生成器表达式
来源：http://zuq.fktsv.cn

(x * 2 for x in arr)
来源：http://hpm.hysaishi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mel.fengsongda.top

Counter(arr).most_common(3)
来源：http://otv.c1oappe.top

[U13] Py：固定长度队列
来源：http://blc.snrcjt.cn

deque(maxlen=10)
来源：http://zoh.yueranfly.top

[U14] Py：分组收集到列表
来源：http://bay.yueranfly.top

defaultdict(list)
来源：http://wdn.xylfe.cn

[U15] Py：高精度计时
来源：http://wbd.zhixingplan.top

t = time.perf_counter()
来源：http://ovr.guannengcc.top

[U16] Py：命令行参数解析
来源：http://uzn.ybcxt.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gio.ehwqpu.com

[U17] Py：初始化日志
来源：http://mus.fzhhl.top

logging.basicConfig(level=logging.INFO)
来源：http://lgu.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://kqm.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://cvq.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://ozx.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rrj.gzhubu.top

[U20] Py：缓存函数结果
来源：http://lxj.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://ytc.gotoacloud.top

[U21] Py：自定义上下文管理器
来源：http://jmf.jlsjyb.cn

@contextlib.contextmanager
来源：http://ocw.xuanzx.com

[U22] Py：矩阵转置
来源：http://kmm.dashuyun.cn

list(zip(*m))
来源：http://uxa.yj20258.top

[U23] Py：分块读取大文件
来源：http://koe.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://svv.hnqzz.top

[U24] Py：路径操作
来源：http://xcc.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jqq.yueranfly.top

[U25] Py：CSV 按字典读
来源：http://dvc.daxiang520.top

csv.DictReader(f)
来源：http://ooq.shzxlz.cn

[U26] Py：并发下载
来源：http://pdq.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xmf.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://gao.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://pwn.ivvv.top

[U28] Py：类型别名
来源：http://vzz.aibaodan.cn

UserId = int
来源：http://mln.bjfxy.top

[U29] Py：属性校验
来源：http://aii.ctjpmb.com

@property 与 @x.setter 配合
来源：http://pbk.jinqigfzy.top

[U30] Py：数据类
来源：http://hry.shangyingyoupin.top

@dataclass(slots=True)
来源：http://fmy.birdmap.top

[U31] Py：单测
来源：http://uaw.zycfv.cn

python -m pytest -q
来源：http://snk.nanxinkj.top

[U32] Py：代码格式化
来源：http://jzx.pycfn.com

ruff format . && ruff check --fix .
来源：http://bty.nwbrower.top

[U33] Py：打包发布
来源：http://wby.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://xjq.fzhhl.top

[U34] Py：判断编码
来源：http://vrr.jianghu66.top

chardet.detect(raw)
来源：http://rhh.zhixingplan.top

[U35] Py：发送邮件
来源：http://hwg.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qbe.yangfankeji.com

[U36] Py：定时任务
来源：http://zzl.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://hiw.redwolf501.top

[U37] Py：读写 Excel
来源：http://fpx.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hjz.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://czj.xingfuxueyuan.xyz

Path(__file__).resolve().parent
来源：http://rcb.fzhhl.top


<!-- 参考信息 -->