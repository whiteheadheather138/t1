代发 wailian999

[T05] Kotlin：when 表达式
来源：http://ctp.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdl.tarul.cn

[T06] Kotlin：集合映射
来源：http://bvt.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jpd.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://itz.daria6918.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lvu.gogol.net.cn

[T08] Kotlin：数据类
来源：http://byl.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://png.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://kcj.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://peo.yueranfly.top

[T10] Kotlin：默认参数
来源：http://djq.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mwp.shzxlz.cn

[T11] Kotlin：协程
来源：http://ahs.yj202588.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://psr.hesvh.cn

[T12] Kotlin：解构声明
来源：http://hrw.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://nue.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://iui.yonumen.top

val m = mapOf("a" to 1)
来源：http://hgs.chenlongwang.top

[T14] Kotlin：循环
来源：http://xdk.nanxinkj.top

for (i in 1..10) println(i)
来源：http://hzp.hysaishi.cn

[T15] Kotlin：接口
来源：http://afe.shuidangran.top

interface Shape { fun area(): Double }
来源：http://aqc.0kj1m.cn

[T16] Swift：Hello World
来源：http://cxe.yuxming.cn

print("Hello")
来源：http://hvv.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://xjd.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://vvu.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://dbw.uphjek.com

"值: \(b)"
来源：http://cpi.pycfn.com

[T19] Swift：可选绑定
来源：http://zvu.ydjk.org.cn

if let n = opt { print(n) }
来源：http://gid.zhoulong.xyz

[T20] Swift：数组操作
来源：http://wwb.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gms.andypj.xyz

[T21] Swift：遍历
来源：http://itd.sweek.top

for x in a { print(x) }
来源：http://qrd.guowangkeji.top

[T22] Swift：字典
来源：http://yom.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://ouc.hammf.cn

[T23] Swift：函数
来源：http://vnn.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xoy.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://qvz.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qai.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://uic.redwolf501.top

struct P { var x: Int }
来源：http://qtt.sweek.top

[T26] Swift：类与重写
来源：http://luj.sysykeji.top

class A: Base { override func f() {} }
来源：http://smb.quarkkingdee.top

[T27] Swift：错误处理
来源：http://ule.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://qpt.havefunace.top

[T28] Swift：枚举
来源：http://siv.gogol.net.cn

enum Color { case red, green }
来源：http://rsb.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://ftk.nwbrower.top

guard let x = opt else { return }
来源：http://nnd.dashuyun.cn

[T30] Swift：协议
来源：http://zxk.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://jpr.ppjwa.cn

[T31] Lua：Hello World
来源：http://hdz.fehbvm.com

print("Hello")
来源：http://htk.redwolf501.top

[T32] Lua：局部变量
来源：http://cuv.yfazqb.com

local a = 1
来源：http://tqs.haohaochexian.top

[T33] Lua：表（数组）
来源：http://nqg.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lte.snrcjt.cn

[T34] Lua：遍历表
来源：http://huu.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kuh.jyoumei.cn

[T35] Lua：字典表
来源：http://bxa.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://xjv.tarul.cn

[T36] Lua：函数
来源：http://uoc.jinqigfzy.top

function add(a, b) return a + b end
来源：http://oyb.ydzc1.top

[T37] Lua：字符串拼接
来源：http://zln.hysaishi.cn

"a" .. "b"
来源：http://evm.pycfn.com

[T38] Lua：条件
来源：http://ugm.nanxuanxn.top

if x > 0 then print("正") end
来源：http://wxd.havefunace.top

[T39] Lua：模式匹配
来源：http://gwd.zhongyouzk.top

string.find(s, "%d+")
来源：http://ofg.yueranfly.top

[T40] Lua：元表
来源：http://kjg.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://umf.yvedp.cn

[T41] Perl：Hello World
来源：http://ccc.fktsv.cn

print "Hello\n";
来源：http://iph.yj202588.top

[T42] Perl：变量类型
来源：http://rdv.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://thx.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://adf.cashguo.top

"值: $a"
来源：http://qcf.hnqzz.top

[T44] Perl：条件
来源：http://ket.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://ybf.yuanzhike.top

[T45] Perl：数组遍历
来源：http://gdq.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://ruc.meibo888.top

[T46] Perl：哈希操作
来源：http://bgc.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bcc.hnqzz.top

[T47] Perl：正则捕获
来源：http://wsf.fktsv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://asr.jqgufenzy.top

[T48] Perl：正则替换
来源：http://euf.jqgfzy.top

$s =~ s/old/new/g;
来源：http://pqs.shanyushiyangtech.top

[T49] Perl：函数
来源：http://jpz.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gso.c1oappe.top

[T50] Perl：逐行读文件
来源：http://iwu.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gco.zhixingplan.top

while (my $line = <$fh>) { print $line; }
来源：http://tqe.ybcxt.top

[T51] Scala：Hello World
来源：http://tjq.jinyuanbaomall.cn

println("Hello")
来源：http://ebw.jqgufenzy.top

[T52] Scala：变量
来源：http://fbq.yvedp.cn

val a = 1;  var b = 2
来源：http://zkh.jyoumei.cn

[T53] Scala：字符串插值
来源：http://pzj.zhijiandao.cn

s"值: $b"
来源：http://ufz.jinyuanbaomall.cn

[T54] Scala：集合映射
来源：http://tsp.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://rki.nwbrower.top

[T55] Scala：集合过滤
来源：http://ooa.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://xlw.sufxvd.cn

[T56] Scala：样例类
来源：http://odn.sysykeji.top

case class User(name: String, age: Int)
来源：http://dex.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://woc.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kqz.hnxiangtu.top

[T58] Scala：函数定义
来源：http://fsx.redwolf501.top

def add(a: Int, b: Int): Int = a + b
来源：http://nra.gzhubu.top

[T59] Scala：循环
来源：http://awk.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://mtk.chenjidiqi.icu

[T60] Scala：折叠
来源：http://dcv.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wot.cheryme.top

================================================================================
来源：http://rdp.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://myd.uphjek.com

================================================================================
来源：http://lff.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://tby.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ode.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://eht.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cje.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://hdw.havefunace.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sgt.chenlongwang.top

[U04] Py：变量调试打印
来源：http://ykl.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uhi.zdqjudy.top

[U05] Py：列表去重且保序
来源：http://kli.yonumen.top

list(dict.fromkeys(arr))
来源：http://ekq.yfazqb.com

[U06] Py：合并两个字典
来源：http://cqi.vehdjk.com

{**a, **b}
来源：http://zhh.zhaomingkeji.xyz

[U07] Py：反转字典键值
来源：http://rva.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://xhr.havefunace.top

[U08] Py：展平二维列表
来源：http://arh.nanxuanxn.top

[y for x in nested for y in x]
来源：http://qfn.ivvv.top

[U09] Py：字典取最大值的键
来源：http://ygc.fanxiaobao.xyz

max(d, key=d.get)
来源：http://kpi.zycfv.cn

[U10] Py：按值排序字典
来源：http://ghx.zhengqikj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mky.sjlbkw.cn

[U11] Py：生成器表达式
来源：http://lje.fehbvm.com

(x * 2 for x in arr)
来源：http://wlr.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://oab.cheryme.top

Counter(arr).most_common(3)
来源：http://dmb.fengsongda.top

[U13] Py：固定长度队列
来源：http://wfd.haohaochexian.top

deque(maxlen=10)
来源：http://rjt.ydzc1.top

[U14] Py：分组收集到列表
来源：http://zro.zdqjudy.top

defaultdict(list)
来源：http://hai.vehdjk.com

[U15] Py：高精度计时
来源：http://cmc.jinghuilouyu.cn

t = time.perf_counter()
来源：http://gyr.yongpay.top

[U16] Py：命令行参数解析
来源：http://kwv.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ycx.hfpthk.cn

[U17] Py：初始化日志
来源：http://hab.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://wsj.hcnkem.com

[U18] Py：预编译正则
来源：http://tjw.c1oappe.top

pat = re.compile(r"\d+")
来源：http://xrf.hcnkem.com

[U19] Py：正则替换带回调
来源：http://hpg.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wpg.jqgufenzy.top

[U20] Py：缓存函数结果
来源：http://yey.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://oww.aibaodan.cn

[U21] Py：自定义上下文管理器
来源：http://ncf.wangdashe.top

@contextlib.contextmanager
来源：http://jyf.zhongyouzk.top

[U22] Py：矩阵转置
来源：http://fqc.zhoulong.xyz

list(zip(*m))
来源：http://wug.yongpay.top

[U23] Py：分块读取大文件
来源：http://ign.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://amk.cashguo.top

[U24] Py：路径操作
来源：http://dka.zhixingplan.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wiv.guannengcc.top

[U25] Py：CSV 按字典读
来源：http://kry.aizwys.cn

csv.DictReader(f)
来源：http://itj.xylfe.cn

[U26] Py：并发下载
来源：http://bin.hongshengwenyu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mja.tanke756.top

[U27] Py：异步 HTTP
来源：http://wlu.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://wsl.hfpthk.cn

[U28] Py：类型别名
来源：http://fky.guowangkeji.top

UserId = int
来源：http://dqc.tianlin.xyz

[U29] Py：属性校验
来源：http://yzn.gogol.net.cn

@property 与 @x.setter 配合
来源：http://tdv.hongshengwenyu.top

[U30] Py：数据类
来源：http://ypf.cdnleiting.top

@dataclass(slots=True)
来源：http://cnt.svipenyu.cn

[U31] Py：单测
来源：http://sdn.ehwqpu.com

python -m pytest -q
来源：http://ldv.haohaochexian.top

[U32] Py：代码格式化
来源：http://dvh.guowangkeji.top

ruff format . && ruff check --fix .
来源：http://xxi.snrcjt.cn

[U33] Py：打包发布
来源：http://hht.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://hfc.dianchejie.cn

[U34] Py：判断编码
来源：http://vkr.fktsv.cn

chardet.detect(raw)
来源：http://jqw.sjlbkw.cn

[U35] Py：发送邮件
来源：http://cok.ppjwa.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://noi.dashuyun.cn

[U36] Py：定时任务
来源：http://xpu.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://nsn.fktsv.cn

[U37] Py：读写 Excel
来源：http://aic.vqdsnc.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cdh.aibaodan.cn

[U38] Py：获取脚本所在目录
来源：http://mnb.ctjpmb.com

Path(__file__).resolve().parent
来源：http://jgi.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://jhf.yonumen.top

sys.stdout.isatty()
来源：http://dlx.fengsongda.top

[U40] Py：打印到标准错误
来源：http://bck.shuidangran.top

print("err", file=sys.stderr)
来源：http://zrs.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://dyb.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xgv.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://qqc.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dbr.yfazqb.com

[U43] PHP：声明命名空间
来源：http://syh.ppjwa.cn

namespace App\Http;
来源：http://hsv.cheryme.top

[U44] PHP：开启严格类型
来源：http://rfs.gogol.net.cn

declare(strict_types=1);
来源：http://wtb.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://keo.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tqh.fanxiaobao.xyz

[U46] PHP：可空类型
来源：http://gaz.sysykeji.top

?string $name = null
来源：http://ikg.yj20258.top

[U47] PHP：联合类型
来源：http://dhb.yueranfly.top

int|string $id
来源：http://lrs.xuanzx.com

[U48] PHP：纯枚举
来源：http://pww.xziqi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ryu.wangdashe.top

[U49] PHP：只读属性
来源：http://peh.fanxiaobao.xyz

public readonly string $name
来源：http://akf.nanxuanxn.top

[U50] PHP：构造器属性提升
来源：http://exe.yj20258888.top

public function __construct(private int $id) {}
来源：http://jpl.nanxuanxn.top

[U51] PHP：数组解构
来源：http://sfa.xuanzx.com

[$a, $b] = $arr;
来源：http://tgj.gzhubu.top

[U52] PHP：箭头函数
来源：http://tsk.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://eko.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://mwi.ctjpmb.com

$v = $a ?? $b ?? "default";
来源：http://zfm.xuanzx.com

[U54] PHP：空安全调用
来源：http://icq.ywan-chungtsiang.top

$obj?->method()
来源：http://ldi.yuxming.cn

[U55] PHP：match 表达式
来源：http://jtp.yongpay.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://anu.aizwys.cn

[U56] PHP：命名参数
来源：http://xtn.sufxvd.cn

f(a: 1, b: 2)
来源：http://zie.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://pbg.zhijiandao.cn

"值: {$a}"
来源：http://cjr.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://alr.andypj.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://txa.nanxinkj.top

[U59] PHP：自定义排序
来源：http://wzh.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lff.yongpay.top

[U60] PHP：JSON 编解码
来源：http://suf.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pcm.dianchejie.cn

[U61] PHP：正则
来源：http://lms.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bvq.bjfxy.top

[U62] PHP：日期对象
来源：http://dmk.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hje.zycfv.cn

[U63] PHP：文件读写
来源：http://vcd.daxiang520.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ylx.yj20258888.top

[U64] PHP：目录遍历
来源：http://els.svipenyu.cn

glob("dir/*.php");  scandir("dir");
来源：http://hoz.snrcjt.cn

[U65] PHP：会话
来源：http://bub.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bik.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://sia.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://arx.chenzaomai.com

[U67] PHP：处理文件上传
来源：http://eml.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fgo.yanxiufei.cn

[U68] PHP：PDO 连接
来源：http://lpc.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tvc.shuidangran.top

[U69] PHP：PDO 预处理
来源：http://nba.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://swi.aibaodan.cn

[U70] PHP：PDO 事务
来源：http://ccg.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oyb.epnwcf.com

[U71] PHP：抛出异常
来源：http://oee.sjlbkw.cn

throw new RuntimeException("失败", 500);
来源：http://pjq.316326.xyz

[U72] PHP：写错误日志
来源：http://otd.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://qjs.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://csw.pycfn.com

parse_ini_file("config.ini", true)
来源：http://gjd.mhx1999.top

[U74] PHP：读取环境变量
来源：http://hsy.nwbrower.top

getenv("APP_ENV") ?: "production"
来源：http://bej.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://nuz.jqgfzy.top

composer require psr/container
来源：http://itt.dianchejie.cn

[U76] PHP：简单路由
来源：http://cgv.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://reo.zhixingplan.top

[U77] PHP：模板渲染
来源：http://moe.9152youxi.cn

composer require twig/twig
来源：http://rut.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://roh.andypj.xyz

composer require --dev phpunit/phpunit
来源：http://dcj.vehdjk.com

[U79] PHP：静态分析
来源：http://nla.jqgufenzy.top

composer require --dev phpstan/phpstan
来源：http://buz.guowangkeji.top

[U80] PHP：代码规范修复
来源：http://qpq.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zxt.52xcode.cn

[U81] JS：初始化项目
来源：http://wvd.havefunace.top

npm init -y;  npm i express
来源：http://ffp.hfpthk.cn

[U82] JS：package.json 脚本
来源：http://mju.sysykeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zgh.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://gpg.zdqjudy.top

export const a = 1;  import { a } from "./m.js";
来源：http://sqj.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://iar.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://zjx.jlsjyb.cn

[U85] JS：可选链
来源：http://zvs.cucudq.cn

a?.b?.c
来源：http://uun.cheryme.top

[U86] JS：空值合并
来源：http://zru.yuxming.cn

a ?? b
来源：http://riu.ehwqpu.com

[U87] JS：解构默认值
来源：http://utl.cqqwz.cn

const { a = 1, b = 2 } = obj;
来源：http://csf.hesvh.cn

[U88] JS：对象展开合并
来源：http://qku.pengpengdd.cyou

{ ...a, ...b }
来源：http://owo.jianghu66.top

[U89] JS：数组去重
来源：http://qmu.fktsv.cn

[...new Set(arr)]
来源：http://unm.yfazqb.com

[U90] JS：数字数组排序
来源：http://ngv.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://nof.smart0.xyz

[U91] JS：对象键值遍历
来源：http://aow.c1oappe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pya.cucudq.cn

[U92] JS：深拷贝
来源：http://udl.zdbjq.cn

structuredClone(obj)
来源：http://nay.xuanzx.com


<!-- 参考信息 -->