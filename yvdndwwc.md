代发 wailian999

while (std::getline(in, line)) { }
来源：http://gfu.cheryme.top

[S49] C++：写文件
来源：http://bqp.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://msw.dashuyun.cn

[S50] C++：格式化数字
来源：http://stf.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hwx.chenzaomai.com

[S51] C++：显式类型转换
来源：http://oin.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://htv.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://wym.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://ypd.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://gyp.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://voj.epnwcf.com

[S54] C++：异常处理
来源：http://ebv.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zen.dianchejie.cn

[S55] C++：结构化绑定
来源：http://bhy.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hbn.bjfxy.top

[S56] C++：optional
来源：http://pfr.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jxj.svipenyu.cn

[S57] C++：编译期常量
来源：http://uwj.xylfe.cn

constexpr int N = 10;
来源：http://ual.wangdashe.top

[S58] C++：命名空间
来源：http://ktv.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://otv.hammf.cn

[S59] C++：静态断言
来源：http://dlw.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mzg.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://xhw.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vlv.cashguo.top

================================================================================
来源：http://kto.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://muz.fengsongda.top

================================================================================
来源：http://ksx.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://uzs.meibo888.top

println("Hello")
来源：http://cht.yanxiufei.cn

[T02] Kotlin：变量
来源：http://wxq.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jda.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://qys.xuanzx.com

"值: $b"
来源：http://xue.xuanzx.com

[T04] Kotlin：空安全
来源：http://lxv.cqqwz.cn

val n: String? = null;  n?.length
来源：http://rnd.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://jzo.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kin.yonumen.top

[T06] Kotlin：集合映射
来源：http://iot.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vlt.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://bus.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lvd.bjfxy.top

[T08] Kotlin：数据类
来源：http://skp.uphjek.com

data class User(val name: String, val age: Int)
来源：http://iwz.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://lps.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://rnm.zycfv.cn

[T10] Kotlin：默认参数
来源：http://kfu.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://mba.wangdashe.top

[T11] Kotlin：协程
来源：http://aoy.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://guf.yongpay.top

[T12] Kotlin：解构声明
来源：http://fqd.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://ayr.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://cwj.vehdjk.com

val m = mapOf("a" to 1)
来源：http://dmm.ybcxt.top

[T14] Kotlin：循环
来源：http://lac.yj202588.top

for (i in 1..10) println(i)
来源：http://jfw.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://qhj.hnqzz.top

interface Shape { fun area(): Double }
来源：http://iyl.cdnleiting.top

[T16] Swift：Hello World
来源：http://oeh.316326.xyz

print("Hello")
来源：http://mwc.guowangkeji.top

[T17] Swift：变量与常量
来源：http://slq.uphjek.com

var a = 1;  let b = 2
来源：http://pld.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://wcb.jiagoushi.top

"值: \(b)"
来源：http://mxc.dashuyun.cn

[T19] Swift：可选绑定
来源：http://umz.hnqzz.top

if let n = opt { print(n) }
来源：http://epm.yfazqb.com

[T20] Swift：数组操作
来源：http://qhz.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gcz.jinqigfzy.top

[T21] Swift：遍历
来源：http://tyh.fzhhl.top

for x in a { print(x) }
来源：http://fvm.sjlbkw.cn

[T22] Swift：字典
来源：http://ntu.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://xls.52xcode.cn

[T23] Swift：函数
来源：http://eyj.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lyo.chenjidiqi.icu

[T24] Swift：闭包
来源：http://xfz.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ilx.wangshuangyany.cn

[T25] Swift：结构体
来源：http://sny.daria6918.cn

struct P { var x: Int }
来源：http://zgz.52xcode.cn

[T26] Swift：类与重写
来源：http://bcj.c1oappe.top

class A: Base { override func f() {} }
来源：http://dez.yueranfly.top

[T27] Swift：错误处理
来源：http://vgp.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://osx.sxryk.cn

[T28] Swift：枚举
来源：http://zww.pycfn.com

enum Color { case red, green }
来源：http://swb.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://wpx.dashuyun.cn

guard let x = opt else { return }
来源：http://hzg.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://tkn.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://vln.haohaochexian.top

[T31] Lua：Hello World
来源：http://fur.uphjek.com

print("Hello")
来源：http://yao.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://edi.9152youxi.cn

local a = 1
来源：http://wcz.gogol.net.cn

[T33] Lua：表（数组）
来源：http://bhk.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://buu.smart0.xyz

[T34] Lua：遍历表
来源：http://itf.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ett.xziqi.cn

[T35] Lua：字典表
来源：http://qem.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://udx.tianlin.xyz

[T36] Lua：函数
来源：http://odz.pycfn.com

function add(a, b) return a + b end
来源：http://jhh.cashguo.top

[T37] Lua：字符串拼接
来源：http://zlg.fktsv.cn

"a" .. "b"
来源：http://osw.yvedp.cn

[T38] Lua：条件
来源：http://nsb.0kj1m.cn

if x > 0 then print("正") end
来源：http://oly.hesvh.cn

[T39] Lua：模式匹配
来源：http://kqh.sweek.top

string.find(s, "%d+")
来源：http://lit.shuidangran.top

[T40] Lua：元表
来源：http://pbm.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://hrr.shzxlz.cn

[T41] Perl：Hello World
来源：http://rcf.jiagoushi.top

print "Hello\n";
来源：http://cad.yfazqb.com

[T42] Perl：变量类型
来源：http://dtw.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ivl.316326.xyz

[T43] Perl：字符串插值
来源：http://kxo.xziqi.cn

"值: $a"
来源：http://eai.zhixingplan.top

[T44] Perl：条件
来源：http://evt.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://ywc.tanke756.top

[T45] Perl：数组遍历
来源：http://pwm.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://rmi.daxiang520.top

[T46] Perl：哈希操作
来源：http://zxt.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oou.yj202588.top

[T47] Perl：正则捕获
来源：http://nvg.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jvz.yj20258888.top

[T48] Perl：正则替换
来源：http://bmi.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://guh.havefunace.top

[T49] Perl：函数
来源：http://ywp.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://siu.fzhhl.top

[T50] Perl：逐行读文件
来源：http://mom.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://alt.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://hof.fktsv.cn

[T51] Scala：Hello World
来源：http://yis.jinqigfzy.top

println("Hello")
来源：http://slp.sysykeji.top

[T52] Scala：变量
来源：http://mxw.9152youxi.cn

val a = 1;  var b = 2
来源：http://iiq.yangfankeji.com

[T53] Scala：字符串插值
来源：http://axj.andypj.xyz

s"值: $b"
来源：http://mco.sufxvd.cn

[T54] Scala：集合映射
来源：http://enn.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://dwv.shuidangran.top

[T55] Scala：集合过滤
来源：http://gbj.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://ekr.0kj1m.cn

[T56] Scala：样例类
来源：http://yql.jlsjyb.cn

case class User(name: String, age: Int)
来源：http://gyn.tianlin.xyz

[T57] Scala：模式匹配
来源：http://mvm.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ncq.316326.xyz

[T58] Scala：函数定义
来源：http://vkr.hongshengwenyu.top

def add(a: Int, b: Int): Int = a + b
来源：http://ddv.cashguo.top

[T59] Scala：循环
来源：http://vkb.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://chn.sysykeji.top

[T60] Scala：折叠
来源：http://rle.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://plp.xylfe.cn

================================================================================
来源：http://eit.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://naj.zdbjq.cn

================================================================================
来源：http://ztr.yonumen.top

[U01] Py：创建虚拟环境
来源：http://bjh.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://mga.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://iyh.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://toi.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://kxg.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zkv.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://khb.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fpq.bjfxy.top

[U05] Py：列表去重且保序
来源：http://llj.jqgfzy.top

list(dict.fromkeys(arr))
来源：http://cwo.xylfe.cn

[U06] Py：合并两个字典
来源：http://mhf.9152youxi.cn

{**a, **b}
来源：http://jym.dianchejie.cn

[U07] Py：反转字典键值
来源：http://mpt.yongpay.top

{v: k for k, v in d.items()}
来源：http://ddo.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://krh.yueranfly.top

[y for x in nested for y in x]
来源：http://cxh.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://alw.ehwqpu.com

max(d, key=d.get)
来源：http://lqr.cucudq.cn

[U10] Py：按值排序字典
来源：http://gre.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fxn.wangshuangyany.cn

[U11] Py：生成器表达式
来源：http://zzw.sxryk.cn

(x * 2 for x in arr)
来源：http://smg.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://rvc.yuanzhike.top

Counter(arr).most_common(3)
来源：http://ers.shangyingyoupin.top

[U13] Py：固定长度队列
来源：http://ffw.guannengcc.top

deque(maxlen=10)
来源：http://rqw.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://fay.yj20258.top

defaultdict(list)
来源：http://vlh.epnwcf.com

[U15] Py：高精度计时
来源：http://myt.tarul.cn

t = time.perf_counter()
来源：http://rhx.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://erq.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ulh.hfpthk.cn

[U17] Py：初始化日志
来源：http://yrk.zhaomingkeji.xyz

logging.basicConfig(level=logging.INFO)
来源：http://rnm.cashguo.top

[U18] Py：预编译正则
来源：http://meh.cucudq.cn

pat = re.compile(r"\d+")
来源：http://gms.shangyingyoupin.top

[U19] Py：正则替换带回调
来源：http://zpn.epnwcf.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hfg.zhoulong.xyz

[U20] Py：缓存函数结果
来源：http://ttk.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://llf.xuanzx.com

[U21] Py：自定义上下文管理器
来源：http://nxn.fehbvm.com

@contextlib.contextmanager
来源：http://itb.316326.xyz

[U22] Py：矩阵转置
来源：http://jme.shanyushiyangtech.top

list(zip(*m))
来源：http://ncn.tianlin.xyz

[U23] Py：分块读取大文件
来源：http://oxa.yj202588.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vux.meibo888.top

[U24] Py：路径操作
来源：http://tgu.hesvh.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iyn.ybcxt.top

[U25] Py：CSV 按字典读
来源：http://gsa.smart0.xyz

csv.DictReader(f)
来源：http://fiy.hfpthk.cn

[U26] Py：并发下载
来源：http://tmw.ctjpmb.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wvo.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://ybc.zhiwuduotai.top

aiohttp.ClientSession() 配合 async with
来源：http://bld.daxiang520.top

[U28] Py：类型别名
来源：http://tpz.zhengqikj.top

UserId = int
来源：http://dyy.gaohongyu789.top

[U29] Py：属性校验
来源：http://eio.yuanzhike.top

@property 与 @x.setter 配合
来源：http://axs.ctjpmb.com

[U30] Py：数据类
来源：http://rdo.jqgufenzy.top

@dataclass(slots=True)
来源：http://vbs.yueranfly.top

[U31] Py：单测
来源：http://jgn.ehwqpu.com

python -m pytest -q
来源：http://tix.xuanzx.com

[U32] Py：代码格式化
来源：http://xkv.vehdjk.com

ruff format . && ruff check --fix .
来源：http://aim.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://tcw.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://jyq.yuxming.cn

[U34] Py：判断编码
来源：http://kgi.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://dyn.hfpthk.cn

[U35] Py：发送邮件
来源：http://yqa.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mbr.daxiang520.top

[U36] Py：定时任务
来源：http://tex.ywan-chungtsiang.top

schedule.every(10).minutes.do(job)
来源：http://qpk.zhiwuduotai.top

[U37] Py：读写 Excel
来源：http://hxq.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://dcc.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://sje.tianlin.xyz

Path(__file__).resolve().parent
来源：http://vyu.feifeiyinyue.top

[U39] Py：判断是否在交互环境
来源：http://yaf.haohaochexian.top

sys.stdout.isatty()
来源：http://qnc.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://zkw.xinyue.icu

print("err", file=sys.stderr)
来源：http://owc.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://nhh.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://clt.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://kks.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://myw.vehdjk.com

[U43] PHP：声明命名空间
来源：http://fhc.guannengcc.top

namespace App\Http;
来源：http://nxl.hysaishi.cn

[U44] PHP：开启严格类型
来源：http://xog.hnqzz.top

declare(strict_types=1);
来源：http://vof.pycfn.com

[U45] PHP：类型声明与返回类型
来源：http://dqk.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://okm.zhoulong.xyz

[U46] PHP：可空类型
来源：http://zoc.nanxuanxn.top

?string $name = null
来源：http://iyp.ctjpmb.com

[U47] PHP：联合类型
来源：http://hju.bbcook.cn

int|string $id
来源：http://hic.smart0.xyz

[U48] PHP：纯枚举
来源：http://kgd.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bho.pycfn.com

[U49] PHP：只读属性
来源：http://bno.wangdashe.top

public readonly string $name
来源：http://tdg.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://avf.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://ryb.epnwcf.com

[U51] PHP：数组解构
来源：http://xuw.jqgfzy.top

[$a, $b] = $arr;
来源：http://cis.316326.xyz

[U52] PHP：箭头函数
来源：http://hci.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://rpo.nanxinkj.top

[U53] PHP：空合并运算符
来源：http://eaa.gogol.net.cn

$v = $a ?? $b ?? "default";
来源：http://pkm.epnwcf.com

[U54] PHP：空安全调用
来源：http://snk.uphjek.com

$obj?->method()
来源：http://ckh.smart0.xyz

[U55] PHP：match 表达式
来源：http://zvc.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vvy.yonumen.top

[U56] PHP：命名参数
来源：http://zmb.daria6918.cn

f(a: 1, b: 2)
来源：http://qbp.nwbrower.top

[U57] PHP：字符串插值
来源：http://zcv.kuanghao11.cn

"值: {$a}"
来源：http://hqz.hongshengwenyu.top

[U58] PHP：数组三件套
来源：http://rqu.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lar.hywenlv.cn

[U59] PHP：自定义排序
来源：http://lqo.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uke.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://dei.dianchejie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fmq.yj20258.top

[U61] PHP：正则
来源：http://gnf.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sfz.zhengqikj.top

[U62] PHP：日期对象
来源：http://nws.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nmi.jyoumei.cn

[U63] PHP：文件读写
来源：http://otj.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bdu.wangdashe.top

[U64] PHP：目录遍历
来源：http://tlu.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://yvv.gogol.net.cn

[U65] PHP：会话
来源：http://ufw.gotoacloud.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jfu.hfpthk.cn

[U66] PHP：设置 Cookie
来源：http://cto.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iuz.xuanzx.com

[U67] PHP：处理文件上传
来源：http://pxc.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ifl.bbcook.cn

[U68] PHP：PDO 连接
来源：http://tdj.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tto.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://nrv.yuxming.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eua.yuxming.cn

[U70] PHP：PDO 事务
来源：http://tia.bbcook.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qxv.xylfe.cn

[U71] PHP：抛出异常
来源：http://nkp.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://fiv.c1oappe.top

[U72] PHP：写错误日志
来源：http://tcp.zhoulong.xyz

error_log("失败: " . $e->getMessage());
来源：http://ekb.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://uxf.cashguo.top

parse_ini_file("config.ini", true)
来源：http://cuu.hammf.cn

[U74] PHP：读取环境变量
来源：http://tes.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://oau.zycfv.cn


<!-- 参考信息 -->