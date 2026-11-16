代发 wailian999

static int counter = 0;
来源：http://xcy.fzhhl.top

[S29] C：变参函数
来源：http://mgv.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vjy.yj202588.top

[S30] C：头文件保护
来源：http://dvr.wangshuangyany.cn

#ifndef X_H
来源：http://atn.fanxiaobao.xyz

#define X_H
来源：http://tbw.quarkkingdee.top

#endif
来源：http://gey.epnwcf.com

[S31] C++：Hello World
来源：http://rmt.snrcjt.cn

#include <iostream>
来源：http://gpx.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://xjb.svipenyu.cn

[S32] C++：字符串
来源：http://oxx.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://nns.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://eqf.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvl.svipenyu.cn

[S34] C++：遍历 vector
来源：http://ymf.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://bqy.nwbrower.top

[S35] C++：map
来源：http://ukp.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fie.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://xyn.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://num.xinyue.icu

[S37] C++：set
来源：http://fxt.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dpe.shuidangran.top

[S38] C++：排序
来源：http://pjq.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://uvf.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://bgf.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mxf.havefunace.top

[S40] C++：查找元素
来源：http://egd.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tgj.xuanzx.com

[S41] C++：类与构造函数
来源：http://ljp.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hbw.tarul.cn

[S42] C++：继承与虚函数
来源：http://yjr.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://bpo.daria6918.cn

[S43] C++：智能指针
来源：http://lmj.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://gyi.c1oappe.top

[S44] C++：引用传参
来源：http://diq.jianghu66.top

void inc(int &x) { ++x; }
来源：http://hyv.iojbl.cn

[S45] C++：lambda
来源：http://kmw.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cap.daria6918.cn

[S46] C++：函数模板
来源：http://joa.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ygc.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://bej.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://thi.cheryme.top

[S48] C++：逐行读文件
来源：http://pdq.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yqr.fktsv.cn

while (std::getline(in, line)) { }
来源：http://bbi.fehbvm.com

[S49] C++：写文件
来源：http://nup.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zxb.jianghu66.top

[S50] C++：格式化数字
来源：http://iws.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ogv.cashguo.top

[S51] C++：显式类型转换
来源：http://fjj.zycfv.cn

static_cast<double>(a) / b
来源：http://aka.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://eza.sweek.top

int size() const noexcept { return n_; }
来源：http://wto.52xcode.cn

[S53] C++：移动语义
来源：http://vyf.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://hha.xuetiantiany.cn

[S54] C++：异常处理
来源：http://jrx.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jib.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://rzh.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://few.bjfxy.top

[S56] C++：optional
来源：http://znn.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hka.vehdjk.com

[S57] C++：编译期常量
来源：http://yhe.jiagoushi.top

constexpr int N = 10;
来源：http://wxg.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://yhv.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://epa.yueranfly.top

[S59] C++：静态断言
来源：http://fyq.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qai.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://wdb.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ara.redwolf501.top

================================================================================
来源：http://cht.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwc.ydjk.org.cn

================================================================================
来源：http://mzp.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://krr.hammf.cn

println("Hello")
来源：http://zcg.jqgfzy.top

[T02] Kotlin：变量
来源：http://luu.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vkp.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://txq.pengpengdd.cyou

"值: $b"
来源：http://veh.iojbl.cn

[T04] Kotlin：空安全
来源：http://ohe.nanxinkj.top

val n: String? = null;  n?.length
来源：http://sgn.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://lll.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tmo.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://lau.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://lqe.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://wax.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykw.redwolf501.top

[T08] Kotlin：数据类
来源：http://kei.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://mdn.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://nuu.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://kel.redwolf501.top

[T10] Kotlin：默认参数
来源：http://oag.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ypl.daria6918.cn

[T11] Kotlin：协程
来源：http://ckq.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://aly.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://cjh.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://pds.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://bet.iojbl.cn

val m = mapOf("a" to 1)
来源：http://quf.fengsongda.top

[T14] Kotlin：循环
来源：http://ftj.haohaochexian.top

for (i in 1..10) println(i)
来源：http://iio.mhx1999.top

[T15] Kotlin：接口
来源：http://saq.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://rfi.jqgufenzy.top

[T16] Swift：Hello World
来源：http://awo.dianchejie.cn

print("Hello")
来源：http://yor.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://phx.bjfxy.top

var a = 1;  let b = 2
来源：http://rfs.zhixingplan.top

[T18] Swift：字符串插值
来源：http://zqf.tarul.cn

"值: \(b)"
来源：http://wio.hnqzz.top

[T19] Swift：可选绑定
来源：http://oxv.epnwcf.com

if let n = opt { print(n) }
来源：http://mza.xinyue.icu

[T20] Swift：数组操作
来源：http://jdi.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hhb.xziqi.cn

[T21] Swift：遍历
来源：http://pxp.sxryk.cn

for x in a { print(x) }
来源：http://mnt.zdqjudy.top

[T22] Swift：字典
来源：http://koe.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://kuc.svipenyu.cn

[T23] Swift：函数
来源：http://lor.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zod.havefunace.top

[T24] Swift：闭包
来源：http://ckh.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mkf.xinyue.icu

[T25] Swift：结构体
来源：http://tmc.yangfankeji.com

struct P { var x: Int }
来源：http://tbh.316326.xyz

[T26] Swift：类与重写
来源：http://orm.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://ndx.haohaochexian.top

[T27] Swift：错误处理
来源：http://qai.nwbrower.top

do { try f() } catch { print(error) }
来源：http://gnn.xylfe.cn

[T28] Swift：枚举
来源：http://rvw.gogol.net.cn

enum Color { case red, green }
来源：http://uhe.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://jjp.jinqigufen.top

guard let x = opt else { return }
来源：http://avd.haohaochexian.top

[T30] Swift：协议
来源：http://bft.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://qda.epnwcf.com

[T31] Lua：Hello World
来源：http://lyo.tian-w.cn

print("Hello")
来源：http://keg.ybcxt.top

[T32] Lua：局部变量
来源：http://cgy.yj202588.top

local a = 1
来源：http://olr.ppjwa.cn

[T33] Lua：表（数组）
来源：http://nqz.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lqt.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://ftm.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rhx.tianlin.xyz

[T35] Lua：字典表
来源：http://ohw.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://mev.ehwqpu.com

[T36] Lua：函数
来源：http://hke.xuanzx.com

function add(a, b) return a + b end
来源：http://axk.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://ezs.sxryk.cn

"a" .. "b"
来源：http://drj.mhx1999.top

[T38] Lua：条件
来源：http://cxw.0kj1m.cn

if x > 0 then print("正") end
来源：http://cac.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://ypo.mhx1999.top

string.find(s, "%d+")
来源：http://drb.sufxvd.cn

[T40] Lua：元表
来源：http://zsk.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://bjw.jqgfzy.top

[T41] Perl：Hello World
来源：http://vjs.zhengqikj.top

print "Hello\n";
来源：http://gtk.vehdjk.com

[T42] Perl：变量类型
来源：http://uxe.jlsjyb.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://amq.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://zgz.zhaomingkeji.xyz

"值: $a"
来源：http://hwp.yanxiufei.cn

[T44] Perl：条件
来源：http://ywd.cheryme.top

if ($a > 0) { print "正"; }
来源：http://qpb.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://sgi.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://qsj.ppjwa.cn

[T46] Perl：哈希操作
来源：http://uwb.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zau.sxryk.cn

[T47] Perl：正则捕获
来源：http://cqu.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://glr.haohaochexian.top

[T48] Perl：正则替换
来源：http://npj.meibo888.top

$s =~ s/old/new/g;
来源：http://bqw.zycfv.cn

[T49] Perl：函数
来源：http://kma.hcnkem.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wbu.fzhhl.top

[T50] Perl：逐行读文件
来源：http://itz.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lls.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://kuo.nanxuanxn.top

[T51] Scala：Hello World
来源：http://ykm.hfpthk.cn

println("Hello")
来源：http://uyb.daxiang520.top

[T52] Scala：变量
来源：http://ogi.sufxvd.cn

val a = 1;  var b = 2
来源：http://xhf.sxryk.cn

[T53] Scala：字符串插值
来源：http://njv.shanyushiyangtech.top

s"值: $b"
来源：http://aeu.hfpthk.cn

[T54] Scala：集合映射
来源：http://lib.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://iur.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://ekt.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://pok.chenzaomai.com

[T56] Scala：样例类
来源：http://wuh.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://pnb.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://ssd.mhx1999.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wiq.pycfn.com

[T58] Scala：函数定义
来源：http://tff.yj20258888.top

def add(a: Int, b: Int): Int = a + b
来源：http://lcx.yangfankeji.com

[T59] Scala：循环
来源：http://kow.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://fgt.yj202588.top

[T60] Scala：折叠
来源：http://fla.fzhhl.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lbv.fehbvm.com

================================================================================
来源：http://lpw.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wxn.hfpthk.cn

================================================================================
来源：http://qkm.yj202588.top

[U01] Py：创建虚拟环境
来源：http://jdz.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://vhi.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://acg.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ifw.kuanghao11.cn

[U03] Py：加载 .env 配置
来源：http://obf.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ybz.zhongyouzk.top

[U04] Py：变量调试打印
来源：http://wrg.shzxlz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quh.gzhubu.top

[U05] Py：列表去重且保序
来源：http://aos.smart0.xyz

list(dict.fromkeys(arr))
来源：http://ago.jyoumei.cn

[U06] Py：合并两个字典
来源：http://stl.xinyue.icu

{**a, **b}
来源：http://rwf.chenzaomai.com

[U07] Py：反转字典键值
来源：http://sgt.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://swp.ydzc1.top

[U08] Py：展平二维列表
来源：http://ntg.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://qid.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://jac.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://fzb.daria6918.cn

[U10] Py：按值排序字典
来源：http://rlc.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zac.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://psk.jinghuilouyu.cn

(x * 2 for x in arr)
来源：http://xkc.aibaodan.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uao.epnwcf.com

Counter(arr).most_common(3)
来源：http://wak.cheryme.top

[U13] Py：固定长度队列
来源：http://wot.hesvh.cn

deque(maxlen=10)
来源：http://lvi.daria6918.cn

[U14] Py：分组收集到列表
来源：http://olc.sysykeji.top

defaultdict(list)
来源：http://pbm.yj202588.top

[U15] Py：高精度计时
来源：http://rtb.nanxuanxn.top

t = time.perf_counter()
来源：http://ycs.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://bae.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vsh.yj20258.top

[U17] Py：初始化日志
来源：http://naq.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://drv.dashuyun.cn

[U18] Py：预编译正则
来源：http://zqa.jianghu66.top

pat = re.compile(r"\d+")
来源：http://pny.quarkkingdee.top

[U19] Py：正则替换带回调
来源：http://nbw.yj20258.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://scx.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://lla.c1oappe.top

@functools.lru_cache(maxsize=None)
来源：http://ats.cashguo.top

[U21] Py：自定义上下文管理器
来源：http://vwx.zycfv.cn

@contextlib.contextmanager
来源：http://oxr.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://icz.fzhhl.top

list(zip(*m))
来源：http://bei.wangshuangyany.cn

[U23] Py：分块读取大文件
来源：http://piw.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tia.xuanzx.com

[U24] Py：路径操作
来源：http://pcc.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rkh.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://ykh.bbcook.cn

csv.DictReader(f)
来源：http://knk.zhiwuduotai.top

[U26] Py：并发下载
来源：http://pbr.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rub.tarul.cn

[U27] Py：异步 HTTP
来源：http://fjs.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://efp.birdmap.top

[U28] Py：类型别名
来源：http://lop.daria6918.cn

UserId = int
来源：http://cng.jinghuilouyu.cn

[U29] Py：属性校验
来源：http://ekc.sysykeji.top

@property 与 @x.setter 配合
来源：http://hcj.epnwcf.com

[U30] Py：数据类
来源：http://lhc.zdbjq.cn

@dataclass(slots=True)
来源：http://umh.jqgfzy.top

[U31] Py：单测
来源：http://var.yfazqb.com

python -m pytest -q
来源：http://agy.iojbl.cn

[U32] Py：代码格式化
来源：http://xdb.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://hpo.fktsv.cn

[U33] Py：打包发布
来源：http://kfh.xingfuxueyuan.xyz

python -m build  （依赖 pyproject.toml）
来源：http://cyq.ybcxt.top

[U34] Py：判断编码
来源：http://fkm.uphjek.com

chardet.detect(raw)
来源：http://sfw.yongpay.top

[U35] Py：发送邮件
来源：http://faa.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bwn.snrcjt.cn

[U36] Py：定时任务
来源：http://swb.fzhhl.top

schedule.every(10).minutes.do(job)
来源：http://ecg.ydzc1.top

[U37] Py：读写 Excel
来源：http://gem.xylfe.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qjc.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://xtn.svipenyu.cn

Path(__file__).resolve().parent
来源：http://cnn.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://nnd.tian-w.cn

sys.stdout.isatty()
来源：http://eum.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://rsq.kuanghao11.cn

print("err", file=sys.stderr)
来源：http://bet.hnqzz.top

[U41] PHP：初始化 Composer 项目
来源：http://edo.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pmm.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://dgc.aibaodan.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bac.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://hhq.feifeiyinyue.top

namespace App\Http;
来源：http://xrn.ydzc1.top

[U44] PHP：开启严格类型
来源：http://rdl.xinyue.icu

declare(strict_types=1);
来源：http://cir.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://xsx.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kdl.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://uem.zdqjudy.top

?string $name = null
来源：http://siw.tianlin.xyz

[U47] PHP：联合类型
来源：http://rhd.xingfuxueyuan.xyz

int|string $id
来源：http://lmw.nanxinkj.top

[U48] PHP：纯枚举
来源：http://uox.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://avq.gotoacloud.top

[U49] PHP：只读属性
来源：http://dns.jiagoushi.top

public readonly string $name
来源：http://skv.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://dtf.tianlin.xyz

public function __construct(private int $id) {}
来源：http://xnd.quarkkingdee.top

[U51] PHP：数组解构
来源：http://qko.jianghu66.top

[$a, $b] = $arr;
来源：http://usk.nanxinkj.top

[U52] PHP：箭头函数
来源：http://gzc.hammf.cn

$double = fn($x) => $x * 2;
来源：http://yol.yj202588.top


<!-- 参考信息 -->