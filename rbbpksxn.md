代发 wailian999

while (std::getline(in, line)) { }
来源：http://qeu.gzhubu.top

[S49] C++：写文件
来源：http://pfz.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xds.jinqigfzy.top

[S50] C++：格式化数字
来源：http://kef.tianlin.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rtl.zdqjudy.top

[S51] C++：显式类型转换
来源：http://mlb.guowangkeji.top

static_cast<double>(a) / b
来源：http://snx.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://fbg.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://une.shangyingyoupin.top

[S53] C++：移动语义
来源：http://qcv.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://yrx.vqdsnc.cn

[S54] C++：异常处理
来源：http://dsx.zhongyouzk.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tsk.andypj.xyz

[S55] C++：结构化绑定
来源：http://zkr.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ary.havefunace.top

[S56] C++：optional
来源：http://vrj.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://emu.hnxiangtu.top

[S57] C++：编译期常量
来源：http://jrh.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://uaw.fktsv.cn

[S58] C++：命名空间
来源：http://jdh.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://hec.pycfn.com

[S59] C++：静态断言
来源：http://rqq.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://afj.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://foh.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cfg.cdnleiting.top

================================================================================
来源：http://vfv.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://syk.zhongyouzk.top

================================================================================
来源：http://tbl.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://bim.nwbrower.top

println("Hello")
来源：http://ney.zycfv.cn

[T02] Kotlin：变量
来源：http://pxf.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zoe.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://luf.nanxuanxn.top

"值: $b"
来源：http://kbp.yvedp.cn

[T04] Kotlin：空安全
来源：http://idd.hysaishi.cn

val n: String? = null;  n?.length
来源：http://vxp.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://mam.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://snv.havefunace.top

[T06] Kotlin：集合映射
来源：http://rno.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bgu.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://myi.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lgu.c1oappe.top

[T08] Kotlin：数据类
来源：http://qzv.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://bgf.316326.xyz

[T09] Kotlin：扩展函数
来源：http://hce.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://mxa.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://ynf.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iyr.yanxiufei.cn

[T11] Kotlin：协程
来源：http://kuk.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://tfm.c1oappe.top

[T12] Kotlin：解构声明
来源：http://mlp.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://ilw.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://vsc.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://hew.52xcode.cn

[T14] Kotlin：循环
来源：http://lfj.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://qay.nwbrower.top

[T15] Kotlin：接口
来源：http://epf.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://rlf.jinqigufen.top

[T16] Swift：Hello World
来源：http://fba.havefunace.top

print("Hello")
来源：http://ptm.0kj1m.cn

[T17] Swift：变量与常量
来源：http://qrn.chenlongwang.top

var a = 1;  let b = 2
来源：http://sed.uphjek.com

[T18] Swift：字符串插值
来源：http://hhl.shanyushiyangkeji.top

"值: \(b)"
来源：http://fnm.andypj.xyz

[T19] Swift：可选绑定
来源：http://fbz.jqgufenzy.top

if let n = opt { print(n) }
来源：http://dvh.ctjpmb.com

[T20] Swift：数组操作
来源：http://ayz.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://kjz.ppjwa.cn

[T21] Swift：遍历
来源：http://fap.0kj1m.cn

for x in a { print(x) }
来源：http://kcw.gaohongyu789.top

[T22] Swift：字典
来源：http://lde.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://bwa.hongshengwenyu.top

[T23] Swift：函数
来源：http://swn.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bma.chenjidiqi.icu

[T24] Swift：闭包
来源：http://gjf.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://noc.hfpthk.cn

[T25] Swift：结构体
来源：http://yqe.cqqwz.cn

struct P { var x: Int }
来源：http://iws.xziqi.cn

[T26] Swift：类与重写
来源：http://tik.epnwcf.com

class A: Base { override func f() {} }
来源：http://gnk.tanke756.top

[T27] Swift：错误处理
来源：http://zbe.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://bpq.yonumen.top

[T28] Swift：枚举
来源：http://ica.ydjk.org.cn

enum Color { case red, green }
来源：http://udj.yonumen.top

[T29] Swift：guard 提前返回
来源：http://bkj.sjlbkw.cn

guard let x = opt else { return }
来源：http://mns.jinghuilouyu.cn

[T30] Swift：协议
来源：http://zhf.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://hpe.yuxming.cn

[T31] Lua：Hello World
来源：http://qnc.jqgfzy.top

print("Hello")
来源：http://rzg.smart0.xyz

[T32] Lua：局部变量
来源：http://kqz.uphjek.com

local a = 1
来源：http://aka.daxiang520.top

[T33] Lua：表（数组）
来源：http://drv.cucudq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kji.sweek.top

[T34] Lua：遍历表
来源：http://sxc.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gle.ctjpmb.com

[T35] Lua：字典表
来源：http://sfp.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://ntk.cqqwz.cn

[T36] Lua：函数
来源：http://jtz.sweek.top

function add(a, b) return a + b end
来源：http://cmz.birdmap.top

[T37] Lua：字符串拼接
来源：http://evb.chenjidiqi.icu

"a" .. "b"
来源：http://mvw.birdmap.top

[T38] Lua：条件
来源：http://bfd.jinqigufen.top

if x > 0 then print("正") end
来源：http://vyd.zdqjudy.top

[T39] Lua：模式匹配
来源：http://civ.tian-w.cn

string.find(s, "%d+")
来源：http://mfm.gogol.net.cn

[T40] Lua：元表
来源：http://vzr.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://okx.fzhhl.top

[T41] Perl：Hello World
来源：http://ssj.c1oappe.top

print "Hello\n";
来源：http://mfj.yuanzhike.top

[T42] Perl：变量类型
来源：http://efd.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jeg.jlsjyb.cn

[T43] Perl：字符串插值
来源：http://fte.pycfn.com

"值: $a"
来源：http://jkn.yonumen.top

[T44] Perl：条件
来源：http://fqj.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://ywk.aibaodan.cn

[T45] Perl：数组遍历
来源：http://ktw.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://yby.smart0.xyz

[T46] Perl：哈希操作
来源：http://ohl.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rwm.yangfankeji.com

[T47] Perl：正则捕获
来源：http://byy.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://odk.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://ilj.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://uyn.wangdashe.top

[T49] Perl：函数
来源：http://osc.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ftz.tian-w.cn

[T50] Perl：逐行读文件
来源：http://lfy.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://isv.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://pcl.wangdashe.top

[T51] Scala：Hello World
来源：http://pyn.zhoulong.xyz

println("Hello")
来源：http://xgc.fehbvm.com

[T52] Scala：变量
来源：http://soy.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://vte.yuxming.cn

[T53] Scala：字符串插值
来源：http://gsl.xingfuxueyuan.xyz

s"值: $b"
来源：http://zrn.dianchejie.cn

[T54] Scala：集合映射
来源：http://vdl.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://jao.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://ozg.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://ppm.tanke756.top

[T56] Scala：样例类
来源：http://qwu.yj202588.top

case class User(name: String, age: Int)
来源：http://rso.jqgfzy.top

[T57] Scala：模式匹配
来源：http://mbo.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xab.sufxvd.cn

[T58] Scala：函数定义
来源：http://nre.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://svv.quarkkingdee.top

[T59] Scala：循环
来源：http://oab.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://klz.zhijiandao.cn

[T60] Scala：折叠
来源：http://tkt.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gkn.zdbjq.cn

================================================================================
来源：http://fqf.hnxiangtu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tbb.dianchejie.cn

================================================================================
来源：http://kpo.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://qeo.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://kpj.hongshengwenyu.top

[U02] Py：导出 / 安装依赖
来源：http://qyy.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://buf.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://nnf.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nvf.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://rnn.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eat.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://yie.aizwys.cn

list(dict.fromkeys(arr))
来源：http://iry.gzhubu.top

[U06] Py：合并两个字典
来源：http://gnf.xingfuxueyuan.xyz

{**a, **b}
来源：http://wwp.shanyushiyangkeji.top

[U07] Py：反转字典键值
来源：http://hmh.wangdashe.top

{v: k for k, v in d.items()}
来源：http://avj.daria6918.cn

[U08] Py：展平二维列表
来源：http://exz.fengsongda.top

[y for x in nested for y in x]
来源：http://bof.uphjek.com

[U09] Py：字典取最大值的键
来源：http://fgl.jqgfzy.top

max(d, key=d.get)
来源：http://mlg.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://vye.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://srn.redwolf501.top

[U11] Py：生成器表达式
来源：http://gmd.shzxlz.cn

(x * 2 for x in arr)
来源：http://fsk.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://jbi.epnwcf.com

Counter(arr).most_common(3)
来源：http://nzy.yj20258.top

[U13] Py：固定长度队列
来源：http://ahd.sweek.top

deque(maxlen=10)
来源：http://ikh.sweek.top

[U14] Py：分组收集到列表
来源：http://oms.jyoumei.cn

defaultdict(list)
来源：http://xfu.havefunace.top

[U15] Py：高精度计时
来源：http://fge.jqgufenzy.top

t = time.perf_counter()
来源：http://lrp.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://oic.aibaodan.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tei.cheryme.top

[U17] Py：初始化日志
来源：http://ght.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://jlw.cashguo.top

[U18] Py：预编译正则
来源：http://bjo.yongpay.top

pat = re.compile(r"\d+")
来源：http://mib.aizwys.cn

[U19] Py：正则替换带回调
来源：http://upx.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cry.daria6918.cn

[U20] Py：缓存函数结果
来源：http://kxt.hnxiangtu.top

@functools.lru_cache(maxsize=None)
来源：http://jzn.fzhhl.top

[U21] Py：自定义上下文管理器
来源：http://fyy.ybcxt.top

@contextlib.contextmanager
来源：http://nfv.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://rfl.nanxuanxn.top

list(zip(*m))
来源：http://mqc.chenzaomai.com

[U23] Py：分块读取大文件
来源：http://jsi.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vpb.tanke756.top

[U24] Py：路径操作
来源：http://emb.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bei.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://nuj.hammf.cn

csv.DictReader(f)
来源：http://mmi.havefunace.top

[U26] Py：并发下载
来源：http://huo.ehwqpu.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://etp.bbcook.cn

[U27] Py：异步 HTTP
来源：http://hyp.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://gri.sysykeji.top

[U28] Py：类型别名
来源：http://snk.jlsjyb.cn

UserId = int
来源：http://gck.birdmap.top

[U29] Py：属性校验
来源：http://xge.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://ueo.snrcjt.cn

[U30] Py：数据类
来源：http://chu.birdmap.top

@dataclass(slots=True)
来源：http://jjv.pycfn.com

[U31] Py：单测
来源：http://lch.guannengcc.top

python -m pytest -q
来源：http://bzf.yueranfly.top

[U32] Py：代码格式化
来源：http://sts.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://hwz.sxryk.cn

[U33] Py：打包发布
来源：http://pmu.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://yfo.cashguo.top

[U34] Py：判断编码
来源：http://zaa.shuidangran.top

chardet.detect(raw)
来源：http://hwi.jlsjyb.cn

[U35] Py：发送邮件
来源：http://gnq.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nbw.yuanzhike.top

[U36] Py：定时任务
来源：http://kzx.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://cot.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://eck.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://jfo.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://fpe.zhaomingkeji.xyz

Path(__file__).resolve().parent
来源：http://uwh.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://utw.snrcjt.cn

sys.stdout.isatty()
来源：http://tkl.wangshuangyany.cn

[U40] Py：打印到标准错误
来源：http://tsl.yueranfly.top

print("err", file=sys.stderr)
来源：http://aam.cucudq.cn

[U41] PHP：初始化 Composer 项目
来源：http://qny.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rsy.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://jbw.xinyue.icu

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iyr.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://foo.jinqigfzy.top

namespace App\Http;
来源：http://kpk.yonumen.top

[U44] PHP：开启严格类型
来源：http://esw.uphjek.com

declare(strict_types=1);
来源：http://qsb.jlsjyb.cn

[U45] PHP：类型声明与返回类型
来源：http://blb.jlsjyb.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://znx.bjfxy.top

[U46] PHP：可空类型
来源：http://ocf.gzhubu.top

?string $name = null
来源：http://cbp.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://mnz.svipenyu.cn

int|string $id
来源：http://ozr.fengsongda.top

[U48] PHP：纯枚举
来源：http://oye.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vkn.svipenyu.cn

[U49] PHP：只读属性
来源：http://vgy.xylfe.cn

public readonly string $name
来源：http://plf.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://hji.pycfn.com

public function __construct(private int $id) {}
来源：http://ijt.aibaodan.cn

[U51] PHP：数组解构
来源：http://zwh.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://aig.jyoumei.cn

[U52] PHP：箭头函数
来源：http://gkm.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://xiw.hesvh.cn

[U53] PHP：空合并运算符
来源：http://fme.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://zjl.snrcjt.cn

[U54] PHP：空安全调用
来源：http://jez.jlsjyb.cn

$obj?->method()
来源：http://uls.ydzc1.top

[U55] PHP：match 表达式
来源：http://bsz.jinyuanbaomall.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cqe.gogol.net.cn

[U56] PHP：命名参数
来源：http://yqz.fehbvm.com

f(a: 1, b: 2)
来源：http://ltm.xinyue.icu

[U57] PHP：字符串插值
来源：http://ojk.fehbvm.com

"值: {$a}"
来源：http://kiv.yongpay.top

[U58] PHP：数组三件套
来源：http://lkt.cheryme.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vpw.hesvh.cn

[U59] PHP：自定义排序
来源：http://vbg.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sch.nanxinkj.top

[U60] PHP：JSON 编解码
来源：http://opq.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jyx.fehbvm.com

[U61] PHP：正则
来源：http://yin.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vqv.snrcjt.cn

[U62] PHP：日期对象
来源：http://eii.shzxlz.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://upp.yvedp.cn

[U63] PHP：文件读写
来源：http://tis.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bof.sxryk.cn

[U64] PHP：目录遍历
来源：http://cwr.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://kxy.fehbvm.com

[U65] PHP：会话
来源：http://bud.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dcc.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://dft.xziqi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://lzr.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://akl.smart0.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sdk.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://qny.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xzv.nwbrower.top

[U69] PHP：PDO 预处理
来源：http://fkj.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mlh.shuidangran.top

[U70] PHP：PDO 事务
来源：http://nft.yangfankeji.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oea.zhongyouzk.top

[U71] PHP：抛出异常
来源：http://mcj.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://snc.yuanzhike.top

[U72] PHP：写错误日志
来源：http://vyn.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://eii.aibaodan.cn

[U73] PHP：读取 ini 配置
来源：http://vic.fengsongda.top

parse_ini_file("config.ini", true)
来源：http://nam.fzhhl.top

[U74] PHP：读取环境变量
来源：http://ytu.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://zsw.yueranfly.top


<!-- 参考信息 -->