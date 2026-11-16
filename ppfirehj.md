代发 wailian999

#include <iostream>
来源：http://lqm.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://gbl.redwolf501.top

[S32] C++：字符串
来源：http://fun.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://hio.c1oappe.top

[S33] C++：vector 增删
来源：http://jhz.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cvt.xinyue.icu

[S34] C++：遍历 vector
来源：http://iwx.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://qzw.fehbvm.com

[S35] C++：map
来源：http://aqs.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jnm.nwbrower.top

[S36] C++：unordered_map
来源：http://sdw.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wtt.c1oappe.top

[S37] C++：set
来源：http://gho.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gjq.hnqzz.top

[S38] C++：排序
来源：http://dnd.yj202588.top

std::sort(v.begin(), v.end());
来源：http://fru.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://amv.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fcl.zhixingplan.top

[S40] C++：查找元素
来源：http://ecg.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mqu.bbcook.cn

[S41] C++：类与构造函数
来源：http://tno.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sqv.pycfn.com

[S42] C++：继承与虚函数
来源：http://dcx.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://lod.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://pel.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://noq.daxiang520.top

[S44] C++：引用传参
来源：http://lyw.zhixingplan.top

void inc(int &x) { ++x; }
来源：http://jvg.pycfn.com

[S45] C++：lambda
来源：http://cll.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://uqa.hfpthk.cn

[S46] C++：函数模板
来源：http://vdn.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sic.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://gvd.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://omo.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://gxa.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://ezk.sxryk.cn

while (std::getline(in, line)) { }
来源：http://bux.aizwys.cn

[S49] C++：写文件
来源：http://tnt.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fzn.uphjek.com

[S50] C++：格式化数字
来源：http://gop.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wpd.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://ekl.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://uzy.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://dup.bbcook.cn

int size() const noexcept { return n_; }
来源：http://mnv.guannengcc.top

[S53] C++：移动语义
来源：http://rao.uphjek.com

std::vector<int> w = std::move(v);
来源：http://vem.sufxvd.cn

[S54] C++：异常处理
来源：http://hbu.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uyb.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://cqp.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bul.guowangkeji.top

[S56] C++：optional
来源：http://qrt.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qex.tarul.cn

[S57] C++：编译期常量
来源：http://hec.cashguo.top

constexpr int N = 10;
来源：http://sth.bjfxy.top

[S58] C++：命名空间
来源：http://hpv.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://lcp.vqdsnc.cn

[S59] C++：静态断言
来源：http://yzl.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xzd.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://exd.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gtz.yueranfly.top

================================================================================
来源：http://ppj.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://spq.hcnkem.com

================================================================================
来源：http://ifm.bjfxy.top

[T01] Kotlin：Hello World
来源：http://xmp.tanke756.top

println("Hello")
来源：http://hpm.yfazqb.com

[T02] Kotlin：变量
来源：http://npd.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kwa.yj202588.top

[T03] Kotlin：字符串模板
来源：http://ocl.epnwcf.com

"值: $b"
来源：http://ldb.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://qaf.chenzaomai.com

val n: String? = null;  n?.length
来源：http://ivx.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://fmx.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ibb.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://jtm.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vju.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://brw.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ohm.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://jrv.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://dlb.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://chl.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://eyd.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://vua.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jnr.shzxlz.cn

[T11] Kotlin：协程
来源：http://sxz.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uyy.ydzc1.top

[T12] Kotlin：解构声明
来源：http://nhr.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://qty.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://pub.hnqzz.top

val m = mapOf("a" to 1)
来源：http://xqx.nwbrower.top

[T14] Kotlin：循环
来源：http://uhm.dianchejie.cn

for (i in 1..10) println(i)
来源：http://yvh.vqdsnc.cn

[T15] Kotlin：接口
来源：http://njh.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://blz.hnxiangtu.top

[T16] Swift：Hello World
来源：http://zkn.jinqigufen.top

print("Hello")
来源：http://zsh.52xcode.cn

[T17] Swift：变量与常量
来源：http://fex.hysaishi.cn

var a = 1;  let b = 2
来源：http://qwl.dashuyun.cn

[T18] Swift：字符串插值
来源：http://kef.ivvv.top

"值: \(b)"
来源：http://xen.chenzaomai.com

[T19] Swift：可选绑定
来源：http://cha.vqdsnc.cn

if let n = opt { print(n) }
来源：http://jyp.fzhhl.top

[T20] Swift：数组操作
来源：http://pqi.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://pmr.hnqzz.top

[T21] Swift：遍历
来源：http://khw.9152youxi.cn

for x in a { print(x) }
来源：http://dia.xuetiantiany.cn

[T22] Swift：字典
来源：http://ijc.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://hsx.daria6918.cn

[T23] Swift：函数
来源：http://ens.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://elu.c1oappe.top

[T24] Swift：闭包
来源：http://fag.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cac.tianlin.xyz

[T25] Swift：结构体
来源：http://eag.epnwcf.com

struct P { var x: Int }
来源：http://kzs.zhengqikj.top

[T26] Swift：类与重写
来源：http://ojw.ctjpmb.com

class A: Base { override func f() {} }
来源：http://zzj.zdbjq.cn

[T27] Swift：错误处理
来源：http://dku.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://wqr.sufxvd.cn

[T28] Swift：枚举
来源：http://jzv.fktsv.cn

enum Color { case red, green }
来源：http://ifb.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://wes.feifeiyinyue.top

guard let x = opt else { return }
来源：http://ton.sysykeji.top

[T30] Swift：协议
来源：http://wnm.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://jrx.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://jve.0kj1m.cn

print("Hello")
来源：http://ffe.tianlin.xyz

[T32] Lua：局部变量
来源：http://vjs.yuanzhike.top

local a = 1
来源：http://vpq.daria6918.cn

[T33] Lua：表（数组）
来源：http://pmx.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kbn.quarkkingdee.top

[T34] Lua：遍历表
来源：http://vjs.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wxe.hnqzz.top

[T35] Lua：字典表
来源：http://exo.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://cmd.jqgufenzy.top

[T36] Lua：函数
来源：http://sjl.guowangkeji.top

function add(a, b) return a + b end
来源：http://oeu.tian-w.cn

[T37] Lua：字符串拼接
来源：http://mdq.c1oappe.top

"a" .. "b"
来源：http://hir.gaohongyu789.top

[T38] Lua：条件
来源：http://lsg.hcnkem.com

if x > 0 then print("正") end
来源：http://qoi.ydzc1.top

[T39] Lua：模式匹配
来源：http://cug.zdqjudy.top

string.find(s, "%d+")
来源：http://eat.xziqi.cn

[T40] Lua：元表
来源：http://gix.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://nbb.ehwqpu.com

[T41] Perl：Hello World
来源：http://qzu.nanxinkj.top

print "Hello\n";
来源：http://hak.gaohongyu789.top

[T42] Perl：变量类型
来源：http://vtt.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dxt.yfazqb.com

[T43] Perl：字符串插值
来源：http://nqr.ybcxt.top

"值: $a"
来源：http://oes.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://snw.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://gcf.uphjek.com

[T45] Perl：数组遍历
来源：http://jnq.birdmap.top

for my $x (@arr) { print $x; }
来源：http://rgu.smart0.xyz

[T46] Perl：哈希操作
来源：http://kvm.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qlc.ivvv.top

[T47] Perl：正则捕获
来源：http://htn.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zck.yfazqb.com

[T48] Perl：正则替换
来源：http://xgs.yonumen.top

$s =~ s/old/new/g;
来源：http://uyb.fehbvm.com

[T49] Perl：函数
来源：http://dyr.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rrm.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://ytd.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vjy.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://gyt.sysykeji.top

[T51] Scala：Hello World
来源：http://tzm.cheryme.top

println("Hello")
来源：http://kcw.dashuyun.cn

[T52] Scala：变量
来源：http://qvx.pycfn.com

val a = 1;  var b = 2
来源：http://vzr.jyoumei.cn

[T53] Scala：字符串插值
来源：http://bat.jqgfzy.top

s"值: $b"
来源：http://lnm.tarul.cn

[T54] Scala：集合映射
来源：http://emp.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://wdo.xuanzx.com

[T55] Scala：集合过滤
来源：http://ymf.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pgo.vqdsnc.cn

[T56] Scala：样例类
来源：http://pqy.tianlin.xyz

case class User(name: String, age: Int)
来源：http://oux.yfazqb.com

[T57] Scala：模式匹配
来源：http://pkd.zhoulong.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://uup.jianghu66.top

[T58] Scala：函数定义
来源：http://dgq.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://pgh.ehwqpu.com

[T59] Scala：循环
来源：http://ert.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://yvp.jiagoushi.top

[T60] Scala：折叠
来源：http://dte.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fgz.jqgfzy.top

================================================================================
来源：http://jaw.cucudq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://itb.shuidangran.top

================================================================================
来源：http://rgw.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://mae.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://jgb.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://tvs.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://atg.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://zbq.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sha.meibo888.top

[U04] Py：变量调试打印
来源：http://kuz.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://epn.yonumen.top

[U05] Py：列表去重且保序
来源：http://gwk.316326.xyz

list(dict.fromkeys(arr))
来源：http://zeh.xylfe.cn

[U06] Py：合并两个字典
来源：http://kbj.zdbjq.cn

{**a, **b}
来源：http://xfg.cheryme.top

[U07] Py：反转字典键值
来源：http://twt.hcnkem.com

{v: k for k, v in d.items()}
来源：http://nzw.sxryk.cn

[U08] Py：展平二维列表
来源：http://bna.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://geu.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://lrl.shuidangran.top

max(d, key=d.get)
来源：http://ieu.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://nwe.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xug.zhixingplan.top

[U11] Py：生成器表达式
来源：http://dfn.c1oappe.top

(x * 2 for x in arr)
来源：http://pic.hywenlv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cfb.cdnleiting.top

Counter(arr).most_common(3)
来源：http://tuy.cucudq.cn

[U13] Py：固定长度队列
来源：http://qun.bbcook.cn

deque(maxlen=10)
来源：http://xyh.shanyushiyangtech.top

[U14] Py：分组收集到列表
来源：http://jfj.zdbjq.cn

defaultdict(list)
来源：http://zzy.jyoumei.cn

[U15] Py：高精度计时
来源：http://tvw.sxryk.cn

t = time.perf_counter()
来源：http://kne.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://ste.0kj1m.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://muz.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://rov.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://wpj.ydjk.org.cn

[U18] Py：预编译正则
来源：http://qcs.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://zmo.guannengcc.top

[U19] Py：正则替换带回调
来源：http://hre.zhijiandao.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vdk.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://pxc.chenzaomai.com

@functools.lru_cache(maxsize=None)
来源：http://mas.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://rwe.nanxuanxn.top

@contextlib.contextmanager
来源：http://bnm.daxiang520.top

[U22] Py：矩阵转置
来源：http://gup.dianchejie.cn

list(zip(*m))
来源：http://bwu.chenlongwang.top

[U23] Py：分块读取大文件
来源：http://wku.yangfankeji.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://plr.hywenlv.cn

[U24] Py：路径操作
来源：http://cho.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xuf.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://ulg.shzxlz.cn

csv.DictReader(f)
来源：http://aij.gaohongyu789.top

[U26] Py：并发下载
来源：http://jhi.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vfm.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://phm.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://hgt.nwbrower.top

[U28] Py：类型别名
来源：http://xeu.nanxinkj.top

UserId = int
来源：http://rrv.xingfuxueyuan.xyz

[U29] Py：属性校验
来源：http://iag.gotoacloud.top

@property 与 @x.setter 配合
来源：http://lmx.yfazqb.com

[U30] Py：数据类
来源：http://zwn.fzhhl.top

@dataclass(slots=True)
来源：http://rtu.meibo888.top

[U31] Py：单测
来源：http://zxr.cheryme.top

python -m pytest -q
来源：http://sud.hywenlv.cn

[U32] Py：代码格式化
来源：http://hce.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://csm.gotoacloud.top

[U33] Py：打包发布
来源：http://htw.hesvh.cn

python -m build  （依赖 pyproject.toml）
来源：http://wxz.redwolf501.top

[U34] Py：判断编码
来源：http://qkw.meibo888.top

chardet.detect(raw)
来源：http://uvv.cdnleiting.top

[U35] Py：发送邮件
来源：http://kdi.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fcm.nwbrower.top

[U36] Py：定时任务
来源：http://cqb.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://xuf.hywenlv.cn

[U37] Py：读写 Excel
来源：http://naw.sjlbkw.cn

pandas.read_excel / DataFrame.to_excel
来源：http://lmb.fktsv.cn

[U38] Py：获取脚本所在目录
来源：http://hzr.zdqjudy.top

Path(__file__).resolve().parent
来源：http://xjf.ppjwa.cn

[U39] Py：判断是否在交互环境
来源：http://bco.yangfankeji.com

sys.stdout.isatty()
来源：http://ucs.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://udf.xingfuxueyuan.xyz

print("err", file=sys.stderr)
来源：http://mrg.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://zph.chenjidiqi.icu

composer init;  composer require guzzlehttp/guzzle
来源：http://nde.yj202588.top

[U42] PHP：PSR-4 自动加载
来源：http://sdn.nwbrower.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dqq.birdmap.top

[U43] PHP：声明命名空间
来源：http://ebu.fengsongda.top

namespace App\Http;
来源：http://fec.ehwqpu.com

[U44] PHP：开启严格类型
来源：http://lsp.cucudq.cn

declare(strict_types=1);
来源：http://kay.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://zvl.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://sdh.jqgufenzy.top

[U46] PHP：可空类型
来源：http://dnw.shzxlz.cn

?string $name = null
来源：http://imf.gogol.net.cn

[U47] PHP：联合类型
来源：http://jqw.yj202588.top

int|string $id
来源：http://sio.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://ohw.xuanzx.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jqp.quarkkingdee.top

[U49] PHP：只读属性
来源：http://lde.epnwcf.com

public readonly string $name
来源：http://awr.bbcook.cn

[U50] PHP：构造器属性提升
来源：http://fch.aibaodan.cn

public function __construct(private int $id) {}
来源：http://xku.bjfxy.top

[U51] PHP：数组解构
来源：http://xfl.sweek.top

[$a, $b] = $arr;
来源：http://tar.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://lsw.zdqjudy.top

$double = fn($x) => $x * 2;
来源：http://vpb.dashuyun.cn

[U53] PHP：空合并运算符
来源：http://ftj.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://prq.vehdjk.com

[U54] PHP：空安全调用
来源：http://qam.zhengqikj.top

$obj?->method()
来源：http://gjz.redwolf501.top

[U55] PHP：match 表达式
来源：http://fzz.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uxh.svipenyu.cn

[U56] PHP：命名参数
来源：http://atw.kuanghao11.cn

f(a: 1, b: 2)
来源：http://xqi.hnxiangtu.top


<!-- 参考信息 -->