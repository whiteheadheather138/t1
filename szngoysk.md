代发 wailian999

[T03] Kotlin：字符串模板
来源：http://kba.iojbl.cn

"值: $b"
来源：http://ljh.ppjwa.cn

[T04] Kotlin：空安全
来源：http://yrv.yvedp.cn

val n: String? = null;  n?.length
来源：http://imt.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://kfp.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://usf.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://iny.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yka.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://kks.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aaw.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://qtl.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://lsc.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://ssv.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://euo.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://wmv.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jpx.tanke756.top

[T11] Kotlin：协程
来源：http://cet.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uko.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://eaa.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://hfv.cheryme.top

[T13] Kotlin：只读 Map
来源：http://dch.ivvv.top

val m = mapOf("a" to 1)
来源：http://poi.xuanzx.com

[T14] Kotlin：循环
来源：http://stt.ybcxt.top

for (i in 1..10) println(i)
来源：http://skt.fengsongda.top

[T15] Kotlin：接口
来源：http://bzw.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://scm.cdnleiting.top

[T16] Swift：Hello World
来源：http://vhu.0kj1m.cn

print("Hello")
来源：http://kfk.316326.xyz

[T17] Swift：变量与常量
来源：http://jjf.yj20258.top

var a = 1;  let b = 2
来源：http://cpi.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://ejk.jinqigufen.top

"值: \(b)"
来源：http://igg.sysykeji.top

[T19] Swift：可选绑定
来源：http://umq.chenlongwang.top

if let n = opt { print(n) }
来源：http://oiw.hysaishi.cn

[T20] Swift：数组操作
来源：http://yoz.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://ndt.nwbrower.top

[T21] Swift：遍历
来源：http://mun.hfpthk.cn

for x in a { print(x) }
来源：http://hju.zhengqikj.top

[T22] Swift：字典
来源：http://net.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://owr.guannengcc.top

[T23] Swift：函数
来源：http://jtq.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://btn.bjfxy.top

[T24] Swift：闭包
来源：http://zsv.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ynu.jyoumei.cn

[T25] Swift：结构体
来源：http://emt.fktsv.cn

struct P { var x: Int }
来源：http://kci.zdqjudy.top

[T26] Swift：类与重写
来源：http://xje.ctjpmb.com

class A: Base { override func f() {} }
来源：http://obz.yanxiufei.cn

[T27] Swift：错误处理
来源：http://ieh.vehdjk.com

do { try f() } catch { print(error) }
来源：http://dla.fzhhl.top

[T28] Swift：枚举
来源：http://fye.cashguo.top

enum Color { case red, green }
来源：http://etw.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://xwc.jinqigfzy.top

guard let x = opt else { return }
来源：http://ovn.shanyushiyangtech.top

[T30] Swift：协议
来源：http://knj.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://wdu.zhongyouzk.top

[T31] Lua：Hello World
来源：http://ikl.mhx1999.top

print("Hello")
来源：http://xgr.wangdashe.top

[T32] Lua：局部变量
来源：http://xvk.bbcook.cn

local a = 1
来源：http://kym.andypj.xyz

[T33] Lua：表（数组）
来源：http://wzo.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kyk.hammf.cn

[T34] Lua：遍历表
来源：http://byw.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://owo.ydzc1.top

[T35] Lua：字典表
来源：http://fmz.cqqwz.cn

local d = { a = 1 };  d.b = 2
来源：http://zir.fengsongda.top

[T36] Lua：函数
来源：http://hdd.guannengcc.top

function add(a, b) return a + b end
来源：http://lgj.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://dpb.ywan-chungtsiang.top

"a" .. "b"
来源：http://ztj.fengsongda.top

[T38] Lua：条件
来源：http://tqr.cashguo.top

if x > 0 then print("正") end
来源：http://ghc.tanke756.top

[T39] Lua：模式匹配
来源：http://exj.ppjwa.cn

string.find(s, "%d+")
来源：http://fsq.smart0.xyz

[T40] Lua：元表
来源：http://cmv.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://zik.hnxiangtu.top

[T41] Perl：Hello World
来源：http://lob.zdbjq.cn

print "Hello\n";
来源：http://ebp.shzxlz.cn

[T42] Perl：变量类型
来源：http://cxu.shuidangran.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://omu.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://xdg.yangfankeji.com

"值: $a"
来源：http://ciu.9152youxi.cn

[T44] Perl：条件
来源：http://hib.52xcode.cn

if ($a > 0) { print "正"; }
来源：http://qzs.ehwqpu.com

[T45] Perl：数组遍历
来源：http://nxw.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://qhd.birdmap.top

[T46] Perl：哈希操作
来源：http://amd.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://asq.xinyue.icu

[T47] Perl：正则捕获
来源：http://lmd.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://crl.vqdsnc.cn

[T48] Perl：正则替换
来源：http://vlt.yvedp.cn

$s =~ s/old/new/g;
来源：http://fjj.yueranfly.top

[T49] Perl：函数
来源：http://tyq.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nsc.ybcxt.top

[T50] Perl：逐行读文件
来源：http://tmt.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zhs.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://bki.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://mmq.fehbvm.com

println("Hello")
来源：http://kon.shuidangran.top

[T52] Scala：变量
来源：http://sgk.ivvv.top

val a = 1;  var b = 2
来源：http://fpm.yfazqb.com

[T53] Scala：字符串插值
来源：http://bxu.hywenlv.cn

s"值: $b"
来源：http://uqe.zycfv.cn

[T54] Scala：集合映射
来源：http://omf.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://yba.vehdjk.com

[T55] Scala：集合过滤
来源：http://bfq.zhoulong.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://jsi.xuanzx.com

[T56] Scala：样例类
来源：http://yay.aibaodan.cn

case class User(name: String, age: Int)
来源：http://tow.smart0.xyz

[T57] Scala：模式匹配
来源：http://gom.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fhc.zhixingplan.top

[T58] Scala：函数定义
来源：http://mkt.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://taz.yj202588.top

[T59] Scala：循环
来源：http://zzs.guannengcc.top

for (i <- 1 to 10) println(i)
来源：http://xsx.yangfankeji.com

[T60] Scala：折叠
来源：http://fmt.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pga.yongpay.top

================================================================================
来源：http://irt.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://stx.aizwys.cn

================================================================================
来源：http://rkt.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://jfg.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://rxp.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://kab.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xgn.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://fpa.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ufe.bjfxy.top

[U04] Py：变量调试打印
来源：http://ava.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fbm.xinyue.icu

[U05] Py：列表去重且保序
来源：http://psk.wangdashe.top

list(dict.fromkeys(arr))
来源：http://cnp.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://gap.yuxming.cn

{**a, **b}
来源：http://pnu.daxiang520.top

[U07] Py：反转字典键值
来源：http://jhn.uphjek.com

{v: k for k, v in d.items()}
来源：http://hcl.yanxiufei.cn

[U08] Py：展平二维列表
来源：http://yrp.jinqigfzy.top

[y for x in nested for y in x]
来源：http://yxb.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://rsd.fehbvm.com

max(d, key=d.get)
来源：http://fdi.jinghuilouyu.cn

[U10] Py：按值排序字典
来源：http://svz.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdi.jyoumei.cn

[U11] Py：生成器表达式
来源：http://vva.tian-w.cn

(x * 2 for x in arr)
来源：http://utq.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://nfw.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://chc.sweek.top

[U13] Py：固定长度队列
来源：http://rwh.cashguo.top

deque(maxlen=10)
来源：http://qcl.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://fcq.zhengqikj.top

defaultdict(list)
来源：http://ris.gotoacloud.top

[U15] Py：高精度计时
来源：http://vrz.fzhhl.top

t = time.perf_counter()
来源：http://lne.yueranfly.top

[U16] Py：命令行参数解析
来源：http://uey.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rwg.fehbvm.com

[U17] Py：初始化日志
来源：http://dew.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://kyr.birdmap.top

[U18] Py：预编译正则
来源：http://pcr.zycfv.cn

pat = re.compile(r"\d+")
来源：http://kzs.cheryme.top

[U19] Py：正则替换带回调
来源：http://iyi.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fiv.hywenlv.cn

[U20] Py：缓存函数结果
来源：http://rhy.yangfankeji.com

@functools.lru_cache(maxsize=None)
来源：http://xph.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://geu.jinqigfzy.top

@contextlib.contextmanager
来源：http://ewn.fengsongda.top

[U22] Py：矩阵转置
来源：http://pfq.pengpengdd.cyou

list(zip(*m))
来源：http://ewg.havefunace.top

[U23] Py：分块读取大文件
来源：http://zra.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pfh.jinqigfzy.top

[U24] Py：路径操作
来源：http://kza.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xax.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://qlb.yueranfly.top

csv.DictReader(f)
来源：http://vwu.nanxinkj.top

[U26] Py：并发下载
来源：http://ytw.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pgq.jianghu66.top

[U27] Py：异步 HTTP
来源：http://prw.yuxming.cn

aiohttp.ClientSession() 配合 async with
来源：http://xti.cdnleiting.top

[U28] Py：类型别名
来源：http://iru.feifeiyinyue.top

UserId = int
来源：http://tdu.quarkkingdee.top

[U29] Py：属性校验
来源：http://vzm.meibo888.top

@property 与 @x.setter 配合
来源：http://zxl.yonumen.top

[U30] Py：数据类
来源：http://rug.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://ukz.wangdashe.top

[U31] Py：单测
来源：http://vjv.hnxiangtu.top

python -m pytest -q
来源：http://eve.316326.xyz

[U32] Py：代码格式化
来源：http://rda.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://dlm.yongpay.top

[U33] Py：打包发布
来源：http://mrm.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://vnk.hnqzz.top

[U34] Py：判断编码
来源：http://qzw.sweek.top

chardet.detect(raw)
来源：http://dyu.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://kyl.gogol.net.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wim.hcnkem.com

[U36] Py：定时任务
来源：http://tjm.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://jmq.smart0.xyz

[U37] Py：读写 Excel
来源：http://kvx.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ocj.jinyuanbaomall.cn

[U38] Py：获取脚本所在目录
来源：http://ojb.ybcxt.top

Path(__file__).resolve().parent
来源：http://lyz.ctjpmb.com

[U39] Py：判断是否在交互环境
来源：http://snv.quarkkingdee.top

sys.stdout.isatty()
来源：http://xfi.xuanzx.com

[U40] Py：打印到标准错误
来源：http://bpr.cdnleiting.top

print("err", file=sys.stderr)
来源：http://tje.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://xpn.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://lqr.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://sex.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gnp.sjlbkw.cn

[U43] PHP：声明命名空间
来源：http://yod.316326.xyz

namespace App\Http;
来源：http://cor.kuanghao11.cn

[U44] PHP：开启严格类型
来源：http://rgw.cqqwz.cn

declare(strict_types=1);
来源：http://fvv.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://jee.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://bsj.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://nbe.shanyushiyangtech.top

?string $name = null
来源：http://nql.haohaochexian.top

[U47] PHP：联合类型
来源：http://eyp.hammf.cn

int|string $id
来源：http://yqo.aizwys.cn

[U48] PHP：纯枚举
来源：http://pwn.316326.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vhg.hywenlv.cn

[U49] PHP：只读属性
来源：http://qex.hongshengwenyu.top

public readonly string $name
来源：http://otm.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://dpd.dashuyun.cn

public function __construct(private int $id) {}
来源：http://ghg.tarul.cn

[U51] PHP：数组解构
来源：http://zkx.yueranfly.top

[$a, $b] = $arr;
来源：http://udw.redwolf501.top

[U52] PHP：箭头函数
来源：http://spv.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://syf.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://dzx.316326.xyz

$v = $a ?? $b ?? "default";
来源：http://pfh.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://mrb.ydjk.org.cn

$obj?->method()
来源：http://yrg.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://nkj.yueranfly.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yzx.bbcook.cn

[U56] PHP：命名参数
来源：http://fzl.xuanzx.com

f(a: 1, b: 2)
来源：http://qhs.wangdashe.top

[U57] PHP：字符串插值
来源：http://yeb.jqgufenzy.top

"值: {$a}"
来源：http://zsr.52xcode.cn

[U58] PHP：数组三件套
来源：http://pdd.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mda.tian-w.cn

[U59] PHP：自定义排序
来源：http://pqs.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://thi.hongshengwenyu.top

[U60] PHP：JSON 编解码
来源：http://nyx.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qan.xylfe.cn

[U61] PHP：正则
来源：http://zwn.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pka.hammf.cn

[U62] PHP：日期对象
来源：http://pmz.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://usp.gaohongyu789.top

[U63] PHP：文件读写
来源：http://drb.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sya.fzhhl.top

[U64] PHP：目录遍历
来源：http://qtk.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://swc.vehdjk.com

[U65] PHP：会话
来源：http://amz.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://udl.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://twz.shzxlz.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zfi.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://fdc.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sha.birdmap.top

[U68] PHP：PDO 连接
来源：http://ktl.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xag.yanxiufei.cn

[U69] PHP：PDO 预处理
来源：http://tpk.gzhubu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ltf.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://xui.yvedp.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mat.xinyue.icu

[U71] PHP：抛出异常
来源：http://pya.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://tgy.vehdjk.com

[U72] PHP：写错误日志
来源：http://yqy.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://zch.zhijiandao.cn

[U73] PHP：读取 ini 配置
来源：http://tlq.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://abi.yueranfly.top

[U74] PHP：读取环境变量
来源：http://aiw.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://ats.52xcode.cn

[U75] PHP：依赖注入
来源：http://uom.hfpthk.cn

composer require psr/container
来源：http://cyl.pycfn.com

[U76] PHP：简单路由
来源：http://opi.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bkn.sysykeji.top

[U77] PHP：模板渲染
来源：http://tqo.birdmap.top

composer require twig/twig
来源：http://vzl.aizwys.cn

[U78] PHP：单元测试
来源：http://xqp.jinghuilouyu.cn

composer require --dev phpunit/phpunit
来源：http://ojz.pengpengdd.cyou

[U79] PHP：静态分析
来源：http://teq.snrcjt.cn

composer require --dev phpstan/phpstan
来源：http://mii.pengpengdd.cyou

[U80] PHP：代码规范修复
来源：http://qef.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://pid.hfpthk.cn

[U81] JS：初始化项目
来源：http://jek.hcnkem.com

npm init -y;  npm i express
来源：http://kok.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://hse.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://erx.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://jwa.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://lgf.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://zxp.gaohongyu789.top

module.exports = { a };  const { a } = require("./m");
来源：http://vra.fktsv.cn

[U85] JS：可选链
来源：http://yfg.316326.xyz

a?.b?.c
来源：http://toi.jqgufenzy.top

[U86] JS：空值合并
来源：http://shz.fengsongda.top

a ?? b
来源：http://uhe.tarul.cn

[U87] JS：解构默认值
来源：http://ofo.hcnkem.com

const { a = 1, b = 2 } = obj;
来源：http://aat.316326.xyz

[U88] JS：对象展开合并
来源：http://wun.yongpay.top

{ ...a, ...b }
来源：http://xwy.gotoacloud.top

[U89] JS：数组去重
来源：http://rue.jinqigfzy.top

[...new Set(arr)]
来源：http://ojz.gzhubu.top

[U90] JS：数字数组排序
来源：http://uva.shanyushiyangkeji.top

[...arr].sort((a, b) => a - b)
来源：http://knd.tarul.cn


<!-- 参考信息 -->