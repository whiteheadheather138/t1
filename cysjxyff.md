代发 wailian999

[S43] C++：智能指针
来源：http://rcx.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://din.jiagoushi.top

[S44] C++：引用传参
来源：http://sbu.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://xyd.yuxming.cn

[S45] C++：lambda
来源：http://iil.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://lpo.gogol.net.cn

[S46] C++：函数模板
来源：http://hly.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qiv.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://lwj.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tfk.c1oappe.top

[S48] C++：逐行读文件
来源：http://rbt.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://adw.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://moo.nanxinkj.top

[S49] C++：写文件
来源：http://eut.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gio.chenlongwang.top

[S50] C++：格式化数字
来源：http://tff.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sva.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://wps.guowangkeji.top

static_cast<double>(a) / b
来源：http://qhn.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://byp.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://duq.aibaodan.cn

[S53] C++：移动语义
来源：http://gua.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://fih.iojbl.cn

[S54] C++：异常处理
来源：http://ydy.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mkt.bjfxy.top

[S55] C++：结构化绑定
来源：http://wrn.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wji.snrcjt.cn

[S56] C++：optional
来源：http://tvi.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tnx.xuanzx.com

[S57] C++：编译期常量
来源：http://pht.daxiang520.top

constexpr int N = 10;
来源：http://qyo.52xcode.cn

[S58] C++：命名空间
来源：http://lqy.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://fps.xziqi.cn

[S59] C++：静态断言
来源：http://pzi.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dew.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://jum.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mel.cheryme.top

================================================================================
来源：http://vza.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zhw.ehwqpu.com

================================================================================
来源：http://jxq.sweek.top

[T01] Kotlin：Hello World
来源：http://ygf.jyoumei.cn

println("Hello")
来源：http://ait.snrcjt.cn

[T02] Kotlin：变量
来源：http://xjw.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://djs.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://qlw.jinqigufen.top

"值: $b"
来源：http://xxt.dianchejie.cn

[T04] Kotlin：空安全
来源：http://hpk.cdnleiting.top

val n: String? = null;  n?.length
来源：http://gbo.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://rux.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ear.ydzc1.top

[T06] Kotlin：集合映射
来源：http://cbu.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://emz.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://abs.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sjd.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://tgi.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://zek.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://hyj.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://cir.ydzc1.top

[T10] Kotlin：默认参数
来源：http://ajc.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mej.shuidangran.top

[T11] Kotlin：协程
来源：http://zyx.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzl.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://etz.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://yom.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://yla.zhaomingkeji.xyz

val m = mapOf("a" to 1)
来源：http://fyi.ivvv.top

[T14] Kotlin：循环
来源：http://dqk.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://abm.mhx1999.top

[T15] Kotlin：接口
来源：http://zyg.epnwcf.com

interface Shape { fun area(): Double }
来源：http://dva.yj20258888.top

[T16] Swift：Hello World
来源：http://bzy.jianghu66.top

print("Hello")
来源：http://zap.zhixingplan.top

[T17] Swift：变量与常量
来源：http://qmp.hfpthk.cn

var a = 1;  let b = 2
来源：http://jzi.hfpthk.cn

[T18] Swift：字符串插值
来源：http://kfa.xziqi.cn

"值: \(b)"
来源：http://ydl.ctjpmb.com

[T19] Swift：可选绑定
来源：http://zdd.0kj1m.cn

if let n = opt { print(n) }
来源：http://xgf.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://ftx.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pfj.hesvh.cn

[T21] Swift：遍历
来源：http://xho.tian-w.cn

for x in a { print(x) }
来源：http://dwm.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://zzc.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gul.jlsjyb.cn

[T23] Swift：函数
来源：http://wry.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wqs.gzhubu.top

[T24] Swift：闭包
来源：http://uzv.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uul.yueranfly.top

[T25] Swift：结构体
来源：http://lzb.sjlbkw.cn

struct P { var x: Int }
来源：http://grb.ivvv.top

[T26] Swift：类与重写
来源：http://iat.dianchejie.cn

class A: Base { override func f() {} }
来源：http://qkn.zhoulong.xyz

[T27] Swift：错误处理
来源：http://joe.redwolf501.top

do { try f() } catch { print(error) }
来源：http://ize.fktsv.cn

[T28] Swift：枚举
来源：http://one.gzhubu.top

enum Color { case red, green }
来源：http://agi.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://ady.pengpengdd.cyou

guard let x = opt else { return }
来源：http://nur.yanxiufei.cn

[T30] Swift：协议
来源：http://yfg.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://zta.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://gsd.gzhubu.top

print("Hello")
来源：http://mti.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://fyd.ppjwa.cn

local a = 1
来源：http://nka.gzhubu.top

[T33] Lua：表（数组）
来源：http://czf.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qjx.ivvv.top

[T34] Lua：遍历表
来源：http://uny.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://edl.sufxvd.cn

[T35] Lua：字典表
来源：http://dcu.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://qsr.iojbl.cn

[T36] Lua：函数
来源：http://ypi.yangfankeji.com

function add(a, b) return a + b end
来源：http://uan.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://uwf.cdnleiting.top

"a" .. "b"
来源：http://pvx.ybcxt.top

[T38] Lua：条件
来源：http://ugw.chenlongwang.top

if x > 0 then print("正") end
来源：http://izb.cdnleiting.top

[T39] Lua：模式匹配
来源：http://usv.0kj1m.cn

string.find(s, "%d+")
来源：http://sjp.hywenlv.cn

[T40] Lua：元表
来源：http://hih.bjfxy.top

setmetatable({}, { __index = base })
来源：http://ngt.cashguo.top

[T41] Perl：Hello World
来源：http://lpf.zdbjq.cn

print "Hello\n";
来源：http://csf.fktsv.cn

[T42] Perl：变量类型
来源：http://shi.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kog.haohaochexian.top

[T43] Perl：字符串插值
来源：http://kgd.ctjpmb.com

"值: $a"
来源：http://eib.hfpthk.cn

[T44] Perl：条件
来源：http://hxc.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://lzg.zhiwuduotai.top

[T45] Perl：数组遍历
来源：http://qum.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://ynx.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://ujd.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://skj.yonumen.top

[T47] Perl：正则捕获
来源：http://ylm.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://tox.zhixingplan.top

[T48] Perl：正则替换
来源：http://xiy.yuxming.cn

$s =~ s/old/new/g;
来源：http://gru.uphjek.com

[T49] Perl：函数
来源：http://lph.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xct.daxiang520.top

[T50] Perl：逐行读文件
来源：http://flp.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jso.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://vib.zdbjq.cn

[T51] Scala：Hello World
来源：http://ere.vehdjk.com

println("Hello")
来源：http://rfk.0kj1m.cn

[T52] Scala：变量
来源：http://ucl.jyoumei.cn

val a = 1;  var b = 2
来源：http://hoe.chenzaomai.com

[T53] Scala：字符串插值
来源：http://fxg.sysykeji.top

s"值: $b"
来源：http://olb.zdqjudy.top

[T54] Scala：集合映射
来源：http://jpw.aizwys.cn

List(1, 2, 3).map(_ * 2)
来源：http://xgz.shuidangran.top

[T55] Scala：集合过滤
来源：http://tpq.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gsh.jqgfzy.top

[T56] Scala：样例类
来源：http://tss.316326.xyz

case class User(name: String, age: Int)
来源：http://cxj.daria6918.cn

[T57] Scala：模式匹配
来源：http://sqg.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sfy.vehdjk.com

[T58] Scala：函数定义
来源：http://plp.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://oke.feifeiyinyue.top

[T59] Scala：循环
来源：http://vts.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://jqd.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://srp.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cxd.nanxinkj.top

================================================================================
来源：http://jnr.9152youxi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sft.aizwys.cn

================================================================================
来源：http://vgj.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://ypn.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://xzh.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://gef.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://opc.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://bbq.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gzw.tian-w.cn

[U04] Py：变量调试打印
来源：http://nyb.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jru.yangfankeji.com

[U05] Py：列表去重且保序
来源：http://ejg.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://lpx.ppjwa.cn

[U06] Py：合并两个字典
来源：http://wcr.jyoumei.cn

{**a, **b}
来源：http://soi.gotoacloud.top

[U07] Py：反转字典键值
来源：http://pzg.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://ppn.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://hgn.snrcjt.cn

[y for x in nested for y in x]
来源：http://mgf.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://fdx.chenjidiqi.icu

max(d, key=d.get)
来源：http://uak.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://ewb.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hlj.chenlongwang.top

[U11] Py：生成器表达式
来源：http://hud.fehbvm.com

(x * 2 for x in arr)
来源：http://cmn.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://zav.dashuyun.cn

Counter(arr).most_common(3)
来源：http://nxn.ywan-chungtsiang.top

[U13] Py：固定长度队列
来源：http://tfm.quarkkingdee.top

deque(maxlen=10)
来源：http://bks.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://mkb.shzxlz.cn

defaultdict(list)
来源：http://hqq.cheryme.top

[U15] Py：高精度计时
来源：http://rts.haohaochexian.top

t = time.perf_counter()
来源：http://cry.gotoacloud.top

[U16] Py：命令行参数解析
来源：http://sfd.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qmo.tianlin.xyz

[U17] Py：初始化日志
来源：http://xgu.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://rrs.fengsongda.top

[U18] Py：预编译正则
来源：http://wkq.c1oappe.top

pat = re.compile(r"\d+")
来源：http://rya.yonumen.top

[U19] Py：正则替换带回调
来源：http://bgx.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qfr.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://aco.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://fdk.ydjk.org.cn

[U21] Py：自定义上下文管理器
来源：http://vyn.ydzc1.top

@contextlib.contextmanager
来源：http://jvh.gzhubu.top

[U22] Py：矩阵转置
来源：http://dlg.jyoumei.cn

list(zip(*m))
来源：http://ier.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://ncb.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jbd.gaohongyu789.top

[U24] Py：路径操作
来源：http://ytw.jlsjyb.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rce.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://eib.redwolf501.top

csv.DictReader(f)
来源：http://zyx.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://eqa.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mjm.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://djj.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://yrn.ydzc1.top

[U28] Py：类型别名
来源：http://wdf.gogol.net.cn

UserId = int
来源：http://vds.kuanghao11.cn

[U29] Py：属性校验
来源：http://yse.yuanzhike.top

@property 与 @x.setter 配合
来源：http://spn.yanxiufei.cn

[U30] Py：数据类
来源：http://kac.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://yts.haohaochexian.top

[U31] Py：单测
来源：http://waf.fanxiaobao.xyz

python -m pytest -q
来源：http://cwt.zhongyouzk.top

[U32] Py：代码格式化
来源：http://kgz.yonumen.top

ruff format . && ruff check --fix .
来源：http://veh.hywenlv.cn

[U33] Py：打包发布
来源：http://xod.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://vxf.yuxming.cn

[U34] Py：判断编码
来源：http://jdk.bbcook.cn

chardet.detect(raw)
来源：http://ovv.guannengcc.top

[U35] Py：发送邮件
来源：http://nwb.jiagoushi.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lfq.ctjpmb.com

[U36] Py：定时任务
来源：http://ujb.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://njp.yanxiufei.cn

[U37] Py：读写 Excel
来源：http://yne.yangfankeji.com

pandas.read_excel / DataFrame.to_excel
来源：http://vfn.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://kyf.gaohongyu789.top

Path(__file__).resolve().parent
来源：http://bou.uphjek.com

[U39] Py：判断是否在交互环境
来源：http://bvu.hesvh.cn

sys.stdout.isatty()
来源：http://nnm.hesvh.cn

[U40] Py：打印到标准错误
来源：http://tqi.hammf.cn

print("err", file=sys.stderr)
来源：http://pnn.chenlongwang.top

[U41] PHP：初始化 Composer 项目
来源：http://iel.shzxlz.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yyp.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://wik.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://etb.zycfv.cn

[U43] PHP：声明命名空间
来源：http://fuf.wangdashe.top

namespace App\Http;
来源：http://pvs.cashguo.top

[U44] PHP：开启严格类型
来源：http://ktn.shanyushiyangkeji.top

declare(strict_types=1);
来源：http://xfq.nwbrower.top

[U45] PHP：类型声明与返回类型
来源：http://zmu.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wpv.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://wwc.jiagoushi.top

?string $name = null
来源：http://tar.tian-w.cn

[U47] PHP：联合类型
来源：http://scj.zhiwuduotai.top

int|string $id
来源：http://snd.tianlin.xyz

[U48] PHP：纯枚举
来源：http://rpz.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mwl.yueranfly.top

[U49] PHP：只读属性
来源：http://hho.jinqigufen.top

public readonly string $name
来源：http://zan.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://tny.chenlongwang.top

public function __construct(private int $id) {}
来源：http://wql.fengsongda.top

[U51] PHP：数组解构
来源：http://roi.yangfankeji.com

[$a, $b] = $arr;
来源：http://emk.zdbjq.cn

[U52] PHP：箭头函数
来源：http://hxl.jinghuilouyu.cn

$double = fn($x) => $x * 2;
来源：http://cmn.yj20258.top

[U53] PHP：空合并运算符
来源：http://czs.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://mvp.gotoacloud.top

[U54] PHP：空安全调用
来源：http://lcd.iojbl.cn

$obj?->method()
来源：http://czu.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://vdb.jyoumei.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ocf.0kj1m.cn

[U56] PHP：命名参数
来源：http://jbe.yuxming.cn

f(a: 1, b: 2)
来源：http://ghg.yuxming.cn

[U57] PHP：字符串插值
来源：http://yij.iojbl.cn

"值: {$a}"
来源：http://pgx.xylfe.cn

[U58] PHP：数组三件套
来源：http://arv.mhx1999.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://egu.hysaishi.cn

[U59] PHP：自定义排序
来源：http://qmk.gzhubu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhy.cheryme.top

[U60] PHP：JSON 编解码
来源：http://pfh.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kox.ppjwa.cn

[U61] PHP：正则
来源：http://tbv.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ghn.haohaochexian.top

[U62] PHP：日期对象
来源：http://yyx.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fwl.quarkkingdee.top

[U63] PHP：文件读写
来源：http://xbm.jqgfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ltq.yj20258.top

[U64] PHP：目录遍历
来源：http://kjb.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://uaz.uphjek.com

[U65] PHP：会话
来源：http://vns.xinyue.icu

session_start();  $_SESSION["uid"] = 1;
来源：http://gfv.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://prn.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kbg.ivvv.top

[U67] PHP：处理文件上传
来源：http://fhq.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vpl.ybcxt.top

[U68] PHP：PDO 连接
来源：http://cvu.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rnh.pengpengdd.cyou


<!-- 参考信息 -->