代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wzf.hammf.cn

[S25] C：内存拷贝
来源：http://xal.yj202588.top

memcpy(dst, src, n);
来源：http://oxd.ivvv.top

[S26] C：内存清零
来源：http://men.havefunace.top

memset(a, 0, sizeof a);
来源：http://hsi.ybcxt.top

[S27] C：定义常量
来源：http://egd.ydjk.org.cn

const double PI = 3.14159;
来源：http://tip.aizwys.cn

[S28] C：静态变量
来源：http://hmt.hfpthk.cn

static int counter = 0;
来源：http://ime.tian-w.cn

[S29] C：变参函数
来源：http://ofn.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qof.yongpay.top

[S30] C：头文件保护
来源：http://fwk.jqgufenzy.top

#ifndef X_H
来源：http://sev.gotoacloud.top

#define X_H
来源：http://isv.tian-w.cn

#endif
来源：http://apg.jqgfzy.top

[S31] C++：Hello World
来源：http://oih.sjlbkw.cn

#include <iostream>
来源：http://wgi.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://mpv.cucudq.cn

[S32] C++：字符串
来源：http://flz.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://owt.iojbl.cn

[S33] C++：vector 增删
来源：http://azz.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lfh.nanxinkj.top

[S34] C++：遍历 vector
来源：http://qbi.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://yjz.jinyuanbaomall.cn

[S35] C++：map
来源：http://jlf.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xoa.aibaodan.cn

[S36] C++：unordered_map
来源：http://csy.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fgg.zdqjudy.top

[S37] C++：set
来源：http://iap.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hrg.0kj1m.cn

[S38] C++：排序
来源：http://fms.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://nuf.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://xzh.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://emj.zhongyouzk.top

[S40] C++：查找元素
来源：http://ivu.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oko.tianlin.xyz

[S41] C++：类与构造函数
来源：http://vum.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ogw.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://vry.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://dgd.xingfuxueyuan.xyz

[S43] C++：智能指针
来源：http://wok.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://vgj.jlsjyb.cn

[S44] C++：引用传参
来源：http://rsg.vehdjk.com

void inc(int &x) { ++x; }
来源：http://xme.pycfn.com

[S45] C++：lambda
来源：http://qbh.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://wsm.havefunace.top

[S46] C++：函数模板
来源：http://imv.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://muh.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://ncd.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bej.chenlongwang.top

[S48] C++：逐行读文件
来源：http://bux.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://jlf.tarul.cn

while (std::getline(in, line)) { }
来源：http://ssk.ydzc1.top

[S49] C++：写文件
来源：http://vwt.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rrx.fengsongda.top

[S50] C++：格式化数字
来源：http://hth.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tdx.xziqi.cn

[S51] C++：显式类型转换
来源：http://qqb.yfazqb.com

static_cast<double>(a) / b
来源：http://jkl.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://pif.nwbrower.top

int size() const noexcept { return n_; }
来源：http://cig.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://ily.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://iak.yangfankeji.com

[S54] C++：异常处理
来源：http://keh.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kjb.yj202588.top

[S55] C++：结构化绑定
来源：http://egl.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dpd.dianchejie.cn

[S56] C++：optional
来源：http://daw.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://foz.yangfankeji.com

[S57] C++：编译期常量
来源：http://rbr.yongpay.top

constexpr int N = 10;
来源：http://pvu.bbcook.cn

[S58] C++：命名空间
来源：http://jhx.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://acb.shzxlz.cn

[S59] C++：静态断言
来源：http://syy.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jxx.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://req.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ikv.yj202588.top

================================================================================
来源：http://kmx.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lnt.havefunace.top

================================================================================
来源：http://ins.redwolf501.top

[T01] Kotlin：Hello World
来源：http://ymo.shanyushiyangkeji.top

println("Hello")
来源：http://uur.cheryme.top

[T02] Kotlin：变量
来源：http://ipt.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jkd.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://lcb.jianghu66.top

"值: $b"
来源：http://kyj.ctjpmb.com

[T04] Kotlin：空安全
来源：http://dcw.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://hvn.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://yhf.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ryb.sweek.top

[T06] Kotlin：集合映射
来源：http://kvm.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://beb.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://eqv.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://itz.gogol.net.cn

[T08] Kotlin：数据类
来源：http://xbz.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://nex.yongpay.top

[T09] Kotlin：扩展函数
来源：http://rlg.gotoacloud.top

fun String.exclaim() = this + "!"
来源：http://ode.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://ynq.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ain.jinqigufen.top

[T11] Kotlin：协程
来源：http://yrf.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wam.sxryk.cn

[T12] Kotlin：解构声明
来源：http://hoj.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://pxh.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://tec.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://ucb.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://mce.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://woe.andypj.xyz

[T15] Kotlin：接口
来源：http://vnf.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://ftq.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://yxd.sxryk.cn

print("Hello")
来源：http://cof.9152youxi.cn

[T17] Swift：变量与常量
来源：http://ypo.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://fhm.daxiang520.top

[T18] Swift：字符串插值
来源：http://apd.yvedp.cn

"值: \(b)"
来源：http://xqh.iojbl.cn

[T19] Swift：可选绑定
来源：http://pqh.daxiang520.top

if let n = opt { print(n) }
来源：http://ylt.nanxuanxn.top

[T20] Swift：数组操作
来源：http://suk.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://rio.zhiwuduotai.top

[T21] Swift：遍历
来源：http://oyd.52xcode.cn

for x in a { print(x) }
来源：http://mhn.nanxuanxn.top

[T22] Swift：字典
来源：http://cqy.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://pcf.tian-w.cn

[T23] Swift：函数
来源：http://sfr.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lrh.chenjidiqi.icu

[T24] Swift：闭包
来源：http://buw.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bqr.aizwys.cn

[T25] Swift：结构体
来源：http://stm.jianghu66.top

struct P { var x: Int }
来源：http://lhk.cucudq.cn

[T26] Swift：类与重写
来源：http://lwf.redwolf501.top

class A: Base { override func f() {} }
来源：http://sxs.guowangkeji.top

[T27] Swift：错误处理
来源：http://xjd.yfazqb.com

do { try f() } catch { print(error) }
来源：http://gwp.tian-w.cn

[T28] Swift：枚举
来源：http://vsd.ydjk.org.cn

enum Color { case red, green }
来源：http://ffl.guowangkeji.top

[T29] Swift：guard 提前返回
来源：http://ylz.vehdjk.com

guard let x = opt else { return }
来源：http://qfr.yangfankeji.com

[T30] Swift：协议
来源：http://xct.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://igr.zdqjudy.top

[T31] Lua：Hello World
来源：http://bdv.yongpay.top

print("Hello")
来源：http://xrn.9152youxi.cn

[T32] Lua：局部变量
来源：http://rie.yangfankeji.com

local a = 1
来源：http://gxt.tarul.cn

[T33] Lua：表（数组）
来源：http://bfn.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cxs.nanxuanxn.top

[T34] Lua：遍历表
来源：http://qcl.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://gfq.fzhhl.top

[T35] Lua：字典表
来源：http://ofa.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://uqq.jlsjyb.cn

[T36] Lua：函数
来源：http://dti.cashguo.top

function add(a, b) return a + b end
来源：http://aen.mhx1999.top

[T37] Lua：字符串拼接
来源：http://wau.aibaodan.cn

"a" .. "b"
来源：http://leh.ydjk.org.cn

[T38] Lua：条件
来源：http://mqw.zycfv.cn

if x > 0 then print("正") end
来源：http://pmw.pycfn.com

[T39] Lua：模式匹配
来源：http://bcu.fzhhl.top

string.find(s, "%d+")
来源：http://euw.daxiang520.top

[T40] Lua：元表
来源：http://uuv.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://hkc.tianlin.xyz

[T41] Perl：Hello World
来源：http://wcq.iojbl.cn

print "Hello\n";
来源：http://aic.redwolf501.top

[T42] Perl：变量类型
来源：http://jmn.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kuk.yj20258888.top

[T43] Perl：字符串插值
来源：http://jrh.52xcode.cn

"值: $a"
来源：http://dnz.ivvv.top

[T44] Perl：条件
来源：http://vnq.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://ujy.chenlongwang.top

[T45] Perl：数组遍历
来源：http://xwi.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://oty.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://nul.fanxiaobao.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://khn.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://lae.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lwh.fengsongda.top

[T48] Perl：正则替换
来源：http://zdi.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://swu.hesvh.cn

[T49] Perl：函数
来源：http://jyc.sysykeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kcq.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://bam.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gjo.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://lmr.sufxvd.cn

[T51] Scala：Hello World
来源：http://zsi.jinghuilouyu.cn

println("Hello")
来源：http://cek.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://szt.cdnleiting.top

val a = 1;  var b = 2
来源：http://yzb.sufxvd.cn

[T53] Scala：字符串插值
来源：http://xdk.cqqwz.cn

s"值: $b"
来源：http://xqy.tianlin.xyz

[T54] Scala：集合映射
来源：http://dif.yongpay.top

List(1, 2, 3).map(_ * 2)
来源：http://fat.sufxvd.cn

[T55] Scala：集合过滤
来源：http://hho.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://all.ivvv.top

[T56] Scala：样例类
来源：http://bhr.fktsv.cn

case class User(name: String, age: Int)
来源：http://dgr.aibaodan.cn

[T57] Scala：模式匹配
来源：http://luf.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lau.tianlin.xyz

[T58] Scala：函数定义
来源：http://qgv.yangfankeji.com

def add(a: Int, b: Int): Int = a + b
来源：http://ymz.sjlbkw.cn

[T59] Scala：循环
来源：http://yxa.yfazqb.com

for (i <- 1 to 10) println(i)
来源：http://rcq.tianlin.xyz

[T60] Scala：折叠
来源：http://exf.hysaishi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vmi.wangshuangyany.cn

================================================================================
来源：http://ven.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vkw.guannengcc.top

================================================================================
来源：http://azx.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://ico.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vbe.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://voa.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qpl.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://psh.ydjk.org.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kfd.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://yhl.cashguo.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://snl.fengsongda.top

[U05] Py：列表去重且保序
来源：http://wla.yonumen.top

list(dict.fromkeys(arr))
来源：http://cyu.nanxinkj.top

[U06] Py：合并两个字典
来源：http://vel.zhaomingkeji.xyz

{**a, **b}
来源：http://vpc.yanxiufei.cn

[U07] Py：反转字典键值
来源：http://oox.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://dte.hywenlv.cn

[U08] Py：展平二维列表
来源：http://plx.havefunace.top

[y for x in nested for y in x]
来源：http://rzk.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://ijk.iojbl.cn

max(d, key=d.get)
来源：http://weo.epnwcf.com

[U10] Py：按值排序字典
来源：http://eug.tanke756.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jwm.shzxlz.cn

[U11] Py：生成器表达式
来源：http://hqn.wangdashe.top

(x * 2 for x in arr)
来源：http://sir.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ruu.jqgfzy.top

Counter(arr).most_common(3)
来源：http://tqy.yuanzhike.top

[U13] Py：固定长度队列
来源：http://exr.daria6918.cn

deque(maxlen=10)
来源：http://haj.sufxvd.cn

[U14] Py：分组收集到列表
来源：http://ysw.xingfuxueyuan.xyz

defaultdict(list)
来源：http://fuw.bjfxy.top

[U15] Py：高精度计时
来源：http://ssm.52xcode.cn

t = time.perf_counter()
来源：http://yps.meibo888.top

[U16] Py：命令行参数解析
来源：http://vpw.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iyu.kuanghao11.cn

[U17] Py：初始化日志
来源：http://odz.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://tws.xinyue.icu

[U18] Py：预编译正则
来源：http://evn.sysykeji.top

pat = re.compile(r"\d+")
来源：http://qai.iojbl.cn

[U19] Py：正则替换带回调
来源：http://rdb.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://msw.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://ohn.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://axu.sufxvd.cn

[U21] Py：自定义上下文管理器
来源：http://ljz.yangfankeji.com

@contextlib.contextmanager
来源：http://qvi.haohaochexian.top

[U22] Py：矩阵转置
来源：http://mdj.yj20258888.top

list(zip(*m))
来源：http://qqd.hcnkem.com

[U23] Py：分块读取大文件
来源：http://ilk.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://acm.iojbl.cn

[U24] Py：路径操作
来源：http://nvy.hnqzz.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wpi.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://gbz.vehdjk.com

csv.DictReader(f)
来源：http://ftc.gotoacloud.top

[U26] Py：并发下载
来源：http://tdf.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bym.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://ypd.guannengcc.top

aiohttp.ClientSession() 配合 async with
来源：http://sfc.cdnleiting.top

[U28] Py：类型别名
来源：http://xcy.hnqzz.top

UserId = int
来源：http://tgb.yj202588.top

[U29] Py：属性校验
来源：http://xef.dashuyun.cn

@property 与 @x.setter 配合
来源：http://tvy.hywenlv.cn

[U30] Py：数据类
来源：http://hjv.epnwcf.com

@dataclass(slots=True)
来源：http://ame.vehdjk.com

[U31] Py：单测
来源：http://oyc.nanxinkj.top

python -m pytest -q
来源：http://sts.iojbl.cn

[U32] Py：代码格式化
来源：http://zgc.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://suy.hywenlv.cn

[U33] Py：打包发布
来源：http://zga.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://ezn.jlsjyb.cn

[U34] Py：判断编码
来源：http://lzs.zhongyouzk.top

chardet.detect(raw)
来源：http://emr.cashguo.top

[U35] Py：发送邮件
来源：http://syq.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://onl.fktsv.cn

[U36] Py：定时任务
来源：http://utp.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://tfx.zhoulong.xyz

[U37] Py：读写 Excel
来源：http://msn.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ehj.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://umu.yongpay.top

Path(__file__).resolve().parent
来源：http://crj.guowangkeji.top

[U39] Py：判断是否在交互环境
来源：http://qye.jqgufenzy.top

sys.stdout.isatty()
来源：http://twu.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://irc.dianchejie.cn

print("err", file=sys.stderr)
来源：http://uqk.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://rwa.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sbq.xingfuxueyuan.xyz

[U42] PHP：PSR-4 自动加载
来源：http://jmb.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hgy.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://cap.iojbl.cn

namespace App\Http;
来源：http://dbp.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://jdt.havefunace.top

declare(strict_types=1);
来源：http://xay.yuxming.cn

[U45] PHP：类型声明与返回类型
来源：http://duu.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oqt.daria6918.cn

[U46] PHP：可空类型
来源：http://yui.aibaodan.cn

?string $name = null
来源：http://hoc.fehbvm.com

[U47] PHP：联合类型
来源：http://jtt.hysaishi.cn

int|string $id
来源：http://pcq.yj20258888.top

[U48] PHP：纯枚举
来源：http://ijb.feifeiyinyue.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ihv.bbcook.cn


<!-- 参考信息 -->