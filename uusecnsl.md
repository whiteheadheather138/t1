代发 wailian999

int size() const noexcept { return n_; }
来源：http://bqg.zhongyouzk.top

[S53] C++：移动语义
来源：http://wfn.hammf.cn

std::vector<int> w = std::move(v);
来源：http://kue.yvedp.cn

[S54] C++：异常处理
来源：http://otu.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rkm.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://lyf.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aej.chenzaomai.com

[S56] C++：optional
来源：http://qud.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ezk.cdnleiting.top

[S57] C++：编译期常量
来源：http://oya.nwbrower.top

constexpr int N = 10;
来源：http://rpo.gaohongyu789.top

[S58] C++：命名空间
来源：http://pwt.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://krd.daxiang520.top

[S59] C++：静态断言
来源：http://vaj.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sir.cheryme.top

[S60] C++：遍历并删除元素
来源：http://avl.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://khb.zycfv.cn

================================================================================
来源：http://xmu.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bar.pycfn.com

================================================================================
来源：http://jfe.guannengcc.top

[T01] Kotlin：Hello World
来源：http://mqz.nanxinkj.top

println("Hello")
来源：http://rcr.zycfv.cn

[T02] Kotlin：变量
来源：http://zpd.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lgx.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://myi.fehbvm.com

"值: $b"
来源：http://pyy.gotoacloud.top

[T04] Kotlin：空安全
来源：http://ynp.zdqjudy.top

val n: String? = null;  n?.length
来源：http://rak.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://cij.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kce.hesvh.cn

[T06] Kotlin：集合映射
来源：http://mtn.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://enz.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://dai.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipr.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://qkb.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://lxo.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://ifa.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://nng.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://whl.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wig.jyoumei.cn

[T11] Kotlin：协程
来源：http://iix.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hpe.daria6918.cn

[T12] Kotlin：解构声明
来源：http://jmi.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://duv.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://ibh.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://vwh.daria6918.cn

[T14] Kotlin：循环
来源：http://koh.dashuyun.cn

for (i in 1..10) println(i)
来源：http://mfq.yj202588.top

[T15] Kotlin：接口
来源：http://luf.zdqjudy.top

interface Shape { fun area(): Double }
来源：http://qae.shzxlz.cn

[T16] Swift：Hello World
来源：http://gom.wangshuangyany.cn

print("Hello")
来源：http://ena.yuanzhike.top

[T17] Swift：变量与常量
来源：http://znz.cheryme.top

var a = 1;  let b = 2
来源：http://jdx.fzhhl.top

[T18] Swift：字符串插值
来源：http://mbc.birdmap.top

"值: \(b)"
来源：http://btr.cheryme.top

[T19] Swift：可选绑定
来源：http://guy.ydjk.org.cn

if let n = opt { print(n) }
来源：http://ezc.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://tza.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pim.tianlin.xyz

[T21] Swift：遍历
来源：http://sgs.guannengcc.top

for x in a { print(x) }
来源：http://leq.jinqigfzy.top

[T22] Swift：字典
来源：http://pff.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://ghw.52xcode.cn

[T23] Swift：函数
来源：http://xgu.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aae.svipenyu.cn

[T24] Swift：闭包
来源：http://apd.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vix.ydjk.org.cn

[T25] Swift：结构体
来源：http://pza.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://sba.jqgufenzy.top

[T26] Swift：类与重写
来源：http://qxf.jinqigufen.top

class A: Base { override func f() {} }
来源：http://edq.dianchejie.cn

[T27] Swift：错误处理
来源：http://mwa.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://cww.bbcook.cn

[T28] Swift：枚举
来源：http://mxw.smart0.xyz

enum Color { case red, green }
来源：http://psy.yonumen.top

[T29] Swift：guard 提前返回
来源：http://yfh.wangshuangyany.cn

guard let x = opt else { return }
来源：http://wsf.sysykeji.top

[T30] Swift：协议
来源：http://kes.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://odo.jyoumei.cn

[T31] Lua：Hello World
来源：http://ucb.jinqigufen.top

print("Hello")
来源：http://oey.cdnleiting.top

[T32] Lua：局部变量
来源：http://cmt.9152youxi.cn

local a = 1
来源：http://vmz.hywenlv.cn

[T33] Lua：表（数组）
来源：http://gaf.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://uql.feifeiyinyue.top

[T34] Lua：遍历表
来源：http://yem.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bwu.gzhubu.top

[T35] Lua：字典表
来源：http://xsh.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://otg.daria6918.cn

[T36] Lua：函数
来源：http://pum.xinyue.icu

function add(a, b) return a + b end
来源：http://nnt.pycfn.com

[T37] Lua：字符串拼接
来源：http://boj.hongshengwenyu.top

"a" .. "b"
来源：http://cxf.uphjek.com

[T38] Lua：条件
来源：http://bnc.zhengqikj.top

if x > 0 then print("正") end
来源：http://vwi.yonumen.top

[T39] Lua：模式匹配
来源：http://tqt.jqgufenzy.top

string.find(s, "%d+")
来源：http://jsp.xuanzx.com

[T40] Lua：元表
来源：http://lpp.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://vik.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://fwu.c1oappe.top

print "Hello\n";
来源：http://bgn.dashuyun.cn

[T42] Perl：变量类型
来源：http://fsu.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rge.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://cgv.yuanzhike.top

"值: $a"
来源：http://zet.jinghuilouyu.cn

[T44] Perl：条件
来源：http://vui.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://rgo.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://vxa.bjfxy.top

for my $x (@arr) { print $x; }
来源：http://tyr.birdmap.top

[T46] Perl：哈希操作
来源：http://yrp.epnwcf.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kyc.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://ngs.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dih.ppjwa.cn

[T48] Perl：正则替换
来源：http://mzu.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://nrd.chenzaomai.com

[T49] Perl：函数
来源：http://qgf.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hqn.jqgfzy.top

[T50] Perl：逐行读文件
来源：http://bxu.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sru.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://psx.havefunace.top

[T51] Scala：Hello World
来源：http://pqp.xingfuxueyuan.xyz

println("Hello")
来源：http://gnd.bbcook.cn

[T52] Scala：变量
来源：http://mlb.ydjk.org.cn

val a = 1;  var b = 2
来源：http://jxa.xziqi.cn

[T53] Scala：字符串插值
来源：http://pyt.xuetiantiany.cn

s"值: $b"
来源：http://zuf.cheryme.top

[T54] Scala：集合映射
来源：http://blb.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://uoa.haohaochexian.top

[T55] Scala：集合过滤
来源：http://wvr.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://mou.zhijiandao.cn

[T56] Scala：样例类
来源：http://rnc.ehwqpu.com

case class User(name: String, age: Int)
来源：http://xcl.wangdashe.top

[T57] Scala：模式匹配
来源：http://wlu.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://loj.jyoumei.cn

[T58] Scala：函数定义
来源：http://rjm.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ron.pengpengdd.cyou

[T59] Scala：循环
来源：http://imx.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://rti.316326.xyz

[T60] Scala：折叠
来源：http://fcu.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://toy.shanyushiyangtech.top

================================================================================
来源：http://ucz.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jut.jqgufenzy.top

================================================================================
来源：http://tsw.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://ush.tian-w.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hki.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://twl.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wkg.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://xnj.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://qhq.yuanzhike.top

[U04] Py：变量调试打印
来源：http://ahp.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yee.uphjek.com

[U05] Py：列表去重且保序
来源：http://isv.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://nxt.ybcxt.top

[U06] Py：合并两个字典
来源：http://ugw.tian-w.cn

{**a, **b}
来源：http://wix.yonumen.top

[U07] Py：反转字典键值
来源：http://tdo.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://wwb.yongpay.top

[U08] Py：展平二维列表
来源：http://lty.vqdsnc.cn

[y for x in nested for y in x]
来源：http://ktw.zhijiandao.cn

[U09] Py：字典取最大值的键
来源：http://car.yfazqb.com

max(d, key=d.get)
来源：http://ezj.guannengcc.top

[U10] Py：按值排序字典
来源：http://jgi.mhx1999.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://doc.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://vxx.hammf.cn

(x * 2 for x in arr)
来源：http://eih.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://fpu.ybcxt.top

Counter(arr).most_common(3)
来源：http://gfp.sweek.top

[U13] Py：固定长度队列
来源：http://ysb.fanxiaobao.xyz

deque(maxlen=10)
来源：http://yqm.guannengcc.top

[U14] Py：分组收集到列表
来源：http://bbg.uphjek.com

defaultdict(list)
来源：http://pdz.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://ztr.wangdashe.top

t = time.perf_counter()
来源：http://ztx.ivvv.top

[U16] Py：命令行参数解析
来源：http://ndb.jqgfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lil.zhixingplan.top

[U17] Py：初始化日志
来源：http://dyl.cqqwz.cn

logging.basicConfig(level=logging.INFO)
来源：http://tly.yanxiufei.cn

[U18] Py：预编译正则
来源：http://ygy.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://vnc.snrcjt.cn

[U19] Py：正则替换带回调
来源：http://udo.vqdsnc.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rqn.shuidangran.top

[U20] Py：缓存函数结果
来源：http://qei.tanke756.top

@functools.lru_cache(maxsize=None)
来源：http://ivy.havefunace.top

[U21] Py：自定义上下文管理器
来源：http://hzk.cheryme.top

@contextlib.contextmanager
来源：http://gqf.tianlin.xyz

[U22] Py：矩阵转置
来源：http://naf.chenlongwang.top

list(zip(*m))
来源：http://ukp.pycfn.com

[U23] Py：分块读取大文件
来源：http://nbb.jinghuilouyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ogh.hesvh.cn

[U24] Py：路径操作
来源：http://rdz.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gqk.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://osm.vqdsnc.cn

csv.DictReader(f)
来源：http://izv.jinghuilouyu.cn

[U26] Py：并发下载
来源：http://twf.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ydu.jlsjyb.cn

[U27] Py：异步 HTTP
来源：http://kyg.tarul.cn

aiohttp.ClientSession() 配合 async with
来源：http://eey.mhx1999.top

[U28] Py：类型别名
来源：http://rwg.ydzc1.top

UserId = int
来源：http://gbi.zhaomingkeji.xyz

[U29] Py：属性校验
来源：http://vsm.316326.xyz

@property 与 @x.setter 配合
来源：http://fpo.yuxming.cn

[U30] Py：数据类
来源：http://pon.aizwys.cn

@dataclass(slots=True)
来源：http://fvh.zhixingplan.top

[U31] Py：单测
来源：http://pef.cheryme.top

python -m pytest -q
来源：http://uiw.iojbl.cn

[U32] Py：代码格式化
来源：http://yqk.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://qfx.gaohongyu789.top

[U33] Py：打包发布
来源：http://vrc.pycfn.com

python -m build  （依赖 pyproject.toml）
来源：http://cmt.iojbl.cn

[U34] Py：判断编码
来源：http://thg.ehwqpu.com

chardet.detect(raw)
来源：http://hmo.vehdjk.com

[U35] Py：发送邮件
来源：http://eku.tanke756.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gyc.snrcjt.cn

[U36] Py：定时任务
来源：http://fhg.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://dup.xingfuxueyuan.xyz

[U37] Py：读写 Excel
来源：http://wjd.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://rhk.sweek.top

[U38] Py：获取脚本所在目录
来源：http://rgn.yj20258888.top

Path(__file__).resolve().parent
来源：http://orh.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://hke.zhiwuduotai.top

sys.stdout.isatty()
来源：http://ywj.zhaomingkeji.xyz

[U40] Py：打印到标准错误
来源：http://yak.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://hna.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://wxx.ydzc1.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ymp.fzhhl.top

[U42] PHP：PSR-4 自动加载
来源：http://pfr.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hby.yj202588.top

[U43] PHP：声明命名空间
来源：http://xdv.hammf.cn

namespace App\Http;
来源：http://nax.guowangkeji.top

[U44] PHP：开启严格类型
来源：http://rqc.xinyue.icu

declare(strict_types=1);
来源：http://bdz.uphjek.com

[U45] PHP：类型声明与返回类型
来源：http://ypm.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fug.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://vwr.gaohongyu789.top

?string $name = null
来源：http://ege.sweek.top

[U47] PHP：联合类型
来源：http://uhw.aibaodan.cn

int|string $id
来源：http://bmj.jqgufenzy.top

[U48] PHP：纯枚举
来源：http://tvo.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://brz.gotoacloud.top

[U49] PHP：只读属性
来源：http://ymk.nanxinkj.top

public readonly string $name
来源：http://uro.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://nxk.c1oappe.top

public function __construct(private int $id) {}
来源：http://rxp.redwolf501.top

[U51] PHP：数组解构
来源：http://xzi.ctjpmb.com

[$a, $b] = $arr;
来源：http://rkx.sweek.top

[U52] PHP：箭头函数
来源：http://mya.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://wsj.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://znp.guowangkeji.top

$v = $a ?? $b ?? "default";
来源：http://joh.xziqi.cn

[U54] PHP：空安全调用
来源：http://upg.zhongyouzk.top

$obj?->method()
来源：http://tqj.hfpthk.cn

[U55] PHP：match 表达式
来源：http://eow.52xcode.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lfr.epnwcf.com

[U56] PHP：命名参数
来源：http://hly.jinghuilouyu.cn

f(a: 1, b: 2)
来源：http://ahz.yj202588.top

[U57] PHP：字符串插值
来源：http://ebu.hnxiangtu.top

"值: {$a}"
来源：http://uvl.xylfe.cn

[U58] PHP：数组三件套
来源：http://qmo.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cav.tian-w.cn

[U59] PHP：自定义排序
来源：http://kpm.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yuz.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://lfg.wangdashe.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jub.jqgfzy.top

[U61] PHP：正则
来源：http://tqm.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baz.sufxvd.cn

[U62] PHP：日期对象
来源：http://uew.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nqg.mhx1999.top

[U63] PHP：文件读写
来源：http://och.zhengqikj.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lbn.svipenyu.cn

[U64] PHP：目录遍历
来源：http://gcj.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://odg.ivvv.top

[U65] PHP：会话
来源：http://hnt.jiagoushi.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pmi.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://qqj.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mqm.zhixingplan.top

[U67] PHP：处理文件上传
来源：http://nio.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://awu.fehbvm.com

[U68] PHP：PDO 连接
来源：http://mtj.sjlbkw.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wke.yfazqb.com

[U69] PHP：PDO 预处理
来源：http://tfj.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xyt.bbcook.cn

[U70] PHP：PDO 事务
来源：http://oow.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://omo.jinqigfzy.top

[U71] PHP：抛出异常
来源：http://zlk.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://yjh.ehwqpu.com

[U72] PHP：写错误日志
来源：http://otr.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://thx.xingfuxueyuan.xyz

[U73] PHP：读取 ini 配置
来源：http://swt.sxryk.cn

parse_ini_file("config.ini", true)
来源：http://aci.cqqwz.cn

[U74] PHP：读取环境变量
来源：http://mlb.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://tvn.yfazqb.com

[U75] PHP：依赖注入
来源：http://qkg.ppjwa.cn

composer require psr/container
来源：http://pxu.tarul.cn

[U76] PHP：简单路由
来源：http://hjq.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rke.xylfe.cn

[U77] PHP：模板渲染
来源：http://jzw.zhongyouzk.top

composer require twig/twig
来源：http://rcj.meibo888.top

[U78] PHP：单元测试
来源：http://rtg.bbcook.cn

composer require --dev phpunit/phpunit
来源：http://xhn.wangshuangyany.cn


<!-- 参考信息 -->