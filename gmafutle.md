代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://dvq.vqdsnc.cn

[S23] C：随机数
来源：http://hja.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://nnt.bbcook.cn

[S24] C：获取本地时间
来源：http://cef.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eqy.xylfe.cn

[S25] C：内存拷贝
来源：http://rtc.jiagoushi.top

memcpy(dst, src, n);
来源：http://gly.ehwqpu.com

[S26] C：内存清零
来源：http://isl.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://adj.hammf.cn

[S27] C：定义常量
来源：http://ljo.gaohongyu789.top

const double PI = 3.14159;
来源：http://tyf.hnxiangtu.top

[S28] C：静态变量
来源：http://bmi.aibaodan.cn

static int counter = 0;
来源：http://igk.cheryme.top

[S29] C：变参函数
来源：http://iuo.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nae.yfazqb.com

[S30] C：头文件保护
来源：http://otp.cucudq.cn

#ifndef X_H
来源：http://qld.52xcode.cn

#define X_H
来源：http://lnj.quarkkingdee.top

#endif
来源：http://olc.zhixingplan.top

[S31] C++：Hello World
来源：http://mat.yj20258888.top

#include <iostream>
来源：http://deo.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://rcg.jinghuilouyu.cn

[S32] C++：字符串
来源：http://dxm.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://tmr.hnxiangtu.top

[S33] C++：vector 增删
来源：http://zmb.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://frn.vehdjk.com

[S34] C++：遍历 vector
来源：http://ajd.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://iqp.gogol.net.cn

[S35] C++：map
来源：http://teg.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jmv.quarkkingdee.top

[S36] C++：unordered_map
来源：http://vwp.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rmt.hesvh.cn

[S37] C++：set
来源：http://iwi.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qvd.sweek.top

[S38] C++：排序
来源：http://nqk.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://res.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://fqw.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xmk.jiagoushi.top

[S40] C++：查找元素
来源：http://xiq.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xyn.epnwcf.com

[S41] C++：类与构造函数
来源：http://isi.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ekf.zycfv.cn

[S42] C++：继承与虚函数
来源：http://phw.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://eje.yueranfly.top

[S43] C++：智能指针
来源：http://gbq.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://myx.cashguo.top

[S44] C++：引用传参
来源：http://dnn.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://ytt.jyoumei.cn

[S45] C++：lambda
来源：http://uqp.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://kmd.c1oappe.top

[S46] C++：函数模板
来源：http://pso.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ijq.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://awi.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hye.guowangkeji.top

[S48] C++：逐行读文件
来源：http://zrg.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://xfw.bjfxy.top

while (std::getline(in, line)) { }
来源：http://soj.chenzaomai.com

[S49] C++：写文件
来源：http://fao.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://auo.yj202588.top

[S50] C++：格式化数字
来源：http://num.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hdy.daxiang520.top

[S51] C++：显式类型转换
来源：http://ysv.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://mfy.svipenyu.cn

[S52] C++：const 与 noexcept
来源：http://bms.bbcook.cn

int size() const noexcept { return n_; }
来源：http://nah.xuetiantiany.cn

[S53] C++：移动语义
来源：http://oon.yonumen.top

std::vector<int> w = std::move(v);
来源：http://dkl.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://hab.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://peg.svipenyu.cn

[S55] C++：结构化绑定
来源：http://iyq.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vcm.zhiwuduotai.top

[S56] C++：optional
来源：http://dym.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mpk.yfazqb.com

[S57] C++：编译期常量
来源：http://vpl.pengpengdd.cyou

constexpr int N = 10;
来源：http://hij.hcnkem.com

[S58] C++：命名空间
来源：http://xjg.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://wln.smart0.xyz

[S59] C++：静态断言
来源：http://mik.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dys.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://ypf.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://phc.iojbl.cn

================================================================================
来源：http://fne.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qah.chenlongwang.top

================================================================================
来源：http://czs.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://duc.jqgfzy.top

println("Hello")
来源：http://xur.shuidangran.top

[T02] Kotlin：变量
来源：http://mjz.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wtz.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://ymx.andypj.xyz

"值: $b"
来源：http://yea.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://tqg.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://ude.yj202588.top

[T05] Kotlin：when 表达式
来源：http://kpg.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kmy.52xcode.cn

[T06] Kotlin：集合映射
来源：http://uke.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://lbx.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://yrv.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nam.guannengcc.top

[T08] Kotlin：数据类
来源：http://gwb.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://kdy.yonumen.top

[T09] Kotlin：扩展函数
来源：http://txm.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://izj.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://rsv.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xoi.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://qzr.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://riq.hnqzz.top

[T12] Kotlin：解构声明
来源：http://nva.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://pkq.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://qki.yj20258.top

val m = mapOf("a" to 1)
来源：http://hxd.uphjek.com

[T14] Kotlin：循环
来源：http://wya.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://fah.quarkkingdee.top

[T15] Kotlin：接口
来源：http://xcu.fengsongda.top

interface Shape { fun area(): Double }
来源：http://tln.jinqigufen.top

[T16] Swift：Hello World
来源：http://wam.tianlin.xyz

print("Hello")
来源：http://ufl.shuidangran.top

[T17] Swift：变量与常量
来源：http://ozk.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://ifz.sweek.top

[T18] Swift：字符串插值
来源：http://fqx.ydjk.org.cn

"值: \(b)"
来源：http://akz.yvedp.cn

[T19] Swift：可选绑定
来源：http://nbu.fehbvm.com

if let n = opt { print(n) }
来源：http://hhd.chenlongwang.top

[T20] Swift：数组操作
来源：http://fid.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://wfy.mhx1999.top

[T21] Swift：遍历
来源：http://lft.smart0.xyz

for x in a { print(x) }
来源：http://amd.shangyingyoupin.top

[T22] Swift：字典
来源：http://qbc.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://uht.hesvh.cn

[T23] Swift：函数
来源：http://nwo.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vrl.yfazqb.com

[T24] Swift：闭包
来源：http://udg.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mil.cdnleiting.top

[T25] Swift：结构体
来源：http://gcr.xuanzx.com

struct P { var x: Int }
来源：http://hly.snrcjt.cn

[T26] Swift：类与重写
来源：http://ood.yangfankeji.com

class A: Base { override func f() {} }
来源：http://bcp.wangdashe.top

[T27] Swift：错误处理
来源：http://nhd.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://ojj.jqgfzy.top

[T28] Swift：枚举
来源：http://ziv.xinyue.icu

enum Color { case red, green }
来源：http://rfx.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://bez.ydjk.org.cn

guard let x = opt else { return }
来源：http://gxz.yuanzhike.top

[T30] Swift：协议
来源：http://tca.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://kfq.kuanghao11.cn

[T31] Lua：Hello World
来源：http://tgf.jinghuilouyu.cn

print("Hello")
来源：http://cps.fehbvm.com

[T32] Lua：局部变量
来源：http://hlt.xinyue.icu

local a = 1
来源：http://hka.jianghu66.top

[T33] Lua：表（数组）
来源：http://ihg.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ezg.iojbl.cn

[T34] Lua：遍历表
来源：http://seg.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uov.hfpthk.cn

[T35] Lua：字典表
来源：http://gpn.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://adr.zhiwuduotai.top

[T36] Lua：函数
来源：http://cdy.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://zsf.bjfxy.top

[T37] Lua：字符串拼接
来源：http://eyf.jinghuilouyu.cn

"a" .. "b"
来源：http://wjv.jqgufenzy.top

[T38] Lua：条件
来源：http://jqs.kuanghao11.cn

if x > 0 then print("正") end
来源：http://wmc.sjlbkw.cn

[T39] Lua：模式匹配
来源：http://gjk.jinqigufen.top

string.find(s, "%d+")
来源：http://oia.nanxuanxn.top

[T40] Lua：元表
来源：http://jof.bbcook.cn

setmetatable({}, { __index = base })
来源：http://nhz.sufxvd.cn

[T41] Perl：Hello World
来源：http://gsa.sufxvd.cn

print "Hello\n";
来源：http://pml.uphjek.com

[T42] Perl：变量类型
来源：http://djk.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ese.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://btb.svipenyu.cn

"值: $a"
来源：http://bph.9152youxi.cn

[T44] Perl：条件
来源：http://ctr.wangdashe.top

if ($a > 0) { print "正"; }
来源：http://iuq.haohaochexian.top

[T45] Perl：数组遍历
来源：http://fcr.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://ecy.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://cwi.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hbs.yueranfly.top

[T47] Perl：正则捕获
来源：http://ixz.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nnv.yongpay.top

[T48] Perl：正则替换
来源：http://hfp.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://upl.tianlin.xyz

[T49] Perl：函数
来源：http://kaz.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xcq.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://cwd.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hws.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://kgq.sxryk.cn

[T51] Scala：Hello World
来源：http://pcc.xuetiantiany.cn

println("Hello")
来源：http://ruw.nwbrower.top

[T52] Scala：变量
来源：http://xeq.hfpthk.cn

val a = 1;  var b = 2
来源：http://ymx.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://ixf.cdnleiting.top

s"值: $b"
来源：http://kse.zdqjudy.top

[T54] Scala：集合映射
来源：http://xoh.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://vah.gogol.net.cn

[T55] Scala：集合过滤
来源：http://btc.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://ssl.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://lby.gogol.net.cn

case class User(name: String, age: Int)
来源：http://ppj.chenlongwang.top

[T57] Scala：模式匹配
来源：http://vyv.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uix.bbcook.cn

[T58] Scala：函数定义
来源：http://xar.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://eda.sjlbkw.cn

[T59] Scala：循环
来源：http://phz.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://lav.svipenyu.cn

[T60] Scala：折叠
来源：http://ddh.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pry.nwbrower.top

================================================================================
来源：http://ojo.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mva.shzxlz.cn

================================================================================
来源：http://vkg.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://xbx.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://zbv.yj20258888.top

[U02] Py：导出 / 安装依赖
来源：http://ykr.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oah.tanke756.top

[U03] Py：加载 .env 配置
来源：http://fyc.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yqz.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://ybf.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vfb.aizwys.cn

[U05] Py：列表去重且保序
来源：http://shi.9152youxi.cn

list(dict.fromkeys(arr))
来源：http://bgs.ivvv.top

[U06] Py：合并两个字典
来源：http://fll.mhx1999.top

{**a, **b}
来源：http://vwv.52xcode.cn

[U07] Py：反转字典键值
来源：http://qam.dashuyun.cn

{v: k for k, v in d.items()}
来源：http://qgp.jiagoushi.top

[U08] Py：展平二维列表
来源：http://hmz.jlsjyb.cn

[y for x in nested for y in x]
来源：http://ngk.yangfankeji.com

[U09] Py：字典取最大值的键
来源：http://iep.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://wnv.meibo888.top

[U10] Py：按值排序字典
来源：http://bfk.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uga.0kj1m.cn

[U11] Py：生成器表达式
来源：http://sxc.redwolf501.top

(x * 2 for x in arr)
来源：http://tlx.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pcy.guowangkeji.top

Counter(arr).most_common(3)
来源：http://hfw.dashuyun.cn

[U13] Py：固定长度队列
来源：http://eso.cdnleiting.top

deque(maxlen=10)
来源：http://bgt.jyoumei.cn

[U14] Py：分组收集到列表
来源：http://ivu.feifeiyinyue.top

defaultdict(list)
来源：http://dah.zdbjq.cn

[U15] Py：高精度计时
来源：http://igr.mhx1999.top

t = time.perf_counter()
来源：http://xdn.yfazqb.com

[U16] Py：命令行参数解析
来源：http://nwq.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rwx.hywenlv.cn

[U17] Py：初始化日志
来源：http://lcy.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://ois.guannengcc.top

[U18] Py：预编译正则
来源：http://qnj.vqdsnc.cn

pat = re.compile(r"\d+")
来源：http://wst.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://gey.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dck.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://rym.iojbl.cn

@functools.lru_cache(maxsize=None)
来源：http://qww.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://uio.fengsongda.top

@contextlib.contextmanager
来源：http://zac.jyoumei.cn

[U22] Py：矩阵转置
来源：http://bix.kuanghao11.cn

list(zip(*m))
来源：http://bus.yvedp.cn

[U23] Py：分块读取大文件
来源：http://jks.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cce.daria6918.cn

[U24] Py：路径操作
来源：http://ove.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qiy.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://ydu.shanyushiyangtech.top

csv.DictReader(f)
来源：http://qej.hysaishi.cn

[U26] Py：并发下载
来源：http://ktl.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://evg.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://mce.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://exk.tarul.cn

[U28] Py：类型别名
来源：http://sjb.pengpengdd.cyou

UserId = int
来源：http://vni.andypj.xyz

[U29] Py：属性校验
来源：http://kyb.bjfxy.top

@property 与 @x.setter 配合
来源：http://cnk.pengpengdd.cyou

[U30] Py：数据类
来源：http://szn.redwolf501.top

@dataclass(slots=True)
来源：http://npd.zhaomingkeji.xyz

[U31] Py：单测
来源：http://qxf.316326.xyz

python -m pytest -q
来源：http://hct.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://tgo.zycfv.cn

ruff format . && ruff check --fix .
来源：http://zhp.yuanzhike.top

[U33] Py：打包发布
来源：http://czv.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://hhh.yfazqb.com

[U34] Py：判断编码
来源：http://kon.chenjidiqi.icu

chardet.detect(raw)
来源：http://cyy.c1oappe.top

[U35] Py：发送邮件
来源：http://sig.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bgq.chenlongwang.top

[U36] Py：定时任务
来源：http://mhh.jqgufenzy.top

schedule.every(10).minutes.do(job)
来源：http://deo.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://ltv.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gzx.fanxiaobao.xyz

[U38] Py：获取脚本所在目录
来源：http://hxb.jinqigfzy.top

Path(__file__).resolve().parent
来源：http://yiy.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://qiw.sufxvd.cn

sys.stdout.isatty()
来源：http://yny.yvedp.cn

[U40] Py：打印到标准错误
来源：http://sas.hfpthk.cn

print("err", file=sys.stderr)
来源：http://nsx.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://cdp.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fzj.hongshengwenyu.top

[U42] PHP：PSR-4 自动加载
来源：http://yut.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rey.yj202588.top

[U43] PHP：声明命名空间
来源：http://xbt.jqgfzy.top

namespace App\Http;
来源：http://dvo.c1oappe.top

[U44] PHP：开启严格类型
来源：http://onw.cdnleiting.top

declare(strict_types=1);
来源：http://hvl.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://ybx.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zml.guannengcc.top

[U46] PHP：可空类型
来源：http://vkz.hysaishi.cn

?string $name = null
来源：http://dpb.jinyuanbaomall.cn


<!-- 参考信息 -->