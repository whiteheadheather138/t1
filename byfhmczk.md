代发 wailian999

[T05] Kotlin：when 表达式
来源：http://stm.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hol.yonumen.top

[T06] Kotlin：集合映射
来源：http://vab.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qti.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://sgo.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxj.zhengqikj.top

[T08] Kotlin：数据类
来源：http://tjf.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://rtq.meibo888.top

[T09] Kotlin：扩展函数
来源：http://qmx.gotoacloud.top

fun String.exclaim() = this + "!"
来源：http://kck.vehdjk.com

[T10] Kotlin：默认参数
来源：http://vsu.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://inn.zhengqikj.top

[T11] Kotlin：协程
来源：http://apr.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fsd.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://uyl.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://aec.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://lsq.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://fgf.andypj.xyz

[T14] Kotlin：循环
来源：http://yie.xylfe.cn

for (i in 1..10) println(i)
来源：http://vgj.guowangkeji.top

[T15] Kotlin：接口
来源：http://pjt.52xcode.cn

interface Shape { fun area(): Double }
来源：http://khp.yongpay.top

[T16] Swift：Hello World
来源：http://lbx.yj20258.top

print("Hello")
来源：http://lum.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://cpi.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://vjj.uphjek.com

[T18] Swift：字符串插值
来源：http://wvm.haohaochexian.top

"值: \(b)"
来源：http://huv.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://rsi.bjfxy.top

if let n = opt { print(n) }
来源：http://hey.kuanghao11.cn

[T20] Swift：数组操作
来源：http://pml.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://zof.zhijiandao.cn

[T21] Swift：遍历
来源：http://krg.ctjpmb.com

for x in a { print(x) }
来源：http://wke.tian-w.cn

[T22] Swift：字典
来源：http://fme.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jdk.wangdashe.top

[T23] Swift：函数
来源：http://orw.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vtd.birdmap.top

[T24] Swift：闭包
来源：http://dxp.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dzl.yuxming.cn

[T25] Swift：结构体
来源：http://eka.daxiang520.top

struct P { var x: Int }
来源：http://ohf.epnwcf.com

[T26] Swift：类与重写
来源：http://wst.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://hod.zhoulong.xyz

[T27] Swift：错误处理
来源：http://uuu.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://qlt.yanxiufei.cn

[T28] Swift：枚举
来源：http://wwv.shzxlz.cn

enum Color { case red, green }
来源：http://uhj.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://wyo.yueranfly.top

guard let x = opt else { return }
来源：http://wkm.meibo888.top

[T30] Swift：协议
来源：http://csp.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://dap.guannengcc.top

[T31] Lua：Hello World
来源：http://azw.redwolf501.top

print("Hello")
来源：http://ykh.316326.xyz

[T32] Lua：局部变量
来源：http://scb.316326.xyz

local a = 1
来源：http://xzt.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://xyk.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cyn.kuanghao11.cn

[T34] Lua：遍历表
来源：http://ffb.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ncm.mhx1999.top

[T35] Lua：字典表
来源：http://ltr.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://hwn.jinghuilouyu.cn

[T36] Lua：函数
来源：http://czi.shzxlz.cn

function add(a, b) return a + b end
来源：http://tqy.yonumen.top

[T37] Lua：字符串拼接
来源：http://lqu.kuanghao11.cn

"a" .. "b"
来源：http://xgl.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://nxd.hammf.cn

if x > 0 then print("正") end
来源：http://kfh.yonumen.top

[T39] Lua：模式匹配
来源：http://nig.hfpthk.cn

string.find(s, "%d+")
来源：http://ktg.snrcjt.cn

[T40] Lua：元表
来源：http://foo.daxiang520.top

setmetatable({}, { __index = base })
来源：http://wzr.sjlbkw.cn

[T41] Perl：Hello World
来源：http://tjc.zhixingplan.top

print "Hello\n";
来源：http://usz.uphjek.com

[T42] Perl：变量类型
来源：http://pfg.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmo.jqgfzy.top

[T43] Perl：字符串插值
来源：http://czt.xylfe.cn

"值: $a"
来源：http://klg.yuxming.cn

[T44] Perl：条件
来源：http://uca.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://nhg.cqqwz.cn

[T45] Perl：数组遍历
来源：http://pgp.yonumen.top

for my $x (@arr) { print $x; }
来源：http://xte.meibo888.top

[T46] Perl：哈希操作
来源：http://hnp.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lpt.yvedp.cn

[T47] Perl：正则捕获
来源：http://cau.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ppw.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://bya.fzhhl.top

$s =~ s/old/new/g;
来源：http://xdc.xuanzx.com

[T49] Perl：函数
来源：http://jjn.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ymi.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://pnn.sjlbkw.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ozx.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://mpa.mhx1999.top

[T51] Scala：Hello World
来源：http://zvg.sufxvd.cn

println("Hello")
来源：http://ltw.xinyue.icu

[T52] Scala：变量
来源：http://gfa.tanke756.top

val a = 1;  var b = 2
来源：http://pcz.bjfxy.top

[T53] Scala：字符串插值
来源：http://bwp.bjfxy.top

s"值: $b"
来源：http://bbd.zhixingplan.top

[T54] Scala：集合映射
来源：http://bhh.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://ibq.snrcjt.cn

[T55] Scala：集合过滤
来源：http://mad.epnwcf.com

List(1, 2, 3).filter(_ > 1)
来源：http://wtk.yuanzhike.top

[T56] Scala：样例类
来源：http://sbr.hfpthk.cn

case class User(name: String, age: Int)
来源：http://gde.daria6918.cn

[T57] Scala：模式匹配
来源：http://daw.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rrs.yfazqb.com

[T58] Scala：函数定义
来源：http://ydw.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://oqa.316326.xyz

[T59] Scala：循环
来源：http://liq.smart0.xyz

for (i <- 1 to 10) println(i)
来源：http://sjr.zdqjudy.top

[T60] Scala：折叠
来源：http://dny.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wzg.zdbjq.cn

================================================================================
来源：http://hln.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://buj.shzxlz.cn

================================================================================
来源：http://bmq.havefunace.top

[U01] Py：创建虚拟环境
来源：http://cep.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dig.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://zxr.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nlp.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://pyn.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mjg.yj202588.top

[U04] Py：变量调试打印
来源：http://ije.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vum.havefunace.top

[U05] Py：列表去重且保序
来源：http://fpi.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://tvk.birdmap.top

[U06] Py：合并两个字典
来源：http://jax.xylfe.cn

{**a, **b}
来源：http://dvt.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://rvx.zhoulong.xyz

{v: k for k, v in d.items()}
来源：http://xog.yueranfly.top

[U08] Py：展平二维列表
来源：http://afp.zdbjq.cn

[y for x in nested for y in x]
来源：http://hbb.316326.xyz

[U09] Py：字典取最大值的键
来源：http://rwm.cdnleiting.top

max(d, key=d.get)
来源：http://hhe.xinyue.icu

[U10] Py：按值排序字典
来源：http://hsv.zdbjq.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lat.sysykeji.top

[U11] Py：生成器表达式
来源：http://ghs.ctjpmb.com

(x * 2 for x in arr)
来源：http://psz.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://xls.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://jvq.yuanzhike.top

[U13] Py：固定长度队列
来源：http://tmz.hnxiangtu.top

deque(maxlen=10)
来源：http://gmt.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://lqg.jqgufenzy.top

defaultdict(list)
来源：http://ykt.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://wah.zhixingplan.top

t = time.perf_counter()
来源：http://vqw.nanxinkj.top

[U16] Py：命令行参数解析
来源：http://sgx.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bsz.316326.xyz

[U17] Py：初始化日志
来源：http://xek.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://isb.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://kjl.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://ofe.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://ftv.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ubj.andypj.xyz

[U20] Py：缓存函数结果
来源：http://ooy.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://wmj.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://qmh.gaohongyu789.top

@contextlib.contextmanager
来源：http://ioh.yuxming.cn

[U22] Py：矩阵转置
来源：http://wvq.svipenyu.cn

list(zip(*m))
来源：http://syg.ywan-chungtsiang.top

[U23] Py：分块读取大文件
来源：http://glr.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://awk.sxryk.cn

[U24] Py：路径操作
来源：http://hhe.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wib.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://zkc.shanyushiyangtech.top

csv.DictReader(f)
来源：http://yvg.yj202588.top

[U26] Py：并发下载
来源：http://ixj.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://thw.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://enr.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://cad.chenlongwang.top

[U28] Py：类型别名
来源：http://mmy.shuidangran.top

UserId = int
来源：http://zdw.zhijiandao.cn

[U29] Py：属性校验
来源：http://sax.yuxming.cn

@property 与 @x.setter 配合
来源：http://ejo.yj20258888.top

[U30] Py：数据类
来源：http://kqs.zhixingplan.top

@dataclass(slots=True)
来源：http://arg.tarul.cn

[U31] Py：单测
来源：http://ukp.yongpay.top

python -m pytest -q
来源：http://akp.dianchejie.cn

[U32] Py：代码格式化
来源：http://xvp.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://zpy.hongshengwenyu.top

[U33] Py：打包发布
来源：http://qbn.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://jqm.c1oappe.top

[U34] Py：判断编码
来源：http://hmn.jqgfzy.top

chardet.detect(raw)
来源：http://oni.yvedp.cn

[U35] Py：发送邮件
来源：http://jqy.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vss.chenzaomai.com

[U36] Py：定时任务
来源：http://sct.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://pom.ctjpmb.com

[U37] Py：读写 Excel
来源：http://fjq.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hdp.sufxvd.cn

[U38] Py：获取脚本所在目录
来源：http://lou.aizwys.cn

Path(__file__).resolve().parent
来源：http://gib.jqgufenzy.top

[U39] Py：判断是否在交互环境
来源：http://wkq.yuanzhike.top

sys.stdout.isatty()
来源：http://uhn.ehwqpu.com

[U40] Py：打印到标准错误
来源：http://hbg.meibo888.top

print("err", file=sys.stderr)
来源：http://dah.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://ryi.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dqf.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://xpa.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fru.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://fto.shangyingyoupin.top

namespace App\Http;
来源：http://sen.vehdjk.com

[U44] PHP：开启严格类型
来源：http://ukt.pengpengdd.cyou

declare(strict_types=1);
来源：http://uoi.epnwcf.com

[U45] PHP：类型声明与返回类型
来源：http://pyw.haohaochexian.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gio.nanxinkj.top

[U46] PHP：可空类型
来源：http://neh.xylfe.cn

?string $name = null
来源：http://wkq.hysaishi.cn

[U47] PHP：联合类型
来源：http://qfd.0kj1m.cn

int|string $id
来源：http://ykj.fengsongda.top

[U48] PHP：纯枚举
来源：http://tfz.gaohongyu789.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rcb.cqqwz.cn

[U49] PHP：只读属性
来源：http://fff.chenzaomai.com

public readonly string $name
来源：http://exv.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://qvu.jyoumei.cn

public function __construct(private int $id) {}
来源：http://whf.bbcook.cn

[U51] PHP：数组解构
来源：http://esb.ydzc1.top

[$a, $b] = $arr;
来源：http://epd.yangfankeji.com

[U52] PHP：箭头函数
来源：http://oih.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://atj.bbcook.cn

[U53] PHP：空合并运算符
来源：http://xif.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://xnu.wangdashe.top

[U54] PHP：空安全调用
来源：http://czl.zhaomingkeji.xyz

$obj?->method()
来源：http://yrw.nwbrower.top

[U55] PHP：match 表达式
来源：http://eno.jiagoushi.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://edc.nanxuanxn.top

[U56] PHP：命名参数
来源：http://iyq.xuetiantiany.cn

f(a: 1, b: 2)
来源：http://cji.bbcook.cn

[U57] PHP：字符串插值
来源：http://whp.tanke756.top

"值: {$a}"
来源：http://fuv.c1oappe.top

[U58] PHP：数组三件套
来源：http://nfz.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://npn.0kj1m.cn

[U59] PHP：自定义排序
来源：http://jmu.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wea.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://ede.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fqc.aibaodan.cn

[U61] PHP：正则
来源：http://bhd.yfazqb.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zth.ybcxt.top

[U62] PHP：日期对象
来源：http://tch.ywan-chungtsiang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rwr.wangdashe.top

[U63] PHP：文件读写
来源：http://uho.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dkc.52xcode.cn

[U64] PHP：目录遍历
来源：http://thb.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://vhy.xuanzx.com

[U65] PHP：会话
来源：http://wuq.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dsn.wangdashe.top

[U66] PHP：设置 Cookie
来源：http://kvl.tianlin.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fec.aizwys.cn

[U67] PHP：处理文件上传
来源：http://jbt.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyf.cashguo.top

[U68] PHP：PDO 连接
来源：http://cji.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uml.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://nrf.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://cxy.zhijiandao.cn

[U70] PHP：PDO 事务
来源：http://mdx.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oog.snrcjt.cn

[U71] PHP：抛出异常
来源：http://jhe.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://pda.yueranfly.top

[U72] PHP：写错误日志
来源：http://xww.nanxuanxn.top

error_log("失败: " . $e->getMessage());
来源：http://irj.xinyue.icu

[U73] PHP：读取 ini 配置
来源：http://oeo.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://iaa.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://eyw.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://yfl.guowangkeji.top

[U75] PHP：依赖注入
来源：http://cqv.sweek.top

composer require psr/container
来源：http://vhi.hcnkem.com

[U76] PHP：简单路由
来源：http://een.birdmap.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gbv.zycfv.cn

[U77] PHP：模板渲染
来源：http://hxx.yangfankeji.com

composer require twig/twig
来源：http://lbp.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://oeo.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://lme.yueranfly.top

[U79] PHP：静态分析
来源：http://imf.ywan-chungtsiang.top

composer require --dev phpstan/phpstan
来源：http://ppy.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://bwm.sweek.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://unq.shangyingyoupin.top

[U81] JS：初始化项目
来源：http://fvs.hysaishi.cn

npm init -y;  npm i express
来源：http://quk.dianchejie.cn

[U82] JS：package.json 脚本
来源：http://vvc.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qfm.pycfn.com

[U83] JS：ES Module 导入导出
来源：http://gxb.ehwqpu.com

export const a = 1;  import { a } from "./m.js";
来源：http://nhk.zhijiandao.cn

[U84] JS：CommonJS 写法
来源：http://eid.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rva.dashuyun.cn

[U85] JS：可选链
来源：http://nqb.dianchejie.cn

a?.b?.c
来源：http://jpu.cheryme.top

[U86] JS：空值合并
来源：http://bcg.kuanghao11.cn

a ?? b
来源：http://cnk.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://jws.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://mti.xingfuxueyuan.xyz

[U88] JS：对象展开合并
来源：http://vnj.havefunace.top

{ ...a, ...b }
来源：http://wdp.hnxiangtu.top

[U89] JS：数组去重
来源：http://pth.jiagoushi.top

[...new Set(arr)]
来源：http://xor.aibaodan.cn

[U90] JS：数字数组排序
来源：http://lcx.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://vwf.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://oeq.yueranfly.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://eqo.dashuyun.cn

[U92] JS：深拷贝
来源：http://pfo.andypj.xyz

structuredClone(obj)
来源：http://tef.vehdjk.com


<!-- 参考信息 -->