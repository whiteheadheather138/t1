代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gcr.kuanghao11.cn

================================================================================
来源：http://dgh.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://naa.chenjidiqi.icu

================================================================================
来源：http://tkm.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://ntd.gzhubu.top

println("Hello")
来源：http://jgx.ehwqpu.com

[T02] Kotlin：变量
来源：http://vza.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gjc.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://gjl.zhengqikj.top

"值: $b"
来源：http://vpc.52xcode.cn

[T04] Kotlin：空安全
来源：http://bjq.andypj.xyz

val n: String? = null;  n?.length
来源：http://mmc.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://lsa.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ndd.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://wxw.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ein.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://uql.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ezl.uphjek.com

[T08] Kotlin：数据类
来源：http://xvo.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://hzs.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://siq.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://ggv.cheryme.top

[T10] Kotlin：默认参数
来源：http://zuq.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zco.jqgfzy.top

[T11] Kotlin：协程
来源：http://xzi.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bbe.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://iiu.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://ukf.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://llm.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://eva.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://oqn.yuanzhike.top

for (i in 1..10) println(i)
来源：http://jaf.shuidangran.top

[T15] Kotlin：接口
来源：http://qsy.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://cqn.shuidangran.top

[T16] Swift：Hello World
来源：http://ksx.shangyingyoupin.top

print("Hello")
来源：http://xri.dashuyun.cn

[T17] Swift：变量与常量
来源：http://wkm.ivvv.top

var a = 1;  let b = 2
来源：http://foj.kuanghao11.cn

[T18] Swift：字符串插值
来源：http://mgn.aibaodan.cn

"值: \(b)"
来源：http://mfy.nwbrower.top

[T19] Swift：可选绑定
来源：http://qcl.hnxiangtu.top

if let n = opt { print(n) }
来源：http://ely.birdmap.top

[T20] Swift：数组操作
来源：http://vwy.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sqw.cdnleiting.top

[T21] Swift：遍历
来源：http://kxs.yfazqb.com

for x in a { print(x) }
来源：http://kfz.ctjpmb.com

[T22] Swift：字典
来源：http://jpx.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://bly.ybcxt.top

[T23] Swift：函数
来源：http://fzo.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ktg.sjlbkw.cn

[T24] Swift：闭包
来源：http://xqv.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ojp.jinqigfzy.top

[T25] Swift：结构体
来源：http://jcm.vqdsnc.cn

struct P { var x: Int }
来源：http://qsv.gotoacloud.top

[T26] Swift：类与重写
来源：http://mti.shuidangran.top

class A: Base { override func f() {} }
来源：http://btw.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://owk.gzhubu.top

do { try f() } catch { print(error) }
来源：http://owa.quarkkingdee.top

[T28] Swift：枚举
来源：http://tnt.hcnkem.com

enum Color { case red, green }
来源：http://lqz.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://naa.daxiang520.top

guard let x = opt else { return }
来源：http://qzp.feifeiyinyue.top

[T30] Swift：协议
来源：http://yml.pycfn.com

protocol Shape { func area() -> Double }
来源：http://wsp.xuanzx.com

[T31] Lua：Hello World
来源：http://muw.hcnkem.com

print("Hello")
来源：http://xyj.jinqigfzy.top

[T32] Lua：局部变量
来源：http://wjt.0kj1m.cn

local a = 1
来源：http://rgp.gzhubu.top

[T33] Lua：表（数组）
来源：http://ufm.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cqy.nanxuanxn.top

[T34] Lua：遍历表
来源：http://rvc.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://kgh.dianchejie.cn

[T35] Lua：字典表
来源：http://ylp.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://yop.hnqzz.top

[T36] Lua：函数
来源：http://tgd.chenzaomai.com

function add(a, b) return a + b end
来源：http://hgq.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://tpa.wangdashe.top

"a" .. "b"
来源：http://pcq.cdnleiting.top

[T38] Lua：条件
来源：http://oqb.yuanzhike.top

if x > 0 then print("正") end
来源：http://qhq.fzhhl.top

[T39] Lua：模式匹配
来源：http://ofs.xinyue.icu

string.find(s, "%d+")
来源：http://cjs.ppjwa.cn

[T40] Lua：元表
来源：http://xtp.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://duw.havefunace.top

[T41] Perl：Hello World
来源：http://wql.snrcjt.cn

print "Hello\n";
来源：http://bvt.daria6918.cn

[T42] Perl：变量类型
来源：http://aky.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gof.hnqzz.top

[T43] Perl：字符串插值
来源：http://rpx.xuetiantiany.cn

"值: $a"
来源：http://wui.svipenyu.cn

[T44] Perl：条件
来源：http://bov.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://xig.daria6918.cn

[T45] Perl：数组遍历
来源：http://yja.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://wci.9152youxi.cn

[T46] Perl：哈希操作
来源：http://iia.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pff.zycfv.cn

[T47] Perl：正则捕获
来源：http://xju.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kbw.yj20258888.top

[T48] Perl：正则替换
来源：http://skh.yfazqb.com

$s =~ s/old/new/g;
来源：http://flr.guannengcc.top

[T49] Perl：函数
来源：http://rsj.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vzw.xylfe.cn

[T50] Perl：逐行读文件
来源：http://jpa.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qbx.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://zlw.xuanzx.com

[T51] Scala：Hello World
来源：http://uqf.wangshuangyany.cn

println("Hello")
来源：http://lhx.jinqigfzy.top

[T52] Scala：变量
来源：http://sra.bbcook.cn

val a = 1;  var b = 2
来源：http://kqh.havefunace.top

[T53] Scala：字符串插值
来源：http://wov.jlsjyb.cn

s"值: $b"
来源：http://lxp.smart0.xyz

[T54] Scala：集合映射
来源：http://sxl.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://nlk.yj20258888.top

[T55] Scala：集合过滤
来源：http://tim.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://gin.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://lyc.hesvh.cn

case class User(name: String, age: Int)
来源：http://dbr.yuxming.cn

[T57] Scala：模式匹配
来源：http://tmx.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nts.epnwcf.com

[T58] Scala：函数定义
来源：http://knj.feifeiyinyue.top

def add(a: Int, b: Int): Int = a + b
来源：http://xug.sxryk.cn

[T59] Scala：循环
来源：http://oqm.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://ffr.xylfe.cn

[T60] Scala：折叠
来源：http://fvn.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fyv.gaohongyu789.top

================================================================================
来源：http://uka.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://abz.yanxiufei.cn

================================================================================
来源：http://dqv.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://nry.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://urp.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://blt.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xvg.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://xpk.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://axk.yj20258.top

[U04] Py：变量调试打印
来源：http://ccv.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fmr.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://tsn.hcnkem.com

list(dict.fromkeys(arr))
来源：http://bru.pycfn.com

[U06] Py：合并两个字典
来源：http://vxe.yj20258.top

{**a, **b}
来源：http://ixr.gogol.net.cn

[U07] Py：反转字典键值
来源：http://zjh.mhx1999.top

{v: k for k, v in d.items()}
来源：http://syg.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://uzg.nanxinkj.top

[y for x in nested for y in x]
来源：http://chf.cashguo.top

[U09] Py：字典取最大值的键
来源：http://lsi.tian-w.cn

max(d, key=d.get)
来源：http://cfw.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://yxs.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zqz.yongpay.top

[U11] Py：生成器表达式
来源：http://uil.shzxlz.cn

(x * 2 for x in arr)
来源：http://hvi.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hpl.ybcxt.top

Counter(arr).most_common(3)
来源：http://woc.guannengcc.top

[U13] Py：固定长度队列
来源：http://zct.shuidangran.top

deque(maxlen=10)
来源：http://wxl.zdqjudy.top

[U14] Py：分组收集到列表
来源：http://ujm.yvedp.cn

defaultdict(list)
来源：http://byv.yangfankeji.com

[U15] Py：高精度计时
来源：http://gnu.pycfn.com

t = time.perf_counter()
来源：http://jkx.cheryme.top

[U16] Py：命令行参数解析
来源：http://fxs.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jie.andypj.xyz

[U17] Py：初始化日志
来源：http://rbz.yfazqb.com

logging.basicConfig(level=logging.INFO)
来源：http://kwd.andypj.xyz

[U18] Py：预编译正则
来源：http://pzx.daxiang520.top

pat = re.compile(r"\d+")
来源：http://tuf.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://dxi.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://waf.shanyushiyangkeji.top

[U20] Py：缓存函数结果
来源：http://nmy.hfpthk.cn

@functools.lru_cache(maxsize=None)
来源：http://gqg.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://byj.cashguo.top

@contextlib.contextmanager
来源：http://ivc.aibaodan.cn

[U22] Py：矩阵转置
来源：http://mah.uphjek.com

list(zip(*m))
来源：http://pzb.zdqjudy.top

[U23] Py：分块读取大文件
来源：http://men.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ohb.cdnleiting.top

[U24] Py：路径操作
来源：http://nzs.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bhw.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://utv.jianghu66.top

csv.DictReader(f)
来源：http://ywz.nanxuanxn.top

[U26] Py：并发下载
来源：http://avo.ydzc1.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lzd.fzhhl.top

[U27] Py：异步 HTTP
来源：http://enk.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://odq.shangyingyoupin.top

[U28] Py：类型别名
来源：http://lsc.feifeiyinyue.top

UserId = int
来源：http://bij.yj20258.top

[U29] Py：属性校验
来源：http://lbu.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://tfc.guannengcc.top

[U30] Py：数据类
来源：http://qvv.havefunace.top

@dataclass(slots=True)
来源：http://hce.pycfn.com

[U31] Py：单测
来源：http://jdu.iojbl.cn

python -m pytest -q
来源：http://owo.redwolf501.top

[U32] Py：代码格式化
来源：http://rte.yvedp.cn

ruff format . && ruff check --fix .
来源：http://cde.ctjpmb.com

[U33] Py：打包发布
来源：http://ajc.c1oappe.top

python -m build  （依赖 pyproject.toml）
来源：http://tlz.zdbjq.cn

[U34] Py：判断编码
来源：http://fvy.bbcook.cn

chardet.detect(raw)
来源：http://cfk.nanxinkj.top

[U35] Py：发送邮件
来源：http://wrg.dashuyun.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://udw.c1oappe.top

[U36] Py：定时任务
来源：http://izv.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://ich.jqgfzy.top

[U37] Py：读写 Excel
来源：http://xyq.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vqe.havefunace.top

[U38] Py：获取脚本所在目录
来源：http://dvz.jinghuilouyu.cn

Path(__file__).resolve().parent
来源：http://gsu.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://njv.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://aly.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://bul.gogol.net.cn

print("err", file=sys.stderr)
来源：http://ebo.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://sci.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jyo.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://zog.hesvh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bel.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://kuy.cheryme.top

namespace App\Http;
来源：http://jeq.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://evv.nanxuanxn.top

declare(strict_types=1);
来源：http://lvt.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://cmb.dashuyun.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jmh.quarkkingdee.top

[U46] PHP：可空类型
来源：http://abc.hnqzz.top

?string $name = null
来源：http://syu.0kj1m.cn

[U47] PHP：联合类型
来源：http://orq.hywenlv.cn

int|string $id
来源：http://brj.zhixingplan.top

[U48] PHP：纯枚举
来源：http://bui.yanxiufei.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvp.nwbrower.top

[U49] PHP：只读属性
来源：http://haf.aizwys.cn

public readonly string $name
来源：http://nhd.yvedp.cn

[U50] PHP：构造器属性提升
来源：http://xur.xuanzx.com

public function __construct(private int $id) {}
来源：http://chx.sysykeji.top

[U51] PHP：数组解构
来源：http://azn.hnqzz.top

[$a, $b] = $arr;
来源：http://ksq.aibaodan.cn

[U52] PHP：箭头函数
来源：http://jai.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://mwv.c1oappe.top

[U53] PHP：空合并运算符
来源：http://oxy.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://owu.bjfxy.top

[U54] PHP：空安全调用
来源：http://fvl.haohaochexian.top

$obj?->method()
来源：http://lbu.ehwqpu.com

[U55] PHP：match 表达式
来源：http://wpe.hesvh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cgm.tian-w.cn

[U56] PHP：命名参数
来源：http://pao.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://syo.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://aje.nanxuanxn.top

"值: {$a}"
来源：http://oyj.xuanzx.com

[U58] PHP：数组三件套
来源：http://sxd.snrcjt.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wmb.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://mxo.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hxj.cashguo.top

[U60] PHP：JSON 编解码
来源：http://bdb.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wvz.wangdashe.top

[U61] PHP：正则
来源：http://llr.shanyushiyangkeji.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jxq.tianlin.xyz

[U62] PHP：日期对象
来源：http://cfs.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nfc.yangfankeji.com

[U63] PHP：文件读写
来源：http://otc.yonumen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xog.jinqigufen.top

[U64] PHP：目录遍历
来源：http://sij.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://mcw.yvedp.cn

[U65] PHP：会话
来源：http://akw.xylfe.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gzn.jinyuanbaomall.cn

[U66] PHP：设置 Cookie
来源：http://lla.havefunace.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cxc.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://lum.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ilr.nanxuanxn.top

[U68] PHP：PDO 连接
来源：http://mdt.shzxlz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nwv.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://ivg.pycfn.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ski.guannengcc.top

[U70] PHP：PDO 事务
来源：http://kvh.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rby.52xcode.cn

[U71] PHP：抛出异常
来源：http://vwn.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://coq.yj20258.top

[U72] PHP：写错误日志
来源：http://smh.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://voj.zhiwuduotai.top

[U73] PHP：读取 ini 配置
来源：http://iij.quarkkingdee.top

parse_ini_file("config.ini", true)
来源：http://oiw.jianghu66.top

[U74] PHP：读取环境变量
来源：http://kyg.hnxiangtu.top

getenv("APP_ENV") ?: "production"
来源：http://lar.fehbvm.com

[U75] PHP：依赖注入
来源：http://gwo.svipenyu.cn

composer require psr/container
来源：http://wlr.ehwqpu.com

[U76] PHP：简单路由
来源：http://did.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://poi.nwbrower.top

[U77] PHP：模板渲染
来源：http://ixu.ydzc1.top

composer require twig/twig
来源：http://ume.cheryme.top

[U78] PHP：单元测试
来源：http://tfw.uphjek.com

composer require --dev phpunit/phpunit
来源：http://sph.shuidangran.top

[U79] PHP：静态分析
来源：http://xgn.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://hnk.havefunace.top

[U80] PHP：代码规范修复
来源：http://kbn.quarkkingdee.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://jzm.ybcxt.top

[U81] JS：初始化项目
来源：http://tte.zhiwuduotai.top

npm init -y;  npm i express
来源：http://lke.cucudq.cn

[U82] JS：package.json 脚本
来源：http://fyr.mhx1999.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wnn.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://ajw.birdmap.top

export const a = 1;  import { a } from "./m.js";
来源：http://cpz.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://qxq.zhongyouzk.top

module.exports = { a };  const { a } = require("./m");
来源：http://wcb.yuxming.cn

[U85] JS：可选链
来源：http://zmq.zdbjq.cn

a?.b?.c
来源：http://lsu.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://cbb.zhoulong.xyz

a ?? b
来源：http://ays.fengsongda.top


<!-- 参考信息 -->