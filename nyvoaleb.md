代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aag.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://wou.haohaochexian.top

static_cast<double>(a) / b
来源：http://lbm.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://dmy.316326.xyz

int size() const noexcept { return n_; }
来源：http://nap.cqqwz.cn

[S53] C++：移动语义
来源：http://rai.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://wkz.fzhhl.top

[S54] C++：异常处理
来源：http://tnh.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ruf.haohaochexian.top

[S55] C++：结构化绑定
来源：http://tkg.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rnu.jinghuilouyu.cn

[S56] C++：optional
来源：http://ran.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rvk.gzhubu.top

[S57] C++：编译期常量
来源：http://utf.zhengqikj.top

constexpr int N = 10;
来源：http://wys.9152youxi.cn

[S58] C++：命名空间
来源：http://bmo.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://pme.xinyue.icu

[S59] C++：静态断言
来源：http://gul.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dht.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://gpl.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mvd.jinyuanbaomall.cn

================================================================================
来源：http://zyr.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jth.yonumen.top

================================================================================
来源：http://nys.cucudq.cn

[T01] Kotlin：Hello World
来源：http://rqd.52xcode.cn

println("Hello")
来源：http://dao.zhengqikj.top

[T02] Kotlin：变量
来源：http://olv.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sir.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://pkn.yangfankeji.com

"值: $b"
来源：http://cfj.cheryme.top

[T04] Kotlin：空安全
来源：http://lha.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://dha.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://asz.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsn.sweek.top

[T06] Kotlin：集合映射
来源：http://jgd.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sly.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://evr.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ssi.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://ebr.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://vvj.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://qwr.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://byv.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://gwg.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://srj.pycfn.com

[T11] Kotlin：协程
来源：http://byg.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eiv.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://gos.xuanzx.com

val (a, b) = Pair(1, 2)
来源：http://omi.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://trm.yj20258888.top

val m = mapOf("a" to 1)
来源：http://ujx.jqgufenzy.top

[T14] Kotlin：循环
来源：http://hbp.hesvh.cn

for (i in 1..10) println(i)
来源：http://olb.meibo888.top

[T15] Kotlin：接口
来源：http://brz.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://sww.9152youxi.cn

[T16] Swift：Hello World
来源：http://jxy.yj202588.top

print("Hello")
来源：http://uva.yongpay.top

[T17] Swift：变量与常量
来源：http://zay.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://fxn.yvedp.cn

[T18] Swift：字符串插值
来源：http://nhp.zdbjq.cn

"值: \(b)"
来源：http://olv.jianghu66.top

[T19] Swift：可选绑定
来源：http://bej.xziqi.cn

if let n = opt { print(n) }
来源：http://wfo.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://gzh.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://fra.hnqzz.top

[T21] Swift：遍历
来源：http://qms.jyoumei.cn

for x in a { print(x) }
来源：http://qum.fanxiaobao.xyz

[T22] Swift：字典
来源：http://yvs.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://bog.yueranfly.top

[T23] Swift：函数
来源：http://trs.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ujp.tanke756.top

[T24] Swift：闭包
来源：http://kem.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://xxx.smart0.xyz

[T25] Swift：结构体
来源：http://syi.0kj1m.cn

struct P { var x: Int }
来源：http://gvz.52xcode.cn

[T26] Swift：类与重写
来源：http://wev.sufxvd.cn

class A: Base { override func f() {} }
来源：http://brb.aizwys.cn

[T27] Swift：错误处理
来源：http://hgp.ivvv.top

do { try f() } catch { print(error) }
来源：http://frz.zhaomingkeji.xyz

[T28] Swift：枚举
来源：http://mbb.nanxinkj.top

enum Color { case red, green }
来源：http://ctx.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://vfb.kuanghao11.cn

guard let x = opt else { return }
来源：http://zfc.jinghuilouyu.cn

[T30] Swift：协议
来源：http://spy.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://biq.pycfn.com

[T31] Lua：Hello World
来源：http://oui.gotoacloud.top

print("Hello")
来源：http://yor.guowangkeji.top

[T32] Lua：局部变量
来源：http://dil.c1oappe.top

local a = 1
来源：http://gej.vehdjk.com

[T33] Lua：表（数组）
来源：http://yfy.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gne.zhengqikj.top

[T34] Lua：遍历表
来源：http://gxd.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://olz.c1oappe.top

[T35] Lua：字典表
来源：http://dxr.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://jid.dashuyun.cn

[T36] Lua：函数
来源：http://eaz.jqgfzy.top

function add(a, b) return a + b end
来源：http://axl.yj20258888.top

[T37] Lua：字符串拼接
来源：http://lfv.shanyushiyangkeji.top

"a" .. "b"
来源：http://pkv.pycfn.com

[T38] Lua：条件
来源：http://igu.hcnkem.com

if x > 0 then print("正") end
来源：http://yjl.sxryk.cn

[T39] Lua：模式匹配
来源：http://mew.fktsv.cn

string.find(s, "%d+")
来源：http://qul.yanxiufei.cn

[T40] Lua：元表
来源：http://fcx.iojbl.cn

setmetatable({}, { __index = base })
来源：http://prp.tianlin.xyz

[T41] Perl：Hello World
来源：http://gwn.jqgufenzy.top

print "Hello\n";
来源：http://ick.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://hie.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rfv.0kj1m.cn

[T43] Perl：字符串插值
来源：http://zxv.yfazqb.com

"值: $a"
来源：http://qjv.wangshuangyany.cn

[T44] Perl：条件
来源：http://lwk.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://ntg.fzhhl.top

[T45] Perl：数组遍历
来源：http://btu.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://upj.aizwys.cn

[T46] Perl：哈希操作
来源：http://oik.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://frt.zycfv.cn

[T47] Perl：正则捕获
来源：http://ubx.nwbrower.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nny.hnxiangtu.top

[T48] Perl：正则替换
来源：http://ybj.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://zgn.uphjek.com

[T49] Perl：函数
来源：http://hxk.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uwm.guannengcc.top

[T50] Perl：逐行读文件
来源：http://sll.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zqv.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://bjz.vqdsnc.cn

[T51] Scala：Hello World
来源：http://sfh.xuanzx.com

println("Hello")
来源：http://agf.shzxlz.cn

[T52] Scala：变量
来源：http://juc.jqgufenzy.top

val a = 1;  var b = 2
来源：http://ahp.shzxlz.cn

[T53] Scala：字符串插值
来源：http://sru.gotoacloud.top

s"值: $b"
来源：http://yvu.gzhubu.top

[T54] Scala：集合映射
来源：http://bqj.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://evw.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://iqy.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://cuz.epnwcf.com

[T56] Scala：样例类
来源：http://zlc.hongshengwenyu.top

case class User(name: String, age: Int)
来源：http://vmc.ivvv.top

[T57] Scala：模式匹配
来源：http://wbq.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nje.mhx1999.top

[T58] Scala：函数定义
来源：http://gio.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://hsp.fanxiaobao.xyz

[T59] Scala：循环
来源：http://sox.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://iwr.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://jvw.feifeiyinyue.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mpi.yueranfly.top

================================================================================
来源：http://yos.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xus.nwbrower.top

================================================================================
来源：http://awa.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://vvu.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zzp.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://umb.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wlz.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://joq.bbcook.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bco.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://joj.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ipo.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://jnp.cheryme.top

list(dict.fromkeys(arr))
来源：http://tgk.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://ams.zhoulong.xyz

{**a, **b}
来源：http://fff.nwbrower.top

[U07] Py：反转字典键值
来源：http://ihc.jianghu66.top

{v: k for k, v in d.items()}
来源：http://tnd.jianghu66.top

[U08] Py：展平二维列表
来源：http://tab.c1oappe.top

[y for x in nested for y in x]
来源：http://kqa.birdmap.top

[U09] Py：字典取最大值的键
来源：http://kfc.yongpay.top

max(d, key=d.get)
来源：http://igl.jinqigufen.top

[U10] Py：按值排序字典
来源：http://jln.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://iyk.fengsongda.top

[U11] Py：生成器表达式
来源：http://ymu.0kj1m.cn

(x * 2 for x in arr)
来源：http://oqz.sufxvd.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gxa.yvedp.cn

Counter(arr).most_common(3)
来源：http://cyt.yuxming.cn

[U13] Py：固定长度队列
来源：http://dsp.svipenyu.cn

deque(maxlen=10)
来源：http://jbi.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://qxo.jqgfzy.top

defaultdict(list)
来源：http://fhg.fengsongda.top

[U15] Py：高精度计时
来源：http://srb.dashuyun.cn

t = time.perf_counter()
来源：http://vxf.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://rjn.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://chs.cashguo.top

[U17] Py：初始化日志
来源：http://wnx.hysaishi.cn

logging.basicConfig(level=logging.INFO)
来源：http://ovd.zhengqikj.top

[U18] Py：预编译正则
来源：http://nrb.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://btz.sweek.top

[U19] Py：正则替换带回调
来源：http://fag.daxiang520.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://war.xylfe.cn

[U20] Py：缓存函数结果
来源：http://kak.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://gdv.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://rbc.shuidangran.top

@contextlib.contextmanager
来源：http://vzd.chenlongwang.top

[U22] Py：矩阵转置
来源：http://vvi.zdbjq.cn

list(zip(*m))
来源：http://szt.c1oappe.top

[U23] Py：分块读取大文件
来源：http://sws.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fkw.hammf.cn

[U24] Py：路径操作
来源：http://bro.cashguo.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pvo.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://ofl.aibaodan.cn

csv.DictReader(f)
来源：http://jvv.pengpengdd.cyou

[U26] Py：并发下载
来源：http://yba.haohaochexian.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tei.shanyushiyangtech.top

[U27] Py：异步 HTTP
来源：http://wjg.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://nhw.xuetiantiany.cn

[U28] Py：类型别名
来源：http://dvz.yongpay.top

UserId = int
来源：http://ros.jiagoushi.top

[U29] Py：属性校验
来源：http://dav.hnqzz.top

@property 与 @x.setter 配合
来源：http://wpd.yueranfly.top

[U30] Py：数据类
来源：http://bit.shzxlz.cn

@dataclass(slots=True)
来源：http://wvc.havefunace.top

[U31] Py：单测
来源：http://hrt.0kj1m.cn

python -m pytest -q
来源：http://wdd.ehwqpu.com

[U32] Py：代码格式化
来源：http://pcq.zhengqikj.top

ruff format . && ruff check --fix .
来源：http://ciz.redwolf501.top

[U33] Py：打包发布
来源：http://dgl.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://xmp.yuxming.cn

[U34] Py：判断编码
来源：http://qoz.hnqzz.top

chardet.detect(raw)
来源：http://mbc.fehbvm.com

[U35] Py：发送邮件
来源：http://dwe.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jiq.c1oappe.top

[U36] Py：定时任务
来源：http://qzt.0kj1m.cn

schedule.every(10).minutes.do(job)
来源：http://rax.zycfv.cn

[U37] Py：读写 Excel
来源：http://sjt.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://gnj.zhijiandao.cn

[U38] Py：获取脚本所在目录
来源：http://ylf.zycfv.cn

Path(__file__).resolve().parent
来源：http://deh.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://uwm.yj20258888.top

sys.stdout.isatty()
来源：http://jli.uphjek.com

[U40] Py：打印到标准错误
来源：http://cxm.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://fxt.hysaishi.cn

[U41] PHP：初始化 Composer 项目
来源：http://gdp.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://udq.ybcxt.top

[U42] PHP：PSR-4 自动加载
来源：http://lws.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jae.redwolf501.top

[U43] PHP：声明命名空间
来源：http://ebh.chenzaomai.com

namespace App\Http;
来源：http://oxg.cashguo.top

[U44] PHP：开启严格类型
来源：http://dql.yj20258888.top

declare(strict_types=1);
来源：http://yae.aizwys.cn

[U45] PHP：类型声明与返回类型
来源：http://jok.hywenlv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gbk.yongpay.top

[U46] PHP：可空类型
来源：http://frg.hongshengwenyu.top

?string $name = null
来源：http://bjr.cashguo.top

[U47] PHP：联合类型
来源：http://que.ydjk.org.cn

int|string $id
来源：http://cum.daria6918.cn

[U48] PHP：纯枚举
来源：http://oro.ydjk.org.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uit.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://upa.sweek.top

public readonly string $name
来源：http://jhg.iojbl.cn

[U50] PHP：构造器属性提升
来源：http://iks.pycfn.com

public function __construct(private int $id) {}
来源：http://yzg.yonumen.top

[U51] PHP：数组解构
来源：http://ccd.andypj.xyz

[$a, $b] = $arr;
来源：http://jvv.nwbrower.top

[U52] PHP：箭头函数
来源：http://wss.xingfuxueyuan.xyz

$double = fn($x) => $x * 2;
来源：http://exi.yfazqb.com

[U53] PHP：空合并运算符
来源：http://tgg.cucudq.cn

$v = $a ?? $b ?? "default";
来源：http://kkt.xylfe.cn

[U54] PHP：空安全调用
来源：http://pbj.jinghuilouyu.cn

$obj?->method()
来源：http://iku.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://xnb.jianghu66.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tgf.fzhhl.top

[U56] PHP：命名参数
来源：http://sov.nanxuanxn.top

f(a: 1, b: 2)
来源：http://sfz.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://cha.c1oappe.top

"值: {$a}"
来源：http://rao.nwbrower.top

[U58] PHP：数组三件套
来源：http://okb.ybcxt.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qju.xinyue.icu

[U59] PHP：自定义排序
来源：http://ppb.bbcook.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mfj.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://jnh.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zha.daria6918.cn

[U61] PHP：正则
来源：http://xsu.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://soq.sweek.top

[U62] PHP：日期对象
来源：http://tqh.0kj1m.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qge.zycfv.cn

[U63] PHP：文件读写
来源：http://ajf.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lhr.haohaochexian.top

[U64] PHP：目录遍历
来源：http://ywj.fehbvm.com

glob("dir/*.php");  scandir("dir");
来源：http://lws.cqqwz.cn

[U65] PHP：会话
来源：http://izl.haohaochexian.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hdl.dashuyun.cn

[U66] PHP：设置 Cookie
来源：http://ybr.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kxw.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://uso.gogol.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zkb.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://zas.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rah.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://lvg.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://eof.316326.xyz

[U70] PHP：PDO 事务
来源：http://tvl.yj20258888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fqo.daria6918.cn

[U71] PHP：抛出异常
来源：http://xrv.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://brk.ppjwa.cn

[U72] PHP：写错误日志
来源：http://cma.yj20258888.top

error_log("失败: " . $e->getMessage());
来源：http://msh.cdnleiting.top

[U73] PHP：读取 ini 配置
来源：http://kev.nanxuanxn.top

parse_ini_file("config.ini", true)
来源：http://wop.pengpengdd.cyou

[U74] PHP：读取环境变量
来源：http://wxn.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://yjo.sweek.top

[U75] PHP：依赖注入
来源：http://lrv.hywenlv.cn

composer require psr/container
来源：http://inv.haohaochexian.top

[U76] PHP：简单路由
来源：http://mqq.aibaodan.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lbr.tian-w.cn


<!-- 参考信息 -->