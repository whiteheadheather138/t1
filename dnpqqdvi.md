代发 wailian999

static int counter = 0;
来源：http://ihi.zhengqikj.top

[S29] C：变参函数
来源：http://uif.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://osp.0kj1m.cn

[S30] C：头文件保护
来源：http://ylb.hcnkem.com

#ifndef X_H
来源：http://kcy.hysaishi.cn

#define X_H
来源：http://iib.zhijiandao.cn

#endif
来源：http://hkh.pycfn.com

[S31] C++：Hello World
来源：http://udl.zycfv.cn

#include <iostream>
来源：http://xdz.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://ceo.shuidangran.top

[S32] C++：字符串
来源：http://gtv.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://mwz.jqgufenzy.top

[S33] C++：vector 增删
来源：http://ciz.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://adm.cheryme.top

[S34] C++：遍历 vector
来源：http://loc.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://jeq.nanxinkj.top

[S35] C++：map
来源：http://esa.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://csk.andypj.xyz

[S36] C++：unordered_map
来源：http://qmz.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsj.smart0.xyz

[S37] C++：set
来源：http://aoz.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dlx.nwbrower.top

[S38] C++：排序
来源：http://yuz.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://eht.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://hvb.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://flc.jyoumei.cn

[S40] C++：查找元素
来源：http://iuq.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fpn.yj202588.top

[S41] C++：类与构造函数
来源：http://ytg.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ptb.guannengcc.top

[S42] C++：继承与虚函数
来源：http://ryl.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://yft.yueranfly.top

[S43] C++：智能指针
来源：http://jwu.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://dxs.gzhubu.top

[S44] C++：引用传参
来源：http://wrr.ydzc1.top

void inc(int &x) { ++x; }
来源：http://gug.ehwqpu.com

[S45] C++：lambda
来源：http://lvn.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bpl.chenjidiqi.icu

[S46] C++：函数模板
来源：http://cdr.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ely.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://xjg.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bcb.sxryk.cn

[S48] C++：逐行读文件
来源：http://xxa.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ksc.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://okc.fehbvm.com

[S49] C++：写文件
来源：http://qfc.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://swc.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://eyy.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aau.havefunace.top

[S51] C++：显式类型转换
来源：http://ikn.mhx1999.top

static_cast<double>(a) / b
来源：http://khi.ivvv.top

[S52] C++：const 与 noexcept
来源：http://fdt.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://kkp.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://hti.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://jcw.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://phh.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fco.aizwys.cn

[S55] C++：结构化绑定
来源：http://ode.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hso.tarul.cn

[S56] C++：optional
来源：http://tgy.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eiy.sufxvd.cn

[S57] C++：编译期常量
来源：http://mwn.c1oappe.top

constexpr int N = 10;
来源：http://sge.xylfe.cn

[S58] C++：命名空间
来源：http://arq.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://vzm.xuetiantiany.cn

[S59] C++：静态断言
来源：http://ilv.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lao.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://huu.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://own.sxryk.cn

================================================================================
来源：http://jzx.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fyq.yfazqb.com

================================================================================
来源：http://jse.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://lkx.epnwcf.com

println("Hello")
来源：http://gci.jlsjyb.cn

[T02] Kotlin：变量
来源：http://rjq.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ftk.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://box.yj20258.top

"值: $b"
来源：http://qlr.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://lhg.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://eoc.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://iix.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wfr.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://nqt.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qkg.yj20258.top

[T07] Kotlin：集合过滤
来源：http://qva.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wrh.0kj1m.cn

[T08] Kotlin：数据类
来源：http://eqv.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://jby.epnwcf.com

[T09] Kotlin：扩展函数
来源：http://uwc.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://jry.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://brc.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nzy.chenzaomai.com

[T11] Kotlin：协程
来源：http://swy.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pit.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://oce.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://uvw.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://ryy.sysykeji.top

val m = mapOf("a" to 1)
来源：http://whm.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://mha.bbcook.cn

for (i in 1..10) println(i)
来源：http://pzi.tianlin.xyz

[T15] Kotlin：接口
来源：http://lkj.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://vat.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://dwi.quarkkingdee.top

print("Hello")
来源：http://jid.ydzc1.top

[T17] Swift：变量与常量
来源：http://iqa.kuanghao11.cn

var a = 1;  let b = 2
来源：http://sad.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://hvp.jyoumei.cn

"值: \(b)"
来源：http://xvi.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://dlh.iojbl.cn

if let n = opt { print(n) }
来源：http://bhh.pycfn.com

[T20] Swift：数组操作
来源：http://pkg.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://rvj.zhixingplan.top

[T21] Swift：遍历
来源：http://nka.ctjpmb.com

for x in a { print(x) }
来源：http://ajh.pycfn.com

[T22] Swift：字典
来源：http://sxa.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://tjo.shzxlz.cn

[T23] Swift：函数
来源：http://dnt.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fdr.aizwys.cn

[T24] Swift：闭包
来源：http://int.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://dqa.hammf.cn

[T25] Swift：结构体
来源：http://ahq.cucudq.cn

struct P { var x: Int }
来源：http://udj.ivvv.top

[T26] Swift：类与重写
来源：http://ioj.yj20258.top

class A: Base { override func f() {} }
来源：http://zjy.cheryme.top

[T27] Swift：错误处理
来源：http://ayu.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://wwl.jlsjyb.cn

[T28] Swift：枚举
来源：http://ugt.snrcjt.cn

enum Color { case red, green }
来源：http://jhf.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://rqq.ybcxt.top

guard let x = opt else { return }
来源：http://hdu.vehdjk.com

[T30] Swift：协议
来源：http://yat.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://ogv.snrcjt.cn

[T31] Lua：Hello World
来源：http://joz.meibo888.top

print("Hello")
来源：http://hvt.zhengqikj.top

[T32] Lua：局部变量
来源：http://ark.gaohongyu789.top

local a = 1
来源：http://nhf.yj20258.top

[T33] Lua：表（数组）
来源：http://rkx.birdmap.top

local t = {1, 2, 3};  t[4] = 4
来源：http://omy.vqdsnc.cn

[T34] Lua：遍历表
来源：http://len.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uec.zdbjq.cn

[T35] Lua：字典表
来源：http://ijk.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://eod.zhongyouzk.top

[T36] Lua：函数
来源：http://hqj.shzxlz.cn

function add(a, b) return a + b end
来源：http://xzc.dianchejie.cn

[T37] Lua：字符串拼接
来源：http://rqi.snrcjt.cn

"a" .. "b"
来源：http://xlg.feifeiyinyue.top

[T38] Lua：条件
来源：http://knk.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://dxf.zdbjq.cn

[T39] Lua：模式匹配
来源：http://uiy.jinqigfzy.top

string.find(s, "%d+")
来源：http://qpz.zhixingplan.top

[T40] Lua：元表
来源：http://qyl.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://nch.0kj1m.cn

[T41] Perl：Hello World
来源：http://aji.yonumen.top

print "Hello\n";
来源：http://xyi.sjlbkw.cn

[T42] Perl：变量类型
来源：http://mop.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gbx.ybcxt.top

[T43] Perl：字符串插值
来源：http://pxt.vqdsnc.cn

"值: $a"
来源：http://ndo.zhiwuduotai.top

[T44] Perl：条件
来源：http://uod.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://ojq.bjfxy.top

[T45] Perl：数组遍历
来源：http://txf.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://upc.nwbrower.top

[T46] Perl：哈希操作
来源：http://dyr.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rbe.xinyue.icu

[T47] Perl：正则捕获
来源：http://oge.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://onx.gzhubu.top

[T48] Perl：正则替换
来源：http://dsw.zhengqikj.top

$s =~ s/old/new/g;
来源：http://bbi.fengsongda.top

[T49] Perl：函数
来源：http://ncl.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gyr.birdmap.top

[T50] Perl：逐行读文件
来源：http://tav.ydjk.org.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kfn.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://zkt.c1oappe.top

[T51] Scala：Hello World
来源：http://vzh.yvedp.cn

println("Hello")
来源：http://umh.jianghu66.top

[T52] Scala：变量
来源：http://ejb.aibaodan.cn

val a = 1;  var b = 2
来源：http://vek.tarul.cn

[T53] Scala：字符串插值
来源：http://sep.fehbvm.com

s"值: $b"
来源：http://wph.dianchejie.cn

[T54] Scala：集合映射
来源：http://uti.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://kpz.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://zzz.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://mxn.wangdashe.top

[T56] Scala：样例类
来源：http://btq.jqgfzy.top

case class User(name: String, age: Int)
来源：http://hnr.yonumen.top

[T57] Scala：模式匹配
来源：http://iwc.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mio.mhx1999.top

[T58] Scala：函数定义
来源：http://rph.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://ymd.jinqigufen.top

[T59] Scala：循环
来源：http://cqn.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://ine.sysykeji.top

[T60] Scala：折叠
来源：http://xbo.hcnkem.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jvj.zhiwuduotai.top

================================================================================
来源：http://pom.tian-w.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ntt.jiagoushi.top

================================================================================
来源：http://uqh.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://yqj.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://bpd.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://oit.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bqu.yj202588.top

[U03] Py：加载 .env 配置
来源：http://xtd.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://kdb.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://foq.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ifg.jqgufenzy.top

[U05] Py：列表去重且保序
来源：http://mqg.uphjek.com

list(dict.fromkeys(arr))
来源：http://nne.sxryk.cn

[U06] Py：合并两个字典
来源：http://ona.ywan-chungtsiang.top

{**a, **b}
来源：http://cnw.xylfe.cn

[U07] Py：反转字典键值
来源：http://vbt.sweek.top

{v: k for k, v in d.items()}
来源：http://yas.yj20258.top

[U08] Py：展平二维列表
来源：http://xii.jinqigfzy.top

[y for x in nested for y in x]
来源：http://yra.hysaishi.cn

[U09] Py：字典取最大值的键
来源：http://nsu.bjfxy.top

max(d, key=d.get)
来源：http://ech.nanxinkj.top

[U10] Py：按值排序字典
来源：http://nbx.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ozg.hywenlv.cn

[U11] Py：生成器表达式
来源：http://rrf.daxiang520.top

(x * 2 for x in arr)
来源：http://urs.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cdk.nwbrower.top

Counter(arr).most_common(3)
来源：http://axo.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://zmy.iojbl.cn

deque(maxlen=10)
来源：http://vjt.meibo888.top

[U14] Py：分组收集到列表
来源：http://iex.chenzaomai.com

defaultdict(list)
来源：http://oub.zycfv.cn

[U15] Py：高精度计时
来源：http://llv.jqgufenzy.top

t = time.perf_counter()
来源：http://xpe.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://xsu.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kpt.mhx1999.top

[U17] Py：初始化日志
来源：http://cpf.zdqjudy.top

logging.basicConfig(level=logging.INFO)
来源：http://ver.redwolf501.top

[U18] Py：预编译正则
来源：http://cpl.sweek.top

pat = re.compile(r"\d+")
来源：http://vrl.fanxiaobao.xyz

[U19] Py：正则替换带回调
来源：http://oqi.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mib.jyoumei.cn

[U20] Py：缓存函数结果
来源：http://izi.cucudq.cn

@functools.lru_cache(maxsize=None)
来源：http://mil.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://txn.iojbl.cn

@contextlib.contextmanager
来源：http://pqk.hongshengwenyu.top

[U22] Py：矩阵转置
来源：http://wsp.epnwcf.com

list(zip(*m))
来源：http://diw.jqgufenzy.top

[U23] Py：分块读取大文件
来源：http://pnh.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eri.cdnleiting.top

[U24] Py：路径操作
来源：http://wzw.sjlbkw.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bcy.9152youxi.cn

[U25] Py：CSV 按字典读
来源：http://oly.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://cvv.iojbl.cn

[U26] Py：并发下载
来源：http://sez.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rnc.uphjek.com

[U27] Py：异步 HTTP
来源：http://tql.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://fuk.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://tob.zdqjudy.top

UserId = int
来源：http://fbp.bjfxy.top

[U29] Py：属性校验
来源：http://iyl.xinyue.icu

@property 与 @x.setter 配合
来源：http://xod.gaohongyu789.top

[U30] Py：数据类
来源：http://qaz.shangyingyoupin.top

@dataclass(slots=True)
来源：http://chg.ivvv.top

[U31] Py：单测
来源：http://pvn.wangdashe.top

python -m pytest -q
来源：http://xzs.xylfe.cn

[U32] Py：代码格式化
来源：http://lfm.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://ejl.sufxvd.cn

[U33] Py：打包发布
来源：http://kfi.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://dzv.dianchejie.cn

[U34] Py：判断编码
来源：http://obe.yongpay.top

chardet.detect(raw)
来源：http://ywe.jiagoushi.top

[U35] Py：发送邮件
来源：http://zms.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dbb.yj20258888.top

[U36] Py：定时任务
来源：http://lgx.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://pto.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://kry.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tdw.quarkkingdee.top

[U38] Py：获取脚本所在目录
来源：http://qyw.xuetiantiany.cn

Path(__file__).resolve().parent
来源：http://fhj.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://hfy.haohaochexian.top

sys.stdout.isatty()
来源：http://bwt.yangfankeji.com

[U40] Py：打印到标准错误
来源：http://xjm.iojbl.cn

print("err", file=sys.stderr)
来源：http://npm.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://nrs.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lcs.wangshuangyany.cn

[U42] PHP：PSR-4 自动加载
来源：http://jzi.birdmap.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vrz.bjfxy.top

[U43] PHP：声明命名空间
来源：http://ppe.yuxming.cn

namespace App\Http;
来源：http://esk.tarul.cn

[U44] PHP：开启严格类型
来源：http://vbd.chenlongwang.top

declare(strict_types=1);
来源：http://kmq.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://bgn.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vyq.daxiang520.top

[U46] PHP：可空类型
来源：http://wtk.zhijiandao.cn

?string $name = null
来源：http://eok.snrcjt.cn

[U47] PHP：联合类型
来源：http://lix.dianchejie.cn

int|string $id
来源：http://ris.fzhhl.top

[U48] PHP：纯枚举
来源：http://sco.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eho.cucudq.cn

[U49] PHP：只读属性
来源：http://ypq.ydzc1.top

public readonly string $name
来源：http://yld.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://cpv.hywenlv.cn

public function __construct(private int $id) {}
来源：http://llm.xylfe.cn

[U51] PHP：数组解构
来源：http://thw.gotoacloud.top

[$a, $b] = $arr;
来源：http://cxb.redwolf501.top

[U52] PHP：箭头函数
来源：http://nlp.hnxiangtu.top

$double = fn($x) => $x * 2;
来源：http://xku.cashguo.top


<!-- 参考信息 -->