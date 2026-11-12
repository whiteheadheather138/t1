代发 wailian999

[T01] Kotlin：Hello World
来源：http://esh.hcnkem.com

println("Hello")
来源：http://agm.bjfxy.top

[T02] Kotlin：变量
来源：http://vbh.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vov.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://zvr.jqgufenzy.top

"值: $b"
来源：http://eqb.nwbrower.top

[T04] Kotlin：空安全
来源：http://rnf.316326.xyz

val n: String? = null;  n?.length
来源：http://tfi.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://lqo.yangfankeji.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fer.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://epr.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nhp.ivvv.top

[T07] Kotlin：集合过滤
来源：http://lgm.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ieo.9152youxi.cn

[T08] Kotlin：数据类
来源：http://gqz.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://ryg.yj20258.top

[T09] Kotlin：扩展函数
来源：http://nlf.havefunace.top

fun String.exclaim() = this + "!"
来源：http://bfc.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://pcw.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vgt.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://gkz.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bgx.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://kif.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://hrz.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://qqs.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://ubv.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://tan.cqqwz.cn

for (i in 1..10) println(i)
来源：http://qnx.zdbjq.cn

[T15] Kotlin：接口
来源：http://kcx.daxiang520.top

interface Shape { fun area(): Double }
来源：http://ucp.yvedp.cn

[T16] Swift：Hello World
来源：http://mkv.xziqi.cn

print("Hello")
来源：http://sch.mhx1999.top

[T17] Swift：变量与常量
来源：http://lok.ydjk.org.cn

var a = 1;  let b = 2
来源：http://zhk.chenzaomai.com

[T18] Swift：字符串插值
来源：http://yhm.feifeiyinyue.top

"值: \(b)"
来源：http://wdf.316326.xyz

[T19] Swift：可选绑定
来源：http://shi.hnxiangtu.top

if let n = opt { print(n) }
来源：http://acd.9152youxi.cn

[T20] Swift：数组操作
来源：http://uot.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://vef.fehbvm.com

[T21] Swift：遍历
来源：http://vqn.sweek.top

for x in a { print(x) }
来源：http://tie.zhoulong.xyz

[T22] Swift：字典
来源：http://jul.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jom.gzhubu.top

[T23] Swift：函数
来源：http://bnq.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fll.ybcxt.top

[T24] Swift：闭包
来源：http://zjy.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cek.shuidangran.top

[T25] Swift：结构体
来源：http://jdy.yueranfly.top

struct P { var x: Int }
来源：http://nzr.sjlbkw.cn

[T26] Swift：类与重写
来源：http://okp.tanke756.top

class A: Base { override func f() {} }
来源：http://oum.zhengqikj.top

[T27] Swift：错误处理
来源：http://nwh.shuidangran.top

do { try f() } catch { print(error) }
来源：http://ate.ydzc1.top

[T28] Swift：枚举
来源：http://ecq.dianchejie.cn

enum Color { case red, green }
来源：http://kus.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://ozx.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://vsv.gotoacloud.top

[T30] Swift：协议
来源：http://kte.sweek.top

protocol Shape { func area() -> Double }
来源：http://amg.hnqzz.top

[T31] Lua：Hello World
来源：http://dew.aibaodan.cn

print("Hello")
来源：http://ufg.ydzc1.top

[T32] Lua：局部变量
来源：http://ppb.uphjek.com

local a = 1
来源：http://oaq.yueranfly.top

[T33] Lua：表（数组）
来源：http://gie.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ojb.iojbl.cn

[T34] Lua：遍历表
来源：http://rca.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xet.quarkkingdee.top

[T35] Lua：字典表
来源：http://sam.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://eol.uphjek.com

[T36] Lua：函数
来源：http://nby.aizwys.cn

function add(a, b) return a + b end
来源：http://two.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://fhc.yuanzhike.top

"a" .. "b"
来源：http://rxr.zhengqikj.top

[T38] Lua：条件
来源：http://diz.yueranfly.top

if x > 0 then print("正") end
来源：http://qnc.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://nyq.zdbjq.cn

string.find(s, "%d+")
来源：http://jbq.jqgufenzy.top

[T40] Lua：元表
来源：http://dnb.xinyue.icu

setmetatable({}, { __index = base })
来源：http://irk.hcnkem.com

[T41] Perl：Hello World
来源：http://wha.ivvv.top

print "Hello\n";
来源：http://wfi.daxiang520.top

[T42] Perl：变量类型
来源：http://fbf.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vga.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://yes.jqgufenzy.top

"值: $a"
来源：http://qxo.hongshengwenyu.top

[T44] Perl：条件
来源：http://vgy.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://pku.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://fvs.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://gdq.fktsv.cn

[T46] Perl：哈希操作
来源：http://dcq.gzhubu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hyv.jianghu66.top

[T47] Perl：正则捕获
来源：http://std.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cnm.kuanghao11.cn

[T48] Perl：正则替换
来源：http://ulx.yuanzhike.top

$s =~ s/old/new/g;
来源：http://hyu.ppjwa.cn

[T49] Perl：函数
来源：http://pqa.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kgl.tanke756.top

[T50] Perl：逐行读文件
来源：http://qpa.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zph.yongpay.top

while (my $line = <$fh>) { print $line; }
来源：http://wno.ctjpmb.com

[T51] Scala：Hello World
来源：http://rti.zycfv.cn

println("Hello")
来源：http://sye.snrcjt.cn

[T52] Scala：变量
来源：http://txm.ctjpmb.com

val a = 1;  var b = 2
来源：http://gde.ybcxt.top

[T53] Scala：字符串插值
来源：http://rnd.vqdsnc.cn

s"值: $b"
来源：http://foe.aizwys.cn

[T54] Scala：集合映射
来源：http://lfx.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://sjc.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://xry.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://yon.sweek.top

[T56] Scala：样例类
来源：http://bqf.haohaochexian.top

case class User(name: String, age: Int)
来源：http://slv.jyoumei.cn

[T57] Scala：模式匹配
来源：http://fht.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://gzi.shuidangran.top

[T58] Scala：函数定义
来源：http://kln.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://lbb.bbcook.cn

[T59] Scala：循环
来源：http://smf.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://nfe.chenzaomai.com

[T60] Scala：折叠
来源：http://nuz.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://izo.dianchejie.cn

================================================================================
来源：http://glf.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://igt.xinyue.icu

================================================================================
来源：http://kme.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://kwt.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://xmd.uphjek.com

[U02] Py：导出 / 安装依赖
来源：http://eqn.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ynl.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://gkm.jinghuilouyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://awe.haohaochexian.top

[U04] Py：变量调试打印
来源：http://kzr.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ymi.sxryk.cn

[U05] Py：列表去重且保序
来源：http://qxt.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://yhc.yuxming.cn

[U06] Py：合并两个字典
来源：http://myl.hnqzz.top

{**a, **b}
来源：http://agn.yonumen.top

[U07] Py：反转字典键值
来源：http://fqf.jianghu66.top

{v: k for k, v in d.items()}
来源：http://ykf.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://lwv.zycfv.cn

[y for x in nested for y in x]
来源：http://jsi.gogol.net.cn

[U09] Py：字典取最大值的键
来源：http://mfo.aizwys.cn

max(d, key=d.get)
来源：http://xes.yj20258888.top

[U10] Py：按值排序字典
来源：http://ppr.wangshuangyany.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ycg.sweek.top

[U11] Py：生成器表达式
来源：http://jtb.yuanzhike.top

(x * 2 for x in arr)
来源：http://kty.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://aeh.sxryk.cn

Counter(arr).most_common(3)
来源：http://bwg.hcnkem.com

[U13] Py：固定长度队列
来源：http://asl.uphjek.com

deque(maxlen=10)
来源：http://xdd.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://yer.vehdjk.com

defaultdict(list)
来源：http://rrl.chenzaomai.com

[U15] Py：高精度计时
来源：http://wqg.hongshengwenyu.top

t = time.perf_counter()
来源：http://pdi.meibo888.top

[U16] Py：命令行参数解析
来源：http://ycc.guowangkeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kth.fktsv.cn

[U17] Py：初始化日志
来源：http://nmm.gaohongyu789.top

logging.basicConfig(level=logging.INFO)
来源：http://gup.sxryk.cn

[U18] Py：预编译正则
来源：http://tly.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://kpu.ivvv.top

[U19] Py：正则替换带回调
来源：http://utc.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://kfe.xziqi.cn

[U20] Py：缓存函数结果
来源：http://jgk.sweek.top

@functools.lru_cache(maxsize=None)
来源：http://tmu.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://yan.guowangkeji.top

@contextlib.contextmanager
来源：http://tzo.havefunace.top

[U22] Py：矩阵转置
来源：http://npl.yueranfly.top

list(zip(*m))
来源：http://udi.fehbvm.com

[U23] Py：分块读取大文件
来源：http://upj.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xaq.fktsv.cn

[U24] Py：路径操作
来源：http://krx.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zqb.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://gnd.fktsv.cn

csv.DictReader(f)
来源：http://flm.svipenyu.cn

[U26] Py：并发下载
来源：http://lmx.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jaw.jyoumei.cn

[U27] Py：异步 HTTP
来源：http://mlm.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://xkt.zycfv.cn

[U28] Py：类型别名
来源：http://omt.hywenlv.cn

UserId = int
来源：http://fvw.gaohongyu789.top

[U29] Py：属性校验
来源：http://ags.bbcook.cn

@property 与 @x.setter 配合
来源：http://ipo.jinyuanbaomall.cn

[U30] Py：数据类
来源：http://jln.hnqzz.top

@dataclass(slots=True)
来源：http://fuk.9152youxi.cn

[U31] Py：单测
来源：http://iji.zhongyouzk.top

python -m pytest -q
来源：http://pia.yanxiufei.cn

[U32] Py：代码格式化
来源：http://sbk.fehbvm.com

ruff format . && ruff check --fix .
来源：http://hpx.hywenlv.cn

[U33] Py：打包发布
来源：http://klh.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://uit.nanxinkj.top

[U34] Py：判断编码
来源：http://yix.yanxiufei.cn

chardet.detect(raw)
来源：http://wga.snrcjt.cn

[U35] Py：发送邮件
来源：http://kbn.kuanghao11.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zlg.yuxming.cn

[U36] Py：定时任务
来源：http://bbm.zdbjq.cn

schedule.every(10).minutes.do(job)
来源：http://cjw.316326.xyz

[U37] Py：读写 Excel
来源：http://ykm.xuanzx.com

pandas.read_excel / DataFrame.to_excel
来源：http://qmz.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://aam.yj20258.top

Path(__file__).resolve().parent
来源：http://xgf.yangfankeji.com

[U39] Py：判断是否在交互环境
来源：http://mbq.chenjidiqi.icu

sys.stdout.isatty()
来源：http://yow.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://wna.yfazqb.com

print("err", file=sys.stderr)
来源：http://sov.bbcook.cn

[U41] PHP：初始化 Composer 项目
来源：http://lbe.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mzp.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://efh.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bvm.fktsv.cn

[U43] PHP：声明命名空间
来源：http://lfx.ehwqpu.com

namespace App\Http;
来源：http://jwq.316326.xyz

[U44] PHP：开启严格类型
来源：http://ewk.gotoacloud.top

declare(strict_types=1);
来源：http://vxi.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://zpf.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sih.yj20258888.top

[U46] PHP：可空类型
来源：http://xpt.yonumen.top

?string $name = null
来源：http://rjr.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://ngl.cheryme.top

int|string $id
来源：http://izz.yangfankeji.com

[U48] PHP：纯枚举
来源：http://ucn.52xcode.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gee.haohaochexian.top

[U49] PHP：只读属性
来源：http://cix.daxiang520.top

public readonly string $name
来源：http://ihf.feifeiyinyue.top

[U50] PHP：构造器属性提升
来源：http://fto.yongpay.top

public function __construct(private int $id) {}
来源：http://avf.zdqjudy.top

[U51] PHP：数组解构
来源：http://iaq.xinyue.icu

[$a, $b] = $arr;
来源：http://qmu.uphjek.com

[U52] PHP：箭头函数
来源：http://lkg.dashuyun.cn

$double = fn($x) => $x * 2;
来源：http://umw.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://iwj.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://cun.pengpengdd.cyou

[U54] PHP：空安全调用
来源：http://xkj.yueranfly.top

$obj?->method()
来源：http://fff.wangdashe.top

[U55] PHP：match 表达式
来源：http://qnq.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://abj.nanxuanxn.top

[U56] PHP：命名参数
来源：http://orq.zycfv.cn

f(a: 1, b: 2)
来源：http://brn.tian-w.cn

[U57] PHP：字符串插值
来源：http://roq.feifeiyinyue.top

"值: {$a}"
来源：http://ytq.ybcxt.top

[U58] PHP：数组三件套
来源：http://liw.zdqjudy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://try.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://xqv.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uxi.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://yjv.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ktr.yj20258888.top

[U61] PHP：正则
来源：http://kox.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qqp.feifeiyinyue.top

[U62] PHP：日期对象
来源：http://rjn.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lyl.hnqzz.top

[U63] PHP：文件读写
来源：http://kfb.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yjn.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://xpq.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://zzq.chenlongwang.top

[U65] PHP：会话
来源：http://xrm.zhaomingkeji.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://zcb.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://zse.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vpk.gogol.net.cn

[U67] PHP：处理文件上传
来源：http://lso.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pro.jianghu66.top

[U68] PHP：PDO 连接
来源：http://jxl.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pdk.redwolf501.top

[U69] PHP：PDO 预处理
来源：http://lpu.epnwcf.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://alx.zhiwuduotai.top

[U70] PHP：PDO 事务
来源：http://khb.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ebf.yvedp.cn

[U71] PHP：抛出异常
来源：http://cop.dianchejie.cn

throw new RuntimeException("失败", 500);
来源：http://vwi.xingfuxueyuan.xyz

[U72] PHP：写错误日志
来源：http://vtc.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://yar.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://bjs.xylfe.cn

parse_ini_file("config.ini", true)
来源：http://izx.pycfn.com

[U74] PHP：读取环境变量
来源：http://hkk.zhijiandao.cn

getenv("APP_ENV") ?: "production"
来源：http://mvs.svipenyu.cn

[U75] PHP：依赖注入
来源：http://rbl.jinqigfzy.top

composer require psr/container
来源：http://hue.sufxvd.cn

[U76] PHP：简单路由
来源：http://ptj.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pad.hesvh.cn

[U77] PHP：模板渲染
来源：http://cfn.hongshengwenyu.top

composer require twig/twig
来源：http://eqx.guannengcc.top

[U78] PHP：单元测试
来源：http://fog.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://pjy.cqqwz.cn

[U79] PHP：静态分析
来源：http://lej.jyoumei.cn

composer require --dev phpstan/phpstan
来源：http://puk.yj202588.top

[U80] PHP：代码规范修复
来源：http://wwh.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xdb.yonumen.top

[U81] JS：初始化项目
来源：http://isx.sysykeji.top

npm init -y;  npm i express
来源：http://pdf.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://lho.bbcook.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hzk.daxiang520.top

[U83] JS：ES Module 导入导出
来源：http://yvy.zhengqikj.top

export const a = 1;  import { a } from "./m.js";
来源：http://dti.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://jxo.52xcode.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jiu.aizwys.cn

[U85] JS：可选链
来源：http://hzh.cheryme.top

a?.b?.c
来源：http://slc.dianchejie.cn

[U86] JS：空值合并
来源：http://lcl.jiagoushi.top

a ?? b
来源：http://cqx.cucudq.cn

[U87] JS：解构默认值
来源：http://uqz.zhongyouzk.top

const { a = 1, b = 2 } = obj;
来源：http://vhh.jyoumei.cn

[U88] JS：对象展开合并
来源：http://niv.gzhubu.top

{ ...a, ...b }
来源：http://zmn.yj20258888.top


<!-- 参考信息 -->