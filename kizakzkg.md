代发 wailian999

[T03] Kotlin：字符串模板
来源：http://zwp.hywenlv.cn

"值: $b"
来源：http://qek.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://sca.jinqigufen.top

val n: String? = null;  n?.length
来源：http://jbr.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://lxt.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqe.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://zzp.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bog.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://uqv.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cie.daria6918.cn

[T08] Kotlin：数据类
来源：http://ttr.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://xkj.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://jmg.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://fkm.sysykeji.top

[T10] Kotlin：默认参数
来源：http://eqh.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tei.gaohongyu789.top

[T11] Kotlin：协程
来源：http://ucw.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zrg.tian-w.cn

[T12] Kotlin：解构声明
来源：http://fap.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://yew.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://hyv.yuxming.cn

val m = mapOf("a" to 1)
来源：http://kxy.jlsjyb.cn

[T14] Kotlin：循环
来源：http://eby.wangdashe.top

for (i in 1..10) println(i)
来源：http://ijo.yueranfly.top

[T15] Kotlin：接口
来源：http://yfp.havefunace.top

interface Shape { fun area(): Double }
来源：http://dgb.guowangkeji.top

[T16] Swift：Hello World
来源：http://qkp.svipenyu.cn

print("Hello")
来源：http://ith.nwbrower.top

[T17] Swift：变量与常量
来源：http://qpk.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://ztk.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://gbr.gaohongyu789.top

"值: \(b)"
来源：http://ufm.cdnleiting.top

[T19] Swift：可选绑定
来源：http://xua.bbcook.cn

if let n = opt { print(n) }
来源：http://uyq.fehbvm.com

[T20] Swift：数组操作
来源：http://lfv.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://rad.ctjpmb.com

[T21] Swift：遍历
来源：http://xzt.svipenyu.cn

for x in a { print(x) }
来源：http://oej.hesvh.cn

[T22] Swift：字典
来源：http://mul.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://ecx.tianlin.xyz

[T23] Swift：函数
来源：http://aob.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ptn.yonumen.top

[T24] Swift：闭包
来源：http://sxg.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jiz.zhongyouzk.top

[T25] Swift：结构体
来源：http://jic.xziqi.cn

struct P { var x: Int }
来源：http://twm.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://omz.jianghu66.top

class A: Base { override func f() {} }
来源：http://lvl.jlsjyb.cn

[T27] Swift：错误处理
来源：http://ncz.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://wlp.birdmap.top

[T28] Swift：枚举
来源：http://jao.chenlongwang.top

enum Color { case red, green }
来源：http://yaa.cashguo.top

[T29] Swift：guard 提前返回
来源：http://unq.cucudq.cn

guard let x = opt else { return }
来源：http://alt.kuanghao11.cn

[T30] Swift：协议
来源：http://jhv.zhengqikj.top

protocol Shape { func area() -> Double }
来源：http://nzg.gogol.net.cn

[T31] Lua：Hello World
来源：http://qoz.hesvh.cn

print("Hello")
来源：http://xpc.c1oappe.top

[T32] Lua：局部变量
来源：http://eqc.aizwys.cn

local a = 1
来源：http://uyh.52xcode.cn

[T33] Lua：表（数组）
来源：http://dce.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vbr.nanxinkj.top

[T34] Lua：遍历表
来源：http://hsf.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oab.316326.xyz

[T35] Lua：字典表
来源：http://fzl.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://xbg.redwolf501.top

[T36] Lua：函数
来源：http://zxv.jqgfzy.top

function add(a, b) return a + b end
来源：http://aqx.epnwcf.com

[T37] Lua：字符串拼接
来源：http://fft.9152youxi.cn

"a" .. "b"
来源：http://oye.andypj.xyz

[T38] Lua：条件
来源：http://voe.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://qzh.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://ayt.yvedp.cn

string.find(s, "%d+")
来源：http://mqy.vehdjk.com

[T40] Lua：元表
来源：http://dze.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://hpa.birdmap.top

[T41] Perl：Hello World
来源：http://nqi.tianlin.xyz

print "Hello\n";
来源：http://jbx.aizwys.cn

[T42] Perl：变量类型
来源：http://xtr.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sws.hnqzz.top

[T43] Perl：字符串插值
来源：http://mqg.yj20258888.top

"值: $a"
来源：http://hhf.xziqi.cn

[T44] Perl：条件
来源：http://bip.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://zaq.ivvv.top

[T45] Perl：数组遍历
来源：http://rkh.tanke756.top

for my $x (@arr) { print $x; }
来源：http://rgn.sxryk.cn

[T46] Perl：哈希操作
来源：http://dbl.birdmap.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://urg.chenlongwang.top

[T47] Perl：正则捕获
来源：http://htn.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://svo.ivvv.top

[T48] Perl：正则替换
来源：http://shv.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://kys.quarkkingdee.top

[T49] Perl：函数
来源：http://feo.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mxi.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://pal.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sko.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://wko.birdmap.top

[T51] Scala：Hello World
来源：http://uhp.yj20258888.top

println("Hello")
来源：http://ndq.shzxlz.cn

[T52] Scala：变量
来源：http://jyz.sxryk.cn

val a = 1;  var b = 2
来源：http://tai.fengsongda.top

[T53] Scala：字符串插值
来源：http://bps.cqqwz.cn

s"值: $b"
来源：http://gjd.sjlbkw.cn

[T54] Scala：集合映射
来源：http://jcc.cdnleiting.top

List(1, 2, 3).map(_ * 2)
来源：http://spk.chenlongwang.top

[T55] Scala：集合过滤
来源：http://omo.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vhf.sysykeji.top

[T56] Scala：样例类
来源：http://ivx.ehwqpu.com

case class User(name: String, age: Int)
来源：http://oxj.jiagoushi.top

[T57] Scala：模式匹配
来源：http://dzn.52xcode.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oev.fengsongda.top

[T58] Scala：函数定义
来源：http://sri.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://msd.smart0.xyz

[T59] Scala：循环
来源：http://yqv.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://shk.fktsv.cn

[T60] Scala：折叠
来源：http://apm.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pxi.tanke756.top

================================================================================
来源：http://dzc.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vnl.jlsjyb.cn

================================================================================
来源：http://ckc.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://dio.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://voa.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://spq.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwp.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://xiy.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pkc.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://xpt.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fan.fktsv.cn

[U05] Py：列表去重且保序
来源：http://phc.zhixingplan.top

list(dict.fromkeys(arr))
来源：http://fwq.epnwcf.com

[U06] Py：合并两个字典
来源：http://upr.uphjek.com

{**a, **b}
来源：http://pxc.9152youxi.cn

[U07] Py：反转字典键值
来源：http://kvk.ivvv.top

{v: k for k, v in d.items()}
来源：http://omk.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://tnj.xingfuxueyuan.xyz

[y for x in nested for y in x]
来源：http://czr.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://scj.vehdjk.com

max(d, key=d.get)
来源：http://rvg.birdmap.top

[U10] Py：按值排序字典
来源：http://cic.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjj.tianlin.xyz

[U11] Py：生成器表达式
来源：http://mqe.jiagoushi.top

(x * 2 for x in arr)
来源：http://bvm.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://pue.yuanzhike.top

Counter(arr).most_common(3)
来源：http://iwi.dashuyun.cn

[U13] Py：固定长度队列
来源：http://xkx.epnwcf.com

deque(maxlen=10)
来源：http://fkd.uphjek.com

[U14] Py：分组收集到列表
来源：http://fnd.cheryme.top

defaultdict(list)
来源：http://gfx.52xcode.cn

[U15] Py：高精度计时
来源：http://ymb.kuanghao11.cn

t = time.perf_counter()
来源：http://uze.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://ixz.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xub.hysaishi.cn

[U17] Py：初始化日志
来源：http://kha.zhoulong.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ecq.tanke756.top

[U18] Py：预编译正则
来源：http://nzq.svipenyu.cn

pat = re.compile(r"\d+")
来源：http://iwh.aibaodan.cn

[U19] Py：正则替换带回调
来源：http://nzg.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nuc.vehdjk.com

[U20] Py：缓存函数结果
来源：http://rsl.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://wjr.sxryk.cn

[U21] Py：自定义上下文管理器
来源：http://vym.jlsjyb.cn

@contextlib.contextmanager
来源：http://pnq.yuxming.cn

[U22] Py：矩阵转置
来源：http://wts.shanyushiyangtech.top

list(zip(*m))
来源：http://bor.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://ocv.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qkg.snrcjt.cn

[U24] Py：路径操作
来源：http://men.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ekr.vqdsnc.cn

[U25] Py：CSV 按字典读
来源：http://swi.xinyue.icu

csv.DictReader(f)
来源：http://sbc.ybcxt.top

[U26] Py：并发下载
来源：http://rki.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gnx.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://bgg.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://zgs.gotoacloud.top

[U28] Py：类型别名
来源：http://bsp.tanke756.top

UserId = int
来源：http://nxt.yuanzhike.top

[U29] Py：属性校验
来源：http://nob.xylfe.cn

@property 与 @x.setter 配合
来源：http://jma.guannengcc.top

[U30] Py：数据类
来源：http://agc.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://qby.aibaodan.cn

[U31] Py：单测
来源：http://reh.dianchejie.cn

python -m pytest -q
来源：http://ghg.zhijiandao.cn

[U32] Py：代码格式化
来源：http://tey.52xcode.cn

ruff format . && ruff check --fix .
来源：http://rqy.dashuyun.cn

[U33] Py：打包发布
来源：http://vjv.jinyuanbaomall.cn

python -m build  （依赖 pyproject.toml）
来源：http://tcv.andypj.xyz

[U34] Py：判断编码
来源：http://ucl.shanyushiyangtech.top

chardet.detect(raw)
来源：http://tmv.xingfuxueyuan.xyz

[U35] Py：发送邮件
来源：http://gwd.cdnleiting.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kax.zhengqikj.top

[U36] Py：定时任务
来源：http://ned.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://fsk.zhixingplan.top

[U37] Py：读写 Excel
来源：http://gnb.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://zfb.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://mck.ehwqpu.com

Path(__file__).resolve().parent
来源：http://ajs.fehbvm.com

[U39] Py：判断是否在交互环境
来源：http://xef.zhengqikj.top

sys.stdout.isatty()
来源：http://llm.redwolf501.top

[U40] Py：打印到标准错误
来源：http://uxu.yuxming.cn

print("err", file=sys.stderr)
来源：http://lji.sxryk.cn

[U41] PHP：初始化 Composer 项目
来源：http://dzb.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zfc.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://aws.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ghq.hesvh.cn

[U43] PHP：声明命名空间
来源：http://mlh.jlsjyb.cn

namespace App\Http;
来源：http://xdt.zhixingplan.top

[U44] PHP：开启严格类型
来源：http://svl.tarul.cn

declare(strict_types=1);
来源：http://kqx.hysaishi.cn

[U45] PHP：类型声明与返回类型
来源：http://ksr.tarul.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fbj.fzhhl.top

[U46] PHP：可空类型
来源：http://ygb.zhijiandao.cn

?string $name = null
来源：http://dvx.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://way.yvedp.cn

int|string $id
来源：http://bzy.9152youxi.cn

[U48] PHP：纯枚举
来源：http://awq.shanyushiyangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://leo.pycfn.com

[U49] PHP：只读属性
来源：http://fdp.9152youxi.cn

public readonly string $name
来源：http://wil.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://ehh.gotoacloud.top

public function __construct(private int $id) {}
来源：http://bec.yuanzhike.top

[U51] PHP：数组解构
来源：http://ldn.sufxvd.cn

[$a, $b] = $arr;
来源：http://svr.sufxvd.cn

[U52] PHP：箭头函数
来源：http://yzh.pycfn.com

$double = fn($x) => $x * 2;
来源：http://djp.fktsv.cn

[U53] PHP：空合并运算符
来源：http://qhh.yanxiufei.cn

$v = $a ?? $b ?? "default";
来源：http://ivl.zhiwuduotai.top

[U54] PHP：空安全调用
来源：http://she.hnxiangtu.top

$obj?->method()
来源：http://sos.9152youxi.cn

[U55] PHP：match 表达式
来源：http://bfb.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ohp.ehwqpu.com

[U56] PHP：命名参数
来源：http://xls.zhoulong.xyz

f(a: 1, b: 2)
来源：http://rws.52xcode.cn

[U57] PHP：字符串插值
来源：http://gig.ywan-chungtsiang.top

"值: {$a}"
来源：http://nyl.cashguo.top

[U58] PHP：数组三件套
来源：http://zdi.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iuy.ehwqpu.com

[U59] PHP：自定义排序
来源：http://gvp.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ouw.iojbl.cn

[U60] PHP：JSON 编解码
来源：http://irn.yj202588.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zhu.sxryk.cn

[U61] PHP：正则
来源：http://ryb.jlsjyb.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ouc.smart0.xyz

[U62] PHP：日期对象
来源：http://khw.ctjpmb.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qjs.jlsjyb.cn

[U63] PHP：文件读写
来源：http://ldq.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wzb.redwolf501.top

[U64] PHP：目录遍历
来源：http://sby.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://aoc.yuxming.cn

[U65] PHP：会话
来源：http://ybr.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kcy.316326.xyz

[U66] PHP：设置 Cookie
来源：http://mvm.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mdq.yueranfly.top

[U67] PHP：处理文件上传
来源：http://bwy.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://shv.cashguo.top

[U68] PHP：PDO 连接
来源：http://fyt.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rdi.havefunace.top

[U69] PHP：PDO 预处理
来源：http://ojn.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rxw.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://prx.tanke756.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rlm.cucudq.cn

[U71] PHP：抛出异常
来源：http://jly.gogol.net.cn

throw new RuntimeException("失败", 500);
来源：http://wtj.shzxlz.cn

[U72] PHP：写错误日志
来源：http://uir.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://hmp.xuanzx.com

[U73] PHP：读取 ini 配置
来源：http://eks.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://kpb.bjfxy.top

[U74] PHP：读取环境变量
来源：http://xvx.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://qza.fengsongda.top

[U75] PHP：依赖注入
来源：http://efv.zhengqikj.top

composer require psr/container
来源：http://ijd.fengsongda.top

[U76] PHP：简单路由
来源：http://rgy.ydjk.org.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kut.fzhhl.top

[U77] PHP：模板渲染
来源：http://ugf.zhixingplan.top

composer require twig/twig
来源：http://hel.yj202588.top

[U78] PHP：单元测试
来源：http://dtp.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://fed.yanxiufei.cn

[U79] PHP：静态分析
来源：http://ttt.tarul.cn

composer require --dev phpstan/phpstan
来源：http://svx.yfazqb.com

[U80] PHP：代码规范修复
来源：http://ihu.ppjwa.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dkz.jqgfzy.top

[U81] JS：初始化项目
来源：http://sqx.zhaomingkeji.xyz

npm init -y;  npm i express
来源：http://vmq.zycfv.cn

[U82] JS：package.json 脚本
来源：http://bba.fktsv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tde.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://wla.snrcjt.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cyb.hammf.cn

[U84] JS：CommonJS 写法
来源：http://hof.fktsv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bmj.vqdsnc.cn

[U85] JS：可选链
来源：http://lqq.sjlbkw.cn

a?.b?.c
来源：http://iet.yj202588.top

[U86] JS：空值合并
来源：http://qmg.yongpay.top

a ?? b
来源：http://uvo.pycfn.com

[U87] JS：解构默认值
来源：http://mby.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://xsv.ivvv.top

[U88] JS：对象展开合并
来源：http://cyh.zdqjudy.top

{ ...a, ...b }
来源：http://rxc.sufxvd.cn

[U89] JS：数组去重
来源：http://osd.gotoacloud.top

[...new Set(arr)]
来源：http://luh.yuanzhike.top

[U90] JS：数字数组排序
来源：http://xel.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://bcb.mhx1999.top


<!-- 参考信息 -->