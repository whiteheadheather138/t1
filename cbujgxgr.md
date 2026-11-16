代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sjj.hnxiangtu.top

================================================================================
来源：http://pmx.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xsx.tarul.cn

================================================================================
来源：http://fkm.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://wyl.zhijiandao.cn

println("Hello")
来源：http://rkg.xuanzx.com

[T02] Kotlin：变量
来源：http://uas.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oub.birdmap.top

[T03] Kotlin：字符串模板
来源：http://rhi.zdqjudy.top

"值: $b"
来源：http://wqr.52xcode.cn

[T04] Kotlin：空安全
来源：http://ifl.birdmap.top

val n: String? = null;  n?.length
来源：http://axz.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://wxe.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tgr.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://pxa.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wbk.sweek.top

[T07] Kotlin：集合过滤
来源：http://muc.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ycx.jyoumei.cn

[T08] Kotlin：数据类
来源：http://dki.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://vvp.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://hky.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://jdc.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://wlh.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vdi.vehdjk.com

[T11] Kotlin：协程
来源：http://kqx.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ryi.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://zoq.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://mjq.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://cjl.xuanzx.com

val m = mapOf("a" to 1)
来源：http://ctz.fehbvm.com

[T14] Kotlin：循环
来源：http://lif.daria6918.cn

for (i in 1..10) println(i)
来源：http://nvd.hysaishi.cn

[T15] Kotlin：接口
来源：http://bfn.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://jbz.redwolf501.top

[T16] Swift：Hello World
来源：http://ccn.nanxinkj.top

print("Hello")
来源：http://vot.9152youxi.cn

[T17] Swift：变量与常量
来源：http://gtt.zhijiandao.cn

var a = 1;  let b = 2
来源：http://fbk.yongpay.top

[T18] Swift：字符串插值
来源：http://wom.hesvh.cn

"值: \(b)"
来源：http://zbl.aizwys.cn

[T19] Swift：可选绑定
来源：http://eij.zdbjq.cn

if let n = opt { print(n) }
来源：http://teq.bjfxy.top

[T20] Swift：数组操作
来源：http://eqz.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://peo.zhongyouzk.top

[T21] Swift：遍历
来源：http://gmx.hywenlv.cn

for x in a { print(x) }
来源：http://cui.iojbl.cn

[T22] Swift：字典
来源：http://xhk.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mes.hongshengwenyu.top

[T23] Swift：函数
来源：http://wkt.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ihi.jinqigufen.top

[T24] Swift：闭包
来源：http://hya.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wxp.jiagoushi.top

[T25] Swift：结构体
来源：http://cgn.jianghu66.top

struct P { var x: Int }
来源：http://ctw.vehdjk.com

[T26] Swift：类与重写
来源：http://kei.chenzaomai.com

class A: Base { override func f() {} }
来源：http://dxy.c1oappe.top

[T27] Swift：错误处理
来源：http://vwt.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://ddq.hesvh.cn

[T28] Swift：枚举
来源：http://znn.cashguo.top

enum Color { case red, green }
来源：http://agw.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://hfk.bjfxy.top

guard let x = opt else { return }
来源：http://jzy.redwolf501.top

[T30] Swift：协议
来源：http://xae.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://rpw.fengsongda.top

[T31] Lua：Hello World
来源：http://bes.jinqigfzy.top

print("Hello")
来源：http://hfj.yfazqb.com

[T32] Lua：局部变量
来源：http://dpt.zhongyouzk.top

local a = 1
来源：http://qox.snrcjt.cn

[T33] Lua：表（数组）
来源：http://gqe.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cxz.vehdjk.com

[T34] Lua：遍历表
来源：http://wxr.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qvl.sufxvd.cn

[T35] Lua：字典表
来源：http://shf.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://sqe.tanke756.top

[T36] Lua：函数
来源：http://bsp.xylfe.cn

function add(a, b) return a + b end
来源：http://vvx.aizwys.cn

[T37] Lua：字符串拼接
来源：http://tbl.fengsongda.top

"a" .. "b"
来源：http://wsm.yanxiufei.cn

[T38] Lua：条件
来源：http://rar.sufxvd.cn

if x > 0 then print("正") end
来源：http://nth.yj20258.top

[T39] Lua：模式匹配
来源：http://svk.zhixingplan.top

string.find(s, "%d+")
来源：http://ope.gaohongyu789.top

[T40] Lua：元表
来源：http://khg.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://caw.sufxvd.cn

[T41] Perl：Hello World
来源：http://ysm.gaohongyu789.top

print "Hello\n";
来源：http://ugy.chenjidiqi.icu

[T42] Perl：变量类型
来源：http://itp.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vgk.ctjpmb.com

[T43] Perl：字符串插值
来源：http://yms.hesvh.cn

"值: $a"
来源：http://ann.chenjidiqi.icu

[T44] Perl：条件
来源：http://vaa.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://oua.yuxming.cn

[T45] Perl：数组遍历
来源：http://gzj.gogol.net.cn

for my $x (@arr) { print $x; }
来源：http://ntf.uphjek.com

[T46] Perl：哈希操作
来源：http://qzh.hesvh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fyw.yueranfly.top

[T47] Perl：正则捕获
来源：http://pyu.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ljc.snrcjt.cn

[T48] Perl：正则替换
来源：http://ghp.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://ywo.0kj1m.cn

[T49] Perl：函数
来源：http://tuq.kuanghao11.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eyz.quarkkingdee.top

[T50] Perl：逐行读文件
来源：http://kpe.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vzv.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://amx.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://tpa.gogol.net.cn

println("Hello")
来源：http://ogn.cucudq.cn

[T52] Scala：变量
来源：http://vwk.jqgfzy.top

val a = 1;  var b = 2
来源：http://cap.shuidangran.top

[T53] Scala：字符串插值
来源：http://ola.chenlongwang.top

s"值: $b"
来源：http://vde.zdbjq.cn

[T54] Scala：集合映射
来源：http://drs.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://awe.pengpengdd.cyou

[T55] Scala：集合过滤
来源：http://mtm.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://tkv.jlsjyb.cn

[T56] Scala：样例类
来源：http://daf.9152youxi.cn

case class User(name: String, age: Int)
来源：http://yib.yj202588.top

[T57] Scala：模式匹配
来源：http://swy.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lvl.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://iqy.ydjk.org.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gxl.shangyingyoupin.top

[T59] Scala：循环
来源：http://ahd.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://ujf.c1oappe.top

[T60] Scala：折叠
来源：http://wlx.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sro.shanyushiyangkeji.top

================================================================================
来源：http://mjs.tianlin.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rkx.cdnleiting.top

================================================================================
来源：http://gxk.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://dsp.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gbg.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://qwn.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jcs.ivvv.top

[U03] Py：加载 .env 配置
来源：http://bjx.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ntp.yonumen.top

[U04] Py：变量调试打印
来源：http://gfu.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cxm.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://dsz.aizwys.cn

list(dict.fromkeys(arr))
来源：http://bxs.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://wzb.epnwcf.com

{**a, **b}
来源：http://nhm.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://uxr.shuidangran.top

{v: k for k, v in d.items()}
来源：http://ftr.zdqjudy.top

[U08] Py：展平二维列表
来源：http://ylr.jyoumei.cn

[y for x in nested for y in x]
来源：http://kyg.epnwcf.com

[U09] Py：字典取最大值的键
来源：http://bii.ehwqpu.com

max(d, key=d.get)
来源：http://xkd.tanke756.top

[U10] Py：按值排序字典
来源：http://grh.sxryk.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gbb.shangyingyoupin.top

[U11] Py：生成器表达式
来源：http://rnv.shzxlz.cn

(x * 2 for x in arr)
来源：http://wdk.havefunace.top

[U12] Py：取出现最多的 3 个元素
来源：http://uxi.tanke756.top

Counter(arr).most_common(3)
来源：http://nnv.9152youxi.cn

[U13] Py：固定长度队列
来源：http://qfr.yfazqb.com

deque(maxlen=10)
来源：http://kzn.yuxming.cn

[U14] Py：分组收集到列表
来源：http://mzf.vqdsnc.cn

defaultdict(list)
来源：http://cmp.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://kvb.chenzaomai.com

t = time.perf_counter()
来源：http://fdy.gzhubu.top

[U16] Py：命令行参数解析
来源：http://rwl.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qop.hammf.cn

[U17] Py：初始化日志
来源：http://qts.epnwcf.com

logging.basicConfig(level=logging.INFO)
来源：http://env.yongpay.top

[U18] Py：预编译正则
来源：http://zmn.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://eiy.hfpthk.cn

[U19] Py：正则替换带回调
来源：http://zob.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wlp.havefunace.top

[U20] Py：缓存函数结果
来源：http://hvo.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://jru.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://pzk.fktsv.cn

@contextlib.contextmanager
来源：http://nbw.fzhhl.top

[U22] Py：矩阵转置
来源：http://nbf.shanyushiyangkeji.top

list(zip(*m))
来源：http://fwx.bbcook.cn

[U23] Py：分块读取大文件
来源：http://sfl.sweek.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ihr.cdnleiting.top

[U24] Py：路径操作
来源：http://iwg.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ier.gaohongyu789.top

[U25] Py：CSV 按字典读
来源：http://hsc.shuidangran.top

csv.DictReader(f)
来源：http://rur.bjfxy.top

[U26] Py：并发下载
来源：http://yhq.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ubi.bjfxy.top

[U27] Py：异步 HTTP
来源：http://rwf.shzxlz.cn

aiohttp.ClientSession() 配合 async with
来源：http://bgv.yj20258.top

[U28] Py：类型别名
来源：http://zwu.chenjidiqi.icu

UserId = int
来源：http://zwj.ctjpmb.com

[U29] Py：属性校验
来源：http://lda.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://ifm.birdmap.top

[U30] Py：数据类
来源：http://plq.nwbrower.top

@dataclass(slots=True)
来源：http://hul.quarkkingdee.top

[U31] Py：单测
来源：http://ueg.dianchejie.cn

python -m pytest -q
来源：http://fkp.quarkkingdee.top

[U32] Py：代码格式化
来源：http://dif.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://jpq.chenlongwang.top

[U33] Py：打包发布
来源：http://dtz.fehbvm.com

python -m build  （依赖 pyproject.toml）
来源：http://iut.hnqzz.top

[U34] Py：判断编码
来源：http://sbn.nanxinkj.top

chardet.detect(raw)
来源：http://urx.c1oappe.top

[U35] Py：发送邮件
来源：http://kbb.aibaodan.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wyy.fktsv.cn

[U36] Py：定时任务
来源：http://sxz.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://ejf.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://nvz.hnqzz.top

pandas.read_excel / DataFrame.to_excel
来源：http://lcy.hnxiangtu.top

[U38] Py：获取脚本所在目录
来源：http://woc.birdmap.top

Path(__file__).resolve().parent
来源：http://fuy.cqqwz.cn

[U39] Py：判断是否在交互环境
来源：http://gop.guannengcc.top

sys.stdout.isatty()
来源：http://urg.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://lez.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://sgn.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://dez.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ocb.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://azo.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ozs.zycfv.cn

[U43] PHP：声明命名空间
来源：http://oqz.chenlongwang.top

namespace App\Http;
来源：http://nxn.cdnleiting.top

[U44] PHP：开启严格类型
来源：http://irz.svipenyu.cn

declare(strict_types=1);
来源：http://fdv.sufxvd.cn

[U45] PHP：类型声明与返回类型
来源：http://bir.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://poe.fehbvm.com

[U46] PHP：可空类型
来源：http://alt.wangshuangyany.cn

?string $name = null
来源：http://qal.aizwys.cn

[U47] PHP：联合类型
来源：http://kdv.sjlbkw.cn

int|string $id
来源：http://jtq.tarul.cn

[U48] PHP：纯枚举
来源：http://dqs.gogol.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://imx.pycfn.com

[U49] PHP：只读属性
来源：http://rlh.hongshengwenyu.top

public readonly string $name
来源：http://tma.ybcxt.top

[U50] PHP：构造器属性提升
来源：http://ucs.sweek.top

public function __construct(private int $id) {}
来源：http://lec.sweek.top

[U51] PHP：数组解构
来源：http://gdb.svipenyu.cn

[$a, $b] = $arr;
来源：http://lsg.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://ogy.mhx1999.top

$double = fn($x) => $x * 2;
来源：http://ttf.ybcxt.top

[U53] PHP：空合并运算符
来源：http://kla.zhixingplan.top

$v = $a ?? $b ?? "default";
来源：http://ril.52xcode.cn

[U54] PHP：空安全调用
来源：http://iis.zhaomingkeji.xyz

$obj?->method()
来源：http://hmu.uphjek.com

[U55] PHP：match 表达式
来源：http://hik.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sua.nanxuanxn.top

[U56] PHP：命名参数
来源：http://oaf.jqgufenzy.top

f(a: 1, b: 2)
来源：http://ukl.cqqwz.cn

[U57] PHP：字符串插值
来源：http://ppt.hysaishi.cn

"值: {$a}"
来源：http://dif.zhengqikj.top

[U58] PHP：数组三件套
来源：http://ohz.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xbs.birdmap.top

[U59] PHP：自定义排序
来源：http://zpj.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aup.daria6918.cn

[U60] PHP：JSON 编解码
来源：http://wcw.tian-w.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://evf.ywan-chungtsiang.top

[U61] PHP：正则
来源：http://tkc.cdnleiting.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vlw.316326.xyz

[U62] PHP：日期对象
来源：http://hjl.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://izw.xuetiantiany.cn

[U63] PHP：文件读写
来源：http://cbc.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://frp.tanke756.top

[U64] PHP：目录遍历
来源：http://mpf.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://knc.guannengcc.top

[U65] PHP：会话
来源：http://uvc.bjfxy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qso.aizwys.cn

[U66] PHP：设置 Cookie
来源：http://url.sysykeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ndw.hnqzz.top

[U67] PHP：处理文件上传
来源：http://pwa.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vda.gzhubu.top

[U68] PHP：PDO 连接
来源：http://aty.ehwqpu.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ivt.ybcxt.top

[U69] PHP：PDO 预处理
来源：http://amm.haohaochexian.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tnc.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://szq.jinqigfzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tjf.ydzc1.top

[U71] PHP：抛出异常
来源：http://iaw.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://roc.hesvh.cn

[U72] PHP：写错误日志
来源：http://nyn.fanxiaobao.xyz

error_log("失败: " . $e->getMessage());
来源：http://rxq.yanxiufei.cn

[U73] PHP：读取 ini 配置
来源：http://wpu.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://gsv.tian-w.cn

[U74] PHP：读取环境变量
来源：http://cqp.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://gvj.dashuyun.cn

[U75] PHP：依赖注入
来源：http://slj.shuidangran.top

composer require psr/container
来源：http://rau.316326.xyz

[U76] PHP：简单路由
来源：http://zin.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dnn.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://qof.jinghuilouyu.cn

composer require twig/twig
来源：http://kui.ppjwa.cn

[U78] PHP：单元测试
来源：http://ipa.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://mfm.gaohongyu789.top

[U79] PHP：静态分析
来源：http://enl.yuxming.cn

composer require --dev phpstan/phpstan
来源：http://dkv.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://orb.jianghu66.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ypn.hammf.cn

[U81] JS：初始化项目
来源：http://oaa.quarkkingdee.top

npm init -y;  npm i express
来源：http://zlh.birdmap.top

[U82] JS：package.json 脚本
来源：http://irx.uphjek.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zup.tian-w.cn

[U83] JS：ES Module 导入导出
来源：http://cxn.daxiang520.top

export const a = 1;  import { a } from "./m.js";
来源：http://woo.hnqzz.top

[U84] JS：CommonJS 写法
来源：http://qpl.c1oappe.top

module.exports = { a };  const { a } = require("./m");
来源：http://muk.vqdsnc.cn

[U85] JS：可选链
来源：http://vrm.vehdjk.com

a?.b?.c
来源：http://dxg.yangfankeji.com

[U86] JS：空值合并
来源：http://wtg.jinghuilouyu.cn

a ?? b
来源：http://bxb.bjfxy.top


<!-- 参考信息 -->