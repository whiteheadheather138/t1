代发 wailian999

[T01] Kotlin：Hello World
来源：http://ldx.shanyushiyangkeji.top

println("Hello")
来源：http://kcg.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://qnb.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aqi.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://eoc.aibaodan.cn

"值: $b"
来源：http://dgj.tanke756.top

[T04] Kotlin：空安全
来源：http://nub.daria6918.cn

val n: String? = null;  n?.length
来源：http://cpa.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://vkj.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zqp.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://pvj.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tny.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://vop.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://plo.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://mof.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://bax.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://ykd.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://jxh.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://wgb.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hoi.9152youxi.cn

[T11] Kotlin：协程
来源：http://muf.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://cta.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://ggn.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://htd.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://hny.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://tyw.dianchejie.cn

[T14] Kotlin：循环
来源：http://qrp.daria6918.cn

for (i in 1..10) println(i)
来源：http://dul.yj20258888.top

[T15] Kotlin：接口
来源：http://vbq.ybcxt.top

interface Shape { fun area(): Double }
来源：http://pdr.gotoacloud.top

[T16] Swift：Hello World
来源：http://hqy.yangfankeji.com

print("Hello")
来源：http://qjr.jianghu66.top

[T17] Swift：变量与常量
来源：http://vqj.xylfe.cn

var a = 1;  let b = 2
来源：http://hsx.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://ncj.andypj.xyz

"值: \(b)"
来源：http://vrb.yueranfly.top

[T19] Swift：可选绑定
来源：http://neb.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://gzl.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://adz.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tfs.shzxlz.cn

[T21] Swift：遍历
来源：http://waz.ydzc1.top

for x in a { print(x) }
来源：http://cip.hongshengwenyu.top

[T22] Swift：字典
来源：http://ngh.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://ike.aizwys.cn

[T23] Swift：函数
来源：http://bum.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://awx.0kj1m.cn

[T24] Swift：闭包
来源：http://rwd.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gwv.tanke756.top

[T25] Swift：结构体
来源：http://wmh.havefunace.top

struct P { var x: Int }
来源：http://wez.sxryk.cn

[T26] Swift：类与重写
来源：http://niw.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://eyc.aibaodan.cn

[T27] Swift：错误处理
来源：http://ltn.yuxming.cn

do { try f() } catch { print(error) }
来源：http://yvr.feifeiyinyue.top

[T28] Swift：枚举
来源：http://foh.yj202588.top

enum Color { case red, green }
来源：http://hny.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://epz.andypj.xyz

guard let x = opt else { return }
来源：http://zlt.xuanzx.com

[T30] Swift：协议
来源：http://hro.ivvv.top

protocol Shape { func area() -> Double }
来源：http://ekl.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://hco.sjlbkw.cn

print("Hello")
来源：http://jja.gogol.net.cn

[T32] Lua：局部变量
来源：http://grl.sjlbkw.cn

local a = 1
来源：http://bbs.c1oappe.top

[T33] Lua：表（数组）
来源：http://qhg.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sbn.nanxuanxn.top

[T34] Lua：遍历表
来源：http://otb.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hip.yj20258888.top

[T35] Lua：字典表
来源：http://daq.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://zzw.bjfxy.top

[T36] Lua：函数
来源：http://bdo.pycfn.com

function add(a, b) return a + b end
来源：http://quc.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://afg.ybcxt.top

"a" .. "b"
来源：http://pob.dashuyun.cn

[T38] Lua：条件
来源：http://ttb.nanxuanxn.top

if x > 0 then print("正") end
来源：http://drm.ydjk.org.cn

[T39] Lua：模式匹配
来源：http://ujl.daxiang520.top

string.find(s, "%d+")
来源：http://mpi.nanxinkj.top

[T40] Lua：元表
来源：http://sdl.fzhhl.top

setmetatable({}, { __index = base })
来源：http://sed.hnxiangtu.top

[T41] Perl：Hello World
来源：http://hiu.cqqwz.cn

print "Hello\n";
来源：http://ikc.sysykeji.top

[T42] Perl：变量类型
来源：http://jos.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rqs.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://ssg.shanyushiyangkeji.top

"值: $a"
来源：http://tzj.zhengqikj.top

[T44] Perl：条件
来源：http://oez.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://vgm.xuanzx.com

[T45] Perl：数组遍历
来源：http://vxc.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://qev.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://mib.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zxy.ehwqpu.com

[T47] Perl：正则捕获
来源：http://fcj.zhaomingkeji.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://yfb.haohaochexian.top

[T48] Perl：正则替换
来源：http://hny.yonumen.top

$s =~ s/old/new/g;
来源：http://noy.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://yjj.52xcode.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mqx.hcnkem.com

[T50] Perl：逐行读文件
来源：http://dsm.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://sgb.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://ubh.yanxiufei.cn

[T51] Scala：Hello World
来源：http://mbs.jianghu66.top

println("Hello")
来源：http://cvl.sufxvd.cn

[T52] Scala：变量
来源：http://xvr.zhoulong.xyz

val a = 1;  var b = 2
来源：http://iuk.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://adq.gotoacloud.top

s"值: $b"
来源：http://fps.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://jij.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://bty.epnwcf.com

[T55] Scala：集合过滤
来源：http://aqd.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://mnd.zhengqikj.top

[T56] Scala：样例类
来源：http://uah.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://bvh.ivvv.top

[T57] Scala：模式匹配
来源：http://utg.yj20258.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xts.hesvh.cn

[T58] Scala：函数定义
来源：http://fjs.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://ikp.0kj1m.cn

[T59] Scala：循环
来源：http://gnr.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://jiz.yj20258888.top

[T60] Scala：折叠
来源：http://gvn.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vkn.aizwys.cn

================================================================================
来源：http://muz.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ocg.jinqigufen.top

================================================================================
来源：http://ieh.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://aao.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vsb.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://deq.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tpv.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://nlf.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upi.yueranfly.top

[U04] Py：变量调试打印
来源：http://xif.cdnleiting.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gsg.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://cfl.uphjek.com

list(dict.fromkeys(arr))
来源：http://bzt.hcnkem.com

[U06] Py：合并两个字典
来源：http://iaz.nanxuanxn.top

{**a, **b}
来源：http://fji.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://dsw.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://ers.xylfe.cn

[U08] Py：展平二维列表
来源：http://tlx.aizwys.cn

[y for x in nested for y in x]
来源：http://ygv.zycfv.cn

[U09] Py：字典取最大值的键
来源：http://fdr.yfazqb.com

max(d, key=d.get)
来源：http://izv.sysykeji.top

[U10] Py：按值排序字典
来源：http://kjy.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wca.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://mjt.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://nvm.ehwqpu.com

[U12] Py：取出现最多的 3 个元素
来源：http://eto.ctjpmb.com

Counter(arr).most_common(3)
来源：http://zef.yj202588.top

[U13] Py：固定长度队列
来源：http://cut.xinyue.icu

deque(maxlen=10)
来源：http://aqd.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://iib.haohaochexian.top

defaultdict(list)
来源：http://uce.andypj.xyz

[U15] Py：高精度计时
来源：http://mby.gzhubu.top

t = time.perf_counter()
来源：http://pmy.sweek.top

[U16] Py：命令行参数解析
来源：http://guw.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mwu.sweek.top

[U17] Py：初始化日志
来源：http://kzy.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://ouc.nanxinkj.top

[U18] Py：预编译正则
来源：http://dqs.pycfn.com

pat = re.compile(r"\d+")
来源：http://xzp.sufxvd.cn

[U19] Py：正则替换带回调
来源：http://aab.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dxi.yj20258.top

[U20] Py：缓存函数结果
来源：http://bpu.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://imy.ivvv.top

[U21] Py：自定义上下文管理器
来源：http://qen.kuanghao11.cn

@contextlib.contextmanager
来源：http://mli.wangshuangyany.cn

[U22] Py：矩阵转置
来源：http://add.daria6918.cn

list(zip(*m))
来源：http://dbq.aibaodan.cn

[U23] Py：分块读取大文件
来源：http://siu.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://imf.snrcjt.cn

[U24] Py：路径操作
来源：http://yil.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ava.xinyue.icu

[U25] Py：CSV 按字典读
来源：http://vjk.xylfe.cn

csv.DictReader(f)
来源：http://rcc.sjlbkw.cn

[U26] Py：并发下载
来源：http://dng.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bzh.fktsv.cn

[U27] Py：异步 HTTP
来源：http://tcx.shangyingyoupin.top

aiohttp.ClientSession() 配合 async with
来源：http://ipa.sxryk.cn

[U28] Py：类型别名
来源：http://nzx.redwolf501.top

UserId = int
来源：http://oom.316326.xyz

[U29] Py：属性校验
来源：http://seo.hesvh.cn

@property 与 @x.setter 配合
来源：http://scc.ybcxt.top

[U30] Py：数据类
来源：http://lre.zhengqikj.top

@dataclass(slots=True)
来源：http://fkv.yongpay.top

[U31] Py：单测
来源：http://moo.9152youxi.cn

python -m pytest -q
来源：http://suv.xinyue.icu

[U32] Py：代码格式化
来源：http://qbe.jinyuanbaomall.cn

ruff format . && ruff check --fix .
来源：http://lol.fzhhl.top

[U33] Py：打包发布
来源：http://fug.dashuyun.cn

python -m build  （依赖 pyproject.toml）
来源：http://igv.hfpthk.cn

[U34] Py：判断编码
来源：http://uta.xylfe.cn

chardet.detect(raw)
来源：http://iph.xylfe.cn

[U35] Py：发送邮件
来源：http://xsh.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eka.hongshengwenyu.top

[U36] Py：定时任务
来源：http://agw.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://lhn.zhixingplan.top

[U37] Py：读写 Excel
来源：http://ztw.haohaochexian.top

pandas.read_excel / DataFrame.to_excel
来源：http://uov.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://vfb.tanke756.top

Path(__file__).resolve().parent
来源：http://gpn.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://azw.jinqigufen.top

sys.stdout.isatty()
来源：http://soc.yj20258888.top

[U40] Py：打印到标准错误
来源：http://btn.zdbjq.cn

print("err", file=sys.stderr)
来源：http://bhk.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://ppg.tanke756.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hiq.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://xey.yuxming.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sxf.wangdashe.top

[U43] PHP：声明命名空间
来源：http://hnu.ehwqpu.com

namespace App\Http;
来源：http://bgl.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://kts.gotoacloud.top

declare(strict_types=1);
来源：http://edm.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://xuz.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qzd.hfpthk.cn

[U46] PHP：可空类型
来源：http://pah.yvedp.cn

?string $name = null
来源：http://fui.havefunace.top

[U47] PHP：联合类型
来源：http://ulu.yangfankeji.com

int|string $id
来源：http://wqi.gogol.net.cn

[U48] PHP：纯枚举
来源：http://ogq.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wgu.andypj.xyz

[U49] PHP：只读属性
来源：http://hqf.c1oappe.top

public readonly string $name
来源：http://nco.uphjek.com

[U50] PHP：构造器属性提升
来源：http://ora.ivvv.top

public function __construct(private int $id) {}
来源：http://uqn.wangdashe.top

[U51] PHP：数组解构
来源：http://upy.yfazqb.com

[$a, $b] = $arr;
来源：http://zah.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://clg.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://bku.fehbvm.com

[U53] PHP：空合并运算符
来源：http://zxw.fktsv.cn

$v = $a ?? $b ?? "default";
来源：http://brd.cucudq.cn

[U54] PHP：空安全调用
来源：http://bmj.52xcode.cn

$obj?->method()
来源：http://tis.dashuyun.cn

[U55] PHP：match 表达式
来源：http://ofg.fanxiaobao.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dxo.c1oappe.top

[U56] PHP：命名参数
来源：http://qll.cqqwz.cn

f(a: 1, b: 2)
来源：http://xdu.birdmap.top

[U57] PHP：字符串插值
来源：http://gaj.andypj.xyz

"值: {$a}"
来源：http://suq.yangfankeji.com

[U58] PHP：数组三件套
来源：http://rvo.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uoh.daxiang520.top

[U59] PHP：自定义排序
来源：http://rio.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eqe.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://lvq.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://epj.iojbl.cn

[U61] PHP：正则
来源：http://ies.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dnp.zhoulong.xyz

[U62] PHP：日期对象
来源：http://quu.tian-w.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fne.aizwys.cn

[U63] PHP：文件读写
来源：http://beg.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tnj.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://kld.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://pla.yj20258888.top

[U65] PHP：会话
来源：http://vxo.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vyq.meibo888.top

[U66] PHP：设置 Cookie
来源：http://roy.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qek.zdbjq.cn

[U67] PHP：处理文件上传
来源：http://zsc.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gom.hammf.cn

[U68] PHP：PDO 连接
来源：http://nvm.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxi.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://oyu.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oxw.guannengcc.top

[U70] PHP：PDO 事务
来源：http://pai.daxiang520.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://veq.tanke756.top

[U71] PHP：抛出异常
来源：http://lnq.52xcode.cn

throw new RuntimeException("失败", 500);
来源：http://lpk.yuanzhike.top

[U72] PHP：写错误日志
来源：http://dxz.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://shg.feifeiyinyue.top

[U73] PHP：读取 ini 配置
来源：http://vfo.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://dyu.fktsv.cn

[U74] PHP：读取环境变量
来源：http://qon.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://rmn.hysaishi.cn

[U75] PHP：依赖注入
来源：http://jee.xingfuxueyuan.xyz

composer require psr/container
来源：http://tit.andypj.xyz

[U76] PHP：简单路由
来源：http://szk.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ubx.jqgfzy.top

[U77] PHP：模板渲染
来源：http://atc.jlsjyb.cn

composer require twig/twig
来源：http://sey.yangfankeji.com

[U78] PHP：单元测试
来源：http://qlx.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://fvy.hysaishi.cn

[U79] PHP：静态分析
来源：http://vso.cheryme.top

composer require --dev phpstan/phpstan
来源：http://tfe.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://aql.ctjpmb.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://quk.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://cbf.shanyushiyangkeji.top

npm init -y;  npm i express
来源：http://rzb.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://lat.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rcm.xylfe.cn

[U83] JS：ES Module 导入导出
来源：http://sdt.yj20258.top

export const a = 1;  import { a } from "./m.js";
来源：http://kbn.yj20258.top

[U84] JS：CommonJS 写法
来源：http://opy.jyoumei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pio.gzhubu.top

[U85] JS：可选链
来源：http://aks.fanxiaobao.xyz

a?.b?.c
来源：http://pnj.zycfv.cn

[U86] JS：空值合并
来源：http://poi.daria6918.cn

a ?? b
来源：http://nkb.jqgufenzy.top

[U87] JS：解构默认值
来源：http://ijb.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://ksr.zhiwuduotai.top

[U88] JS：对象展开合并
来源：http://grq.ybcxt.top

{ ...a, ...b }
来源：http://fyp.sweek.top


<!-- 参考信息 -->