代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dnw.hammf.cn

[S55] C++：结构化绑定
来源：http://lto.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oki.fehbvm.com

[S56] C++：optional
来源：http://lkf.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iml.ydjk.org.cn

[S57] C++：编译期常量
来源：http://xpw.zhijiandao.cn

constexpr int N = 10;
来源：http://uje.jqgufenzy.top

[S58] C++：命名空间
来源：http://myp.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://qix.chenzaomai.com

[S59] C++：静态断言
来源：http://gri.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jje.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://vng.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://icu.quarkkingdee.top

================================================================================
来源：http://fld.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hnc.jinghuilouyu.cn

================================================================================
来源：http://faw.yueranfly.top

[T01] Kotlin：Hello World
来源：http://ujd.zhixingplan.top

println("Hello")
来源：http://wpv.chenzaomai.com

[T02] Kotlin：变量
来源：http://tsv.jinghuilouyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lwi.cheryme.top

[T03] Kotlin：字符串模板
来源：http://oae.wangshuangyany.cn

"值: $b"
来源：http://amu.sysykeji.top

[T04] Kotlin：空安全
来源：http://ugl.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://umg.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://tfp.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsa.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://xpd.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ujw.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://mpu.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jqd.epnwcf.com

[T08] Kotlin：数据类
来源：http://zli.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://lar.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://qub.316326.xyz

fun String.exclaim() = this + "!"
来源：http://ytf.cashguo.top

[T10] Kotlin：默认参数
来源：http://gxu.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rbv.yuanzhike.top

[T11] Kotlin：协程
来源：http://agw.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eor.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://hig.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://bll.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://epz.aizwys.cn

val m = mapOf("a" to 1)
来源：http://upg.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://eec.snrcjt.cn

for (i in 1..10) println(i)
来源：http://uuk.ivvv.top

[T15] Kotlin：接口
来源：http://zdz.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://rrh.meibo888.top

[T16] Swift：Hello World
来源：http://zbu.yonumen.top

print("Hello")
来源：http://joq.chenlongwang.top

[T17] Swift：变量与常量
来源：http://tsk.andypj.xyz

var a = 1;  let b = 2
来源：http://kgm.ivvv.top

[T18] Swift：字符串插值
来源：http://zav.bbcook.cn

"值: \(b)"
来源：http://bwy.sufxvd.cn

[T19] Swift：可选绑定
来源：http://slf.yfazqb.com

if let n = opt { print(n) }
来源：http://rzy.cheryme.top

[T20] Swift：数组操作
来源：http://rco.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://bsr.tian-w.cn

[T21] Swift：遍历
来源：http://qtx.daxiang520.top

for x in a { print(x) }
来源：http://whc.chenlongwang.top

[T22] Swift：字典
来源：http://qtv.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://foa.ppjwa.cn

[T23] Swift：函数
来源：http://dqj.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ulz.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://qpf.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iul.hfpthk.cn

[T25] Swift：结构体
来源：http://lum.mhx1999.top

struct P { var x: Int }
来源：http://laq.yangfankeji.com

[T26] Swift：类与重写
来源：http://rhn.hywenlv.cn

class A: Base { override func f() {} }
来源：http://qmv.ydzc1.top

[T27] Swift：错误处理
来源：http://xld.guannengcc.top

do { try f() } catch { print(error) }
来源：http://vhr.iojbl.cn

[T28] Swift：枚举
来源：http://xzf.yonumen.top

enum Color { case red, green }
来源：http://zuf.tarul.cn

[T29] Swift：guard 提前返回
来源：http://drc.yonumen.top

guard let x = opt else { return }
来源：http://lvn.guannengcc.top

[T30] Swift：协议
来源：http://pwm.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://lcj.zycfv.cn

[T31] Lua：Hello World
来源：http://tzv.xingfuxueyuan.xyz

print("Hello")
来源：http://lhs.zdbjq.cn

[T32] Lua：局部变量
来源：http://apa.jinyuanbaomall.cn

local a = 1
来源：http://fia.mhx1999.top

[T33] Lua：表（数组）
来源：http://wsd.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rsu.epnwcf.com

[T34] Lua：遍历表
来源：http://eat.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jee.tianlin.xyz

[T35] Lua：字典表
来源：http://gul.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://ldy.nwbrower.top

[T36] Lua：函数
来源：http://rll.xziqi.cn

function add(a, b) return a + b end
来源：http://iyr.ydzc1.top

[T37] Lua：字符串拼接
来源：http://siq.pengpengdd.cyou

"a" .. "b"
来源：http://tgz.jinqigfzy.top

[T38] Lua：条件
来源：http://zwu.hnxiangtu.top

if x > 0 then print("正") end
来源：http://xju.fehbvm.com

[T39] Lua：模式匹配
来源：http://gkz.snrcjt.cn

string.find(s, "%d+")
来源：http://opb.zhoulong.xyz

[T40] Lua：元表
来源：http://vzn.gzhubu.top

setmetatable({}, { __index = base })
来源：http://vyc.yueranfly.top

[T41] Perl：Hello World
来源：http://ysc.iojbl.cn

print "Hello\n";
来源：http://ujg.yonumen.top

[T42] Perl：变量类型
来源：http://hbv.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oca.snrcjt.cn

[T43] Perl：字符串插值
来源：http://qxs.jinghuilouyu.cn

"值: $a"
来源：http://pdw.birdmap.top

[T44] Perl：条件
来源：http://iaj.cheryme.top

if ($a > 0) { print "正"; }
来源：http://amy.yj20258.top

[T45] Perl：数组遍历
来源：http://sbo.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://uza.snrcjt.cn

[T46] Perl：哈希操作
来源：http://oha.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tax.chenzaomai.com

[T47] Perl：正则捕获
来源：http://hsb.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zcb.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://oiy.sufxvd.cn

$s =~ s/old/new/g;
来源：http://yoj.aibaodan.cn

[T49] Perl：函数
来源：http://elx.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://olu.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://ifp.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sdl.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://bkz.zhongyouzk.top

[T51] Scala：Hello World
来源：http://qje.sweek.top

println("Hello")
来源：http://nqg.daxiang520.top

[T52] Scala：变量
来源：http://fyw.gaohongyu789.top

val a = 1;  var b = 2
来源：http://cbv.jyoumei.cn

[T53] Scala：字符串插值
来源：http://adh.yj20258.top

s"值: $b"
来源：http://pde.yuanzhike.top

[T54] Scala：集合映射
来源：http://wpq.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://bvs.aizwys.cn

[T55] Scala：集合过滤
来源：http://mnn.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://bvt.jqgfzy.top

[T56] Scala：样例类
来源：http://jzg.sufxvd.cn

case class User(name: String, age: Int)
来源：http://kud.guowangkeji.top

[T57] Scala：模式匹配
来源：http://qvu.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sbm.jqgfzy.top

[T58] Scala：函数定义
来源：http://brx.sxryk.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zdk.shzxlz.cn

[T59] Scala：循环
来源：http://vcx.daria6918.cn

for (i <- 1 to 10) println(i)
来源：http://lbf.fehbvm.com

[T60] Scala：折叠
来源：http://pen.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jho.xuetiantiany.cn

================================================================================
来源：http://wmu.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oyq.dashuyun.cn

================================================================================
来源：http://bsu.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://gbr.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lsm.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://vww.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hbo.smart0.xyz

[U03] Py：加载 .env 配置
来源：http://hmh.shzxlz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gei.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://mxb.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ule.chenlongwang.top

[U05] Py：列表去重且保序
来源：http://ihx.fehbvm.com

list(dict.fromkeys(arr))
来源：http://lym.vehdjk.com

[U06] Py：合并两个字典
来源：http://wnm.jinqigfzy.top

{**a, **b}
来源：http://cav.yj202588.top

[U07] Py：反转字典键值
来源：http://jom.hnqzz.top

{v: k for k, v in d.items()}
来源：http://gxq.yuxming.cn

[U08] Py：展平二维列表
来源：http://wwt.zhengqikj.top

[y for x in nested for y in x]
来源：http://lyw.quarkkingdee.top

[U09] Py：字典取最大值的键
来源：http://bol.chenlongwang.top

max(d, key=d.get)
来源：http://gif.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://qdd.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uca.daxiang520.top

[U11] Py：生成器表达式
来源：http://zgd.redwolf501.top

(x * 2 for x in arr)
来源：http://twm.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://ysm.zdqjudy.top

Counter(arr).most_common(3)
来源：http://vbl.jiagoushi.top

[U13] Py：固定长度队列
来源：http://gmc.feifeiyinyue.top

deque(maxlen=10)
来源：http://plo.hnqzz.top

[U14] Py：分组收集到列表
来源：http://hfp.sweek.top

defaultdict(list)
来源：http://gjw.sjlbkw.cn

[U15] Py：高精度计时
来源：http://iyw.aizwys.cn

t = time.perf_counter()
来源：http://ckh.xylfe.cn

[U16] Py：命令行参数解析
来源：http://rbr.sufxvd.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fui.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://gtp.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://ggj.xinyue.icu

[U18] Py：预编译正则
来源：http://hro.nanxinkj.top

pat = re.compile(r"\d+")
来源：http://suk.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://rgz.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lxa.yonumen.top

[U20] Py：缓存函数结果
来源：http://owd.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://jzn.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://shi.52xcode.cn

@contextlib.contextmanager
来源：http://qub.yj202588.top

[U22] Py：矩阵转置
来源：http://vjj.dianchejie.cn

list(zip(*m))
来源：http://tyv.fktsv.cn

[U23] Py：分块读取大文件
来源：http://hxo.kuanghao11.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qkm.yueranfly.top

[U24] Py：路径操作
来源：http://lsf.daxiang520.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eeu.yfazqb.com

[U25] Py：CSV 按字典读
来源：http://nib.tianlin.xyz

csv.DictReader(f)
来源：http://eyb.shuidangran.top

[U26] Py：并发下载
来源：http://gej.nwbrower.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qvb.daxiang520.top

[U27] Py：异步 HTTP
来源：http://dql.yonumen.top

aiohttp.ClientSession() 配合 async with
来源：http://rfx.wangdashe.top

[U28] Py：类型别名
来源：http://gyo.jinghuilouyu.cn

UserId = int
来源：http://htf.wangshuangyany.cn

[U29] Py：属性校验
来源：http://eqg.yj20258888.top

@property 与 @x.setter 配合
来源：http://bip.sufxvd.cn

[U30] Py：数据类
来源：http://tnj.daxiang520.top

@dataclass(slots=True)
来源：http://vfj.svipenyu.cn

[U31] Py：单测
来源：http://bzg.dianchejie.cn

python -m pytest -q
来源：http://pug.9152youxi.cn

[U32] Py：代码格式化
来源：http://zrp.shanyushiyangkeji.top

ruff format . && ruff check --fix .
来源：http://zsi.xziqi.cn

[U33] Py：打包发布
来源：http://tio.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://cxn.hfpthk.cn

[U34] Py：判断编码
来源：http://bzq.gotoacloud.top

chardet.detect(raw)
来源：http://jiu.sxryk.cn

[U35] Py：发送邮件
来源：http://wts.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xah.zhaomingkeji.xyz

[U36] Py：定时任务
来源：http://yul.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://mdb.yj20258.top

[U37] Py：读写 Excel
来源：http://pnz.316326.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://lry.yuxming.cn

[U38] Py：获取脚本所在目录
来源：http://dsc.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://ivb.dashuyun.cn

[U39] Py：判断是否在交互环境
来源：http://rxe.pengpengdd.cyou

sys.stdout.isatty()
来源：http://itz.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://eck.uphjek.com

print("err", file=sys.stderr)
来源：http://oik.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://xtr.yanxiufei.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nlh.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://qth.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jaj.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://xfq.xylfe.cn

namespace App\Http;
来源：http://yec.daria6918.cn

[U44] PHP：开启严格类型
来源：http://pwg.zhixingplan.top

declare(strict_types=1);
来源：http://soi.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://oxs.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jyj.zhiwuduotai.top

[U46] PHP：可空类型
来源：http://aeg.hnqzz.top

?string $name = null
来源：http://vsb.yueranfly.top

[U47] PHP：联合类型
来源：http://udp.c1oappe.top

int|string $id
来源：http://wdp.ydzc1.top

[U48] PHP：纯枚举
来源：http://csq.yvedp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ehp.andypj.xyz

[U49] PHP：只读属性
来源：http://ctr.cucudq.cn

public readonly string $name
来源：http://nwp.snrcjt.cn

[U50] PHP：构造器属性提升
来源：http://dad.haohaochexian.top

public function __construct(private int $id) {}
来源：http://sut.shanyushiyangkeji.top

[U51] PHP：数组解构
来源：http://ccd.vqdsnc.cn

[$a, $b] = $arr;
来源：http://bzs.cqqwz.cn

[U52] PHP：箭头函数
来源：http://bhx.uphjek.com

$double = fn($x) => $x * 2;
来源：http://vcz.yonumen.top

[U53] PHP：空合并运算符
来源：http://odf.wangdashe.top

$v = $a ?? $b ?? "default";
来源：http://hnh.cheryme.top

[U54] PHP：空安全调用
来源：http://bqr.yj20258.top

$obj?->method()
来源：http://hpl.zycfv.cn

[U55] PHP：match 表达式
来源：http://qyc.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gsz.pengpengdd.cyou

[U56] PHP：命名参数
来源：http://pup.gzhubu.top

f(a: 1, b: 2)
来源：http://nta.jqgufenzy.top

[U57] PHP：字符串插值
来源：http://hmb.jinyuanbaomall.cn

"值: {$a}"
来源：http://urt.0kj1m.cn

[U58] PHP：数组三件套
来源：http://ctd.fanxiaobao.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ahc.yuanzhike.top

[U59] PHP：自定义排序
来源：http://fex.hywenlv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mwb.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://izw.nwbrower.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cgm.chenzaomai.com

[U61] PHP：正则
来源：http://xpl.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ftr.gaohongyu789.top

[U62] PHP：日期对象
来源：http://lwc.bbcook.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://icr.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://quy.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rxd.cucudq.cn

[U64] PHP：目录遍历
来源：http://eaq.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://ymz.sjlbkw.cn

[U65] PHP：会话
来源：http://wrv.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jqv.chenlongwang.top

[U66] PHP：设置 Cookie
来源：http://bct.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vuu.vqdsnc.cn

[U67] PHP：处理文件上传
来源：http://xob.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lui.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://pfr.ywan-chungtsiang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uax.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://kdj.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://piq.52xcode.cn

[U70] PHP：PDO 事务
来源：http://jlu.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kej.xingfuxueyuan.xyz

[U71] PHP：抛出异常
来源：http://enj.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://jvv.shanyushiyangkeji.top

[U72] PHP：写错误日志
来源：http://gaa.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://qgh.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://oqe.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://cio.fengsongda.top

[U74] PHP：读取环境变量
来源：http://ewm.cheryme.top

getenv("APP_ENV") ?: "production"
来源：http://eco.jqgfzy.top

[U75] PHP：依赖注入
来源：http://avg.sysykeji.top

composer require psr/container
来源：http://uev.yfazqb.com

[U76] PHP：简单路由
来源：http://kdw.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://auq.9152youxi.cn

[U77] PHP：模板渲染
来源：http://fvb.snrcjt.cn

composer require twig/twig
来源：http://fds.fehbvm.com

[U78] PHP：单元测试
来源：http://umw.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://xsb.xziqi.cn

[U79] PHP：静态分析
来源：http://agh.ydzc1.top

composer require --dev phpstan/phpstan
来源：http://lsl.hesvh.cn

[U80] PHP：代码规范修复
来源：http://lte.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ogy.pengpengdd.cyou


<!-- 参考信息 -->