代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://jzi.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oie.gotoacloud.top

[S48] C++：逐行读文件
来源：http://zma.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://qmb.ydzc1.top

while (std::getline(in, line)) { }
来源：http://syz.gotoacloud.top

[S49] C++：写文件
来源：http://zct.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nst.nanxuanxn.top

[S50] C++：格式化数字
来源：http://aic.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wrc.wangdashe.top

[S51] C++：显式类型转换
来源：http://eby.ctjpmb.com

static_cast<double>(a) / b
来源：http://gwk.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://amr.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://dar.snrcjt.cn

[S53] C++：移动语义
来源：http://zsb.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://xrr.sweek.top

[S54] C++：异常处理
来源：http://nmw.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wae.ydzc1.top

[S55] C++：结构化绑定
来源：http://dib.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lwk.yueranfly.top

[S56] C++：optional
来源：http://ziu.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gcf.gzhubu.top

[S57] C++：编译期常量
来源：http://hkr.jyoumei.cn

constexpr int N = 10;
来源：http://orp.kuanghao11.cn

[S58] C++：命名空间
来源：http://eqr.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://kax.jianghu66.top

[S59] C++：静态断言
来源：http://qnu.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqh.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://wjq.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dbj.9152youxi.cn

================================================================================
来源：http://sqe.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rng.gotoacloud.top

================================================================================
来源：http://fpu.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://pai.tarul.cn

println("Hello")
来源：http://fxd.wangdashe.top

[T02] Kotlin：变量
来源：http://rwt.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cxq.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://gur.hongshengwenyu.top

"值: $b"
来源：http://tll.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://zva.nanxinkj.top

val n: String? = null;  n?.length
来源：http://llg.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://aqe.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wjl.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://phk.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://amc.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://tjz.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppp.svipenyu.cn

[T08] Kotlin：数据类
来源：http://cjv.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://mlm.sweek.top

[T09] Kotlin：扩展函数
来源：http://kub.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://bpg.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://bla.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://enh.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://pxw.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ytv.gzhubu.top

[T12] Kotlin：解构声明
来源：http://lvm.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://ixg.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://kli.fehbvm.com

val m = mapOf("a" to 1)
来源：http://sas.sxryk.cn

[T14] Kotlin：循环
来源：http://xot.zycfv.cn

for (i in 1..10) println(i)
来源：http://kni.ehwqpu.com

[T15] Kotlin：接口
来源：http://ypb.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://mcm.andypj.xyz

[T16] Swift：Hello World
来源：http://hxa.chenlongwang.top

print("Hello")
来源：http://dgu.zdqjudy.top

[T17] Swift：变量与常量
来源：http://lfr.bbcook.cn

var a = 1;  let b = 2
来源：http://rsh.cdnleiting.top

[T18] Swift：字符串插值
来源：http://bbp.jiagoushi.top

"值: \(b)"
来源：http://qsi.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://pgj.gogol.net.cn

if let n = opt { print(n) }
来源：http://ryy.yvedp.cn

[T20] Swift：数组操作
来源：http://zgz.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jaw.jianghu66.top

[T21] Swift：遍历
来源：http://pgp.xylfe.cn

for x in a { print(x) }
来源：http://mzd.aizwys.cn

[T22] Swift：字典
来源：http://bov.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://fgk.yonumen.top

[T23] Swift：函数
来源：http://cio.nanxinkj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aew.shzxlz.cn

[T24] Swift：闭包
来源：http://jal.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uvt.yj20258888.top

[T25] Swift：结构体
来源：http://yzu.jinqigfzy.top

struct P { var x: Int }
来源：http://bco.fengsongda.top

[T26] Swift：类与重写
来源：http://ifj.sweek.top

class A: Base { override func f() {} }
来源：http://yqe.zhixingplan.top

[T27] Swift：错误处理
来源：http://baz.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://lkk.xuanzx.com

[T28] Swift：枚举
来源：http://wve.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://qdy.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://ome.hfpthk.cn

guard let x = opt else { return }
来源：http://qeg.meibo888.top

[T30] Swift：协议
来源：http://jcj.tanke756.top

protocol Shape { func area() -> Double }
来源：http://gea.iojbl.cn

[T31] Lua：Hello World
来源：http://asw.yuxming.cn

print("Hello")
来源：http://toz.chenlongwang.top

[T32] Lua：局部变量
来源：http://hfr.andypj.xyz

local a = 1
来源：http://daa.gogol.net.cn

[T33] Lua：表（数组）
来源：http://nok.epnwcf.com

local t = {1, 2, 3};  t[4] = 4
来源：http://azp.jiagoushi.top

[T34] Lua：遍历表
来源：http://nqt.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ebu.cashguo.top

[T35] Lua：字典表
来源：http://rjv.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://wfr.pycfn.com

[T36] Lua：函数
来源：http://hfm.jqgfzy.top

function add(a, b) return a + b end
来源：http://yna.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://awi.kuanghao11.cn

"a" .. "b"
来源：http://jnu.0kj1m.cn

[T38] Lua：条件
来源：http://kof.xylfe.cn

if x > 0 then print("正") end
来源：http://rqo.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://arz.fktsv.cn

string.find(s, "%d+")
来源：http://gjp.snrcjt.cn

[T40] Lua：元表
来源：http://zvk.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://tnx.cqqwz.cn

[T41] Perl：Hello World
来源：http://czk.aibaodan.cn

print "Hello\n";
来源：http://poh.zycfv.cn

[T42] Perl：变量类型
来源：http://plk.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qgr.sufxvd.cn

[T43] Perl：字符串插值
来源：http://okx.316326.xyz

"值: $a"
来源：http://tys.yfazqb.com

[T44] Perl：条件
来源：http://xyr.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://uvz.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://hfh.ppjwa.cn

for my $x (@arr) { print $x; }
来源：http://xwu.ctjpmb.com

[T46] Perl：哈希操作
来源：http://glj.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://roj.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://hwh.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aqm.nwbrower.top

[T48] Perl：正则替换
来源：http://wwm.wangdashe.top

$s =~ s/old/new/g;
来源：http://bdx.andypj.xyz

[T49] Perl：函数
来源：http://pxd.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ahk.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://vqt.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gqf.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://ghn.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://uwq.jyoumei.cn

println("Hello")
来源：http://vcz.xuanzx.com

[T52] Scala：变量
来源：http://fza.quarkkingdee.top

val a = 1;  var b = 2
来源：http://wru.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://ime.bjfxy.top

s"值: $b"
来源：http://dau.zycfv.cn

[T54] Scala：集合映射
来源：http://hak.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://zrf.dashuyun.cn

[T55] Scala：集合过滤
来源：http://dlo.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ycj.yuanzhike.top

[T56] Scala：样例类
来源：http://ein.fengsongda.top

case class User(name: String, age: Int)
来源：http://iqh.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://ogr.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://goh.iojbl.cn

[T58] Scala：函数定义
来源：http://dkb.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://ynt.jqgufenzy.top

[T59] Scala：循环
来源：http://llu.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://cbv.daxiang520.top

[T60] Scala：折叠
来源：http://fzf.9152youxi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://riw.fehbvm.com

================================================================================
来源：http://vza.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://htq.yanxiufei.cn

================================================================================
来源：http://fbm.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://ryn.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fry.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://iij.vqdsnc.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yjc.yfazqb.com

[U03] Py：加载 .env 配置
来源：http://reg.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bnf.jiagoushi.top

[U04] Py：变量调试打印
来源：http://mji.fzhhl.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://aqp.bjfxy.top

[U05] Py：列表去重且保序
来源：http://hnf.jyoumei.cn

list(dict.fromkeys(arr))
来源：http://cwh.hfpthk.cn

[U06] Py：合并两个字典
来源：http://olj.yj20258888.top

{**a, **b}
来源：http://kou.dashuyun.cn

[U07] Py：反转字典键值
来源：http://zoi.ydzc1.top

{v: k for k, v in d.items()}
来源：http://rce.fengsongda.top

[U08] Py：展平二维列表
来源：http://onw.jqgufenzy.top

[y for x in nested for y in x]
来源：http://cpn.yuxming.cn

[U09] Py：字典取最大值的键
来源：http://whn.cheryme.top

max(d, key=d.get)
来源：http://cjq.zhixingplan.top

[U10] Py：按值排序字典
来源：http://rva.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qlr.uphjek.com

[U11] Py：生成器表达式
来源：http://kwf.svipenyu.cn

(x * 2 for x in arr)
来源：http://pze.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://zbu.hywenlv.cn

Counter(arr).most_common(3)
来源：http://cix.gaohongyu789.top

[U13] Py：固定长度队列
来源：http://wpa.hesvh.cn

deque(maxlen=10)
来源：http://oev.havefunace.top

[U14] Py：分组收集到列表
来源：http://keb.hongshengwenyu.top

defaultdict(list)
来源：http://wkf.zhongyouzk.top

[U15] Py：高精度计时
来源：http://gok.hcnkem.com

t = time.perf_counter()
来源：http://ovd.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://qzw.zycfv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ylv.xylfe.cn

[U17] Py：初始化日志
来源：http://sua.jinghuilouyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://zgo.jinqigfzy.top

[U18] Py：预编译正则
来源：http://dks.fengsongda.top

pat = re.compile(r"\d+")
来源：http://tep.kuanghao11.cn

[U19] Py：正则替换带回调
来源：http://uuk.sufxvd.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rbm.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://dhn.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://hev.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://asi.fanxiaobao.xyz

@contextlib.contextmanager
来源：http://kwf.zdbjq.cn

[U22] Py：矩阵转置
来源：http://hnx.ydjk.org.cn

list(zip(*m))
来源：http://zjc.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://nkk.guowangkeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qvl.316326.xyz

[U24] Py：路径操作
来源：http://yya.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pwm.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://fpy.gotoacloud.top

csv.DictReader(f)
来源：http://lef.hammf.cn

[U26] Py：并发下载
来源：http://jjp.smart0.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dsr.xylfe.cn

[U27] Py：异步 HTTP
来源：http://cbr.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://riu.ppjwa.cn

[U28] Py：类型别名
来源：http://qcz.316326.xyz

UserId = int
来源：http://iqw.quarkkingdee.top

[U29] Py：属性校验
来源：http://dge.fzhhl.top

@property 与 @x.setter 配合
来源：http://ezz.haohaochexian.top

[U30] Py：数据类
来源：http://riz.hesvh.cn

@dataclass(slots=True)
来源：http://jvz.jianghu66.top

[U31] Py：单测
来源：http://shv.chenzaomai.com

python -m pytest -q
来源：http://ubi.xuanzx.com

[U32] Py：代码格式化
来源：http://ieq.ydzc1.top

ruff format . && ruff check --fix .
来源：http://pnm.kuanghao11.cn

[U33] Py：打包发布
来源：http://hmr.yueranfly.top

python -m build  （依赖 pyproject.toml）
来源：http://tol.chenjidiqi.icu

[U34] Py：判断编码
来源：http://jpi.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://syy.tarul.cn

[U35] Py：发送邮件
来源：http://lby.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://djn.haohaochexian.top

[U36] Py：定时任务
来源：http://wie.gaohongyu789.top

schedule.every(10).minutes.do(job)
来源：http://doa.cdnleiting.top

[U37] Py：读写 Excel
来源：http://mxr.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://nrw.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://npt.mhx1999.top

Path(__file__).resolve().parent
来源：http://vtl.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://oon.316326.xyz

sys.stdout.isatty()
来源：http://hjk.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://nfl.yj20258888.top

print("err", file=sys.stderr)
来源：http://dbc.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://dqq.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ytn.yuxming.cn

[U42] PHP：PSR-4 自动加载
来源：http://gzn.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rhd.0kj1m.cn

[U43] PHP：声明命名空间
来源：http://dvz.svipenyu.cn

namespace App\Http;
来源：http://riu.smart0.xyz

[U44] PHP：开启严格类型
来源：http://din.hcnkem.com

declare(strict_types=1);
来源：http://jed.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://cmh.jinghuilouyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uco.guannengcc.top

[U46] PHP：可空类型
来源：http://hry.xinyue.icu

?string $name = null
来源：http://cpc.redwolf501.top

[U47] PHP：联合类型
来源：http://ozn.guowangkeji.top

int|string $id
来源：http://uqu.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://vni.yfazqb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ifo.epnwcf.com

[U49] PHP：只读属性
来源：http://eqv.sjlbkw.cn

public readonly string $name
来源：http://uaw.chenlongwang.top

[U50] PHP：构造器属性提升
来源：http://kpu.xinyue.icu

public function __construct(private int $id) {}
来源：http://ici.sjlbkw.cn

[U51] PHP：数组解构
来源：http://ngr.sweek.top

[$a, $b] = $arr;
来源：http://nle.mhx1999.top

[U52] PHP：箭头函数
来源：http://aix.yonumen.top

$double = fn($x) => $x * 2;
来源：http://hqv.jlsjyb.cn

[U53] PHP：空合并运算符
来源：http://twq.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://vgw.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://gqb.xylfe.cn

$obj?->method()
来源：http://ofe.yfazqb.com

[U55] PHP：match 表达式
来源：http://eeb.ctjpmb.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://esf.havefunace.top

[U56] PHP：命名参数
来源：http://zrf.epnwcf.com

f(a: 1, b: 2)
来源：http://suq.cucudq.cn

[U57] PHP：字符串插值
来源：http://axf.ydzc1.top

"值: {$a}"
来源：http://cqk.hnqzz.top

[U58] PHP：数组三件套
来源：http://udo.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dwy.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://zeb.cucudq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://khb.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://bun.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hgd.andypj.xyz

[U61] PHP：正则
来源：http://yhs.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rev.ydzc1.top

[U62] PHP：日期对象
来源：http://afn.sufxvd.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lhe.uphjek.com

[U63] PHP：文件读写
来源：http://nzw.dashuyun.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hvp.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://cwg.jinghuilouyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://qms.zhiwuduotai.top

[U65] PHP：会话
来源：http://agc.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hnm.sxryk.cn

[U66] PHP：设置 Cookie
来源：http://qnr.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fat.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://xdt.zhongyouzk.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nnq.bjfxy.top

[U68] PHP：PDO 连接
来源：http://nkf.9152youxi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vvt.zhengqikj.top

[U69] PHP：PDO 预处理
来源：http://zbg.jinqigufen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ljh.ivvv.top

[U70] PHP：PDO 事务
来源：http://drl.hysaishi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zfc.yuxming.cn

[U71] PHP：抛出异常
来源：http://lip.cheryme.top

throw new RuntimeException("失败", 500);
来源：http://rsf.jinyuanbaomall.cn

[U72] PHP：写错误日志
来源：http://mnv.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://ygv.jinqigfzy.top


<!-- 参考信息 -->