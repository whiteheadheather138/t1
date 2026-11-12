代发 wailian999

[S43] C++：智能指针
来源：http://cst.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://yey.zhongyouzk.top

[S44] C++：引用传参
来源：http://xjv.cashguo.top

void inc(int &x) { ++x; }
来源：http://ddo.xuanzx.com

[S45] C++：lambda
来源：http://kch.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fao.haohaochexian.top

[S46] C++：函数模板
来源：http://ejb.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hcg.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://nab.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://egg.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://bsv.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bfw.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://yxd.cucudq.cn

[S49] C++：写文件
来源：http://hqa.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mff.haohaochexian.top

[S50] C++：格式化数字
来源：http://ggg.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qla.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://pli.sxryk.cn

static_cast<double>(a) / b
来源：http://ckf.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://rih.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://cbt.nwbrower.top

[S53] C++：移动语义
来源：http://eyc.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://eej.yanxiufei.cn

[S54] C++：异常处理
来源：http://vsn.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vqt.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://miu.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://blm.cashguo.top

[S56] C++：optional
来源：http://svq.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ftd.hywenlv.cn

[S57] C++：编译期常量
来源：http://xfp.zhiwuduotai.top

constexpr int N = 10;
来源：http://sje.gogol.net.cn

[S58] C++：命名空间
来源：http://oaa.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://frn.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://ikw.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://big.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://xoe.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jkl.jqgufenzy.top

================================================================================
来源：http://cus.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fst.zhixingplan.top

================================================================================
来源：http://jix.nwbrower.top

[T01] Kotlin：Hello World
来源：http://udo.zycfv.cn

println("Hello")
来源：http://ipv.9152youxi.cn

[T02] Kotlin：变量
来源：http://jxg.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tou.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://wna.yuanzhike.top

"值: $b"
来源：http://jxu.zycfv.cn

[T04] Kotlin：空安全
来源：http://sgs.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://fun.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://usb.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iuk.meibo888.top

[T06] Kotlin：集合映射
来源：http://zrf.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aib.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://zft.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lim.bjfxy.top

[T08] Kotlin：数据类
来源：http://mwb.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://ecg.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://obf.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://uak.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://hip.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://uzq.vqdsnc.cn

[T11] Kotlin：协程
来源：http://cmo.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uti.cheryme.top

[T12] Kotlin：解构声明
来源：http://ftc.xziqi.cn

val (a, b) = Pair(1, 2)
来源：http://pdu.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://toi.hammf.cn

val m = mapOf("a" to 1)
来源：http://anj.zhixingplan.top

[T14] Kotlin：循环
来源：http://scg.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://fsd.dianchejie.cn

[T15] Kotlin：接口
来源：http://rdv.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://gla.kuanghao11.cn

[T16] Swift：Hello World
来源：http://olh.yanxiufei.cn

print("Hello")
来源：http://yda.52xcode.cn

[T17] Swift：变量与常量
来源：http://ztv.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://xyq.ctjpmb.com

[T18] Swift：字符串插值
来源：http://nbe.jqgufenzy.top

"值: \(b)"
来源：http://qro.daria6918.cn

[T19] Swift：可选绑定
来源：http://otn.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://rml.daria6918.cn

[T20] Swift：数组操作
来源：http://lwb.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://kra.yangfankeji.com

[T21] Swift：遍历
来源：http://nzt.yuanzhike.top

for x in a { print(x) }
来源：http://vqs.sufxvd.cn

[T22] Swift：字典
来源：http://wdl.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://jhr.redwolf501.top

[T23] Swift：函数
来源：http://nnq.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uue.hammf.cn

[T24] Swift：闭包
来源：http://oed.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wtp.fengsongda.top

[T25] Swift：结构体
来源：http://gtw.vqdsnc.cn

struct P { var x: Int }
来源：http://hpu.yj20258.top

[T26] Swift：类与重写
来源：http://fsx.ivvv.top

class A: Base { override func f() {} }
来源：http://esh.yj202588.top

[T27] Swift：错误处理
来源：http://sns.yangfankeji.com

do { try f() } catch { print(error) }
来源：http://qdv.wangdashe.top

[T28] Swift：枚举
来源：http://dul.pengpengdd.cyou

enum Color { case red, green }
来源：http://oyp.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://jii.jiagoushi.top

guard let x = opt else { return }
来源：http://zhv.snrcjt.cn

[T30] Swift：协议
来源：http://gbo.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://bku.xuanzx.com

[T31] Lua：Hello World
来源：http://kxp.zhiwuduotai.top

print("Hello")
来源：http://sua.316326.xyz

[T32] Lua：局部变量
来源：http://bhk.xuanzx.com

local a = 1
来源：http://bsy.tarul.cn

[T33] Lua：表（数组）
来源：http://mqe.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fxk.birdmap.top

[T34] Lua：遍历表
来源：http://nox.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qwv.ybcxt.top

[T35] Lua：字典表
来源：http://uln.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://zhm.jiagoushi.top

[T36] Lua：函数
来源：http://ald.52xcode.cn

function add(a, b) return a + b end
来源：http://ert.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://itb.jqgfzy.top

"a" .. "b"
来源：http://hsz.9152youxi.cn

[T38] Lua：条件
来源：http://zrd.52xcode.cn

if x > 0 then print("正") end
来源：http://ilf.sweek.top

[T39] Lua：模式匹配
来源：http://gdk.hcnkem.com

string.find(s, "%d+")
来源：http://qlb.yangfankeji.com

[T40] Lua：元表
来源：http://vya.sxryk.cn

setmetatable({}, { __index = base })
来源：http://kdd.gotoacloud.top

[T41] Perl：Hello World
来源：http://tcb.zhengqikj.top

print "Hello\n";
来源：http://ife.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://tae.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xjl.nanxinkj.top

[T43] Perl：字符串插值
来源：http://ncr.hnqzz.top

"值: $a"
来源：http://bqr.hysaishi.cn

[T44] Perl：条件
来源：http://wis.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://fvs.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://qnj.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://jcj.svipenyu.cn

[T46] Perl：哈希操作
来源：http://hyo.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ofn.zdbjq.cn

[T47] Perl：正则捕获
来源：http://hwk.hysaishi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wpa.yuanzhike.top

[T48] Perl：正则替换
来源：http://gsw.tanke756.top

$s =~ s/old/new/g;
来源：http://qih.zycfv.cn

[T49] Perl：函数
来源：http://xbt.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pxv.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://sxm.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rsb.gaohongyu789.top

while (my $line = <$fh>) { print $line; }
来源：http://omi.aibaodan.cn

[T51] Scala：Hello World
来源：http://vbi.ydjk.org.cn

println("Hello")
来源：http://amm.hywenlv.cn

[T52] Scala：变量
来源：http://vac.bjfxy.top

val a = 1;  var b = 2
来源：http://aqr.ybcxt.top

[T53] Scala：字符串插值
来源：http://duk.zhijiandao.cn

s"值: $b"
来源：http://tux.vqdsnc.cn

[T54] Scala：集合映射
来源：http://zwi.cqqwz.cn

List(1, 2, 3).map(_ * 2)
来源：http://eop.gotoacloud.top

[T55] Scala：集合过滤
来源：http://mfr.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wag.zhiwuduotai.top

[T56] Scala：样例类
来源：http://sny.yonumen.top

case class User(name: String, age: Int)
来源：http://acb.cheryme.top

[T57] Scala：模式匹配
来源：http://hbg.fengsongda.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kmx.yonumen.top

[T58] Scala：函数定义
来源：http://pxu.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://xeh.jqgfzy.top

[T59] Scala：循环
来源：http://yzm.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://gil.bjfxy.top

[T60] Scala：折叠
来源：http://vvh.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nrz.tarul.cn

================================================================================
来源：http://zbl.shangyingyoupin.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://soc.tarul.cn

================================================================================
来源：http://eqr.pycfn.com

[U01] Py：创建虚拟环境
来源：http://wnf.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://kno.zhoulong.xyz

[U02] Py：导出 / 安装依赖
来源：http://yjh.sjlbkw.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rdo.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://kye.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wmc.daxiang520.top

[U04] Py：变量调试打印
来源：http://cwi.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xhc.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://hfy.yonumen.top

list(dict.fromkeys(arr))
来源：http://ewz.yueranfly.top

[U06] Py：合并两个字典
来源：http://hdx.haohaochexian.top

{**a, **b}
来源：http://uaf.mhx1999.top

[U07] Py：反转字典键值
来源：http://lmp.hammf.cn

{v: k for k, v in d.items()}
来源：http://jvm.c1oappe.top

[U08] Py：展平二维列表
来源：http://ett.pycfn.com

[y for x in nested for y in x]
来源：http://cxr.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://wpy.zhijiandao.cn

max(d, key=d.get)
来源：http://daf.yuanzhike.top

[U10] Py：按值排序字典
来源：http://xpj.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qut.fengsongda.top

[U11] Py：生成器表达式
来源：http://nyy.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://pad.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://nlz.redwolf501.top

Counter(arr).most_common(3)
来源：http://wij.sysykeji.top

[U13] Py：固定长度队列
来源：http://scl.yangfankeji.com

deque(maxlen=10)
来源：http://uqb.52xcode.cn

[U14] Py：分组收集到列表
来源：http://tzo.feifeiyinyue.top

defaultdict(list)
来源：http://tbz.fehbvm.com

[U15] Py：高精度计时
来源：http://sqb.316326.xyz

t = time.perf_counter()
来源：http://qhv.xziqi.cn

[U16] Py：命令行参数解析
来源：http://jpb.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pzz.yfazqb.com

[U17] Py：初始化日志
来源：http://gzj.fktsv.cn

logging.basicConfig(level=logging.INFO)
来源：http://wfi.zhoulong.xyz

[U18] Py：预编译正则
来源：http://dfg.hnqzz.top

pat = re.compile(r"\d+")
来源：http://ciq.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://aau.daria6918.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vop.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://pdm.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://hjc.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://inu.jinyuanbaomall.cn

@contextlib.contextmanager
来源：http://udu.fanxiaobao.xyz

[U22] Py：矩阵转置
来源：http://eqf.sweek.top

list(zip(*m))
来源：http://hsp.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://cmj.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ljg.meibo888.top

[U24] Py：路径操作
来源：http://xtk.havefunace.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zxs.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://ggs.cdnleiting.top

csv.DictReader(f)
来源：http://xka.ydzc1.top

[U26] Py：并发下载
来源：http://irb.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://muj.daria6918.cn

[U27] Py：异步 HTTP
来源：http://zdq.zdbjq.cn

aiohttp.ClientSession() 配合 async with
来源：http://jcp.cdnleiting.top

[U28] Py：类型别名
来源：http://noj.xuetiantiany.cn

UserId = int
来源：http://yhw.52xcode.cn

[U29] Py：属性校验
来源：http://dhf.yueranfly.top

@property 与 @x.setter 配合
来源：http://xvf.zhaomingkeji.xyz

[U30] Py：数据类
来源：http://rcw.zhaomingkeji.xyz

@dataclass(slots=True)
来源：http://puh.bjfxy.top

[U31] Py：单测
来源：http://yze.xylfe.cn

python -m pytest -q
来源：http://rel.yangfankeji.com

[U32] Py：代码格式化
来源：http://ebh.cucudq.cn

ruff format . && ruff check --fix .
来源：http://gvb.yueranfly.top

[U33] Py：打包发布
来源：http://gyf.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://xjp.birdmap.top

[U34] Py：判断编码
来源：http://nvg.yuanzhike.top

chardet.detect(raw)
来源：http://thu.svipenyu.cn

[U35] Py：发送邮件
来源：http://ekw.shangyingyoupin.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bky.hysaishi.cn

[U36] Py：定时任务
来源：http://nif.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://hue.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://oeg.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://naw.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://eih.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://jtx.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://xet.jyoumei.cn

sys.stdout.isatty()
来源：http://wiy.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://wli.yvedp.cn

print("err", file=sys.stderr)
来源：http://vem.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://pst.wangshuangyany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rwx.svipenyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://nba.jlsjyb.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mhc.bbcook.cn

[U43] PHP：声明命名空间
来源：http://uju.xuetiantiany.cn

namespace App\Http;
来源：http://mju.vqdsnc.cn

[U44] PHP：开启严格类型
来源：http://dlk.hesvh.cn

declare(strict_types=1);
来源：http://rhv.hfpthk.cn

[U45] PHP：类型声明与返回类型
来源：http://qnw.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://eqm.svipenyu.cn

[U46] PHP：可空类型
来源：http://gda.shanyushiyangtech.top

?string $name = null
来源：http://ypx.zhijiandao.cn

[U47] PHP：联合类型
来源：http://dal.tanke756.top

int|string $id
来源：http://qah.ivvv.top

[U48] PHP：纯枚举
来源：http://tyy.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kdn.uphjek.com

[U49] PHP：只读属性
来源：http://ptd.tanke756.top

public readonly string $name
来源：http://hxw.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://dtp.aibaodan.cn

public function __construct(private int $id) {}
来源：http://qdf.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://uwz.jiagoushi.top

[$a, $b] = $arr;
来源：http://ddd.nanxinkj.top

[U52] PHP：箭头函数
来源：http://hya.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://scx.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://pvr.yangfankeji.com

$v = $a ?? $b ?? "default";
来源：http://dcr.tian-w.cn

[U54] PHP：空安全调用
来源：http://fkp.yfazqb.com

$obj?->method()
来源：http://nbl.yueranfly.top

[U55] PHP：match 表达式
来源：http://yez.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jit.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://kox.hcnkem.com

f(a: 1, b: 2)
来源：http://zrs.zhoulong.xyz

[U57] PHP：字符串插值
来源：http://ucp.hesvh.cn

"值: {$a}"
来源：http://dff.zdbjq.cn

[U58] PHP：数组三件套
来源：http://grc.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://csl.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://vrp.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://trp.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://kgv.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ucp.cashguo.top

[U61] PHP：正则
来源：http://aqq.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zsy.havefunace.top

[U62] PHP：日期对象
来源：http://xaf.sysykeji.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ehm.cheryme.top

[U63] PHP：文件读写
来源：http://svz.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hef.meibo888.top

[U64] PHP：目录遍历
来源：http://dog.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://jmz.tian-w.cn

[U65] PHP：会话
来源：http://dxp.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://krd.birdmap.top

[U66] PHP：设置 Cookie
来源：http://zzv.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dkq.hammf.cn

[U67] PHP：处理文件上传
来源：http://qph.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rso.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://prz.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kjk.cucudq.cn


<!-- 参考信息 -->